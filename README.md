# loon-lounge-voice-agent
A working ElevenLabs Conversational AI agent built for The Loon Lounge, a three-property lakefront rental business on Green Lake, Maine, that I run. The agent handles booking inquiries, answers questions about the three houses, and gives local recommendations for the Acadia area.

## Why I built this

Voice carries trust signals that text can't: inflection, pacing, pauses. For a business, that's not one-size-fits-all. A lakefront rental with three distinct houses, real accessibility differences between them, and a,protective privacy boundary around guest information needs an agent that gets the specific facts right, not a generic FAQ bot.

Building this surfaced the actual hard part of voice AI for a business: not the voice quality, but making sure the agent won't confidently state
something wrong. An early test had the agent claim a house slept more people than its beds allow. Fixing that meant building an exact capacity table and a rule against rounding up, not just a better prompt.

## What's here

- `system-prompt.md`: the agent's full instructions, covering booking
  flow, house-by-house facts, capacity rules, and a privacy boundary for
  guest data
- `knowledge-base.md`: the uploaded local-recommendation knowledge base,
  with sourcing and safety rules for area activities
