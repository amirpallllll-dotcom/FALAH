# FALAH Architecture — Initial Design

## Product definition
FALAH is a scene director and animation production pipeline for one selected 2D visual style. It is not a model fine-tune and not merely a prompt file.

## Pipeline

1. **Reference intake**
   - Accept a legally usable local video file.
   - Record duration, frame rate, dimensions, audio presence, and technical integrity.
   - Never infer motion from a handful of stills and call it full analysis.

2. **Reference analysis**
   - Segment the reference into shots and meaningful action beats.
   - For each shot, document character actions, body mechanics, facial changes, camera, environment, transitions, effects, and sound timing.
   - Mark observations as verified, estimated, or unknown.

3. **Style Bible**
   - Store stable visual principles: line quality, proportions, palette, lighting, staging, camera language, motion quality, timing, and effects vocabulary.
   - Do not store the reference's exact scene choreography as a default template.

4. **New-story interpretation**
   - Read the new script and narration.
   - Identify story beats, intent, emotional changes, characters, props, and environment.
   - Build a fresh shot list for the new story.

5. **Scene direction**
   - Write a scene-specific direction brief before animation code.
   - Specify staging, action, body mechanics, facial performance, camera, environment, transitions, and sound cues.
   - Explain why each major movement belongs to this scene.

6. **Animation implementation**
   - Reuse low-level tools: rigs, joints, interpolation, constraints, camera primitives, particles, lighting/effect components.
   - Compose new motion from the scene direction.
   - Avoid blindly replaying a reference action or a generic preset.

7. **Audio timing**
   - Use narration timestamps when available.
   - Otherwise label timing as approximate and provide a review step.
   - Place sound effects against story events, not arbitrary timestamps.

8. **Visual QA**
   - Render short previews first.
   - Inspect representative frames and motion continuity.
   - Compare against the Style Bible and scene brief.
   - Revise before full-length rendering.

## Separation from What If
- FALAH development must happen in its own repository when repository creation access is available.
- Until then, do not write to the What If default branch.
- Any temporary integration must be isolated on a dedicated branch and must not alter Rewind or CopyPaste.
- The rendering backend is replaceable; FALAH's analysis and direction data should not be coupled to Remotion-specific implementation details.

## Zero-budget baseline
- Prefer local/open-source utilities already available.
- Do not require paid APIs, subscriptions, paid credits, or user-supplied API keys.
- A free/open-source agent does not imply free model inference. Clearly report model limits, hardware requirements, and any usage caps.
- If a step cannot be performed with available free resources, stop and describe the limitation rather than silently switching to a paid service.
