# SafeStart Cyber Workshop

An interactive, single-file cybersecurity incident-response workshop for small groups. Players role-play as incident responders at a fictional driving academy that has just been hit by ransomware. Over ~2 hours, they investigate emails, explore system logs, audit user accounts, reconstruct the attack timeline, and submit an incident-response plan.

## How to run

No build step, no server. Just open `index.html` in any modern browser.

To host it for multiple groups, drop the file on any static host (Netlify, GitHub Pages, S3, etc.).

## Logins

Valid credentials for groups and individual participants:

| Username                | Password      |
| ----------------------- | ------------- |
| `group1` – `group10`    | `SafeRoad1` – `SafeRoad10` |
| `employee1` – `employee10` | `SafeRoad1` – `SafeRoad10` |

(The number at the end of the username must match the number at the end of the password.)

## Workshop structure

1. **Ransomware screen** — sets the scene. A 2-hour countdown runs in the background.
2. **Incident Response Portal** — 5 tabs:
   - **Email Logs** — analyze every email; flag phishing vs. legitimate.
   - **Terminal** — read-only forensic snapshot with `ls`, `cd`, `cat`, `grep`.
   - **User Audit** — identify suspicious accounts among 17 employees.
   - **Timeline Builder** — drag 8 events into correct chronological order.
   - **IR Plan** — choose the best response plan from 4 options.
3. **Pop quizzes** — fire automatically after all emails are analyzed.
4. **Review questions** — gate the timeline results.
5. **Reflection questions** — graded.
6. **Results screen** — final score, rank, timeline review.
7. **Discussion prompts** — 4 open-ended questions for group debrief.

## Features

- Group progress is tracked in-memory; **Reset Progress** button wipes state.
- Live countdown timer visible in both the ransomware screen and portal header.
- Post-submission timeline review shows correct vs. placed events with dates.
- All answers are in the HTML source (single-file constraint). Light obfuscation could be added, but the workshop is designed to reward learning, not gate knowledge.

## Scoring (max 410 pts)

| Section | Max |
| --- | --- |
| Email Analysis | 95 |
| Pop Quizzes (x5, 15 pts each) | 75 |
| User Audit | 45 |
| Timeline Reconstruction | 50 |
| Incident Response Plan | 100 |
| Reflection Questions | 45 |
