# Chasely

**Get paid on time without the awkward follow-ups.**

Chasely is a web app that automatically sends polite, escalating payment reminders for overdue invoices, so freelancers and small businesses can stop chasing clients and focus on their work.

---

## The Problem

Late payments are a constant headache for freelancers, consultants, and small agencies. Chasing clients is:

- **Awkward**: nobody likes nagging a client about money.
- **Easy to forget**: reminders slip through the cracks when you're busy.
- **Inconsistent**: tone and timing vary from one email to the next.

The result is delayed cash flow, wasted time, and strained client relationships.

## The Solution

Chasely takes over the follow-up process. Add your invoices, choose a reminder schedule, and Chasely sends the right message at the right time, starting friendly and becoming firmer only if needed. A simple dashboard shows who owes what and how overdue it is.

## Key Features (MVP)

- **Invoice tracking**: add invoices manually or import them via CSV (client, amount, due date, status).
- **Automated reminders**: scheduled emails sent before the due date, on the due date, and at set intervals afterward.
- **Escalating tone**: friendly nudge → firm reminder → final notice.
- **Editable templates**: customize wording, with placeholders such as `{{client_name}}`, `{{amount}}`, `{{due_date}}`, `{{invoice_number}}`.
- **Overdue dashboard**: total outstanding, overdue amounts, and aging buckets (1–7, 8–30, 30+ days).
- **One-click "Mark as paid"**: stops all future reminders instantly.
- **Reminder history**: see exactly what was sent and when, per invoice.

## How It Works

1. **Add** your invoices (manual entry or CSV upload).
2. **Pick** a reminder schedule and template set.
3. **Relax**: Chasely sends reminders automatically.
4. **Mark paid**: reminders stop the moment the invoice is settled.

## Target Users

- Freelancers (designers, developers, writers, consultants)
- Small agencies and studios
- Solo service businesses with a handful to a few dozen active invoices

## Planned Roadmap

**v1.0: MVP**
- Account signup and login
- Invoice CRUD and CSV import
- Reminder scheduling and email delivery
- Template editor
- Overdue dashboard

**v1.1**
- Client-facing payment link or "I've paid" confirmation button
- Reply-to forwarding so client replies land in your inbox
- Custom sending domain

**v2.0**
- Integrations with accounting tools (Stripe, QuickBooks, Xero, FreshBooks)
- Late-fee notices
- Multi-user teams
- Weekly cash-flow summary email

## Proposed Tech Stack

> Suggestions only; finalize before building.

| Layer | Option |
|---|---|
| Frontend | React / Next.js |
| Backend | Node.js (Next.js API routes) or similar |
| Database | PostgreSQL |
| Auth | Email + password, or a hosted auth provider |
| Email delivery | Transactional email service (Resend, Postmark, or SendGrid) |
| Scheduling | Cron job or queue-based worker for reminders |
| Hosting | Vercel / Render / Fly.io |
| Payments (billing) | Stripe |

## Pricing Idea (Draft)

| Plan | Price | Includes |
|---|---|---|
| Free | $0 | Up to 3 active invoices |
| Pro | ~$9/month | Unlimited invoices, custom templates, reminder history |
| Business | ~$19/month | Custom sending domain, multiple users, integrations |

## Success Metrics

- Average days-to-payment reduced for users
- Percentage of overdue invoices recovered after reminders
- Weekly active users and invoices added per user
- Free-to-paid conversion rate

## Project Status

**Planning stage.** No code has been written yet.

## Getting Started

_Setup instructions will be added once development begins._

## Contributing

_Contribution guidelines to be added._

## License

_To be decided._
