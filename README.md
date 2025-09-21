# macOS-Shortcut-Automations

A collection of workflows, shell scripts, and prompt templates to automate repetitive tasks on macOS using the **Shortcuts app** and command-line tools.

## Overview

This open-source project helps you streamline your daily macOS tasks with custom Shortcuts, shell scripts, and prompt templates. Whether you're organizing files, updating software, or triggering actions with input, this repo has building blocks to get you started.

> [!NOTE]
> macOS 26 has updated some UI elements, so the “Pin on Menu” option is no longer available inside the Shortcuts app. Instead, it can be found in the Control Center:
> * Click the Control Center button in the menu bar → Edit Controls → select Shortcut and add it to the menu bar.
> * Here, you have two options: either set the shortcut icon to show a dropdown of all available shortcuts, or pin a specific shortcut directly.

## Repository Structure

```
│── Prompt template/   # Prompt templates for generating scripts or workflows
│── Script/            # Shell scripts used inside Shortcuts
├── Workflow/          # Ready-to-use Shortcut workflows
├── CONTRIBUTING.md    # Contributing guidelines
├── Idea.md            # List of automation ideas and notes
│── LICENSE
└── README.md
```

### Directory Details

* **Script/** – Contains shell scripts for actions like updating packages, renaming files, etc.
* **Prompt template/** – Contains AI prompts to help you generate or improve scripts and workflows.
* **Workflow/** – Includes exported Shortcuts (.shortcut files) ready to import into the Shortcuts app.
* **Idea.md** – Brainstormed automation ideas that can be implemented using Shortcuts or shell scripts.

## Example Use Cases

* One-click Homebrew update
* Auto-renaming and moving screenshots
* Uninstall Homebrew packages via input prompt
* Schedule or trigger actions using Automator + Shortcuts
* Run shell scripts via Shortcut with real-time output

## Contribute

This project is open to contributions!

* Submit a **Pull Request** with new scripts, prompt templates, or workflows.
* Improve or optimize existing ones.
* Add new ideas to `Idea.md`.

Whether you're scripting for the first time or building advanced workflows—your contribution is welcome.
**Please read the [`CONTRIBUTING.md`](CONTRIBUTING.md) file before starting to understand the guidelines.**

## Learn More

Read the guide: [macOS Automations Using Shortcut](https://medium.com/@kumaran-s/macos-automations-using-shortcut-f8e19e41bc07)

## License

This project is licensed under the [MIT License](LICENSE).
