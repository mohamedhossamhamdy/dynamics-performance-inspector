# Dynamics Performance Inspector

**Track the events. Find the bottlenecks. Understand the session.**

Dynamics Performance Inspector is a browser extension for investigating runtime performance in Microsoft Dynamics 365 and Dataverse model-driven apps.

It helps developers follow activity during a test session, inspect captured events, and review performance findings without manually piecing together every detail from separate browser tools.

> Independent community project. Not affiliated with or endorsed by Microsoft.

## Features

- **Live Monitor** — Observe captured UI activity, API calls, network events, JavaScript-related events, and errors during a recording.
- **Session Timeline** — Review the order of captured events across the investigation.
- **Performance Analysis** — Inspect slow events, repeated requests, and potential bottlenecks.
- **Diagnostics** — Review available capture and session information.
- **Exportable Reports** — Export captured session data in supported formats, including HTML, JSON, CSV, and TXT.

## Installation

This extension is distributed as a ZIP file and can be loaded locally in Microsoft Edge or Google Chrome.

1. Download the latest ZIP from the [Releases](../../releases) page.
2. Extract the ZIP file to a folder on your computer.
3. Open the extensions page in your browser:
   - Microsoft Edge: `edge://extensions`
   - Google Chrome: `chrome://extensions`
4. Enable **Developer mode**.
5. Select **Load unpacked**.
6. Choose the extracted extension folder containing `manifest.json`.
7. Open your Dynamics 365 or Dataverse environment and launch the extension.

## How to Use

1. Open the Dynamics 365 model-driven app you want to investigate.
2. Open **Dynamics Performance Inspector** from the browser toolbar.
3. Press **Record** to start capturing a session.
4. Reproduce the scenario you want to investigate, such as opening a form, changing tabs, or saving a record.
5. Press **Stop** when the test is complete.
6. Review the captured activity in Live Monitor, Timeline, and Analysis.
7. Export a report if you need to share or examine the findings further.

**Tip:** Start with a non-production or UAT environment when testing the extension.

## Compatibility

- Microsoft Edge
- Google Chrome
- Microsoft Dynamics 365 and Dataverse model-driven apps

The extension's host permissions may limit which environment URLs it can inspect. Check the manifest and release notes for the supported host patterns.

## Important Notes

- This tool is intended for client-side runtime investigation.
- It does not directly measure server-side plug-in execution time. Use server-side tracing or other diagnostic tools for that data.
- Captured data and exported reports may contain environment details or business information. Review and sanitize reports before sharing them.
- Performance findings are diagnostic clues, not guaranteed root-cause conclusions. Validate them against the application and its environment.

## Feedback and Contributions

Bug reports, feature requests, and suggestions are welcome.

When reporting an issue, include:
- Browser and version
- Dynamics environment type
- Steps to reproduce
- What you expected to happen
- What actually happened
- Relevant sanitized logs or screenshots

Do not include passwords, access tokens, personal data, or confidential production information.

## Author

**Created by Mohamed Hossam**

## License

Add a license before accepting contributions or redistributing modified versions.