# Win11-Copilot-App-Debloat #

This .reg file disables Copilot UI integrations and various AI features across the system and apps like Paint, Snipping Tool, and Windows Search. This will not uninstall the apps but will turn off Copilot and AI integrations wherever possible, including the taskbar button and Bing in Search.

It achieves automation of:

- Removing taskbar Copilot
- Stripping AI features from Paint, Snipping Tool, etc.
- Blocking Bing/Copilot integrations in Search
- Disabling AI popups in Edge (if installed)

Currently, Notepad is the only major built-in app where Microsoft has not provided any official or unofficial way to disable or remove Copilot integrations (like “Explain with Copilot”) without uninstalling the app entirely.

# CAUTION This will uninstall Notepad entirely. Find an older version online or use something like Notepad++ that has no baked-in AI features.

If you want to proceed, open Powershell as admin and run the following command:

Get-AppxPackage *Microsoft.WindowsNotepad* | Remove-AppxPackage
