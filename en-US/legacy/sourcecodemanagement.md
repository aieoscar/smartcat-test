# Source Code Management

## Branches

- You can visit [Foonie Magus github Page](https://github.com/FoonieMagusn) for those repos.

- There are 4 type of branches. **Deployment Branch**, **Release Branch**, **Feature Branch** , **Developer Branch**, **Developer Feature Branch**,

  - **Deployment Branches** production, staging, beta, alpha, development
    - branches for different environments
    - alpha for internal testing
    - beta for external testing
    - staging for testing before promote to production, staging should have same setup as production.
    - make changes only by pull request. Prefer branch promotion path will be development -> alpha -> beta -> staging -> production.
    - run testing after push
    - only deploy to servers after all tests run success
    - reviewed
  - **Release Branches**
    - use Semantic versioning, X.Y.Z.
    - Major version X (X.y.z | X > 0) MUST be incremented if any backwards incompatible changes are introduced to the public API.
    - Minor version Y (x.Y.z | x > 0) MUST be incremented if new, backwards compatible functionality is introduced to the public API. It MAY be incremented if substantial new functionality or improvements are introduced within the private code
    - Patch version Z (x.y.Z | x > 0) MUST be incremented if only backwards compatible bug fixes are introduced. A bug fix is defined as an internal change that fixes incorrect behavior.
    - refer here for more details https://semver.org/spec/v1.0.0.html.
  - **Development Branches** master, develop, [feature_name]
    - [feature_name] is branch of feature in development
    - how many develoment branches are subject to the team's decision
    - make changes only by pull request
    - reviewed
  - **Developer Branches** , dev/[user name]/master
    - branch of developer
    - only commit and push by the developer name
    - developer can decide what to commit or push by himself/herself
  - **Developer Feature Branches**, dev/[user name]/[feature name]
    - branch of feature by developer
    - use this branch to submit pull request to **Development branch**
    - always use this for pull requst, since every push for a branch will count to the pull request fired.

- we use **branch pull request** instead of **repo pull request** for pull request before merging to **Development Branch**.

## Source Code Review Workflow

All code need to be at least reviewed by a senior developer before merging to the **Development Branch**.

- Create a **Developer Feature Branch** and develop the feature.

- Rebase from the **Development Branch** you are going to submit pull request.
- Push your branch to public repo.

- Submit a pull request via github from the branch you just pushed against the **Development Branch** branch. Add reviewer in the pull request. Sometimes, against **Feature Branch**, depends on situation.

- Update appropiately based on reviewer's comments.

- You can then merge the branch once the pull request has been accepted.

- Delete the **Developer Feature Branch** if it will not be used anymore.

- You can visit following link to know more about different workflow. https://www.atlassian.com/git/tutorials/making-a-pull-request

- When to promoting **Development Branch** from **Release Branch** is subject to your team's own decision.

- **Warning** rebase is not encourage if the branch has already been reviewed. It is acceptable before review. There are 2 main reasons.
  - Rebase need to use force push to get rid of remote branch. Since force push is super danger.
  - After review, rebase with conflict will remove history of merge. If there are problem in conflict resolution, the action is not reversible after you force push.

## Source Code Unit Test

TBD
