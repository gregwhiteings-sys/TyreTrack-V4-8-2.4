TYRETRACK V4.8.2 — CORRECTED WINDOWS GITHUB REPOSITORY

FIX: Previous kit explicitly imported scipy._cyutility, which is not provided by pinned SciPy 1.13.1. This kit removes that incorrect import and tests YOLO model.track() directly, including inside the packaged EXE.

IMPORTANT: GitHub website uploads do not reliably preserve hidden .github folders.

EASIEST METHOD — GITHUB WEB UPLOAD:
1. Create a new empty repository.
2. Extract this ZIP to your PC.
3. Select ALL top-level files (not the containing folder) and upload to GitHub root; commit.
4. Click Add file > Create new file; enter exactly .github/workflows/build-windows.yml
5. Open the extracted .github/workflows/build-windows.yml in Notepad, copy ALL text into GitHub new file, commit.
6. Go to Actions > Build TyreTrack Windows - SciPy Fixed > Run workflow (main).
7. After green success, download the artifact from Summary > Artifacts.

Alternative: upload the repository with Git command line (git add -A) to preserve folders.

This is the CPU-only V4.8.2 single-camera app, not V5 dual camera.
The workflow includes model.track() checks in Python and the packaged EXE, but real-world tyre counting must still be tested.
