# kairoscc.io website

Static site for **Kairos Consulting Collective, LLC**, served by GitHub Pages.

## Page hierarchy
| Path | Page |
|---|---|
| `/` | Company: who we are, what we do, products, contact |
| `/data-systems/` | Kairos Data Systems: the Universal Lakehouse Factory and pricing |
| `/data-systems/small-team/` | Small Team Edition spec and **Paddle checkout** |
| `/data-systems/developer/` | Developer tier spec |
| `/rackside/` | Rackside app: features, free and Pro, support |
| `/legal/terms`, `/legal/privacy`, `/legal/refund`, `/legal/eula` | Legal pages (paths kept stable: Paddle has them on file) |
| `/small-team/`, `/developer/` | Redirects to the pages above, kept for old links |

## Integrations: don't break these
- **Paddle checkout** (`/data-systems/small-team/`): the live client token, `priceId` and `customData.github_username` must not change. Make.com reads `github_username` from Paddle's webhook to send the GitHub invite.
- **Paddle approved domains:** checkout only works on domains approved in Paddle (Checkout settings). Add a new domain there *before* the site moves to it.
- **Make.com** runs off Paddle's webhook, not this site, so page paths don't affect it.
- **Legal paths** stay at `/legal/*`.
