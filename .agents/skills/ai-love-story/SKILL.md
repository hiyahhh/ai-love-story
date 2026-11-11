---
name: ai-love-story
description: Plan and direct cinematic AI love-story and wedding short films, especially fictional promotional samples. Use when asked for a wedding-film concept, consistent character/location references, a timed storyboard, generation prompts, take review, or an edit plan. Supports a full production workflow or a single stage; does not itself supply a video-generation service.
---

# AI Love Story

Turn an emotional idea into a reproducible film package: brief → locked assets → timed shots → generation prompts → selected takes → edit.

## Start from the user's goal

Identify whether this is a fictional promotional sample or a real couple's personalized film. Default to a fictional promotional sample when the user asks for portfolio or marketing examples. Do not ask for a real couple's biography to begin a sample. Invent fictional characters and events, state that they are fictional, and avoid presenting the result as a real client wedding or testimonial.

For a sample, propose a concise concept and proceed with a clearly stated default of 30 seconds, 16:9, photoreal cinematic imagery and no dialogue. Use the user's choices instead when supplied. Leave spend unset until known. If asked only for a concept, assets, prompts or critique, complete that stage without forcing the entire pipeline.

For a real couple, use supplied facts; flag gaps that affect the story. Ask only for missing decisions that materially affect the requested output. Continue independent preparation while waiting. Do not invent biography, physical features, cultural details or reference attachments.

Read [direction and continuity](references/direction.md) before writing final shot prompts. Read [source notes](references/source-notes.md) when explaining the tutorial's method or selecting a model. Read [production and review](references/production.md) before planning paid generations or evaluating takes. Load only the references needed for the current stage.

## 1. Write the creative brief

Use [the brief template](templates/brief.md). For a promotional sample, fill it with fictional characters, one recognizable emotional hook, one obstacle or hesitation, a choice, and a payoff. Mark all invented story details as fiction. Prefer one or two locations and a distinctive recurring prop for the first sample. A historical or multi-era montage is an optional creative choice, not a requirement.

Describe what the sample demonstrates: likeness consistency, emotional acting, an era transformation, or a personal motif. Set duration, aspect ratio and sound direction. Separate proposed choices from locked decisions. The sample should feel like a complete short story, not a list of attractive shots.

Deliverable: a filled brief with assumptions and next action.

## 2. Lock reusable assets

Use [prompt templates](templates/prompts.md) for character sheets and location plates; track assets in [assets.csv](templates/assets.csv).

Create stable IDs for each character + wardrobe, location and important prop. Each character sheet has portrait, front full body and back full body views with consistent proportions and clothing. A real person's identity comes from supplied photos; fictional characters can be designed, then held to their accepted reference sheets.

Specify location geometry, key light direction, time, palette and fixed objects. Add a relative-scale sketch or spatial storyboard when required. Review reference images before treating them as accepted. If image tools are available and generation is requested, use them; otherwise provide ready-to-run prompts and mark assets as missing. Never fabricate generated asset paths or accepted review status.

Deliverable: reference prompts, asset register and explicit missing/accepted states.

## 3. Plan the story in time

Use [shots.csv](templates/shots.csv). Every shot needs emotional purpose, duration, framing, observable action, reference IDs, entry/exit state, continuity and sound. The durations must sum to the film length with no accidental timeline gaps or overlaps.

Keep one main action per shot. Describe acting as a task (recognize, search, decide, reassure), supported by small visible behavior. Maintain screen direction, eyelines, prop ownership and hand, costume and light between cuts. Reserve slow motion for a deliberate emotional beat. For complex action, use a storyboard or simplify before generation.

Deliverable: a timed shot list and a brief explanation of the emotional progression. See [the fictional pilot](examples/one-more-coffee/brief.md) as a worked starting point, not a mandatory story.

## 4. Write executable scene prompts

When both skills are installed, use Cinematic Prompt Director (`$cinematic-prompt-director`) for shot feasibility, physical blocking, optics, creative devices, model translation and repair. Keep this skill responsible for the film process. The companion is optional; standalone installations can use the templates below.

Use the video template in [prompts.md](templates/prompts.md). Include reference definitions, a shared technical block, timed action, acting task, continuity and sound. Refer only to assets available or explicitly marked as prerequisites. Match asset IDs to the actual provider elements before submitting; plain names and copied tutorial UUIDs do not bind references.

Reuse the technical block across related scenes. Translate each scene into the chosen model's supported duration, reference count, aspect ratio and sound controls. Check current capabilities rather than relying on the tutorial's model names. Keep output shot timing distinct from generation length: the editor can trim a longer take. Split a sequence when too much action is packed into one generation.

Deliverable: versioned prompts, required reference list, intended UI settings, and blockers before submission. Exact timing and likeness are goals, not guarantees.

## 5. Test, generate and select

Start with a five-second identity/motion test, preferably a simple two-person interaction without difficult hand contact. Review real outputs before scaling up. If a user requests generation and a suitable tool is available, execute within their authorized scope and known budget. If no tool is connected, say so and finish the prompt package; do not imply a video was created.

Log attempts with [takes.csv](templates/takes.csv). Preserve the exact prompt version, reference versions, model/settings, cost unit, output path and failure reason. Begin with up to two attempts per shot, then reassess. Do not spend past an explicit budget or invent prices. Change the cause of a failure, not just the random seed indefinitely.

Deliverable: reviewed test or clearly marked unexecuted package, then selected takes and a remaining-work list.

## 6. Edit for the promotional use

Create an assembly plan with selected take IDs, in/out points, transitions, sound, title and final call to action if requested. Use a recurring prop, gesture or sound to bridge time. Add names, dates, captions and marketing text in the editor for reliable spelling. Do not fabricate client claims. Distinguish fictional sample captions from factual marketing claims.

Review likeness, emotion, geography, anatomy, continuity, audio, title spelling, total duration and export playback. Consider the intended display and aspect ratio; plan vertical framing separately if needed. Keep private source media out of a public repository and use only assets the user can use for the intended promotion.

Deliverable: edit plan or actual export when tools/assets permit, review findings and an accurate statement of what was generated versus only planned.

## Output discipline

Save project-specific outputs under a named project directory and leave this skill unchanged unless asked to improve it. Copy templates before filling them. Record accepted creative choices so later stages reuse them. Finish the requested stage with concrete artifacts, not merely a suggestion to continue.

Before handing off, check local links, asset-ID consistency and shot timing. For generated media, inspect the media itself. Do not mark a film ready based only on prompt quality.
