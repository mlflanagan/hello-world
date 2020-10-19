# hello-world

## Basic happy path workflow
1. Set up a remote repo with a single branch called "main" with an empty README
   file
    - Click the green New button
    - Fill in the repository name as "hello-world" (without the quotes)
    - Check the README checkbox to create a new empty README file
2. Clone the repo to your local with:
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
8. Push your changes to teh remote repo with:
   git push -u origin update-readme

## Notes:
- Check out and create the new branch with one command with:
  git checkout -b update-readme
- Show branches and the active branch with:
  git branch
- Combine add and commit steps with:
  git commit -am "commit message"

