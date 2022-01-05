# Github for Group Project

- Not going to be doing branching at this time
- Working on one main branch / timeline, but both partners pushing commits
  
## Steps
1. Create an organization
2. Create a repository that belongs to the organization
3. Invite other team member to organization
   - Make them an owner
   - Make them a collborator
4. Clone repository locally `git clone REPOSITORY_URL`
5. Create README
6. `add`, `commit`, and `push` the README
   
Other team member will
    - Accept invitation
    - Clone repository 

## Workflow

1. Add, commit, and push like normal
   `git push origin main`
2. To get up to date, so a pull
   `git pull origin main`

## Merge Conflicts

- When both team members change the same line in the same file, a merge conflict will occur. This is how git says that it doesn't know how to merge the changes together.

- A merge conflict will happen after you run git pull. You will need to handle the merge conflict before continuing work.

When a merge conflict occurs:

1. Use `git status` frequently to check out what's going on.

2. Fix the conflicting file. Either:

    - Manually edit the file and put it into the state that you want.
    - Use one of the commands below to use one version of the file. `git checkout --ours FILE` to use your version,`git checkout --theirs FILE` to use your team's version

3. `git add` the conflicting file(s).

4. `git commit` to conclude the merge.

Git will prepopulate a commit message for the merge. You can simply save and exit your text editor at this point.

## Helpful Commands

During a merge conflict (Replace `FILE` with your specific file):

- Use your version of the file:

    >`git checkout --ours FILE`

- Use the version of the file from GitHub:

    >`git checkout --theirs FILE`

- Return the file to the original conflicted state:

    >`git checkout -m FILE`

### Avoiding Merge Conflicts

- Each team member should have their own "working" notebook so that two people aren't editing the same notebook.
- Eventually the individual works will be merged to a final notebook.
- Communicate clearly about who is working in this final notebook, only one person should be adding, comitting, and pushing this notebook at a time.