## Activity 1
**Research GitHub actions focusing on running tests**
GitHub Actions - A CI/CD platform used to automate a developers build, test, and deplotment pipeline. CI/CD stands for Continuous Integration/Continuous Delivery.  Developer are able to create workflows that build and test every pull request to a respository. 

GitHub actions also let the developer run workflows when other events happen in a repo. A workflow can be run to automatically add labels when someone creates a new issue in a repo, for example. 

Some components of GitHub Actions include the following:
* Workflow - A configurable process that is automated and will run one or more jobs.  These are defined by a YAML file that runs when triggered by an event in a repo. Workflow definitions are stored in a .github/workflows directory in a repo. Repos do not have to be held to only one workflow either. They can have multiple workflows, all performing different tasks. 
* Event - An activity that happens in a repo that triggers a workflow. For example, if someone creates a pull request or pushes a commit, these would be considered events that would trigger a workflow.
* Job - The set of steps that make up a workflow. These steps can be she scripts that are executed when triggered, or they can be an action that will run once triggered. These steps all execute on the same runner. Therefore, data can be shared between steps.
* Actions - Pre-defined sets of jobs or code that perform specific tasks in a workflow. These actions are able to be reused. The help to reduce the amount of code that is repeated in the workflow file. Actions cal also pull a repository from GitHub, set up the correct toolchain for a build environment, or set up authentication to a cloud provider.
* Runners - A server that runs a workflow when it is triggered. Each runner is able to run a single job at a time. GitHub provides the following runners to be able to run workflows:
* * Ubuntu
* * Windows
* * macOS
