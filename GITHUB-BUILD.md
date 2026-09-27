# GitHub Windows EXE Build

1. Create a new GitHub repository.
2. Upload the contents of this folder to the repository root.
3. Keep `.github/workflows/build-exe.yml` in place.
4. Commit to `main`.
5. Open **Actions** → **Build FRIDAY Windows EXE**.
6. Select **Run workflow**.
7. After the run succeeds, download **FRIDAY-Windows-EXE** from Artifacts.

The project source files are already at repository root. Do not upload the outer ZIP folder as an extra directory.

The workflow installs runtime dependencies directly from the project's `pyproject.toml` dependency list and builds:
- `FRIDAY-Server.exe`
- `FRIDAY-Voice.exe`

API credentials should not be committed. Create a `.env` locally from `.env.example` when running the application.
