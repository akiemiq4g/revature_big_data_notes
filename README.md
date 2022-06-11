# amplifier_notes_week_1

# These are the Amplifier group notes for week 1 of Big Data. Changes and corrections are welcome

# Checklist for contributing a bug fix or feature to an open source GitHub repo
* Set up a virtual env
* GitHub's contributing to open source guidelines
* Example from kinto on how to contribute
* GitHub workflow

### Contribute checklist:

* Fork repository and clone locally. Detailed instructions to sync a fork of a repository to keep it up-to-date with the upstream repo.
* Create a branch for local development: git checkout -b name-of-your-bugfix-or-feature
* Commit your changes and push your branch to GitHub:


> git add .

> git commit -m "Your detailed description of your changes."

> git push origin name-of-your-bugfix-or-feature
 
* Submit a pull request through the GitHub website.

#### When contributing a bug fix:

1. Write a test that reproduces the problem. It should fail because of the bug.
2. Fix the faulty piece of code.
3. The test should now pass.


#### When contributing a new feature:

1. Do not rush on the code.
2. Step by step, you'll write tests for each aspect and each edge case of the feature.
3. Start very small: one simple test for the simplest solution.
4. Check tests still pass for CI
5. Write docs for new feature


#### Iterating with test driven development

1. Add a new test that will fail because the code does not handle the new case.
2. Make the test pass with some new code.
3. Track your changes: git add -A
4. Refactor and clean-up if necessary. If you're lost, go back to the previous step with: git checkout <file>
5. Commit the changes: git commit -am "feature X"
6. Go to step 1
  
#### Pull request guidelines

1. Open a pull request even if contribution is not ready. It can be discussed and improved collaboratively. There will be a discussion about the proposed changes.
2. The pull request should include tests.
3. If the pull request adds functionality, the docs should be updated.

