# Windows Program Standard

Whenever the user requests a Windows program, deliver a real standalone portable Windows GUI `.exe`, not a .bat, Python launcher or only source code.

- Embed a real application-specific Windows icon in PE resources and set titlebar, taskbar and Alt+Tab icons.
- Put a small N8 symbol and an **Install Updates** control in the lower-right of the window, with truthful availability notifications.
- Test the PE architecture and resource, and smoke-test on Windows whenever possible.
- Never represent an update URL opener as a verified self-installer. Require authentic release signatures/checksums for installing updates.
- Prefer one tested build artifact and no additional runtimes; preserve features, data and settings.
- Do not call an incomplete dashboard shell a complete application. List every unimplemented integration accurately.
