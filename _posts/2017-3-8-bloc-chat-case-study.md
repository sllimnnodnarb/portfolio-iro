---
layout: post
title: A Case Study on Bloc Chat
---
As the old saying goes, "Please, don't offer me anything, I will tell you what I want."  Bloc Chat is just that.  A communications application that eliminates all the nonsense.  Finally, a chat app without the constant barrage of advertisements. Let's talk.

---
{:.center} 
![]({{ site.baseurl }}/img/3-bloc-chat-home.png)


If you enjoy play-by-play analysis, you will find that this case study covers a number of critical steps in the development of Bloc Chat. During development, challenges arose that were made solvent with pure ingenuity.  Read on to see those challenges explained in further detail.

---

The home page for Bloc Chat is as seen above.  The first challenge that emerged was that it was in fact possible to enter the chat arena without first naming oneself.  The obvious problem here is that messages could then be sent, but the recipient of the message would have no idea who the message came from.  The solution?  Resolution came in the form of directing all users to an inescapable modal window on the home screen that requires a username input before proceeding to the website...voila!

{:.center} 
![]({{ site.baseurl }}/img/1-bloc-chat-username.png)


---

Once a username has been recorded, the user may then enter the site and proceed to the 'Rooms' page.  This is where all the action is happening.  You will notice a list of chatrooms on the left hand margin of the screen, an 'Add Room' button located near the top, and the rest of the screen reserved for displaying the active room as well as message interactions.

{:.center} 
![]({{ site.baseurl }}/img/chat-rooms.png)

---

Originally, the design for Bloc Chat only included a fixed number of rooms, and the names of the rooms were preset values.  Of course for added flexibility the user needed the option to create a room of their liking, which resulted in the creation of an 'Add Room' button.  This button launches a modal state where the user can define a new room name to their liking.

{:.center} 
![]({{ site.baseurl }}/img/open-modal.png)

{:.center} 
![]({{ site.baseurl }}/img/room-modal.png)

---

Once the room name is entered and the user clicks 'Create room', the new room name is pushed to an array with a unique identifier that is later referenced by each message that is sent.  Then the modal is closed and the user can get back to messaging.

{:.center} 
![]({{ site.baseurl }}/img/room-created.png)

---

Another dilemma that arose was ensuring that all messages retrieved from the database were not displayed in every chat room.  For instance, conversations about what type of food should be ordered for lunch didn't need to be intermingled with the messages concerning accounting (although studies show accountants do need to eat also).  This problem was remedied by restricting the messages retrieved from the database to only those associated with the ID established in the creation of the room in the first place.  Observe that each active room only displays the messages that were composed within that room (containing the same reference ID).


{:.center} 
![]({{ site.baseurl }}/img/pantomime-room.png)

Pantomime messages are for the Pantomime room, and lawn bowling messages are for the sports room.  Although the two would make and interesting combo!


{:.center} 
![]({{ site.baseurl }}/img/lawn-bowling.png)

---

At completion, Bloc Chat resolved to be a user-friendly messaging application that gets the job done without fuss.  The application offers the flexibility of navigation between chat rooms, and posting and reading messages to ensure the lines of communication are wide open.  And best of all, no advertisements impede user experience!

---

To learn more [about](/about) the author or the content herein, just [ask](/contact/).