# Project rules

- This is a single-user, local-only fitness/workout app. Do not add accounts, auth,
  backend sync, analytics, telemetry, third-party health integrations, or AI/LLM features.
  If a task seems to need one, stop and ask.
- Data is stored only on the device. Sample/seed data must be invented.
- Never commit secrets, real personal data, or `.env` files. Use `.env.example` with placeholders.
- Do not add third-party content (exercise databases, images, icons) unless its license
  is compatible with MIT; record the source and license in the README.
- Commits: small, one logical change each, descriptive message. Keep `Co-Authored-By`.
  Never rewrite history, squash, or force-push.
- Keep README.md (what / who / stack / how to run) and ROADMAP.md up to date when
  features land; tick off roadmap items as they're done.
- Every feature ships with tests for its logic.
