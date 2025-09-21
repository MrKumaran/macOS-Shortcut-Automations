# **Prompt Templates for macOS Shortcuts Automation**

## **Purpose**

These prompt templates help users ask AI tools (like ChatGPT) to create automation scripts or workflows using the **Shortcuts app on macOS**.

> **Follow [contribution.md](../CONTRIBUTING.md)** to add more prompts!

---

## 1. Auto Organize Downloads Folder by File Type

**Prompt:**

```
Create a macOS Shortcut workflow that organizes files in the Downloads folder by file type (e.g., images to "Images", PDFs to "Documents", ZIPs to "Archives"). Move them into appropriate folders. It should run every 2 hours or on demand.
```

---

## 2. Mute System Volume During Work Hours

**Prompt:**

```
Create a macOS Shortcut to mute system volume from 9 AM to 5 PM on weekdays automatically. Use built-in system controls or terminal commands.
```

---

## 3. Batch Rename Screenshots on Desktop

**Prompt:**

```
Create a macOS Shortcut that finds all screenshots on the Desktop, renames them to include date format (e.g., Screenshot-2025-06-17), and moves them into a folder named "Screenshots".
```

---

## 4. Set Focus Mode and Launch Apps

**Prompt:**

```
Create a macOS Shortcut that turns on Focus Mode, opens Visual Studio Code, Safari, and Spotify, and switches to Do Not Disturb for 2 hours.
```

---

## 5. Run Homebrew Update Commands

**Prompt:**

```
Write a shell script to run 'brew update', 'brew upgrade', and 'brew cleanup', and integrate it into a macOS Shortcut. It should be one-click and show output once done.
```

---

## 6. Auto-Connect to VPN on Public Wi-Fi

**Prompt:**

```
Create a Shortcut that detects if the current Wi-Fi name is not "HomeWiFi", then automatically connects to a specified VPN app or triggers a shell script to connect.
```

---

## 7. Start Work Session Timer with Notification

**Prompt:**

```
Create a Shortcut that starts a 25-minute Pomodoro timer, sends a notification saying "Focus Time Started", and silences notifications.
```

## 8. Real-time File Organizer Based on File Type

**Prompt:**

```
Create a macOS Shortcut workflow that organizes files in the Downloads folder based on their file type.
Each file type should go into its matching folder (e.g., Images → "Pictures", PDFs → "Documents").

Then, provide Automator instructions to trigger this Shortcut automatically whenever a new file is added to Downloads.

Output the shell script if needed, the shortcut steps, and Automator setup steps.
```

