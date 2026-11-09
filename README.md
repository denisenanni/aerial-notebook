# Aerial Notebook

*Quaderno Aereo* in Italian.

A personal training notebook for aerial acrobatics, starting with static trapeze.
It tracks which skills you are learning, which ones you have nailed, what they
unlock next, and reminds you to review the ones you already know before you
forget them.

It is a notebook, not a coach. It helps you remember what you did and what to
practise; your teacher still decides the lesson and judges your technique.

> **Status:** planning. There is no app code yet. This repo holds the project
> rules, this README and the [roadmap](ROADMAP.md).

## Who it is for

One person: an aerialist training with a teacher who wants to train more
systematically between classes. It may be shared with a few friends later, but
it is designed as a single-user, local-only app. There are no accounts and no
server.

## What it does (planned)

- **Skill catalog.** Static trapeze skills grouped into families based on the
  FEDEC static trapeze manual: Foundations (*Fondamentali*), Transitions
  (*Transizioni*), Basic moves (*Figure base*), Hangs (*Appesi*), Balances
  (*Equilibri*), Drops (*Cadute*), Advanced (*Avanzate*), plus conditioning
  (*Preparazione fisica*). Every skill has an Italian and an English name,
  because pose names are easy to forget. For example: *Appeso alle ginocchia* /
  Hocks hang, *Nido sotto la sbarra* / Bird's nest, *Seduta* / Sitting on the bar.
- **Progression.** A skill unlocks when all its prerequisites are nailed.
  A skill is nailed (*chiusa*) after 3 "solid" ratings on 3 different days.
- **Spaced review.** Nailed skills come back for review after 3, 7, 14, 30 and
  60 days. A "solid" rating moves a skill up a step, "unsure" keeps it, "lost"
  sends it back to step 1, and two "lost" in a row put it back into learning.
- **Daily session.** Tell the app how much time you have and whether a teacher
  or spotter is there; it proposes warm-up, conditioning, skills to learn and
  reviews. A "class mode" just logs what you did in a lesson.
- **Safety.** Skills marked "spotter or mat only" are never suggested for solo
  practice. A return session after a break of 14+ days, a weekly volume warning,
  and pain tracking by body area.
- **Your own path.** Set goal skills, hide skills you don't care about, rename
  skills, add your own, use your school's levels, and import skill packs from a
  JSON file.
- **Media.** An illustration per skill, plus your own photo when you nail it, as
  a reminder of what you have achieved (not for form feedback).
- **Backup.** Export and import all your data as a JSON file.

Static trapeze comes first, but the data model is apparatus-agnostic so that
aerial hoop, rope, silks and others can be added later.

## Stack (planned)

- [Expo](https://expo.dev/) (React Native) with expo-router
- expo-sqlite for on-device storage
- expo-notifications for local review reminders
- expo-image-picker for personal photos
- JSON file export/import for backup and skill packs
- Inline bilingual strings, `tr('it', 'en')`, Italian and English
- Training logic as pure functions in `src/lib`, tested with `node --test`

All data stays on the device. No backend, no analytics, no third-party health
integrations.

## How to run

There is nothing to run yet. Once the app is scaffolded, this section will list
the setup steps (install Node and dependencies, start Expo, run the tests).

## Content and licenses

- **Skill catalog.** Drafted from the FEDEC static trapeze manual (chapter 2)
  and still under review with a teacher: many Italian names are translations
  that need confirming, and some descriptions are intentionally left empty
  rather than guessed. It is not in this repo yet.
- **Skill illustrations.** Made in Canva. Their license for redistribution in an
  MIT-compatible repo has not been checked yet, so they are not in this repo.
  They will be added only once that is resolved, with the source and license
  recorded here.

No license has been chosen for the code yet.
