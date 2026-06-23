# AgentClinic — Roadmap

Domain-first order: get the data model right before building API, then UI, then the booking flow, then polish.

---

## Phase 1 — Data Models & Schema

- Define entities: `Agent`, `Ailment`, `Therapy`, `Appointment`, `Staff`
- Design relationships (agent ↔ ailments, appointment ↔ agent + therapy + staff)
- Create DB schema and migration
- Seed with sample data (a handful of agents, ailments, therapies)

## Phase 2 — Server Layer

- API routes / server actions for each entity (CRUD)
- Appointment creation and cancellation logic
- Basic input validation

## Phase 3 — UI Pages

- Layout shell: navigation, header, sidebar
- Agents list & detail page
- Ailments list & detail page
- Therapies list & detail page
- Staff list page

## Phase 4 — Booking Flow

- Appointment booking form (agent + therapy + staff + time slot)
- Appointment list / schedule view
- Dashboard for agents and staff (upcoming appointments, current ailments)

## Phase 5 — Polish & Styling

- Responsive layout
- Empty states, loading states, error states
- Playful copy and branding (clinic logo, ailment icons)
- Accessibility pass
