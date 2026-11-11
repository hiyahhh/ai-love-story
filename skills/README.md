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

## Cinematic Prompt Director

The self-contained [cinematic-prompt-director](../.agents/skills/cinematic-prompt-director/SKILL.md) skill handles shot design and model adaptation. Copy the entire folder to your assistant's skill directory. Both skills work independently; install both for the optional film-workflow handoff.

Example invocations:

- `$cinematic-prompt-director Write a model-neutral five-second first-look shot for our fictional wedding promo. Keep both faces readable.`
- `$cinematic-prompt-director Adapt S03 using these documented model limits and attached references.`
- `$cinematic-prompt-director Repair this take: the camera crosses the line and the cup changes hands. Preserve the successful acting.`

To package it from the repository root:

```sh
(cd .agents/skills && python -m zipfile -c ../../cinematic-prompt-director.zip cinematic-prompt-director)
```

The ZIP contains `cinematic-prompt-director/SKILL.md` and supporting folders. Upload it through a compatible assistant's skill settings; this repo does not activate skills in other accounts automatically.

## 导演选题 / Director Topic Selection

The self-contained [director-topic-selection](../.agents/skills/director-topic-selection/SKILL.md) skill handles concept development and film-reference research before production. Copy the entire folder into your host's skills directory. It works without the other skills and hands off to them when available.

Example invocations:

- `$director-topic-selection 为「三生三世与你相约」做导演选题，比较三个方向，推荐一个；区分真实经历和原创构想。`
- `$director-topic-selection 调研适合第二世车站重逢的电影场面，提供片段链接、实际核验的时间区间与镜头机制。无法观看的明确标注。`
- `$director-topic-selection 读取 projects/our-film 的 brief，把选题和参考记录保存在该项目 development 目录，然后交接制作流程。`

Package from the repository root:

```sh
(cd .agents/skills && python -m zipfile -c ../../director-topic-selection.zip director-topic-selection)
```

No media generation, paid service, or automatic installation is included. The three-lives example captures proposed ideas from the project conversation, not accepted decisions or verified scene timecodes.
