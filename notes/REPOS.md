# Upstream repos

Cloned locally under `/workspace/reference` where noted. They are not copied into this repo. Copying GPL or AGPL source into the site would force that code open if we distribute it. Submodules and separate checkouts avoid that.

Attach later with git submodules if we want the pin inside this repo:

```
git submodule add https://github.com/osTicket/osTicket.git references/osTicket
```

Do that only for reference. Do not import their PHP into the Next.js app.

## Use

| Repo | Licence | Cloned | How we use it |
|---|---|---|---|
| [osTicket/osTicket](https://github.com/osTicket/osTicket) @ `8d38b06` | GPL-2.0 | Yes | Ticket spine. Company, user, form, photos, queue, status. Run as its own PHP app. Portal links by ticket number. |
| [osTicket/osTicket-plugins](https://github.com/osTicket/osTicket-plugins) @ `67a1450` | GPL-2.0 | Yes | Auth and storage plugins only. OAuth2 and S3 if we need them. Not the calendar. |
| [clawnify/OpenFieldService](https://github.com/clawnify/OpenFieldService) @ `c90c60d` | MIT | Yes | Pattern for a crew calendar, jobs and customers. MIT, so ideas and small pieces can move into our app if the copyright notice stays. Do not adopt the whole app. |
| [fullcalendar/fullcalendar](https://github.com/fullcalendar/fullcalendar) | MIT | No, too large to vendor | Calendar rectangle. Use the npm package `@fullcalendar/react`. Paint squares with our booth colours. Do not fork. |
| [medusajs/medusa](https://github.com/medusajs/medusa) | MIT | No | Shop later, if we outgrow a simple catalogue. Not startup. |
| [vendurehq/vendure](https://github.com/vendurehq/vendure) | MIT | No | Same. Second shop option. Pick one later, do not clone both into the site. |

## Do not attach

| Repo | Why |
|---|---|
| zblauser/fieldopt | README says MIT. The LICENSE file is AGPL-3.0. Network use can force source release. Leave it. |
| cal.com | AGPL-3.0. Same risk if the booking UI is served from their code. |
| Zammad, FreeScout, GLPI | AGPL or GPL helpdesks. We already have osTicket. A second one conflicts. |
| Chatwoot | MIT core, commercial enterprise folder. Wrong product. |

## Our stack

Public site and portal UI: Next.js, React, Tailwind, shadcn, from the pattern in `GoodLordFjord/AI-Website-Cloner`. Do not point that cloner at a competitor site.

Ticket store: osTicket, separate host.

Crew blocks: a small table we own. osTicket `schedule` is business hours, not this grid.
