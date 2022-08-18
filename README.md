# Bulk run frontend tests. | [![Frontend tests health](https://github.com/gp201/oppia-frontend-tests-oppia/actions/workflows/frontend_tests_health.yml/badge.svg)](https://github.com/gp201/oppia-frontend-tests-oppia/actions/workflows/frontend_tests_health.yml)

This is an action that allows you to bulk run (50 times) the frontend tests for a specific PR made to [Oppia](https://github.com/oppia/oppia).
This can be useful for checking if your changes are breaking or introducing a flake in the frontend tests.

> **Note**  
> The staus badge (Frontend tests health) for the health of the frontend test for the latest develop branch is displayed above.
> Every week the health of the frontend tests for the latest develop branch are updated. 


## How to run bulk run the frontend tests

1. Fork the repository
2. Go to the actions tab and click the `Frontend tests flake check` action.
3. Click the `Run worlfow` button. A dialog will open asking the following inputs.
    - `Flags` (Optional): The flags to be passed to the frontend tests. Default is `--run_minified_tests --skip_install --check_coverage --verbose`.
    - `Run frontend tests for a specific PR` (Required): The PR number to run the frontend tests for.
    - `Reason` (Optional): The reason for running the frontend tests.
    - `Store karma coverage report as an artifact` (Optional): Whether to store the karma coverage report as an artifact.
4. Click the `Run worlfow` button (Green in color).
5. The frontend tests will be run for the given PR number. It will take approximately 30 minutes to run the tests.

## How to sync the fork.

Follow the instructions provided in the [GitHub Docs](
https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork#syncing-a-fork-branch-from-the-web-ui) to sync the fork.
