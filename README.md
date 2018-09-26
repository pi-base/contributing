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
- If the branch changes are acceptable, they should be merged into master
  using the server command-line tools.
  - Using a machine that has shared a public key with GitHub, ssh using
    `ssh username@server.pi-base.org`. (If this does not work, contact
    <jamesdabbs@gmail.com>.)
  - Move into the data repo with `cd /app/data/repo.git`
  - Use `pibase branch` commands merge the reviewed branch into `master`
  - This triggers the update of the GitHub repo, closing the PR (TODO does it?)
- If the branch changes are unacceptable (e.g. lacking references), 
  discussion can take place on the GitHub PR.
  - The user can resubmit new changes.
  - If the changes are abandoned, the user's branch can be archived and
    replaced with master (by request of the user).
