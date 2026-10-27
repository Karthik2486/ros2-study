# Failure log

## YYYY-MM-DD, Chapter N, Exercise N.N
- Symptom: what I saw
- Expected: what I predicted
- Diagnosis: what was actually wrong, and how I found out
- Fix:
- Lesson:

## 2026-10-27, Setup, study repo
- Symptom: build/install/log were committed despite .gitignore, and git status listed my whole home folder.
- Expected: only README, failure-log and .gitignore would be committed.
- Diagnosis: I ran git init and created the files in ~ instead of ~/ros2-study. .gitignore rules are relative to the file's location, so they matched nothing.
- Fix: moved ~/.git aside, moved the files, ran git init in ~/ros2-study, and force-pushed.
- Lesson: check the prompt or run pwd before git init. A command run in the wrong folder still "works".
