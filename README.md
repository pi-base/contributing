# contributing
README for contributors/reviewers

## Reviewer workflow

- Contributions are received via pull requests on the GitHub data repo.
  - <https://github.com/pi-base/data/pull/>
  - A list of touched files is given, but to review their connections and
    make tweaks, it's best to check those changes in the viewer.
  - To check changes, log into the viewer, then change your branch as
    appropriate.
    - If you don't have access to the branch under review,
      (TODO add instructions to add permissions in the database)
  - Minor editorial changes can be made directly like this.
  - More involved editorial changes (made via discussion with the contributor)
    may be made by cloning the repo on the server and manipulating it directly.
    - `git clone /app/data/repo.git ~/data`
    - `git checkout branchname`
    - make your changes
    - `sudo git push origin branchname:branchname` 
    - `sudo chown -R pibase /app/data/repo.git`
- If the branch changes are acceptable, they should be merged into master
  using the server command-line tools.
  - Using a machine that has shared a public key with GitHub, ssh using
    `ssh username@server.pi-base.org`. (If this does not work, contact
    <jamesdabbs@gmail.com>.)
  - Move into the data repo with `cd /app/data/repo.git`
  - Use `pibase branch` commands merge the reviewed branch into `master`
    - For now, use `sudo`, followed by `sudo chown -R pibase /app/data/repo.git`
      to handle file permission issues
  - `git push` from the repo to update the GitHub repo, closing the PR
- If the branch changes are unacceptable (e.g. lacking references), 
  discussion can take place on the GitHub PR.
  - The user can resubmit new changes.
  - If the changes are abandoned, the user's branch can be archived and
    replaced with master (by request of the user).
