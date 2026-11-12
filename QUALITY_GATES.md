# FALAH Quality Gates

A feature is not considered complete because code exists. It must pass observable tests.

## Gate 0 — Safety of the existing project
- No changes to What If `main`.
- No changes to Rewind or CopyPaste.
- No package installation or unrelated refactor.
- All work is isolated and reversible.

## Gate 1 — Reference analysis credibility
- Duration, dimensions, frame rate, and audio stream are recorded.
- Shot boundaries and key action beats have timestamps.
- Character, camera, background, effects, and audio are assessed separately.
- Every claim is marked verified, estimated, or unknown.
- Sampling gaps are disclosed.

## Gate 2 — Style extraction
- Stable style rules are separated from scene-specific actions.
- The Style Bible describes how motion should feel, not a fixed sequence of motions.
- The style rules can be applied to a different story without copying its actions.

## Gate 3 — Scene-specific direction
- A new script produces a new scene plan.
- Each scene's action is justified by its narrative beat.
- The plan is not just a sentence-to-preset lookup.
- Camera, facial performance, body mechanics, environment, and effects are considered.

## Gate 4 — Animation quality
- Body parts move in coordinated, plausible ways.
- Weight shifts, anticipation, follow-through, and foot contact are considered where relevant.
- Facial expression and gaze change with the performance.
- Camera movement supports the scene rather than being random decoration.
- Background and effects have intentional timing.

## Gate 5 — Audio alignment
- Narration timing is measured or explicitly marked approximate.
- Major actions align with meaningful words or beats.
- Sound effects have scene-specific cues.
- No claim of word-level lip sync unless tested.

## Gate 6 — Two-story anti-repetition test
- Test two substantially different scripts.
- Compare scene plans and motion timelines.
- Shared low-level rig tools are acceptable.
- Repeated complete choreography without a story reason is a failure.
- Both tests must pass before FALAH is described as flexible.

## Gate 7 — Rendering and resource limits
- Short previews pass before long renders.
- Free compute limits and time are recorded.
- No paid service is silently introduced.
