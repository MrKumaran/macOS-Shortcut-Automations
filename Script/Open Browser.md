# **Open Browser Script**

## **Purpose**

This script is designed to be used inside the **macOS Shortcuts app** using the “Run Shell Script” action. It opens a
selected browser and loads a specific URL.

---

## **Script**

```bash
# Set the browser command
# Options: google-chrome, firefox, brave-browser, microsoft-edge, Safari (use open -a Safari)
BROWSER="open -a 'Google Chrome'"  # For Safari: open -a Safari

# Set the URL
URL="https://www.google.com" # for automation try to get url/searchkey as input and pass it to here.

# Open the URL in the selected browser
$BROWSER "$URL"
```

---

## **How to Use in Shortcuts App**

1. Open the **Shortcuts** app on macOS.
2. Create a new shortcut.
3. Add the action: **Run Shell Script**.
4. Paste the above script into the shell input box.
5. Leave **Input** and **Shell** as default unless needed.
6. Optionally, enable **“Pin in Menu Bar”** for quick access.

For a full beginner-friendly guide on using macOS Shortcuts with
scripts, [read this article](https://kumaran-s.medium.com/macos-automations-using-shortcut-f8e19e41bc07).

---

## **Supported Browsers on macOS**

| Browser        | Command Example            |
|----------------|----------------------------|
| Google Chrome  | `open -a 'Google Chrome'`  |
| Safari         | `open -a Safari`           |
| Firefox        | `open -a Firefox`          |
| Brave          | `open -a 'Brave Browser'`  |
| Microsoft Edge | `open -a 'Microsoft Edge'` |

> **Note**: App name must match exactly with the name in the **Applications** folder.