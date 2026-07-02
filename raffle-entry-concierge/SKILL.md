# Skill: raffle-entry-concierge
> Automates the entry process for high-heat sneaker raffles across major retailers to maximize your chances of winning limited releases.

## Workflow

1. **Raffle Discovery**
   - Input: Specific SKU or release name.
   - Use the `drop-day-war-room` logic to aggregate all active raffle links from major retailers (e.g., A Ma Maniere, Social Status, Feature, Extra Butter, etc.).

2. **Profile Management**
   - Securely utilizes stored user profile data (name, shipping address, shoe size, and payment method) to populate raffle forms.
   - Supports multiple profiles if configured by the user.

3. **Automated Entry**
   - Use `use_browser` to navigate to each raffle URL.
   - Automatically identifies form fields and populates them with the relevant profile data.
   - Handles common raffle mechanics like Captcha (via `request_user_assistance` if needed) and email verification.

4. **Tracking & Confirmation**
   - Monitors for "Entry Confirmed" screens or emails.
   - Logs all successful entries in a centralized dashboard for the user to review.
   - Alerts the user of any failed entries or required manual actions.

## Usage
"Enter all active raffles for the Jordan 1 Chicago (DZ5485-612) in Size 10."
"Find and enter raffles for the upcoming Foamposite Tianjin."
"Show me a list of all raffles I've entered this week."

## Note on Environment
This skill requires `use_browser` for form interaction. Users are responsible for ensuring their profile data is accurate and that they comply with each retailer's terms of service regarding raffle entries.