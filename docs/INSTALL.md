# Installation and first use

1. Download the Apple Silicon DMG from this repository's Releases page.
2. Open the DMG and drag Codex Quota Monitor to Applications. Eject the disk image and open the installed app.
3. Install Codex from its official source and sign in to Codex. The quota app reuses that local session; it does not ask for your Codex password.
4. The app discovers Codex in Applications or your existing CLI path. If you use a different Codex data folder, choose **Choose Codex Data Folder** in the application menu, then reopen.
5. Open the menu bar item or the full panel. Failed or stale readings remain labeled; public posts are not account quota evidence.

Choose English or Simplified Chinese from **Language** or Settings and reopen the app. Public-source checks and local quota checks use separate schedules. Closing the panel leaves the menu bar app running; Quit stops its workers. **Open at Login** is optional.

Paid queries are optional. Configure provider keys and current pricing in Settings before enabling them. A model-list connection check does not generate analysis. A paid analysis test requires its own confirmation. Budget settings are app-side safeguards, not provider-enforced spending caps; the optional record-only policy does not block spending.

## Legacy import

Choose **Import Legacy Records**, select the old CodexResetForecast data folder, and follow the result. Import uses a fresh destination, retains the original, preserves cost types and unknown amounts, and strips credential references. Reconfigure credentials after import. It does not resubmit old paid requests. Keep the old app closed if you no longer want it to keep monitoring; the new product does not remove it automatically.

## Updates and uninstall

Use **Check for Updates**. **Receive Beta Updates** is an explicit opt-in; automatic installation is off. Keep Gatekeeper enabled; do not remove quarantine flags to install this app.

To uninstall, disable Open at Login, quit the app, and move the application to Trash. Application data and Keychain entries remain unless you explicitly remove them. The app does not install the older product's LaunchAgents.
