# Digital Prototype

Here, we present *Look Club*: a social platform that allows users to watch TV shows asynchronously on a schedule and chat about them with others. This is the result of a long, iterative design process, so let’s take a step back and look at how we got here.

From the beginning, we knew that we wanted to create a platform that facilitated the creation of new bonds between users—particularly as COVID-19 has made online connections all the more important. Focusing on entertainment, we found existing social spaces impersonal to talk in and unlikely to spark such connections. After surveying users, it was evident we weren’t alone: people like to talk about entertainment in small groups and there currently isn’t a platform that facilitates this while still letting you easily meet new people.

Excited to explore this direction, we started thinking about what such a product might look like. Early in our discussions, we decided to focus on TV shows specifically because they lend themselves well to repeated interactions over a long period of time, and we drew inspiration from the structure of book clubs: a tried and true example of long-form discussion that has molded society’s social fabric long before the internet. This shaped the set of features we wanted to implement:
- Matching people based on shows they want to watch, shows they’ve already watched, genres they like, and how many episodes they have time to watch per week
- Allowing groups to create and edit watch schedules so everyone watches at a similar pace
- An anti-spoiler feature which makes sure users have finished their weekly watch homework before jumping into that week’s discussion
- A friend system so users can create more selective watch parties and keep in touch even after finishing a show

This was it. We were about to become the next trillion dollar startup. We were sure of it. But then we opened the dark void known as VS Code, and we had to actually start building the thing. 

As is the inevitable fate of all cool and ambitious projects, we had to do a good amount of downsizing. Fortunately, we were able to implement all of the basic (and advanced) chat functionalities through [Stream](https://getstream.io/chat/), a supercharged chat API, so we could focus on some of the more novel features around entertainment discussion. We were able to implement matching in a slightly less sophisticated form (it only matches on a single show of interest and watch frequency), a very simplistic watch schedule system, a decent anti-spoiler system, and an invite link for adding friends to groups rather than a fully fleshed out friend system. That said, we successfully accomplished most of the tasks we set out to complete: A fully functioning account creation and log-in system, the ability to chat with other users in real time, and unique group chatting features like scheduling out watch schedules complete with spoiler protection on group-agreed milestones.

To tie all of these pieces together, we used what is known as the MERN stack: a NodeJS + ExpressJS backend, a React frontend, and a MongoDB database. Each part was supplemented with a connection to Stream to enable chat functionality. Check out the project here: https://github.com/UWSocialComputing/Vitamin-CS-Project 

## Tour of Look Club

Let us take a look at some of the pieces of Look Club.

![Image of login screen](/Vitamin-CS/images/g7/g7-image1.png)

This is our Login Page, allowing for users to log into existing accounts or create new ones, complete with cookie functionality to save their sessions between website visits.

![Image of home screen with messaging](/Vitamin-CS/images/g7/g7-image2.png)

This is the main view of the website where the user’s groups are laid out and group specific messages are shown. It includes the ability to send messages, emojis, media like files or gifs, and reacting to other group members’ messages.  

![Image of screen to create a group](/Vitamin-CS/images/g7/g7-image3.png)

This is where users can create two different kinds of groups. One is geared to finding new people, which means that they will be matched to other users looking for a similar show to watch and watch frequency. Their selection remains pending until at least 2 other pending group requests are found that are similar enough to be matched. The other option is to create a bare bones, empty group such that friends can be invited using our invitation system.

![Image of screen to invite others](/Vitamin-CS/images/g7/g7-image4.png)

This is the invitation popup from the ‘Invite Friends’ button on the group chat page. This is a custom invitation link that allows users to log into their account on LookClub and be automatically joined with the group that they were invited to.

![Image of screen to set watch schedule](/Vitamin-CS/images/g7/g7-image5.png)

This is the schedule screen, where users can set recurring dates for watch milestones, set to repeat on whatever day of the week that they choose. This leads to the spoiler system, blocking the chat from view on the milestone date until the user gives confirmation that they are caught up, in order to avoid chat spoilers. 

![Image of screen with spoiler shield](/Vitamin-CS/images/g7/g7-image6.png)

In this case, this group is watching Game of Thrones and in this example, they were meant to watch up to episode 5 by the 7th of March, and it is a few days later. They are presented with this ‘Spoiler Shield’ until they click the button to confirm that they are caught up.

There are many more features that we would love to add given additional time, such as a friend system, a mobile-friendly version, and the ability to get matched based on a list of shows rather than just one. However, given the time constraint, we believe that Look Club has reached the point where it is both functional and functionally useful, and we are all proud of the result.