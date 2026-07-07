LOCK RELEASE GITHUB UPDATE SYSTEM

How updates work:
1. Upload this LockReleaseElectron folder to a GitHub repository.
2. GitHub Actions builds a Windows app ZIP on every push to main/master.
3. The app checks the latest GitHub Release every time it opens.
4. If a newer release exists, it asks to download and install it.

Important:
- The repository should be PUBLIC unless you add GitHub token support.
- GitHub Actions must be enabled for the repository.
- The workflow automatically sets update-config.json to your repo name when GitHub builds the release.
- The app keeps your database folder during updates.

For your first GitHub release:
1. Create a new GitHub repository.
2. Upload everything inside this LockReleaseElectron folder to the repo root.
3. Commit/push to main.
4. Wait for the Actions tab to finish.
5. Go to Releases and confirm Lock_Release_Windows.zip exists.
6. Install/open a GitHub-built release once. After that, updates are automatic on app open.

Local test build:
If you build locally with BUILD REAL APP.exe, edit github-repo.txt in the outer folder first.
Example:
jacpelletie07/Lock-Release

Then run BUILD REAL APP.exe.
