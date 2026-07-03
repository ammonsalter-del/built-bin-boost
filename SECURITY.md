# Security Policy

## Overview

Build, Bin, Boost is a client-side educational game. It is a single HTML file that runs entirely in the browser: no accounts, no logins, no server-side components, and no personal data collected through gameplay. Game state exists only in the player's browser.

## Data Handling

- Gameplay involves no accounts, no authentication, and no transmission of game data to any server (there are none)
- The in-game AI advisor, Devi, is fully scripted within the game file — it makes no calls to any external AI service
- Game progress and settings are stored locally in the browser only

## Analytics (opt-in only)

The game includes Google Analytics for anonymous usage counting, and it is **off by default**:

- No analytics code loads until the player explicitly consents via the cookie banner
- Declining leaves the game fully functional, with no tracking of any kind
- Consent can be reviewed and withdrawn at any time in "About This Game"
- If consent is granted, standard Google Analytics processing applies (see Google's privacy documentation)

## For University IT and Data Protection Teams

- **No personal data is processed through gameplay.** No names, emails, student numbers, or accounts.
- **Analytics is strictly consent-based.** Nothing loads before an explicit opt-in, which satisfies the ePrivacy consent requirement; students who decline are not tracked at all.
- **No integration with university systems.** No LMS, no authentication, no licences. Students open a web page.
- **Fully auditable.** The complete source code, including the consent gate, is public in this repository.
- **Offline option.** The HTML file can be downloaded and run locally or from institutional servers, with no network activity beyond font loading, which also disables analytics entirely.

In our assessment no DPIA is required for classroom use; institutions applying their own thresholds are welcome to contact us.

## Third-Party Resources

The game loads the following external resources:
- Google Fonts (fonts.googleapis.com)
- Creative Commons licence button images (licensebuttons.net)
- Google Analytics (googletagmanager.com) — only after explicit consent, as above

Users concerned about external dependencies can review the source code and host their own copies.

## Reporting a Vulnerability

If you discover a security issue — for example a cross-site scripting vulnerability, or a problem with how external content is loaded — please report it responsibly.

**Email**: ammon.salter@wbs.ac.uk

Please include a description of the vulnerability, steps to reproduce it, and the potential impact. Do not open a public issue for security vulnerabilities. We will acknowledge receipt within 7 days and aim to address confirmed vulnerabilities promptly.

## What This Policy Does Not Cover

- Vulnerabilities in browsers, operating systems, or third-party services (GitHub Pages, Google, CDNs)
- Issues arising from user modifications to the source code
- Gameplay bugs (please use the bug report issue template for those)

Thank you for helping keep this project safe.
