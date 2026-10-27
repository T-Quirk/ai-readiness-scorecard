# AI Readiness Scorecard — Precision Projects

A static scorecard page for qualifying workshop and podcast leads. It's hosted free on GitHub Pages and needs no form subscription.

- **Live:** https://t-quirk.github.io/ai-readiness-scorecard/
- **Workshop link / QR:** `?utm_source=workshop` (`qr-workshop.png`, `qr-workshop.svg`)
- **Per-host links:** add `?utm_source=<host>`, for example `aspe-gg`, `precon-pod`, `takeoff`, `aspe-dfw`, `flux`
- **Test mode:** add `test=1` to the link. It sends nothing and logs the outcome to the console.

## How it works

1. There are 10 questions. Nine are scored 0–3 (max 27). Q8, the systems question, isn't scored and is there for routing.
2. Knock-outs override the score: turnover under 2m, location "Other", or a sign-off answer of "Don't know".
3. Leads scoring 17+ with no knock-out are redirected to https://www.precisionproject.org/apply. Everyone else sees the nurture page, with three workflow tips.
4. Every submission is emailed to `info@precisionproject.org` via FormSubmit (free, no account). The email includes name, email, company, utm_source, score, outcome, knock-outs and every answer.
5. FormSubmit needs a one-time activation: the first submission sends a confirmation email to info@, and you click it once.

## Embed

```html
<iframe src="https://t-quirk.github.io/ai-readiness-scorecard/?utm_source=website" width="100%" height="2400" style="border:0;max-width:680px" title="AI Readiness Scorecard"></iframe>
```

When the page is embedded, the redirect for qualified leads opens /apply inside the iframe. For workshops, use the direct link or QR instead.

## Scoring (reconstructed 27 Oct 2026)

Grok's original spec never reached Claude. These point values were rebuilt from Grok's summary of the ten topics, max 27, book at 17+, plus the three knock-outs. Edit `QUESTIONS` in `index.html` to change them.
