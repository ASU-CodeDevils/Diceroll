# Contributing
Contributions are always encouraged and welcome!

## Get Started
1. Clone the repo localy `git clone https://github.com/ASU-CodeDevils/Diceroll.git`
2. Create a branch for local development `git checkout -b some_meaningful_branch_name`
3. Commit and push changes regularly with `git commit -m "Write a short meaninful msg."`
4. When the user story is ready for test, submite a pull request on github.

## Detailed Workflow
- All User Story and feature development will take place in separate branches that will be branched from the Development branch.
  - Each US will be branched and development for that US will be kept separate from the Development branch.

    - All commits will have a proper title and more detailed information section
    - Commits should be made often.
    - Commits shall be grouped in a logical way, with files that belong with each other and pertain to the commit title.
    - Commits shall be pushed to the remote repository often, at a minimum of at the end of each coding session.

  - When a US is done, the Development branch will be merged into the US branch and tested so that the commit to the Development branch will be a
    Fast Forward.

  - When a US is ready for merge back into Development a pull request will be created
    - Each pull request will be reviewed by a separate team member and then will be approved for merge.
    - Reviews of Pull Requests shall include good comments

  - Any time the Development branch changes, it will be announced in the dice-roll-GitHub channel.
    - All team members should merge the new Development branch into their US as soon as possible

  - When the Development branch is complete for the Sprint a pull request will be made to merge it back into master
    - All merges to master shall be fast forwards
    - Pull requests to master will be tested and reviewed by at least two team members
    - Once reviewed by two team members the Project Lead will approve the Pull Request for merge into master
