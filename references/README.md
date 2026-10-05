# References

These folders are git submodules. They are pinned checkouts, not our code.

- `osTicket` at `8d38b06`, GPL-2.0. Ticket spine. Run separately. Do not import into the Next.js app.
- `osTicket-plugins` at `67a1450`, GPL-2.0. Auth and storage only.
- `OpenFieldService` at `c90c60d`, MIT. Calendar and job patterns. Copyright notice stays if any piece is reused.

FullCalendar, Medusa and Vendure stay as npm or a later choice. They are not submodules.

AGPL repos are not attached. See `notes/REPOS.md`.

Clone with the pins:

```
git clone --recurse-submodules https://github.com/GoodLordFjord/Spraybooth-inc.git
```
