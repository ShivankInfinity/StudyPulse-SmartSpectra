# StudyPulse SmartSpectra

StudyPulse is an Android app that uses the Presage SmartSpectra SDK to estimate student focus readiness from camera-based vitals.

## Inspiration

Students often study, code, or prepare for exams while tired, stressed, or mentally overloaded. They may not realize when their body is showing signs that they should take a short reset before deep work.

StudyPulse was built to explore how camera-based vitals can help students make better study decisions.

## What it does

StudyPulse uses the SmartSpectra SDK to collect camera-based vitals such as:

- Pulse rate
- Breathing rate
- HRV RMSSD
- Facial expression
- Breathing and arterial pressure waveforms

The app then converts pulse, breathing rate, and HRV into a simple student focus-readiness result:

- Ready to Focus
- Light Study Recommended
- Reset Needed
- Recovery First

It also gives a short recommendation, such as starting a focus session, doing light review, or taking a reset break.

## How to use it

1. Open the Android app.
2. Allow camera permission.
3. Tap Start.
4. Wait for SmartSpectra to collect vitals.
5. Read the StudyPulse Focus Readiness result and recommendation.

## How it was built

StudyPulse was built using:

- Kotlin
- Android Studio
- Presage SmartSpectra SDK
- Android Camera PreviewView
- Rule-based focus-readiness logic

The SmartSpectra SDK provides camera-based measurements. StudyPulse adds a student-specific interpretation layer on top of those vitals.

## Focus-readiness logic

The app uses a simple risk score:

- Pulse rate above 100 adds 1 risk point
- Breathing rate above 22 adds 1 risk point
- HRV RMSSD below 40 adds 1 risk point

Result mapping:

- 0 risk points: Ready to Focus
- 1 risk point: Light Study Recommended
- 2 risk points: Reset Needed
- 3 risk points: Recovery First

## Screenshots / Demo

Screenshots or a short demo video will be added after running the app with the SmartSpectra API key.

## Disclaimer

StudyPulse is for wellness and productivity awareness only. It is not a medical device and does not diagnose, treat, or prevent any medical condition.
