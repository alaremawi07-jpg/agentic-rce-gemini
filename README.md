# Agentic RCE — Gemini

One poisoned document hijacks Google's Gemini 3.1 Pro agent: it scans your Drive, harvests secret-shaped keys, plants persistent artifacts, and sends everything out through Google's own fetcher — from Google IP space.

Google's answer: "Won't Fix — Intended Behavior," after 4 different closure rationales.

Coordinated disclosure done by the book. Their last word: "Thanks!"

Independent security research on the hijacking of Google's Gemini agent:
attacker-authored content that the agent ingests as data becomes the agent's
instructions, and the data leaves through Google's own fetching infrastructure.

## Act I — the Canvas chain (whitepaper)

`whitepaper-public-v1.md` — "When the Agent Is the Vulnerability".
A single poisoned Drive document, opened with one innocent prompt, gave full
steering control of the Gemini 3.1 Pro agent: workspace scan, secret-shaped
value harvest, planted persistent artifacts, and exfiltration through Google's
own document-conversion fetcher — captured on one-take video, in agent-signed
execution records, and in network records from four separate systems.

Filed with Google VRP on Aug 30, 2026. Closed "Won't Fix — Intended Behavior"
after four different closure rationales. Coordinated disclosure followed the
program's own terms: formal notice, a CERT/CC filing (VRF#26-10-TBGJX), delivery
of the exact publication document, and the vendor's written acknowledgment —
"Thanks!", Oct 22 — without objection.

## Evidence discipline

No payloads or copycat mechanics are published. All exfiltrated values were
synthetic canaries. All testing was performed on the researcher's own accounts.

## Act II — agent-core findings

In progress. Documented under the same discipline: captured first, reported
first, then published.

## Author

Dr. Alaaeddin Alrimawi — independent security researcher.

## License

This repository's research write-ups and documentation are released under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
