# GuardianAI - GitHub Pages Version

**GuardianAI: An Intelligent Digital Safety Companion for Youth Protection**

This is the **plain HTML/CSS/JavaScript version** of GuardianAI, made for the
**SafeTech Africa Hacklab Youth Social Innovation Challenge 2026**.

It needs **no build step, no database, and no server**:

- Open `index.html` directly in a browser, **or**
- Publish it free with **GitHub Pages** (instructions below)

> Mission: *Helping youth identify online risks, understand digital rights, and
> stay safer in digital spaces.*

## Pages

| Page | File | What it does |
| --- | --- | --- |
| Landing Page | `index.html` | Branding, mission hero, Start Safety Check / Ask GuardianAI / Learn Digital Safety |
| AI Safety Assistant | `assistant.html` | Chat with structured safety responses (try "Someone is threatening me online") |
| AI Risk Detection | `risk-detection.html` | Paste a suspicious message - returns category, risk level (score /100), and actions. The example returns **Phishing Attempt - High (92/100)** |
| Learning Hub | `learn.html` | Online Privacy, Cyberbullying Awareness, Scam Prevention, Digital Rights, Technology-Facilitated Violence Awareness + a scam-spotting quiz |
| Support & Reporting | `support.html` | Reporting steps, evidence guide, emergency panel (placeholder - add verified local helplines before launch) |
| User Profile | `profile.html` | Private on-device activity summary (browser storage only, clearable any time) |
| About | `about.html` | Mission, how it works, design principles, safeguarding |

## Publish on GitHub Pages (free)

1. Create a new repository on GitHub, e.g. `guardianai`.
2. Upload **all files and folders in this project** (`index.html`, the other
   `.html` pages, and the `assets` folder) to the repository. Keep
   `index.html` at the top level of the repository.
3. In your repository, go to **Settings -> Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select the
   `main` branch and `/ (root)`, then **Save**.
5. After a minute or so, GitHub shows your live address, usually:
   `https://YOUR-USERNAME.github.io/guardianai/`

Share that link with judges and testers.

> Tip: if you name the repository `YOUR-USERNAME.github.io`, the site opens at
> `https://YOUR-USERNAME.github.io/` instead.

## Run locally

Just open `index.html` in any browser - no installation needed.
(For best results with browser storage on the Profile page, you can also run
`python3 -m http.server` in this folder and open http://localhost:8000 )

## How the safety features work

`assets/app.js` contains a transparent, rule-based safety engine (phishing,
threats/harassment, cyberbullying, scams, exploitation risk, urgent support).
The assistant uses the same engine and always answers in the structure:
**risk identified -> safety advice -> reporting actions**.

For a production version, connect this front end to an AI model/moderation API
with youth safeguarding review - and never collect passwords or private photos.

## Customising

- Colours: CSS variables at the top of `assets/styles.css`
- Lessons and wording: edit the matching `.html` page
- Risk rules: edit `RULES` in `assets/app.js`
- Helplines: replace the placeholder in `support.html` with verified numbers

## Files

```
index.html  assistant.html  risk-detection.html  learn.html
support.html  profile.html  about.html
assets/
  styles.css
  app.js
```

No `src`, no `node_modules`, no build - what you upload is what opens.
