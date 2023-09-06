# zendrix-workflow

Master Branch (prod):
The master branch should always represent the latest production-ready code.
Releases will be tagged from this branch on the 25th of every month.

Develop Branch (dev):
Create a develop branch to serve as the integration branch for ongoing development work.
All feature branches and bug fixes should be merged into this branch when they are ready for testing and integration.
Continuous Integration (CI) pipelines should be set up to automatically build and test the code from the develop branch.

Feature Branches (feature/<feature_name>):
Developers should create feature branches based on the develop branch for their respective tasks.
Naming convention for feature branches: feature/<feature-name> or feature/<issue-number>.
Once a feature is complete and tested, it should be merged back into the develop branch.

Release Branches:
Naming convention for release branches: release/<release-version>.
Any bug fixes or fine-tuning for the release should be done on the release branch. QA and testing should occur on the release branch.

Hotfix Branches:
If critical bugs or security issues are discovered in production, create a hotfix branch based on the master branch.
Naming convention for hotfix branches: hotfix/<issue-number> or hotfix/<description>.
Once the hotfix is complete, it should be merged into both master and develop branches to ensure that the fix is applied to the latest production code as well as the ongoing development code.
