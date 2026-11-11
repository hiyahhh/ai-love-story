# Prompt templates

Replace all bracketed fields. These are original templates adapted from the workflow, not the author's downloadable Claude skill. Attach the actual references; text-only asset names do not bind an identity by themselves.

## Character sheet

Create a three-panel reference sheet of [PARTNER ID] from the attached photos: close-up portrait, full-body front, full-body back. Preserve their actual facial geometry, asymmetry, skin tone, hairline, proportions and distinguishing features; no beautification or age change. Outfit: [EXACT CLOTHING, SHOES, ACCESSORIES]. Same identity and wardrobe in every panel. Neutral background, even diffuse light, natural skin texture, whole hands and feet visible in full-body views; front/back at equal scale and on one ground line. No labels. [ASPECT RATIO].

Review resemblance before accepting. Create new version IDs for material changes.

## Location plate

Create a photoreal location reference for [LOCATION ID]: [SETTING AND PERIOD]. Show [FIXED GEOGRAPHY, ENTRANCES, LANDMARKS AND IMPORTANT OBJECTS]. Time/weather: [VALUES]. Key light from [DIRECTION]; palette [VALUES]. Camera position and view: [VALUES]. No lead characters, no readable signs. [ASPECT RATIO AND LOOK]. Preserve this layout and light in subsequent shots.

## Scene-writing assistant

You are helping plan a wedding short film. Use the attached brief, shot list and accepted references. Never invent personal history or claim an unattached asset is available. First flag missing inputs. Use exactly these asset names: [ELEMENT LIST]. Return a prompt for [SHOT OR SCENE ID], with reference definitions, shared technical block, timed shots, acting tasks, continuity constraints and sound. Stay within [DURATION]. Describe observable action and motivation; keep one main action per shot. Split the scene if its actions exceed the model's supported duration. State which provider settings must be selected in the UI. Do not promise exact output timing or likeness.

## Video scene

REFERENCE DEFINITIONS
[ASSET ID]: [what must match: identity / wardrobe / geography / prop].
[PROVIDER ELEMENT MAPPING]: [actual attached element names or IDs].

TECHNICAL BLOCK
[ASPECT RATIO], [DURATION], [RESOLUTION IF SUPPORTED]. Photoreal [LOOK]; [LENS/FRAMING], [CAMERA STYLE], [LIGHT DIRECTION], [PALETTE]. [REAL TIME OR EXPLICIT SLOW-MOTION SEGMENT]. Audio: [SFX / DIALOGUE / EXTERNAL MUSIC PLAN].

SHOT [ID] — [START–END]
Purpose: [STORY CHANGE].
Framing and camera: [CONCRETE VIEW AND MOVEMENT].
Action: [SINGLE OBSERVABLE ACTION].
Acting task: [WHAT THE PERSON IS TRYING TO DO].
Start state: [POSITIONS, GAZE, PROPS].
End state: [STATE NEEDED BY NEXT SHOT].
Continuity: [SCREEN DIRECTION, WARDROBE, PROP HAND, LIGHT].
Sound: [SPECIFIC CUES].
Avoid: identity drift, extra limbs, floating objects, changing wardrobe, unintended text. Add only constraints relevant to this scene.

LOG AFTER GENERATION
Record exact submitted prompt/version, model, UI settings, reference versions, cost, output location and review result in the take log.
