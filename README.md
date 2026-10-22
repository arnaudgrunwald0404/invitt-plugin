# Invitt: event planning and invitations for your AI assistant

Invitt helps you plan an event and get people there, right from Claude, Cursor or any remote MCP client. Tell it about a team offsite, a client dinner, a customer evening at your shop, a dinner at home or a birthday. Invitt suggests places to host sized to your group, proposes an RSVP deadline and sets everything up, drawing on your past events for context. Then it emails the invitations and keeps everything on track, from the guest list and the vendors to the timeline and the reminders, so everything is ready, in place and on time. Nothing falls through the cracks. It's the easiest way to pull off a successful event.

Guests don't need an account or an app. Invitations go out by email or WhatsApp, and guests RSVP in one tap. Hosts can share the invite to WhatsApp after sending, and guests can opt in to WhatsApp reminders (coming soon).

**Connect URL:** `https://agent.invitt.net/mcp`

## Starter prompts
Once connected, your assistant shows these as one-click starters (slash commands or menu items, depending on the client):

| Prompt | What it does |
|---|---|
| `plan_an_event` | Start planning. Invitt asks one question at a time, starting with who it's for. Optional: `occasion`. |
| `invite_my_guests` | Collect the guest list and review the send summary before anything goes out. Optional: `event`. |
| `check_my_rsvps` | See who has replied and get one suggested next step. Optional: `event`. |
| `whats_left_to_do` | Get the top 3 things left to do for an event. Optional: `event`. |

## What you can ask
- "Help me plan a team offsite for 14 next month in Oakland: suggest a place and an RSVP deadline, then set it up."
- "We're hosting a customer evening at our shop on Nov 20. Suggest an RSVP deadline, then set it up."
- "Plan a client dinner for 8 near Union Square next Thursday and suggest three restaurants."
- "Set up a dinner at my place next Friday at 7 and give me an RSVP link for our WhatsApp group."
- "Plan my daughter's 7th birthday at a park near us on Saturday at 2pm, about 15 kids. Count kids and adults separately."
- "Who hasn't RSVP'd to the offsite yet? Remind them."

The agent always shows you what it's about to send and asks before anything goes out.

## Set up

### Cursor (one click)
[Add to Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=invitt&config=eyJ1cmwiOiJodHRwczovL2FnZW50Lmludml0dC5uZXQvbWNwIn0=), then sign in to Invitt when Cursor prompts you.

Or add this to `~/.cursor/mcp.json`:
```json
{ "mcpServers": { "invitt": { "url": "https://agent.invitt.net/mcp" } } }
```

### Claude.ai
Open Settings, then Connectors, and add a custom connector. Paste `https://agent.invitt.net/mcp` and sign in to Invitt.

### Claude Code
```bash
claude mcp add --transport http invitt https://agent.invitt.net/mcp
```
Then run `/mcp` and sign in.

### Grok Bot and Muse
Add a custom connector with `https://agent.invitt.net/mcp`, then sign in to Invitt.

### Any other remote MCP client
Point it at `https://agent.invitt.net/mcp`. Sign-in uses standard OAuth with an email link, no password.

## What's included
**Plan:** venue ideas near you sized to your group, a suggested RSVP deadline, your past events for context, and creating and updating events as plans change.

**Invite and follow up:** add guests, invitations by email or WhatsApp after you confirm, one RSVP link for any group chat, RSVP status and headcounts (adults and kids), and reminders to people who haven't replied. Hosts can share the invite to WhatsApp after sending, and guests can opt in to WhatsApp reminders (coming soon).

## Pricing
Invitt is free during launch.

## Links
- Website: https://invitt.net
- Docs: https://invitt.net/docs
- Support: support@invitt.net
- Privacy: https://invitt.net/privacy · Terms: https://invitt.net/terms

This repo holds the listing, setup docs and plugin manifest only. Invitt's server runs at `agent.invitt.net`.

## License
MIT (covers this repo's docs and manifest only).
