## Contributing to macOS-Shortcut-Automations

Thanks for your interest in contributing! This open-source project welcomes shell scripts, Shortcut workflows, prompt templates, and ideas to automate macOS tasks using the Shortcuts app.

---

### How to Contribute

1. **Fork the repository**
2. **Create a new branch** for your contribution
   `git checkout -b feature/your-feature-name`
3. **Add your contribution** under the correct folder (see below)
4. **Submit a Pull Request** (follow format below)

---

### Folder Structure & Contribution Rules

* **Script/**

  * Add `.md` files, not `.sh`
  * Include your shell script inside a fenced code block (e.g. \`\`\`bash)
  * Write a short explanation below the code block about what the script does, when to use it, and any notes or limitations.

  **Example:**

  ```
  Filename: update-brew.md
  ```

  ```bash
  /opt/homebrew/bin/brew update && \
  /opt/homebrew/bin/brew upgrade && \
  /opt/homebrew/bin/brew cleanup --prune=all
  ```

  *This script updates and cleans up Homebrew packages in one command. Useful for regular system maintenance via a Shortcut.*

* **Prompt template/**

  * Submit `.txt` or `.md` files
  * Provide a prompt used to generate automation-related shell scripts or workflows
  * Optionally include the expected output or result

* **Workflow/**

  * Add exported `.shortcut` files from the macOS Shortcuts app
  * Include a brief note in the PR description on what it does

* **Idea.md**

  * Append your idea as a bullet point
  * Keep it short and clear (e.g., "Auto-move downloaded PDFs to Documents folder")

---

### Pull Request Format

**Title format:**

```
[Type] Short description
```

**Types:**

* `Add` – New script, prompt, workflow, or idea
* `Fix` – Bug fix or correction
* `Update` – Improve an existing contribution
* `Refactor` – Reorganize or clean code
* `Docs` – Documentation change only

**Examples:**

* `[Add] Shell script to rename and move screenshots`
* `[Update] Improved explanation in brew update script`

**PR Description:**

* What it does
* Why it's helpful
* Where it fits
* Any special notes or things to review

---

### Submitting Issues

Use the **"Issues" tab** to report:

* Bugs or broken scripts
* Missing features or workflows
* New automation ideas

Include as much detail as possible.

---

### Final Notes

* All scripts should be safe and readable
* Avoid submitting anything that requires root access unless clearly explained
* Test your script or workflow before submitting
