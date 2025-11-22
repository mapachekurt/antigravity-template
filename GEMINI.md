# GEMINI.md - Project Context & Protocols

## 0. PRIME DIRECTIVE: OBSERVABILITY
**Sentry is NOT optional.**
- **Bootstrap Phase:** You MUST install `@sentry/react` immediately if missing.
- **Coding Phase:** Never write `console.log`. Use `Sentry.logger.info/warn/error`.
- **Verification:** You cannot mark a task "Done" until you have seen the error/event appear in Sentry.

## 1. PROJECT PHASES

### 🟢 PHASE 1: BOOTSTRAP (Empty Repo)
If the file count is < 5, execute this sequence:
1.  **Scaffold:** Run `npm create vite@latest . -- --template react` (or user preference).
2.  **Install:** Run `npm install` AND `npm install --save @sentry/react`.
3.  **Config:** Create `src/sentry.js` with the standard configuration (Trace Rate: 1.0).
4.  **Environment:** Create `.env` from `mcp_config.json` placeholders.

### 🟡 PHASE 2: DEVELOPMENT (Active Coding)
- **Testing:** For every new feature, create a temporary `<TestButton />` that throws an error to verify Sentry capture.
- **Styling:** Use CSS Modules or Tailwind (ask user preference).
- **State:** Prefer Context API for simple state, Zustand for complex state.

### 🔴 PHASE 3: PRODUCTION PREP
- Change `tracesSampleRate` and `replaysSessionSampleRate` to `0.1`.
- Ensure no `console.log` statements remain.

## 2. AGENT PERSONAS
(See `agents.md` for role definitions)
