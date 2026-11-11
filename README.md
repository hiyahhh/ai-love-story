# AI Love Story

A repeatable GenAI production process for personalized wedding short films.

Start with a true story, lock the couple's likeness and visual world, then generate and edit short scenes. This repository is a production kit; it does not yet call generation APIs or render films.

## Reusable skills

Use `$ai-love-story` in Codex with this repository open. The [portable skill](.agents/skills/ai-love-story/SKILL.md) covers fictional promotional samples, reference assets, scene prompts, take review and editing. See [installation and examples](skills/README.md) for reuse in other projects or assistants.

Use `$cinematic-prompt-director` for model-agnostic shot direction, prompt writing and failed-shot repair. Its [portable package](.agents/skills/cinematic-prompt-director/SKILL.md) separates cinematic intent from provider settings and reference syntax.

Our current focus is fictional promotional samples. We can design sample characters and stories without waiting for a real couple's biography. The first output is a reviewed creative package, followed by references and a short motion test.

## Start the first film

1. Copy `projects/_template/` to `projects/<film-slug>/`.
2. Complete `brief.md` with the couple. Confirm the story beats before writing final prompts.
3. Follow [the production workflow](docs/workflow.md). Register and review character sheets, locations, wardrobe and props in `assets.csv`.
4. Fill `shots.csv`, then use [the prompt templates](prompts/templates.md) with the actual attached references.
5. Generate a short identity/motion test. Review it before spending on full scenes. Record every attempt in `takes.csv`.
6. Assemble selected takes, sound and titles; review the film against the delivery checklist.

See [the fictional 30-second pilot](examples/one-more-coffee/brief.md) for a worked starting point. It is a proposed creative direction, not a real couple's story or a generated film.

## What's here

- `docs/article-notes.md`: attributed lessons and our adaptations.
- `docs/workflow.md`: production stages, review criteria and budget controls.
- `prompts/templates.md`: reference-sheet, location and scene-writing templates.
- `projects/_template/`: brief, asset register, shot list and take log.
- `examples/one-more-coffee/`: fictional brief, timed shot plan and pilot scene prompt.

Keep personal photographs, voices, unreleased films and private briefs outside this public repository. Use private storage paths in working copies; publish only material the couple has agreed to share. The `.gitignore` is a convenience, not an access-control system.

## First milestone

A reviewed couple brief, two accepted character sheets, one accepted location plate, and a 5-second test that preserves both identities. Then expand to a 30-second rough cut. Duration, format, platform and spend remain project decisions.
