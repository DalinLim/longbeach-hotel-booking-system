# Longbeach Hotel — Booking Demo

A React 18 + Vite + Tailwind CSS hotel website with a multi-step reservation experience.

## Run locally

```bash
npm install
npm run dev
```

## Build for Vercel

```bash
npm run build
```

Deploy the project root to Vercel using the Vite preset. Build command: `npm run build`; output directory: `dist`.

## Booking demo features

- Date search with check-in/check-out validation
- Adult, child and room-count selection
- Room capacity filtering and sample nightly rates
- Optional breakfast with per-person pricing
- Itemised subtotal, estimated tax and total
- Demo sign-in / account creation stored in browser localStorage
- Guest details and mock card checkout
- Local demo booking confirmation and reference

## Important demo limitations

This is a front-end portfolio prototype. It does not query live hotel inventory, prevent double bookings across devices, send confirmation emails, or process real payments. Account credentials and bookings are stored in the current browser's localStorage and are not secure authentication. Payment form values are not saved. Use a real authentication provider and a PCI-compliant payment gateway (such as Stripe) before accepting real bookings. Never store raw card numbers or CVC values.

## Future database structure

A PostgreSQL starter schema is provided at `src/data/booking-schema.sql` for profiles, room types, physical rooms, dated rates/inventory, bookings, booking items and payment records. It is a blueprint only; Supabase or another database is not connected yet. The booking UI should later call server-side functions to check inventory, calculate authoritative prices and create bookings atomically.

## Sample pricing

Rates are illustrative USD portfolio-demo values in `src/data.js`. Confirm and replace all rates, taxes, currency, hotel policies and contact details with the hotel's actual information before publishing as a real booking site.
# longbeach-hotel-booking-system
