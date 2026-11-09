# Roadmap

Items are ticked off as they land. Order within a section is rough priority.

## 0. Planning

- [x] Project rules (`CLAUDE.md`)
- [x] README and roadmap
- [x] Research on aerial training and the FEDEC static trapeze manual
- [x] Skill catalog draft: 65 static trapeze skills in 7 families, Italian + English names
- [x] Training logic spec draft: skill states, "nailed" rule, spaced review, session generator, safety
- [ ] Teacher review of the catalog (Italian names, prerequisites, "spotter only" flags)
- [ ] Answer the open questions in the training logic spec
- [ ] Resolve the license of the Canva skill illustrations

## 1. Foundations

- [ ] Scaffold the Expo app (expo-router, expo-sqlite, test runner)
- [ ] Catalog JSON format, apparatus-agnostic, bundled with the app
- [ ] Add the reviewed static trapeze catalog to the repo
- [ ] SQLite schema: skill state, sessions, ratings, custom skills, overrides, photos, settings
- [ ] Inline bilingual strings, `tr('it', 'en')`

## 2. Training logic (pure functions, with tests)

- [ ] Skill states and unlock rule (all prerequisites nailed)
- [ ] "Nailed" rule: 3 solid ratings on 3 different days, last rating not "lost"
- [ ] Spaced review steps 3 → 7 → 14 → 30 → 60 days
- [ ] Implicit reviews: practising a skill reviews its nailed prerequisites
- [ ] Break handling: shift due dates after 14+ days away
- [ ] Daily session generator (time budget, learning cap, due reviews, exclusions)
- [ ] Safety rules: spotter-only skills, return session, weekly volume warning, pain tracking

## 3. MVP app

- [ ] First run: mark the skills you already know
- [ ] Catalog browser by family, with Italian and English names
- [ ] Skill detail: description, prerequisites, what it unlocks, illustration
- [ ] Today's session: propose, edit, rate each skill
- [ ] Class mode: log what you did in a lesson
- [ ] History of sessions and ratings
- [ ] Local review reminders
- [ ] JSON backup export and import

## 4. Personalisation

- [ ] Goal skills with the missing prerequisite chain
- [ ] Hide skills
- [ ] Rename skills and confirm Italian names
- [ ] Custom skills
- [ ] Import skill packs from a JSON file
- [ ] School levels instead of 1-5
- [ ] Personal photo when a skill is nailed

## Later

- [ ] More apparatus: aerial hoop, rope, silks
- [ ] Sharing with friends (needs its own decision first: the app is local-only today)
