## Git Commands

- `git push || pull`, will sync every branch between remote and local
- `git push || pull branch_name`, will sync only that particular branch


## Rules for working
- Pull the updated code from the remote `git pull`.
- Checkout to main `git checkout main`.
- checkout to new branch from the updated code(main) `git checkout -b branch_name`.
- Complete the work and do commits on the Work Branch.
- Before pushing the Work branch to remote,
    - Again Pull the Updated code from remote(main).
    - using `git merge main` merge the updated in your work branch.
    - `git merge main`: check the status of work branch with the main, 
        - if work branch is ahead of main then it will do the merging.
        - if any conflicts are there, conflicts will be displayed in the merge changes. staged changes will have no conflicts files.
        - Resolve the conflicts and do commit.
- Push the updated codde to the remote.
- create a Pull Request to merge work branch into the main.