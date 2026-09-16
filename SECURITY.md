# Security Policy

## Supported versions

MarkPad++ is distributed through the Microsoft Store, which delivers updates
automatically. Only the latest version available in the Store is supported.

| Version | Supported |
| --- | --- |
| 1.0.3 (current) | Yes |
| Older versions | No — please update through the Microsoft Store |

## Reporting a vulnerability

Please report security vulnerabilities **privately**, not in public issues.

- Preferred: use GitHub's private vulnerability reporting for this repository
  (the **Security** tab → **Report a vulnerability**).

<!-- TODO: add a dedicated security contact email if you want one published here, instead of relying only on GitHub private reporting. -->

Please include:

- The MarkPad++ version and your Windows version.
- A description of the issue and its potential impact.
- Steps to reproduce, and a sample file if relevant.

You will receive a response acknowledging the report. Please give a reasonable
amount of time for the issue to be addressed before any public disclosure.

## Scope and context

MarkPad++ works entirely offline, requires no account, and sends no telemetry, so
it has no server-side or network component to attack. Reports most relevant to
this application include issues such as unsafe handling of file input, or problems
in how documents are parsed, rendered or exported.
