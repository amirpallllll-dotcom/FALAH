# Reference Analysis Record — Draft Schema

This is a human-readable schema for the first analysis reports. It is not yet an implemented parser.

## Media metadata
- filename:
- duration:
- width / height:
- frame_rate:
- audio_present:
- audio_notes:
- analysis_coverage:

## Shot record
Each shot should include:

- shot_id:
- start_time:
- end_time:
- confidence: verified | estimated | unknown
- visual_summary:
- characters:
  - identity/design:
  - action:
  - body mechanics:
  - posture/weight shift:
  - facial expression:
  - gaze:
- camera:
  - shot_size:
  - angle:
  - movement:
  - framing/composition:
- environment:
  - setting:
  - background_motion:
  - props:
- visual_effects:
- transition_in / transition_out:
- narration_or_dialogue:
- sound_effects / music:
- timing_beats:
- reusable_style_principles:
- scene_specific_choreography_not_to_copy:
- open_questions:

## Separation rule
The `reusable_style_principles` field may inform the Style Bible.
The `scene_specific_choreography_not_to_copy` field documents what happened in the reference but must not become a default action preset.
