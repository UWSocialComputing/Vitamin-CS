# Low-Fidelity Prototype
## Our Research Report
We initially set out to create a messaging platform that prioritized meeting new people and having meaningful conversations. We wanted to create small discussion groups organized around shared topics of interest in entertainment to allow users to build their network organically. With advice from our instructor, Amy, we decided to narrow our focus on specific areas of entertainment. To foster long term connections through discussions, we would need a longer running form of entertainment. Introducing Look Club - a platform that creates small (friend) groups centered around watching a TV Show together. Users can join groups that suit their interests of TV Shows and their cadence of watching episodes. We created a Figma prototype to simulate our platform by showing the flow and different features of our application. Since our application engages the user over a longer period of time, we created the flows to show the interaction between the user and the application over several weeks. 

The components of our prototype included logging into an account and creating a request for a group based on the user’s preferences. The user can use a slider to indicate the number of episodes they want to watch per week. This does not work in the prototype and is set to a default of 2. The user can also choose the TV Show(s) they want to watch, there is limited capability of adding “Squid Games” to the request watch list. The user would then later get a notification to join the group they had requested. The group page shows various components like the group size, TV show name, and the next episode scheduled to be watched. There is also a calendar displaying the monthly schedule. Although preset, the user can open the calendar and reschedule a particular episode for another day. This creates a proposal for the date changes where all group members can vote to approve or deny the change. The prototype also has a preset messaging feature for the  for in the group. After each scheduled episode's deadline, the application has a spoiler lock that hides the conversation unless the user authorizes that they’re caught up to the schedule. There’s also a screen to change the group settings like the name of the group and add new members to the group. 
The prototype implements all features and components to some extent using the “wizardry” or Figma. This allowed us to get great feedback from the testers before we set out to structure and create our application.

### Images from out low-fidelity prototype:
![screen1](/Vitamin-CS/images/g3/g3-image1.png)
![screen2](/Vitamin-CS/images/g3/g3-image2.png)
![screen3](/Vitamin-CS/images/g3/g3-image3.png)
![screen4](/Vitamin-CS/images/g3/g3-image4.png)
![screen5](/Vitamin-CS/images/g3/g3-image5.png)

## Findings
The goal of this prototyping was to gain an understanding of how our testers want to use Look Club and how the current design facilitates this need. In particular, we used the prototype to gauge interest in the various features that we have included. While we love to see how multiple real users interact, this wasn’t possible to compress the nature of long-term TV show watching into a short period of time. Here are some of our major findings: 

There is some confusion on whether Look Club is meant for synchronous or asynchronous TV watching. This is worsened by calling groups “Watch Parties.”

Users are interested in discussing in small groups, particularly if with strangers, but they proposed the usefulness in larger groups for existing communities.

We currently have a spoiler system that prevents you from contributing to and reading the chat until you have caught up. While users believed this could encourage being caught up, they also thought it restrictive, particularly if there was something they wanted to share before they got caught up.

There was positive feedback about the calendar system. Users thought that Look Club could create an initial watch schedule and allow groups to modify it as best fits their needs. Besides some minor design changes, this reinforces our plan. All users agreed that they would like to use Look Club with their friends. One suggested they did not have any interest in being in groups with random people. This somewhat counteracts our goal for them to meet new friends, so we need to continue to solve this question. There were concerns about random people joining groups. One proposed solution was to allow the group to “vote” to let the person in based on profile information. Overall, while there were many specific pieces of feedback about the way certain features work, most users agreed that Look Club could be useful. This is promising and allows us to continue work on this project while rethinking many aspects of Look Club.

### Using our user testing feedback, the elements that we will be keeping are the following:

Our system of voting for schedule changes whenever there is a schedule issue or just a consensus on changing the watching times. 

The spoiler system was a source of debate for us. However, in order to actually avoid complicating the user discussion channels by adding discussions per milestone or episode, we believe it is more important to keep the discussion structured on a per-milestone-basis. 

To avoid spoilers, we could allow users to set spoiler tags themselves, but this could prove to be too much work and tedious, so for our initial design we think it is the most intuitive to allow the users to unlock the chat one time once caught up for a milestone.

Our profile system works well with the watchlist and already watch sections for getting an idea of user interest in TV shows.


### Elements in need of revising include the following:

Creating groups with friends as well as strangers, since our testing indicated motivation to use our platform will rely on creating groups with existing friends alongside finding new people to watch with.

Adding a voting system for adding new members to groups, and also a vetting process that includes displaying the new user’s profile information to group members.

Changing group size limit to be potentially unlimited (or just really big).

Allowing for more precise controls for schedule proposals, like allowing for ‘binging’ watch habits.
