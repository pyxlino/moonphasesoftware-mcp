# Moon Phase Software MCP app

See the Moon wherever you are.

Ask what the Moon looks like tonight or on any date, when the next full Moon is and what it is called, when the Moon rises where you are, which eclipses happen this year, or what sign the Moon is in. The app answers with the same calculations as moonphasesoftware.com, in your city or time zone, with a picture of the Moon.

- Website: https://moonphasesoftware.com
- Documentation: https://moonphasesoftware.com/app
- Privacy: https://moonphasesoftware.com/privacy
- Terms: https://moonphasesoftware.com/terms

This repository documents the hosted connector. It does not contain the
website or its code.

## Connect

- Endpoint: `https://moonphasesoftware.com/api/mcp`
- Transport: Streamable HTTP
- Authentication: none (no account, sign-in or API key)

```json
{ "mcpServers": { "moon-phase-software": { "url": "https://moonphasesoftware.com/api/mcp" } } }
```

In ChatGPT, add it as a custom MCP server with no authentication. In
Claude, open Customize, then Connectors, choose Add custom connector and enter the URL.

## Tools

All tools are read-only.

| Tool | What it does |
|---|---|
| `get_moon_phase` | Returns the Moon's phase, percent lit, lunar age and waxing or waning direction right now, at 12:00 on a date, or at a clock time on a date, in a time zone or city. |
| `get_moonrise_moonset` | Returns moonrise, moonset and the Moon's highest point on a local date for a city from the website's list of world cities, or for any latitude and longitude, with compass directions and the Moon's phase that day. |
| `find_full_moons` | Returns every full Moon of a calendar year with its date and time in a time zone, its traditional name such as Wolf Moon or Harvest Moon, its distance from Earth and whether it is a supermoon or a Blue Moon. |
| `get_moon_calendar` | Returns every day of a month with the Moon's phase and percent lit at 12:00 local time, and the exact times of that month's new Moon, first quarter, full Moon and last quarter in a time zone. |
| `list_eclipses` | Returns the lunar and solar eclipses of a calendar year with their type, the time of greatest eclipse in a time zone, the contact times of lunar eclipses, where solar eclipses are greatest and which of 16 major world cities see each one. |
| `get_moon_sign` | Returns the zodiac sign the Moon is in at a date and local time, in a time zone or city, with its degree in the sign and the next sign change. |
| `get_moon_distance` | Returns the Moon's distance from Earth in kilometres and miles at a date and time, its apparent width, the previous and next perigee and apogee, and the next full Moon's distance with whether that full Moon is a supermoon. |

## Try asking

- "What phase is the Moon on 25 December 2026 in Tokyo?"
- "When does the Moon rise and set in Chicago on 14 November 2026?"
- "List every full Moon of 2027 with its name."

## Report an issue

Open an issue in this repository or email support@moonphasesoftware.com.

## License

The documentation files in this repository are MIT licensed (see
[LICENSE](LICENSE)). The Moon Phase Software website, its content, data and brand are
not covered by this license.
