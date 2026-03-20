# Post-Discharge Social Needs Screener
Knight Baptist Innovation Fellowship Project

A lightweight single-page tool that identifies social needs affecting hospital readmission risk and connects South Florida patients to local 211 resources. Pure HTML/JS — open `index.html` in any modern browser or visit [www.vulnerablepatients.com](https://www.vulnerablepatients.com).

## How it works
- **Eight-question screener:** Users answer questions about medications, health literacy, appointment adherence, transportation, support network, prior hospital use, housing, and confidence managing health. Each answer is scored 0–2 for a maximum total of 16.
- **Risk tiers:** Scores ≤5 show a low-risk label, 6–11 show medium risk, and ≥12 show high risk. Each tier includes a distinct icon for colorblind accessibility.
- **Localized 211 guidance:** Selecting Miami-Dade/Monroe, Broward, Palm Beach/Treasure Coast, or another South Florida area swaps in the corresponding 211 provider name, phone (with clickable `tel:` links), and website.
- **Need-based suggestions:** The page highlights 211 topics such as transportation, housing, social support, health literacy help, medication management, and frequent ER use based on any elevated response (score ≥ 1). All suggestions are fully translated.
- **Multilingual:** English, Spanish, and Haitian Creole — all UI text, resource descriptions, and 211 guidance translate instantly via the language selector.
- **Call 211 Now:** A prominent button lets mobile users tap to call their local 211 directly.
- **Print Summary:** Generates a clean printable handout with results and 211 contact info for care teams.

## Accessibility
- WCAG 2.1 AA focus indicators on all interactive elements
- `fieldset`/`legend` grouping for screen reader question context
- `aria-live` regions for dynamic result announcements
- 44px minimum touch targets for radio buttons
- Color-independent risk indicators (icons + text + color)
- Dynamic `<html lang>` attribute updates for correct screen reader pronunciation
- Skip-to-content link

## Usage
1. Open `index.html` in your browser.
2. Choose a language and your county/region.
3. Answer all eight questions, then click **Calculate risk score**.
4. Review the risk result and the tailored 211 guidance. Tap **Call 211 Now** or use the links to connect.
5. Use **Print Summary** to generate a handout for the care team.
6. Click **Start over** to screen another patient.

## Analytics
The tool includes a lightweight anonymous event tracking system (no PII, no cookies). Set the `ANALYTICS_ENDPOINT` variable in the script to enable. Events tracked:
- `screening_complete` — score, tier, flagged needs, language, county
- `call_211_click` — when the Call 211 button is tapped
- `language_change` — language switches
- `print` / `reset`

> This tool is for demonstration and screening purposes only. It is not a medical device and should not replace clinical judgment or treatment decisions.
