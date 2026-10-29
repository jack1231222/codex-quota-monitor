# Privacy Notice

## Local quota

The application uses the locally installed Codex app-server and your existing Codex sign-in to read account rate limits. It stores derived quota snapshots, settings, public-source records, alert read state, and an optional API cost ledger in its own Application Support directory. Codex may contact its own service when answering a quota request. The application does not copy your Codex authentication data to its update or feedback services, modify conversations, or resume them. Coordination lock files protect quota reads during a compatible local account switch.

## Public sources and optional paid services

Free public-source checks contact public announcement, search, and source-verification services. They send public search terms and public post identifiers, not private conversation content. All network services receive ordinary connection metadata such as IP addresses.

Paid X search and AI analysis are disabled on first installation. They run only after manual actions and configuration. AI receives selected public posts and public documentation for analysis. API credentials are sent only to the corresponding configured API endpoint and are stored in a dedicated macOS Keychain service. Review provider terms and pricing before enabling requests. The app's cost ledger may contain actual, estimated, reserved, or unknown charges; it is not an official invoice.

Background receipt reconciliation retrieves existing responses; it does not generate a replacement response or replay a paid POST. Importing legacy records copies selected records and cost history, strips credential references, retains unknown costs, and leaves paid calls disabled. The original folder is kept.

## Updates and feedback

Sparkle checks the selected update feed hosted on GitHub Pages and downloads signed releases from GitHub. Automatic installation is disabled. Beta updates require opt-in. No separate product telemetry or marketing account is used. Feedback is voluntary; redact identifiers, paths, credentials, and private records before submitting it.
