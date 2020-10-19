# hello-world

## Basic happy path workflow
1. Set up a remote repo with a single branch called "main" with an empty README
   file
    - Click the green New button
    - Fill in the repository name as "hello-world" (without the quotes)
    - Check the README checkbox to create a new empty README file
2. Clone the repo to your local with **either**:
   git clone ssh://git@hgithub.com/mlflanagan/hello-world, **or**
   git clone https://github.com/mlflanagan/hello-world
3. Create a new branch called update-readme with:
   git branch update-readme
4. Check out the new branch with:
   git checkout update-readme
5. Edit the README file
6. Stage the file for commit
   git add README.md
7. Commit the change to your local repo with:
   git commit -m "Updated README file" to commit
8. Push your changes to the remote repo with:
   git push -u origin update-readme
9. On github, create a pull request:
   - Click the "main" dropdown button to see all branches
   - Select the update-readme branch. It will say something like "This branch
     is 2 commits ahead of main."
   - Click the "Pull request" link to create a pull request
   - Click the green "Create pull request" button
10. Merge the pull request with the main branch
   - Click the green "Merge pull request" button and click "Confirm merge"
   - You should see "Pull request successfully merged and closed. You’re all
     set — the update-readme branch can be safely deleted."
   - Click the green "Delete branch" button to delete the update-readme branch

## Notes:
- Check out and create the new branch with one command with:
  git checkout -b update-readme
- Show branches and the active branch with:
  git branch
- Combine add and commit steps with:
  git commit -am "commit message"
- After merging and deleting the update-readme branch, clean up your local repo
  with:
  - git checkout main to make the main branch active
  - git pull to merge the remote changes with the local main branch
  - git branch -d update-readme to delete the update-readme branch in the local
    repo

