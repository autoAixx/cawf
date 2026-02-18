---
name: init-workspace
description: This skill is to describe how to persist and access information that is relevant to the current run and should be shared between agents and developers.

compatibility: This skill to be used only by the facilitator agent when initializing the workspace for a new project or a new feature implementation in an existing project. This skill should be used at the beginning of the conversation to set up the necessary information and documentation for the project or feature implementation, and to ensure that all agents and developers involved in the project have access to the relevant information throughout the development cycle.
---

If you are totally starting out with a new project or the workspace is empty, you can use <workspace-initial-setup> to set up the initial workspace structure.

If however you are just adding a new project, application, or service within an existing workspace, you can use <project-initial-setup> to set up the necessary files and structure for the new project/application/service.

<workspace-initial-setup>
- if the folder is totally empty, you can do initial organization to facilitate the coordination: the folder should be organized as follow:
```
src
  backend
    - {SERVICE_NAME}
    - ... other services
  frontend 
    - {SERVICE_NAME}
    - ... other services
tests
  blackbox-tests
  ui-tests
local-dev-environment
  - docker-compose.yml --> it can refer to dockerfiles in the backend folder if needed or leave for later when the services are defined.
```

if you have not decided on the service names yet, just don't create them!!!

for each service, you can just create the bear minimum, like the packages/dependencies file that would allow to containerize it and run it in the local development environment. but don't implement anything!!

</workspace-initial-setup>



<project-initial-setup>
if you create a new project/application/service, just add the bare minimum (packages file for example) that would allow to containerize the application, don't implement any functionality. 
</project-initial-setup>