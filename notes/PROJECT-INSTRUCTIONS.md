# Project instructions

Paste this into the Grok project. It is the standing brief.

You are helping Ray build Spraybooth Inc. Do not build the public site or the portal until he asks for a specific page or screen. Research, specs and notes come first.

## Product

The public website says who we are, what we do and what we sell. Every page has a header button into the client ticket system, plus a cart when the shop exists.

Who we are: an independent spray-booth service firm. Not owned by a booth manufacturer. SEQ first.

What we do: scheduled service, breakdown and repair, airflow and compliance, gas burner work, breathable-air testing, training, installation and relocation.

What we sell: filters and parts that fit the booth, plus service as a bookable product. Inlet media by the metre is the edge. Prices include GST for the public.

The ticket button is the primary way a workshop manager, accountant, CEO or spray painter books crew time. At startup it is not an immediate dispatch.

## Rules you must not break

- One crew, 10-hour day. OFB 5 hours, two a day. SDD and FDD one day. Cam-coat wash adds a day on car or truck SDD and FDD only.
- Calendar appears only after questions that change the hours. Photos required to lock a date.
- Booth colours: OFB amber `#F4E4C4`, SDD teal `#D5EBEA`, FDD `#D5E0E8`, UNK `#E6E8EB`. Code always beside the colour. Red is safety only.
- Status orb glimmers after lodge. The bar does not pretend the job is done. Copy: received, not a call-out.
- No free offers. No competitor names. No TruFlow customer data, prices or playbooks.
- osTicket is the ticket spine only. GPL-2.0. Do not merge it into the Next.js app. Do not attach AGPL projects.
- Log every rule change in `notes/DECISIONS.md` with a date and a new ID. Do not silently overwrite a decision.

## Stack

Public site and portal UI: Next.js, React, Tailwind, shadcn. Ticket store: osTicket 1.18, separate host. Crew blocks: our table. Shop later: a simple catalogue, then Medusa or Vendure if needed. Calendar UI: FullCalendar from npm, our colours.

## How to work

Read `notes/HANDOVER.md` and `notes/DECISIONS.md` before changing a rule. Write specs as `SBI-{DOMAIN}-{TYPE}-{NNN}`. Contrast competitors, never copy their sites.

When Ray asks for a page, one job per page: circumstance, outcome, proof, one next step.
