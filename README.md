# JaxTech Repairs — Website Project

**Locally Owned Tech Support & House Call Service | Crossville, TN**

---

## About the Business

JaxTech Repairs is a privately owned electronics support and repair service based in Crossville, TN. Founded approximately 3 months ago by a locally certified technician who also works full-time as a **Wireless Phone Expert at Walmart**.

**What makes JaxTech different:**
- **House calls are the specialty** — I come to you, no hauling devices across town
- Years of hands-on experience serving local schools, churches, and the Crossville community
- Locally certified in Crossville, TN
- Honest service, fair pricing, no hidden fees

---

## Current Services

### Active Right Now
- 📱 **Phone Support** — troubleshooting, setup, data transfer, software help (iPhone & Android)
- 📟 **Tablet Support** — iPad, Samsung Tab, Amazon Fire — setup, connectivity, performance
- 💻 **Computer / Laptop Support** — Windows & Mac — virus removal, performance, software
- 📺 **Smart TV Setup & Support** — Samsung, LG, Sony, TCL — WiFi, apps, display issues
- 🖨️ **Printer Setup & Support** — HP, Canon, Epson, Brother — wireless, drivers, paper jams
- 🌐 **Remote Support Sessions** — secure screen-share for software issues
- 🏠 **House Calls / On-Site Visits** — the primary service delivery method

### Expanding Soon
- Screen replacements (phones & tablets)
- Battery replacements
- Broader physical device repairs

---

## Business Details

| Field         | Value                            |
|---------------|----------------------------------|
| Business Name | JaxTech Repairs                  |
| Location      | Crossville, TN                   |
| Phone         | 931-248-6663                     |
| SMS           | 931-248-6663                     |
| Email         | jaxtechrepairs@gmail.com         |
| Hours         | Wednesday: All Day               |
|               | Mon/Tue/Thu/Fri/Sun: By Appt     |
|               | Saturday: Closed                 |
| Service Area  | Crossville, TN and surrounding   |

---

## Website Pages

| Page           | Path           | Description                                          |
|----------------|----------------|------------------------------------------------------|
| Home           | index.html     | Hero, services overview, reviews carousel, FAQ       |
| Services       | services.html  | Full service cards with filter bar                   |
| Pricing        | pricing.html   | Transparent pricing tiers + comparison table         |
| About          | about.html     | Real business story, owner profile, values, community|
| Contact        | contact.html   | Contact form, hours, directions, FAQ                 |
| Book Support   | booking.html   | Multi-step booking form → saves to DB                |
| Admin          | admin.html     | Full CRUD dashboard for clients, appointments, tickets|

---

## Database (3 Tables)

### `clients`
Fields: id, full_name, phone, email, address, notes, total_tickets, status

### `appointments` (14 fields)
Fields: id, client_name, client_phone, client_email, device_type, device_model, support_type, issue_description, appointment_date, appointment_time, status, technician, estimated_cost, tech_notes

### `support_tickets`
Fields: id, client_name, client_phone, client_email, device_type, device_model, issue_category, issue_description, priority, ticket_status, assigned_to, resolution_notes, ticket_number

**Seed data:** 17 clients, 17 appointments (March 2026), 22 support tickets (TKT-1001 through TKT-1012 + JTR- series)

---

## Key Features

- ✅ Booking form creates records in all 3 tables simultaneously
- ✅ Contact form saves new client to DB
- ✅ Admin panel: full CRUD, calendar view, KPI stats, filters, delete/edit
- ✅ Live ticket status checker on homepage (search by ticket number)
- ✅ Review carousel (6 reviews, auto-advance every 5s)
- ✅ Live open/closed badge on contact page (Wednesday = open all day)
- ✅ Responsive design across all pages
- ✅ Schema.org LocalBusiness structured data (index.html)

---

## Tech Stack

- Pure HTML5 / CSS3 / Vanilla JavaScript
- Google Fonts (Inter)
- Font Awesome 6.4.0 (CDN)
- RESTful Table API (built-in cloud DB)
- No frameworks or build tools required

---

## Deployment

Deploy via the **Publish tab** → Cloudflare Pages.
After publishing, connect a custom domain (e.g. `jaxtechrepairs.com`) via Cloudflare Dashboard → Pages → Custom Domains.

---

## Pending / Future Improvements

- [ ] Add real owner name and photo to about.html
- [ ] Replace placeholder reviews with actual customer testimonials once collected
- [ ] Add Google Maps embed with actual Crossville address
- [ ] Connect real social media profile URLs (Facebook, Instagram, Google Business)
- [ ] Add Google Business Profile link
- [ ] Expand services when physical repairs launch (screen/battery)
- [ ] Add SMS notification integration when bookings are submitted
