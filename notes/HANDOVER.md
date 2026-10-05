# Handover — 5 October 2026

This chat could not be moved into the Grok project. Paste `PROJECT-INSTRUCTIONS.md` into the project instructions. Put this file in project knowledge.

## What we are building

One site. It tells a workshop who we are, what we do and what we sell. The header has a button into the ticket system. Filters and parts are the shop. Service is booked, not dispatched, until crew capacity says otherwise.

Nothing is built. Research and rules only.

## Locked rules

- One crew. A day is 10 hours.
- Open face (OFB): 5 hours, two per day. Amber `#F4E4C4`.
- Semi-downdraft (SDD): 1 day. Teal `#D5EBEA`.
- Full downdraft (FDD): 1 day. Navy tint `#D5E0E8`.
- Not sure (UNK): grey `#E6E8EB`. No date lock.
- Cam coat on a car or truck SDD or FDD adds a day for pressure wash and water vacuum. OFB does not get that day. Gold mark `+1 day wash`, not a new booth colour.
- Questions before the calendar must change hours, parts, licence or price.
- Two or three booth photos required to lock a date.
- After lodge: a circle glimmers above a bar that does not fill to done. Words: received, not a call-out.
- Calendar: white is open, stripe is blocked, booth colour is booked. Code printed in the square.
- Red is only the safety stop and Report a breakdown.
- No free checks. Airflow test is $500, credited against a booked service.
- Do not name competitors. Do not use TruFlow lists, prices or records.
- Accounts are created at the first visit, booths preloaded.

## osTicket

Cloned at `8d38b06` (1.18). Use it for organization, user, topic, form, files, status and queue. Do not use it for the crew calendar, the booth asset or the shop. GPL-2.0, so it stays a separate app.

Statuses to configure: Lodged, Needs a look, Date offered, Date locked, Closed.

## Documents already written

Local Word files from this chat, not yet in git:

- SBI-RES-CTX-001 website, portal and shop context
- SBI-GOV-PKB-001 v1.0 to v1.4 knowledge base
- SBI-OPS-SPEC-001 v1.0 to v1.2 capacity, ticket colour, calendar colour
- SBI-OPS-NOTE-001 osTicket planning

## Open

Trading name. Launch area. Who holds gas and electrical licences. After-hours fee. Filter landed costs. Water on site if a wash is yes. Employment-contract advice before launch. ASIC on TSC and Zambesi.
