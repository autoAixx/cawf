---
name: collab
description: This skill is to describe how to persist and access information that is relevant to the current run and should be shared between agents and developers.
---

This skill is to describe how to persist and access information that is relevant to the current run and should be shared between agents and developers. 

Use the directory `./collab/{TICKET_ID}` where TICKET_ID is a unique identifier given by the user when they initialize the conversation. This will help to keep the information organized and easily accessible for all agents and developers involved in the project.

Add the date and time when you last updated the information so that other agents and developers can keep track of the most recent updates.

Write the information in concise way. don't over elaborate, just write the necessary information that is relevant to the current run and should be shared between agents and developers. 

Write your stuff inside a subfolder with your agent name, this will help to keep the information organized and easily accessible for all agents and developers involved in the project.
For example, if the ticket ID is "1234" and the agent name is "facilitator", you can write the information in the file `./collab/1234/facilitator/{fileName}.md`.

Use markdown format to write the information, this will help to make the information more readable and organized for all agents and developers involved in the project.

Always create a new file with postfix `_round` + idx where idx is the number of times you updated the information. For example, if you are updating the information for the first time, you can create a file named `{fileName}_round1.md`, and if you update it again, you can create a file named `{fileName}_round2.md`, and so on. This way, all agents and developers can easily track the history of changes and updates made to the information throughout the project.


Use the following format to write the information in the markdown file:

```
# {fileName}
Timestamp: {date and time}
Ticket ID: {TICKET_ID}
Agent Name/Creator: {agentName}
Target Agent(s): {agentName1,agentName2,...}
```

When reading the files, make sure to read only the files relevant to the current run which is determined by the TICKET_ID. This will help to ensure that you are accessing the most relevant and up-to-date information for the current project.

Additionally, consider only the files that are targeted to you or created by you (as indicated in the Target Agent(s) field), this will help to ensure that you are accessing the relevant information and not overstepping your boundaries as an agent or doing other agents' work.
