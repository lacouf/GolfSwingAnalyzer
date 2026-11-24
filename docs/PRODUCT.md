# Product outline

## User problem

Reviewing a long practice recording to find useful swings is tedious. The app should make it quick to find, replay, and compare swings from two complementary camera angles.

## Intended first user

A golfer practicing with two recent iPhones on tripods, recording a few minutes of swings and importing the recordings to a MacBook.

## MVP workflow

1. Import two separate videos and label each as down-the-line or face-on.
2. Align the recordings using a shared visible light cue, with manual offset adjustment as a fallback.
3. Find swing segments, initially allowing the user to mark or correct them.
4. Select two swings and compare the synchronized views side by side.
5. Draw a 2D skeleton overlay from estimated body landmarks on each view.

## MVP boundaries

- macOS app; local video processing and storage.
- No launch monitor integration, cloud account, 3D body reconstruction, automatic coaching diagnosis, or paid content.
- The overlay is a visual aid. It should indicate uncertain or missing landmarks rather than imply exact joint tracking.

## Success criteria

- User can import the two recordings without transcoding them manually.
- User can align the videos and inspect the same swing in both views.
- User can compare two swings without scrubbing through the full practice session.
- The pose overlay remains understandable when some joints are occluded or uncertain.
