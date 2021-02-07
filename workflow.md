
## The Workflow

`master` represents the official history and should ALWAYS be deployable. For each feature, a developer creates a new branch. For clarity, make sure to add your name as prefix and use descriptive names like `biruk.github-workflow` for your branches.

To create a branch:

1. Checkout to master: 
    * `git checkout master`
2. Pull latest changes: 
    * `git pull`
3. Create a new branch and switch to it: 
    * `git checkout -b your-name.new-feature-branch`
    
### Branch management

While working on a new feature branch, it is a good idea to commit often. This allows to move forward without fear since if something goes wrong you can revert back easily without losing too much work. Keep in mind that it's better to divide the work into small chunks so that each commit is easily digestible by every developer.

### Commit your code

1. Get the status:
    * `git status`
    
    This command will give you a list of all the updated, added and deleted files. 

2. Files can be added individually or all at once:
    * `git add FILE` or `git add -A`

3. Now we are ready to create a commit with changes:
    * `git commit`

This will open selected text editor two write a commit message. 

If the change is not complicated:

    * `[CHANGE_TYPE] + one line commit message` 

If the change is complicated: 
    
    * `[CHANGE_TYPE] + one line commit message + an empty line + detailed explanation lines`

A good commit message would look like:
    
    * `[doc] Add Github workflow`

As seen above, we prefer to use imperative form for simplicity. The change type is in brackets. Some other examples of change type could be your team's name or specific technology like `[mobile], [map], [web], [db]` etc.

Please be consistent and follow the conventions.

### Create a Pull Request

- To push the new feature branch to the remote repo, simply do the following: 
    * `git push -u origin your-name.new-feature-branch`
    
At this point, you are ready to create a `Pull Request` for the new feature.


1. Click on `compare and open pull request` on the project site. (should come up after pushing your branch to github) 
2. Add `one or two` reviewers.
3. Click `open pull request`

The reviewers should review the PR in **24 hours** and leave their comments. Note that we do not allow any direct pushes to masters without creating a PR and getting an approval from reviewers. Once you addressed all the comments on your PR, it's time to push your changes.
- In case of a merge conflict, you can resolve the conflicts either on the github online editor or offline then commit the changes to make

1. Click on the merge and commit dropdown and select the squash and merge option.

Congratulations! You are ready to contribute!

*Guide adapted from the A2SV contributors guide*
