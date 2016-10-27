# Process

Software has been through a long process of refining how it is built. The current approach since around 2000 has been to use agile practices with the current industry standard splitting into two approaches:

- Scrum
- Kanban

It is a good idea to pick an existing process, follow it and change it as is required once painpoints are found (not before).

The single most important idea from all of this is "the team should be delivering the next most important function to the business". That should be the only priority! A good example of this is don't start with a login function for a system. Building a login doesn't do anything for a user. Build the thing they want to use. Hard code the plumbing.

## Remote Work

Team members working remotely is the future of software development. Try to pick tools that take this into account. Face to face meetings are great but remember to write things down in a very concise form to keep as a reference.

## Scrum

1. Pick a product owner, a person who represents all stake holders of the product - this person **must** have the vision of the product in their head and be able to sketch out an idea of how it will work.
2. Pick a scrum master, this is a person who is in charge of making sure the process is adhered to. Often this will be the product owner.
3. Pick a sprint time, a sprint is a fixed length of time that the team will work on a set of features. Usually 2 weeks works well.
4. Product owner - come up with a set of the most important features.
5. Run a sprint planning session - in this session each feature is explained by the product owner, questioned by the team, estimated (use Small, Medium, Large, XL to start) and entered into a tracking tool (e.g. Trello, Jira, Sprintly).
6. Commence sprint - features are locked in for the sprint duration. If there is any change to features, the sprint is reset and the process starts again.
7. Daily stand ups - have timeboxed meeting (15 minutes is good) where everyone answers the following questions - what did you do yesterday, what are you planning on doing today, is there anything blocking you. It is also important to note that anyone can pass. Breakout any discussions that form.
8. Run a retrospective (before next sprint planning) - get participants to write down answers to these questions on sticky notes: What went well? What didn’t go so well? What have I learned? What still puzzles me? Discuss and address issues.
9. Rinse and repeat.

Other things:

- Walking the board: during standups it can help to "walk the board" where you lean on what is in the board based on what is going to be done.
- Change the process: feel free to adjust how things work during retrospectives.
- If you want to keep a list of features that aren't important to the sprint, make sure they are in an icebox and are kept away from the sprint.

## Kanban

1. Pick a product owner, a person who represents all stake holders of the product - this person **must** have the vision of the product in their head and be able to sketch out an idea of how it will work.
2. Decide on a work structure/pipeline. Kanban focuses on more of a pipeline approach so rather then creating a ticket for a task, a feature is followed through it's lifecycle. (See below for example).
3. Assign a WIP limit (maximum number of tasks for a column) for every doing column.
4. Have regular planning meetings where features are discussed but estimation is not required.
5. Run stand up meetings and retrospectives in the same structure as Scrum.
6. Rinse and repeat.

## Example Pipeline

```
+------------+------------------------------+----------------------------+------------+-------------+
|            |                              |                            |            |             |
|    Plan    |       Design/Prototype       |          Develop           |    Test    |   Deploy    |
|            |                              |                            |            |             |
+----------------------------+-----------------------------+--------------------------+-------------+
             |               |              |              |             |
             |     Doing     |     Done     |    Doing     |    Done     |
             |               |              |              |             |
             +---------------+--------------+--------------+-------------+

```

## Estimation

Software estimation is notoriously hard and almost never correct. Agile promotes the removal of time based estimation in favour of broad estimates which compare one task to another. Asking a developer for a time estimation goes against agile practices and whatever they tell you will probably be very wrong. Working to the simplest possible feature that drives the highest business value tends to render estimates useless.

## Beta Group

A common practice is to recruit a group of users that you trust and enlist them to use your software while features are in development. This trend has seen a massive improvement in software for well respected companies.

## Developers and designers

There are a bunch of different ways that designers can work with developers. Each is valid and will need to be evaluated based on the type of project. For example design first is very relavant for website projects but a prototype driven approach usually works better for data heavy apps. Taking the team into account is very important when making this choice.

1. Design first - designers complete pixel perfect designs and hand them over to development
2. Prototype driven - designers and developers prototype flows together and put them infront of a beta group before refining
3. Development first - developers work up a working version of the software and design corrects the software as it is built

## Delivery

1. Smoke test document - this document lists a set of steps to follow to test the project before deployment. Make sure it is run successfully before any deployment.
2. Feature flags - are settings in the database that specify if a feature is enabled for a user/role.
3. User communication - as projects are delivered an enhanced, user communication becomes critical. Consider using a tool like intercom to have in project messaging that can be controlled by someone with a communications skillset. Also pay attention to email and mobile communication upfront. It should never be an after thought.
4. Content management - there are two flavours of content management, one is for the pages that are in a project (the large forms of copy) and the other is for the labels that are used in the project (internationalisation tools are often used for this). Between these two approaches it is possible to externalise all text so it can be changed by a non-developer. Choosing the correct approach really depends on the project.
