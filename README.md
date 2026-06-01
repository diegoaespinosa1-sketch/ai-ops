# Diego Espinosa | AI Ops

**Grok-powered agents that create real operational leverage.**

This is the landing page for Diego Espinosa's AI Operations consulting — helping technical teams and founders reclaim 20+ hours per week with custom-built Grok agents.

## Positioning

- **Voice**: Sharp, no-fluff, battle-tested. "Borrowed time" mindset.
- **Promise**: Measurable time back. Zero theater.
- **Primary CTA**: DM on X (@DiegoEspinosaAI)
- **Complements**: [sarka-ops.com](https://sarka-ops.com) — the human ops excellence layer (Šárka Espinosa).

## Tech

- Single-file `index.html`
- Tailwind via CDN (zero dependencies, instant preview + deployment)
- Font Awesome icons
- Pure vanilla JS for interactions
- Extremely fast and easy to edit

This stack is intentional: maximum velocity, zero maintenance burden, beautiful results.

## Quick Start

1. Open `index.html` directly in any browser.
2. Edit copy, colors, or sections directly in the file.
3. When ready, deploy anywhere that serves static files.

## Customization Points

Look for these easy-to-edit areas in `index.html` (search for the text or IDs):

| Area                  | What to change                          | Notes |
|-----------------------|-----------------------------------------|-------|
| Hero hook             | Search for "I build Grok agents"        | Keep it lethal |
| Metrics / Proof       | Search for "COLD HARD RESULTS"          | Update with real wins when you have them |
| Signature Systems     | Search for "Signature systems" or the 4 agent cards | The 4 agent cards — your actual offers |
| About / Borrowed Time | Search for "The Difference" or "I don't have time" | The "borrowed time" story |
| Contact form          | Search for `id="contact-form"`          | Update Formspree endpoint + fields |
| CTAs                  | Multiple (X is primary)                 | All point to X currently |
| Accent color          | `#67e8f9` (cyan)                        | Search/replace if you want a different accent |
| og:url + title        | `<head>` section (already set to ai.sarka-ops.com) | Only change if you switch domains |

## Deployment — Vercel + ai.sarka-ops.com (Current Target)

> **Note**: You are currently using Netlify DNS (nameservers). This guide covers the quick way to point the subdomain while staying on Netlify DNS. A cleaner long-term setup (moving DNS to Cloudflare) is documented later in this file.

### 1. Push to GitHub (Recommended path)

Run these commands one by one:

```bash
cd ~/ai-ops

# Initialize git
git init

# Add all files
git add .

# Create first commit
git commit -m "Initial Diego AI Ops landing page"

# Create a new repo on GitHub first (recommended name: diego-ai-ops or ai-ops)
# Then connect it (replace the URL below with your actual repo URL)
git remote add origin https://github.com/YOUR_USERNAME/diego-ai-ops.git

# Push to GitHub
git branch -M main
git push -u origin main
```

After pushing, go to Vercel and import the GitHub repo.

### 2. Deploy on Vercel
1. Go to [vercel.com](https://vercel.com) → New Project
2. Import your GitHub repo (`ai-ops`)
3. Vercel should auto-detect it as a static site (it uses `vercel.json`)
4. Deploy

### 3. Add Custom Domain `ai.sarka-ops.com`
1. In your Vercel project → **Settings → Domains**
2. Add `ai.sarka-ops.com`
3. Vercel will give you the exact DNS records needed (usually an A record or CNAME to `cname.vercel-dns.com`)
4. Add the records at your domain registrar (where `sarka-ops.com` is managed)
5. Wait for propagation (can take a few minutes to 48h)
6. In Vercel, click **Verify** once DNS is live

### 4. Contact Form (Formspree)

**Formspree is already configured** with this endpoint:
`https://formspree.io/f/mojbbgvp`

The form is ready to receive submissions. You can log into Formspree to:
- Turn on spam filtering
- Set up email notifications
- Add an autoresponder message

The form already has a honeypot (`_gotcha`) and solid validation built in.

### Quick Local Testing
Just open `index.html` in a browser. The form will fail gracefully until you put a real Formspree endpoint in.

### Environment
This is a pure static site. No build step required. Perfect for fast iteration on Vercel.

## Future Evolution Ideas

- Move to Next.js 15 + Tailwind (when you want server components, blog, better form handling, analytics, etc.)
- Add Calendly embed for "Book a strategy call" as a secondary high-intent CTA
- Add real case studies / proof once you have 2–3 documented wins
- Add a "Grok in action" demo / Loom section
- If you outgrow Formspree: switch to Resend + React Email + Vercel serverless functions

## Voice & Tone Reference

From Diego's X content engine:
- Alpha, cheeky, dead serious, lethal
- Dry, sharp, no fluff
- Hook hard → one killer insight → subtle flex → strong CTA
- "Borrowed time taught me..." as quiet credibility, never victimhood
- Roast laziness. Reward action.

The current copy follows this voice.

## Assets

Currently self-contained. When you want custom photography or logos:
- Drop them in an `/assets` folder
- Reference locally (better for performance + branding)

## Questions / Next Steps

DM @DiegoEspinosaAI on X or just edit the file and tell me what to sharpen.

---

**Built with Grok. No wasted moves.**
