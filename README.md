# CareFlow

A hospital workflow dashboard prototype. It shows how a patient moves through a hospital, from reception to billing, and gives each kind of staff member a view that fits their job.

**Live demo:** https://careflow-tau-five.vercel.app/

> **This is a prototype.** It runs on made-up demo data that lives in the browser and resets on refresh. It is not a medical system and must not be used with real patient information.

## What it shows

- Dashboard with key numbers and a weekly patient-visits chart
- Patient directory with search
- Care workflow queue: At reception → Awaiting vitals → With doctor → At pharmacy → Ready for billing → Completed, with status changes
- Role preview for Admin, Reception, Nurse, Doctor and Pharmacist
- Staff directory, add-staff form, and staff import and export with CSV
- Pharmacy, billing and analytics screens
- Responsive layout with a sidebar and top bar

The role switcher is for previewing screens only. It is not real login or permission control.

## Tech

| Part | Used |
|---|---|
| Front end | React 18, Vite |
| Charts and icons | Recharts, Lucide |
| Backend (next step) | Supabase client helper is in place but not connected |
| Hosting | Vercel |

## Run it locally

You need [Node.js](https://nodejs.org) (LTS).

```bash
cd CareFlowVs
npm install
npm run dev
```

Open the address Vite prints, usually http://localhost:5173.

## Roadmap

Before anything like this could touch real records, it needs:

1. A Supabase project with a proper schema, sign-in and Row Level Security, so the database decides who can see what
2. Audit logs, backups and consent and retention rules
3. Review against Nigerian data-protection and healthcare requirements

## Folder

```
CareFlowVs/
  src/App.jsx          the whole dashboard
  src/lib/supabase.js  Supabase client (not connected yet)
  src/styles.css
  index.html
  package.json
```

## Credits

Designed and built by Kidddarts (Augustine Ucheaga). Contact: augustineucheaga@gmail.com
