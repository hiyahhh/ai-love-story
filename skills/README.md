# Reusable AI Love Story skill

The installable skill lives at [`.agents/skills/ai-love-story`](../.agents/skills/ai-love-story/SKILL.md). It is self-contained: its references, templates and fictional example travel with it.

## In Codex

Open this repository as the workspace. Codex can discover repository skills in `.agents/skills/`. Invoke `$ai-love-story`, or ask for the workflow by name. For use across repositories, copy the entire `ai-love-story` directory into your Codex user skills directory (normally `~/.agents/skills/`), then start a new session if needed. Do not copy only `SKILL.md`.

## In Claude or another skill-compatible assistant

Package the contents of this directory as a ZIP with `ai-love-story/SKILL.md` and its supporting folders at the top level. Upload it using the assistant's skill settings if supported. Installation paths and supported formats vary by host; this repository does not install or activate a skill in another account automatically.

## Example invocations

- `$ai-love-story Create a fictional 30-second wedding-film promo: the same couple finds each other in three eras. Start with a brief, reference plan and timed shots.`
- `$ai-love-story Use this brief and these character sheets to write five-second test prompts. Keep the asset names exact.`
- `$ai-love-story Review these takes for likeness, continuity and emotional clarity; select the best and propose fixes.`
- `$ai-love-story Turn the selected takes into a 30-second edit plan with a fictional-sample caption and a final CTA.`

The skill adapts the article's method; it is not the author's downloadable Claude skill. No generation tool or paid account is bundled. Project templates elsewhere in the repo remain useful standalone examples; the copies inside the skill make it portable.
