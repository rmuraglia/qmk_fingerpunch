how I set up this second fork of qmk, since the git ui wouldn't let me:

1. create dir: `mkdir qmk_fingerpunch`
2. cd in: `cd qmk_fingerpunch`
3. create the repo: `git init`
4. add fingerpunch as a remote: `git remote add upstream git@github-personal:sadekbaroudi/qmk_firmware.git`
5. fetch his code: `git fetch upstream`
6. make my main branch that tracks his master: `git checkout -b main upstream/master`
7. add my fork as a remote: `git remote add origin git@github-personal:rmuraglia/qmk_fingerpunch.git`
8. push the branch up: `git push -u origin main`

This repo now tracks `rmuraglia/qmk_fingerpunch` as origin and `sadekbaroudi/qmk_firmware` as upstream for ease of pulling in his future changes.
