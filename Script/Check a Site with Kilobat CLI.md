# Check a site with Kilobat CLI

```sh
#!/bin/sh
# Pass the Ask for Input result to this action as arguments.
for kilobat_cli in /opt/homebrew/bin/kilobat /usr/local/bin/kilobat; do
    [ -x "$kilobat_cli" ] && break
done
if [ ! -x "$kilobat_cli" ]; then
    printf '%s\n' 'Install Kilobat CLI with Homebrew first. See https://kilobat.app.'
    exit 0
fi
if [ -z "$1" ]; then
    printf '%s\n' 'Enter a hostname such as example.com.'
    exit 0
fi
kilobat_report=$("$kilobat_cli" why "$1" --json 2>/dev/null) || :
kilobat_answer=$(printf '%s' "$kilobat_report" | /usr/bin/plutil -extract ok raw -o - - 2>/dev/null) || kilobat_answer=unknown
case "$kilobat_answer" in
    true) printf '%s\n' 'The connection check passed from this Mac.' ;;
    false) printf '%s\n' 'The connection check found a problem. Run kilobat why with the same site in Terminal for details.' ;;
    *) printf '%s\n' 'The check could not run. Check the hostname and your Kilobat CLI installation.' ;;
esac
```

Ask for a hostname, pass the answer **as arguments** to a Run Shell Script action using `/bin/sh`, and show its output with Show Result. A ready-to-import workflow is in `Workflow/Check a Site with Kilobat CLI.shortcut`; it is also available [via iCloud](https://www.icloud.com/shortcuts/44c8fb2634b548d8a35a4c24646f5d8d).

Requires macOS 14 or later, Homebrew and the separate Kilobat CLI (`brew install seifip/kilobat/kilobat`), plus **Allow Running Scripts** in Shortcuts settings. Enabling that setting permits scripting actions in other shortcuts too; inspect shortcuts before running them. The script looks only in the usual Apple Silicon and Intel Homebrew paths. It reports a summary, not a complete diagnosis; use `kilobat why` in Terminal for details. The check makes network requests to assess the entered host.

I am the maker of Kilobat. The CLI is open source under GPL-3.0; the separate desktop app is proprietary and is not required for this shortcut.
