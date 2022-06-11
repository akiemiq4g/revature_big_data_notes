# amplifier_notes_week_1

# These are the Amplifier group notes for week 1 of Big Data. Changes and corrections are welcome

Checklist for contributing a bug fix or feature to an open source GitHub repo
Set up a virtual env
GitHub's contributing to open source guidelines
Example from kinto on how to contribute
GitHub workflow
Contribute checklist:

Fork repository and clone locally. Detailed instructions to sync a fork of a repository to keep it up-to-date with the upstream repo.
Create a branch for local development: git checkout -b name-of-your-bugfix-or-feature
Commit your changes and push your branch to GitHub:
git add .
git commit -m "Your detailed description of your changes."
git push origin name-of-your-bugfix-or-feature
Submit a pull request through the GitHub website.
When contributing a bug fix:

Write a test that reproduces the problem. It should fail because of the bug.
Fix the faulty piece of code.
The test should now pass.
When contributing a new feature:

Do not rush on the code.
Step by step, you'll write tests for each aspect and each edge case of the feature.
Start very small: one simple test for the simplest solution.
Check tests still pass for CI
Write docs for new feature
Iterating with test driven development

Add a new test that will fail because the code does not handle the new case.
Make the test pass with some new code.
Track your changes: git add -A
Refactor and clean-up if necessary. If you're lost, go back to the previous step with: git checkout <file>
Commit the changes: git commit -am "feature X"
Go to step 1
Pull request guidelines

Open a pull request even if contribution is not ready. It can be discussed and improved collaboratively. There will be a discussion about the proposed changes.
The pull request should include tests.
If the pull request adds functionality, the docs should be updated.
Travis CI integration tests should be green. It will make sure the tests pass with every supported version of Python.
