# vulnerablepatient
Knight Baptist Project
# Vulnerable Patient Readmission Checker

A lightweight single-page mockup that screens for potential hospital readmission risk and recommends local 211 resources in South Florida. The tool is HTML/JS only—open `index.html` in any modern browser to try it.

## How it works
- **Eight-question risk screener:** Users answer questions about medications, health literacy, appointment adherence, transportation, support network, prior hospital use, housing, and confidence managing health. Each answer is scored 0–2 for a maximum total of 16.
- **Risk tiers:** Scores ≤5 show a low-risk label, 6–11 show medium risk, and ≥12 show high risk. The calculated score and tier appear above a brief message tailored to the result.
- **Localized 211 guidance:** Selecting Miami-Dade/Monroe, Broward, Palm Beach/Treasure Coast, or another South Florida area swaps in the corresponding 211 provider name, phone, and website.
- **Need-based suggestions:** The page highlights 211 topics such as transportation, housing, social support, health literacy help, medication management, and frequent ER use based on the highest-risk responses. If nothing specific is flagged, it still encourages calling 211 for general assistance.
- **Multilingual text:** English, Spanish, and Haitian Creole strings are bundled in the page and switch instantly via the language selector.

## Usage
1. Open `index.html` in your browser.
2. Choose a language and your county/region.
3. Answer all eight questions, then click **Calculate risk score**.
4. Review the risk result and the tailored 211 guidance list. Use the included links or phone numbers to reach the matching 211 service.

> This mockup is for demonstration only and is not a medical device.
