# Journeyed MCP server: Los Angeles hotel facts

A remote [Model Context Protocol](https://modelcontextprotocol.io) server. No key, read-only.

[![smithery badge](https://smithery.ai/badge/luke-zsfm/journeyed)](https://smithery.ai/servers/luke-zsfm/journeyed)

On Smithery: https://smithery.ai/servers/luke-zsfm/journeyed

- Endpoint (streamable HTTP): `https://journeyed.org/mcp`
- Manifest: https://journeyed.org/.well-known/mcp.json
- Docs for agents: https://journeyed.org/agents/
- Official registry entry: `org.journeyed/hotels` (https://registry.modelcontextprotocol.io/v0/servers?search=journeyed)

## Tools
| Tool | What it returns |
|---|---|
| `answer_question` | Routes a plain question ("hotels near LAX with free parking") to the published page and returns its sourced answer |
| `get_hotel` | One hotel's fact sheet: every verified fact with source and checked date, score, class, awards, distances, what is not known |
| `search_hotels` | Hotels by name, former name, brand or city, optionally near a place |
| `hotels_near` | Ranked hotels near a landmark, venue, airport or neighborhood, optionally for a need (parking, pets, breakfast, kitchen, pool) |
| `best_hotels` | The published best-of list for a place or need, with the points each hotel earned and the formula |
| `get_report` | A data report about LA hotels as a whole: parking, resort fees, pets, check-in times, venues, what hotel websites leave out |
| `list_places` | The landmarks, venues, airports and neighborhoods covered |

Every fact names its source (the hotel's own website, an open place record, an awarding body's list) and the date it was checked.
No reviews, no room prices, no booking. Rankings come from published code; labelled sponsored placements never change a score, rank or tool result.

## Add it
Claude Desktop / Claude.ai custom connector, ChatGPT developer-mode connector, Cursor, Codex: add a remote MCP server with the URL `https://journeyed.org/mcp`.

Claude Code: `claude mcp add --transport http journeyed https://journeyed.org/mcp`

Operated by Cloute LLC. Terms: https://journeyed.org/terms/ · Privacy: https://journeyed.org/privacy/
