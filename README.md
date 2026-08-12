# Mann Ki Gita - Landing Page (frontend)

Fast, self-contained landing page (`index.html`) + post-payment page (`thankyou.html`).
Zero external fonts/frameworks. Meta Pixel + Razorpay checkout in a popup.

Backend (settings, checkout, lead capture) is the Frappe app:
https://github.com/tcbinfotechpvtltd/mann_ki_gita_admin

## Configure
Edit `CONFIG` at the top of the `<script>` in `index.html`:
- `frappeBase` : your Frappe site origin (e.g. https://mkg.example.com)
- `hasBackend` : true once the Frappe app is live
- `razorpayKeyId` : your Razorpay key id (public)

Date, time, price, WhatsApp link, VSL video, hero copy, teacher, testimonials are all
served live from the Frappe app (`mann_ki_gita.api.get_settings`).
