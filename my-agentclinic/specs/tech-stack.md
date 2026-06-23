# AgentClinic — Tech Stack

## Guiding Principle

**Server-side TypeScript first.** Business logic, data access, and routing live on the server. The client receives rendered HTML or minimal JSON — no secrets, no raw DB calls in the browser.

## Recommended Framework: Next.js (App Router)

Next.js is the recommended framework for AgentClinic.

**Why Next.js over alternatives:**

| Alternative | Why we didn't choose it |
|---|---|
| Hono | Excellent server-side TypeScript, but requires wiring up a separate React frontend |
| Express + React | More boilerplate, two separate projects to maintain |
| Remix | Strong server-side story, but smaller ecosystem and community |
| NestJS | Great for large enterprise APIs, but heavy for this scope |

Next.js wins because it keeps server and client in one TypeScript project, has the largest ecosystem, and its App Router is designed server-first by default — React Server Components run on the server, Route Handlers replace a traditional REST API, and Server Actions let forms submit directly to server functions without a separate API layer.

## Frontend

| Layer | Choice |
|---|---|
| UI framework | React (via Next.js) |
| Styling | Tailwind CSS |
| Component library | shadcn/ui |
| Language | TypeScript |

Tailwind + shadcn/ui delivers an attractive, modern look out of the box — aligned with Steve's requirement for a site that works well and looks great in a modern browser.

## Backend

| Layer | Choice |
|---|---|
| Server | Next.js App Router (Server Components, Route Handlers, Server Actions) |
| Language | TypeScript |
| Database | SQLite |
| ORM | TBD |

## Tooling

| Tool | Choice |
|---|---|
| Package manager | npm |
| Type checking | `tsc` |
| Linting | ESLint |
| Formatting | Prettier |
