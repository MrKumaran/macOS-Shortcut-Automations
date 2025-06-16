# **Start Docker Daemon Script (macOS Shortcuts)**

## **Purpose**

This script starts the Docker daemon using the Docker Desktop app on macOS.

---

## **Script**

```bash
# Start Docker Desktop (starts the daemon in macOS)
open -a "Docker"
```

---

## **How to Use in Shortcuts App**

1. Open the **Shortcuts** app.
2. Create a new shortcut.
3. Add the action: **Run Shell Script**.
4. Paste the script above.
5. Optional: Check “Runs with administrator privileges” if needed.
6. Pin to the menu bar for quick access.

👉 Full shortcut guide here: [macOS Automations Using Shortcuts](https://kumaran-s.medium.com/macos-automations-using-shortcut-f8e19e41bc07)

---

## **Note**

* Docker Desktop must be installed.
* This only **starts Docker**, it doesn’t verify readiness. Docker may take a few seconds to become fully available.