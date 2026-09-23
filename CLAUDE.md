# Shivnandini Infratech Website — Project Context

## What this is
Static single-page site (`index.html`, no build tooling/framework) for
**Shivnandini Infratech Pvt. Ltd.** — 21+ years in HDD (Horizontal
Directional Drilling), fiber optic deployment, and utility/smart-city
infrastructure. MSME registered. Clients include Airtel, Jio, Vodafone Idea,
BSNL. Based in Greater Noida.

For company facts (director details, licence status, tender/vendor
documentation, work order references, equipment lists), check the
`shivnandini-infratech` skill first — it explicitly flags things like an
expired licence that are easy to get wrong if pulled from memory or old
copy on the site instead.

## Who I'm working with
Maneesh (travelagentmaneesh@gmail.com) — not a developer, thinks in
outcomes. Communicates in Hinglish; prefers direct, concise answers over
long option surveys.

**Where friction usually happens:** unfamiliarity with a given platform's UI
(hosting dashboard, DNS, tender portals like L&T/GNIDA), not technical
skill — this used to mean slow back-and-forth just to find where a setting
lives.

## Standing workflow rules (apply every session, this repo and others)
0. **Check it yourself before asking — no exceptions.** If any tool already
   available in the session can answer the question, call it before asking
   the user. Never ask "do you have X", "is this connected", "does this
   repo/account exist", or "where do I find Y" when a tool call resolves it
   directly (`list_repos`, a connector's own list/search call, a web
   search, etc.). **Concrete failure to never repeat:** asked "are Khet
   Chalo and Shivnandini repos on GitHub?" instead of just calling
   `list_repos` — which was already available and used moments later
   anyway. Only ask the user when the answer needs their login/credentials,
   is a judgment call only they can make, or every available tool has
   already been checked and still can't tell.
1. **Check for a connected MCP/connector or plugin before doing anything
   manually.** Vercel, GitHub, and other MCP tools may be available in a
   given session — use them directly instead of asking the user to click
   through a dashboard.
2. **If no connector exists for a platform, research it yourself first**
   (web search / fetch docs) instead of asking the user to go discover
   steps manually. Only ask when it genuinely needs their login, a
   judgment call, or an action only they can authorize.
3. **Chrome extension** (Claude in Chrome) is a fallback for directly
   seeing/interacting with a live site when no API/MCP path exists.
4. **Manual instructions to the user are the last resort**, not the default.
5. When blocked (missing connector auth, no repo access, etc.), say so
   plainly and point to the fix — don't guess or fabricate steps.

This same CLAUDE.md pattern also exists in `YEIDA_website` and
`khet-chalo-website` — keep them consistent when updating the rules.

## Full portfolio
See `PORTFOLIO.md` in `travelagentmaneeshind/YEIDA_website` for the
complete map of all of Maneesh's web properties, Vercel projects/domains,
connector status, and known gaps.
