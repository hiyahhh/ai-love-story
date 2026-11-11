# Wedding film production workflow

## 1. Discover or invent the story

For a fictional promotional sample, invent the meeting, characters, recurring detail and turning point, and label the story as fiction. For a real couple, complete the brief from their own account. Define what the audience should feel at the end. Mark factual, dramatized and symbolic beats. Choose duration, screen format, deadline, audio direction and a maximum spend before production.

Exit: the creative direction is accepted; for a real couple, confirm the story and depiction with them. Unresolved factual details remain explicit blanks.

## 2. Lock the visual references

For fictional characters, generate and accept their initial designs first. For real people, collect clear, current reference photos privately: front, three-quarter and profile views with natural light. Record which person each reference depicts. Create a portrait/front/back sheet for each wardrobe and register every version in `assets.csv`. Review likeness against accepted fictional designs or review resemblance with the real couple. Make one location plate per setting, fixing layout, time of day, light direction and palette. Register important props and which hand carries them. Add a two-person scale/layout sketch only when necessary.

Exit: accepted references with stable IDs, such as `partner_a_cafe_v1`, `partner_b_cafe_v1`, `cafe_v1`, `cup_blue_v1`. Provider element names must match these IDs or have an explicit mapping in the register. Never paste example element UUIDs from the article into our prompts.

## 3. Plan the edit before generating

Complete `shots.csv`. Each shot has one readable action, a clear emotional purpose, entry/exit state, reference IDs and a duration. Durations must total the delivery length. Keep screen direction, wardrobe, prop ownership and lighting consistent across adjacent shots. Choose the technical block once per sequence.

Exit: a timed storyboard/animatic or reviewed shot plan. A 30-second timeline can contain several generated clips; it does not require a single 30-second generation.

## 4. Prove likeness and motion

Use the simplest two-person shot as a 5-second test. Check faces during movement, gaze, hands, relative height, wardrobe and light. If likeness fails, repair references or simplify the framing before generating more scenes.

Exit: accepted test plus known model, settings and actual cost. No paid generation is automated by this repo.

## 5. Generate and select

Attach the accepted references, translate IDs to the provider's actual element syntax, and generate short scene batches. Log every attempt in `takes.csv`, including rejected takes. Start with at most two attempts per shot, then review the failure before retrying. This is a proposed iteration cap, not a provider limit.

Set the total budget and retain a reserve for fixes. Before each batch, compare the provider's displayed estimate with remaining budget. Stop if the next batch would exceed it. Do not assume a credit-to-currency conversion.

Judge: recognizable faces, intended emotion, valid anatomy and contact, coherent space, matching continuity, useful start/end frames and clean audio. Record specific failure reasons. Change one major variable per retry. Split a complex action rather than repeatedly submitting the same overloaded prompt.

## 6. Edit, sound and delivery

Trim selected takes to the shot plan. Carry room tone and sound across cuts; add licensed music or supplied audio if chosen. Add names/date only after spelling is confirmed. Preserve a clean master and export the agreed format; reframe intentionally for vertical delivery rather than blindly cropping faces.

Final review: likeness, factual details, clothing/cultural details, no accidental strangers or text artifacts, consistent grade, intelligible audio, correct names/date, exact duration, no black frames and playback on the actual display when possible. Review the complete promotional cut with the project owner; for a real couple, get their review before sharing it publicly.

Archive the final prompt versions, asset versions, selected takes, edit project and actual spend in private project storage.
