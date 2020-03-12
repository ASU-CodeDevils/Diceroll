### Quality Policy
**GitHub Workflow**
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

**Static Analysis
  TODO - code style enforcement (possibly use ES Lint)


**Continuous Integration testing
  - All commits will be automatically tested using Travis-CI integration in GitHub.
  - No branches shall be merged into Development or Master without passing Travis CI tests on their most recent commit.

**Functional Testing
  - Function testing shall be conducted by developers as they implement and change features.
  - Additional function testing shall be conducted by team-members when they are reviewing code for pull-requests.

**Code Review**

  All new code will be reviewed by at least the Developer and one additional reviewers prior to merging into the Development branch. Two independent reviewers will review code prior to merge into the Master branch. The checklists below will be utilized and copied into the comments of the pull request review.

**Code Review Checklist**

#### Codestyle

1. No hardcoded values, use constants values.
2. Avoid multiple if/else blocks.
3. No commented out code.
4. No unnecessary comments: comments that describe the how.
5. Add necessary comments where needed. Necessary comments are comments that describe the why.

#### ES6/7

1. Use ES6 features.
2. Use const over let (avoid var).
3. Use import and export.
4. Use template literals.


#### React code review

1. Are components have defined propTypes?
2. Keep components small.
3. Functional components for components that don't use state.
4. No api calls in containers, delegate to Sagas
5. No state updates in loop.
6. No useless constructor.
7. Minimize logic in the render method.
8. Don’t use mixins, prefer HOC and composition.

#### ESLint

1. Code has no any linter errors or warnings.
2. No console.logs.

#### CSS/CSS in JS

1. Consistent naming conventions are used (BEM, OOCSS, SMACSS, e.t.c.).
2. CSS selectors are only as specific as they need to be; grouped logically.
3. Is any 'CSS in JS' library was used?
4. Use Hex color codes #000 unless using rgba().
5. Avoid absolute positioning.
6. Use flexbox.
7. Do not animate width, height, top, left and others. Use transform instead.
8. Use same units for all project.
9. Avoid inline styles.

#### Testing

1. Does the code function properly.
2. Are there any uncaught exceptions?
3. Does the use of edge case values return expected results?

#### Git

1. Commits are small and divided into logical parts.
2. Commits messages are small and understandable.
3. Use branches for new features.
4. Make sure no dist files, editor/IDE files, etc are checked in. There should be a .gitignore for that.

#### Other

1. Security.
2. Usability.
