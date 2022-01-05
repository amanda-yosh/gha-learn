# A Guide trought Github Actions and Workflows

## Quick overview
When an event ocurrs into an github repository a trigger runs an workflow.


An workflow contains jobs and each job performs steps.


An step can perform an action, like deploy or test, or can run a shell command.


All this workflow runs into a virtual enviroment provided by github.

## Events
An event can be a `push`, a `pull request`, a `merged pull request`, an `issue created` or `closed` or etc., can also be schedule or even an external event.

## Jobs
A job need an virtual machine instance to run into, that's why there is the `runs-on` command, to tell what's the type of the machine.


It can be `linux`, `windows`, `MacOS`, or a `Docker Container`


The machine can be either a GitHub-hosted runner, or a self-hosted runner.

## Runner
A runner is any machine with GitHub Actions runner aplication instaled.


It is responsible for runnig the jobs when an event ocurrs and display back the results.


It can be hosted by GitHub or you can host your own runner. The ones hosted by GitHub are maintained by then, it can be a `linux`, `windows` or `MacOS` virtual enviroment, but you cannot customize the hardware configuration.