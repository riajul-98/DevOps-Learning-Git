# DevOps-Learning-Git
Repository containing notes on git which I learnt through the CoderCo git module

## What is Git?
Git is a distributed version control system which allows users to collaborate on projects, track changes, merge code changes efficiently, manage branches and have a history of changes which is useful for rolling back to a previous version if needed.

## Why is Git so important
Git integrates with many DevOps tools such as CICD tools and cloud platforms. Provides developers with flexibility to manage their code. Git allows for accountability as you are able to see who made a specific change. Allows for developers to work on different aspects of the project simultaniously without interfering with each others work through the use of branching. These can then be combined using merging. This results in an improvement in efficiency as developers do not have to wait for other work to get completed first before starting on their part. Branching also allows developers to experiment with code without negatively impacting the project.

## Linking Local and Remote Repository
To link a local and remote repo, you would first create a remote repository such as on GitHub. You would need to first set up git on your system using the below commands;

`git config --global user.name "git-username"`
`git config --global user.email "example@example.com"`

Following this, you go back to your remote repository and copy the clone HTTPS link and run the below command;

`git clone https://github.com/git-username/repo-name.git`

## README Markdown File
The README file acts as documentation for your repository, providing an overview of your project as well as how to use it. It explains what the project is about, enabling readers to learn about the project, the functionality and what it is trying to solve. It also allows contributers to understand the project structure, how to get started and guidelines for contributions.

The README file is often the first thing contributers and users see when they view your repository and therefore a clear and informative README file can create a strong impression of the project.

## Git workflow
In order to push a files from your local repository to your remote repository, follow the below steps:
- `git add README.md`: Moves specified files from working directory to the staging area.
- `git status`: Shows the current repository status (optional but helpful)
- `git commit -m "Enter message here"`: Records a snapshot of the file at the time of the commit and adds a message.
- `git push origin main`: Pushes changes to the remote repository
- `git pull`: Updates local repository (handy when working in a team)

## Commits
Commits ensure code quality and also enables feedback within merge requests. This encourages collaboration. Records a snapshot of the file at the time of the commit and adds a message which helps isolate and document changes, making project management easier. Commits also records who made the change, allowing for accountability. It can be very useful when you need to revert to an older version of your code. 

### Commit Best Practices
- Commit often
- Write clear commit messages
- Use command style in messages
- Commit related changes together
- Test before committing
- Avoid commiting generated files
- Break down large changes
- Use consistent message styles
- Include references

## Branching
Branching allows developers to work on different features at the same time without affecting the main / production environment. This is useful as each feature can be developed and tested before merging back into the main branch. This means that any changes or bug fixes will not interfere or affect any other feature. New features can also be developed and tested in a separate branch before being merged into the main branch. 

## Pull Requests
