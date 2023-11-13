# OML_GPT

[![Build Status](https://app.travis-ci.com/melaasar/cs130-template.svg?branch=master)](https://app.travis-ci.com/github/melaasar/cs130-template)
[![Release](https://img.shields.io/github/v/release/melaasar/cs130-template?label=release)](https://github.com/melaasar/cs130-template/releases/latest)

This repo serves as a template for a repository that follows the Scrum process. The following information describes how the native features/workflows of Github can be customized to work in a scrum development process.

## Issues

An issue is a unit of tracking work. Issues can be classified into different classes using `labels`. This can be used to classify issues in the scrum process as follows.

### Epic

An [epic](https://dev.to/jorenrui/a-look-into-how-i-manage-my-personal-projects-my-git-github-workflow-1e7h#epic-issue) is an issue with the label `epic`. It represents a large story that can be broken into stories, which can be addressed over multiple sprints. An epic issue references its story issues as a task list in its description. A Github action has been added to automatically check/uncheck the story task items when they get closed/reopened.
1. Asynchronous Processing\
Develop and implement the API necessary for transforming the natural language into SPARQL.

2. User Interaction\
Develop the user interface to interact with the OML GPT, submit queries UI, and receive responses.

3. ChatGPT Integration\
Using the ChatGPT model for natural language understanding and response generation, which makes sending the SPARQL query back easier.

4. API Development\
Create and integrate backend application programming interfaces (APIs) that convert natural language inquiries into SPARQL queries and then translate the results back into comprehensible natural language answers.

5. Documentation and Training\
Create comprehensive documentation and provide training materials for future developers and users.
Develop thorough documentation and prepare educational content for the orientation and use of subsequent developers and users.

6.Deployment and Monitoring\
Launch the application in a live production setting and establish suitable systems for monitoring and logging to ensure smooth operation.

### Story

A [story](https://www.atlassian.com/agile/project-management/epics-stories-themes) is an issue with the label `story`. It may represent a new feature or an enhancement to an existing feature. A story issue can be broken into sub-tasks, which are added as a task list in the description of the story issue. These sub task items can be checked manually by the developer to indicate completion.
1. Parse Query Results\
As a backend service, my goal is to transform the results from SPARQL queries into a structured format that ChatGPT can interpret, enabling it to convert these results into comprehensible natural language.

2. Submit Query\
As a user, I want to use the natural language to ask questions since I can phrase the questions in the most familiar way.

3. Generate SPARQL Query\
As a backend service, I hope to get the SPARQL Query which is converted from the natural language, so I can get the data from the SPARQL directly. 

4. API Development\
As a backend developer, I want to design and implement APIs that can translate natural language queries into SPARQL queries, so that the system can understand and process user requests efficiently.

5. Documentation and Training\
As a technical writer, I want to create detailed documentation and training materials for the system, so that future developers and users can easily understand and use the application.

6. Deployment and Monitoring\
As a DevOps engineer, I want to deploy the application in a production environment with effective monitoring and logging, so that we can ensure its continuous operation and quickly address any issues that arise.

### Bug

A bug is an issue with the label `bug`. It represents a problem with the existing code that needs to be fixed.

### Question

A question is an issue with the label `question`. It represents a question raised by anyone that may get converted into other types of issues.

## Labels

In addition to the [standard labels](https://docs.github.com/en/free-pro-team@latest/github/managing-your-work-on-github/managing-labels#about-default-labels) above, you can add new labels to issues to classify them into different classes like `documentation`, `frontend`, etc, or to add metadata like `duplicate`, `invalid` etc.

## Milestones

A [milestone](https://docs.github.com/en/free-pro-team@latest/github/managing-your-work-on-github/tracking-the-progress-of-your-work-with-milestones) groups issues that are expected to be delivered at some point in time. It also allows ordering (prioritizing) these issues and tracking their progress (percentage of issues completed so far). In the scrum context, a milestone can be used as a sprint. So, you can create your sprints and give them names like Sprint1, Sprint2, etc., and set their due dates respectively.

## Projects

A [project](https://docs.github.com/en/free-pro-team@latest/github/managing-your-work-on-github/tracking-the-progress-of-your-work-with-project-boards) is a kanban-style board that can aggregate a set of issues for any purpose. In the scrum context, we can create one project called `Scrum Board` and choose its template as `Automated kanban with reviews`. (This will create a set of initial notes that you can delete).

## Scrum Boards
### Scrum Board (Frontend)
| Task                                                                                         | Implementation Status    | Team Member Assigned |
|----------------------------------------------------------------------------------------------|--------------------------|----------------------|
| Set up the project structure using React                                                     | Done                     | Ziwei                |
| Configure build tools                                                                        | Done                     |                      |
| Create mockups for the UI, showing how the user will interact with the system                | Done                     |                      |
| Define the color scheme, typography, and overall style guide                                 | Done                     |                      |
| Develop reusable components such as buttons, input fields, modals, etc.                      | Done                     |                      |
| Implement the UI for users to submit queries                                                 | Done                     |                      |
| Basic layout and navigation structure                                                        | Done                     |                      |
| Set up services to interact with the backend API endpoints                                   | In-progress              |                      |
| Handle HTTP requests and responses, including error handling                                 | In-progress              |                      |
| Implement the UI for displaying the results in natural language                              | In-progress              |                      |
| Handle form submission and validation on the client side                                     | To-do                    |                      |
| Ensure the state updates are reflected across the UI components                              | To-do                    |                      |
| Create components for displaying the status of the submitted query (loading, success, error) | To-do                    |                      |
| Implement the mechanism to submit user feedback on responses                                 | To-do                    |                      |
| Pagination or scrolling for results                                                          | To-do                    |                      |

### Scrum Board (Backend)
| Task                                                                              | Implementation Status | Team Member Assigned |
|-----------------------------------------------------------------------------------|-----------------------|----------------------|
| Set up version control                                                            | Done                  | Ziwei                |
| Define directory structure and initial files                                      | Done                  |                      |
| Set up virtual environment and dependencies                                       | Done                  |                      |
| Basic Django project setup with REST framework integration                        | Done                  |                      |
| Initial models, views, and URLs                                                   | Done                  |                      |
| Define UserQuery model                                                            | Done                  |                      |  
| Set up basic task to handle background processing                                 | Done                  |                      |
| submit-query API: Receive queries and start background job                        | Done                  |                      |
| query-status API: Check the status of a background job                            | Done                  |                      |
| fetch-result API: Retrieve the final result from a background job                 | Done                  |                      |
| Set up the testing framework and write initial tests                              | In progress           | Zeyu                 |
| Integrate ChatGPT for natural language processing                                 | In progress           |                      |
| Develop the logic to translate natural language queries to SPARQL queries         | To-do                 |                      |
| Implement and test the execution of SPARQL queries against the endpoint           | To-do                 |                      |
| Develop and test logic to parse SPARQL results into a format suitable for ChatGPT | To-do                 |                      |
| Install and configure Celery with Redis for asynchronous processing               | To-do                 |                      |



## Branches

The `master` branch is the main branch used for releases. Other branches can be created. For example, a branch called `gh-pages` is often used to create a website for the repository (for more information check this [link](https://pages.github.com/)). Other branches can be created to address the issues of the repository, one branch per issue (called an `issue` branch). Such branches can then be used to create pull requests, where they get peer-reviewed and eventually merged into the `master` branch. For more information on branches, check this [link](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/about-branches).

## Pull Requests

A [pull request](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/about-pull-requests) is a request to merge commits from one branch to another branch. This is typically used to merge commits from an `issue` branch into the `master` branch. A pull request is how the process of peer review is carried out. Reviewers can comment on the code changes to show approval or request changes (which will need to be addressed by additional commits to the `issue` branch). When a CI pipeline is configured for a repository (see below), it will run on any `issue` branch that is part of a pull request. When the peer review process has concluded, the new commits can merged into the `master` branch. The recommended merge option is `Squash and merge`, (i.e., squash all commits into a single commit) since it makes the repository's history simple and linear.

## Tags

Tags can be used to mark release points in a repository's commit history. Typically, after some work goal has been achieved, with a set of commits, a tag (typically a version number like 1.0.0, 1.0.1, etc.) is [pushed to the respository](https://stackoverflow.com/questions/18216991/create-a-tag-in-a-github-repository) to mark this point. This results in the tag showing up in the repository's [tags page](https://docs.github.com/en/free-pro-team@latest/github/administering-a-repository/viewing-your-repositorys-releases-and-tags).

## Workflows

### Creating issues

An issue can be created from the `issues` tab of a repository. An issue type (bug, story, epic, question) is first chosen then its corresponding template can be sufficiently filled.

### Triaging issues

The Product Owner goes frequently to the `Scrum Board` project and clicks on the `Add Cards` link to triage new issues in the repository to the board's `To do` column, which acts here as the `Product Backlog`. Product Owner can also added unbaked ideas to the `To do` column as notes, which are placeholders that can later be converted into issues. Issues and notes can then be ordered in the `To do` column to show their priority.

### Planning sprints

The Scrum Master creates a new milestone and gives it a suitable name (e.g., Sprint1) and a due date. Then, in the `Scrum Board`, issues from the top of the `To do` column (assuming they have been ordered based on priority) can be assigned to that milestone and to the developers who will work on them.

### Working on issues

Developers go to the `Scrum Board` where they can filter it for the issues assigned to them in a given milestone. They can pick ones to work on by moving them to the `In progress` column (this is important since this is not automated).

### Reviewing progress

In the daily standup, the `Scrum Master` can review progress by going to the `Scrum Board` and filtering it by the current milestone (sprint). Developers can then reference issues in the various columns when they answer the usual standup questions, e.g., issues they work on (`In progress`), finished (`Done`), or yet to work on (`To do`).

### Working with issue branches

Before developers can work on an issue, they should check out and pull the `master` branch to ensure that they have all the latest commits locally. Then, they should create a new local `issue` branch and name it `issue-[number]` (replacing `[number]` with the issue number). Several `issue` branches can be created concurrently, one for each issue, but it is important to make them independent from each other by checking out the `master` branch before creating each of them. This allows them to be pushed and merged independently from each other (and with the least conflicts).

Each `issue` branch can accumulate commits to address the issue. When ready, it can then be pushed to a corresponding remote branch that can then be used to create a pull request into the `master` branch. The pull request template needs to be filled at this point. Once created, a pull request can be reviewed by a peer reviewer who may request changes. These changes can be made using new commits in the local `issue` branch that can subsequently be pushed to the corresponding remote `issue` branch. When all peer reviews have concluded, the pull request can then be `squash merged` into the `master` branch ([read more here](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/about-pull-request-merges#squash-and-merge-your-pull-request-commits)), and the `issue` branch [can be deleted](https://docs.github.com/en/free-pro-team@latest/github/administering-a-repository/managing-the-automatic-deletion-of-branches). If the pull request description includes the words `fixes #[number]` (where `[number]` is an issue number), the issue with that number will [automatically be closed](https://docs.github.com/en/free-pro-team@latest/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword).

> It is recommended to not push commits to the master branch directly but to always go through a peer review process using an `issue` branch.

### Creating releases

It is recommended to [create periodic releases](https://docs.github.com/en/free-pro-team@latest/github/administering-a-repository/managing-releases-in-a-repository#creating-a-release) from a repository, at least at the end of each sprint but can be more frequent. These releases should be working versions of the component(s) being developed in the repository. To create such releases, a new tag representing a version number (e.g., 1.0.0) is added to the local `master` branch and then pushed to the remote `master` branch. A new release can then be created in GitHub using this tag.

### Using a CI/CD pipeline

Every repository needs to have a way to build its artifacts headlessly. It is a good idea to run tests as part of such a build. Instructions on how to build the components in a repository need to be documented in the repository's README.md.

A repository can also be set up to build continuously whenever a commit is pushed to the `master` branch by setting up a CI script (e.g., [Travis CI](https://www.travis-ci.com/)) in its root folder. Such script will configure the build environment (as a virtual machine) and invoke the build script on the `master` branch. If the script fails for some reason, the committer will be notified to fix it. It is a good practice to add a build [badge](https://shields.io/category/version) to the README.md file to visibly indicate the status of the last CI build (Travis CI provides such badges). 

The CI script will also be run when a new pull request is created or when more commits are pushed to its linked `issue` branch. Such a build assures peer reviewers that the new commits when accepted will not break the build. In fact, a successful CI build can be a prerequisite for peer reviewers to look at the changes.

When a tag is pushed to the `master` branch, the CI script will additionally deliver and/or deploy the built artifact(s). The script can also be configured to create a Github release based on the tag.
