# Wrap-up notes! 

Event: Software Carpentries (R) 
Organizer: Frances 
Date: May 18 & 25, 2021
Venue: Online 
Event page: https://franceswong.github.io/2021-05-18-UoftCoders/

## Overall 

* Well done, we made it!! 

* 20 participants signed up, between 17-22 in the virtual classroom at each time (including between 4-5 instructors/helpers). 

## Timing 

* Helpers logged on 30 mins ahead of the first day to help with install problems - no issues at all 
    * This workflow did not have any R packages, not install problems 
    * Some were alerted of packages needing to be installed when a new markdown document was opened for the first time - install was by a button and not a problem.
    * Going forward, perhaps we only need to log on 15 mins early? 
* Two full days. While these were very long days, the predictable breaks helped everyone survive and we felt it was better than 4 half days where we anticipate more attrition or people not blocking off as much dedicated time for it. 
    * Perhaps we need to make more clear in the advertisements/pre-workshop emails that this will be a code-along session and they will need to block off time (synchronously).

May 18

"The Unix Shell" AM
Instructor - Haidy
Helpers - Mike

"Programming with R" (parts 1-8) PM
Instructor - Johnny
Helpers - Lise

May 25th

"Version Control with Git" AM
Instructor - Frances
Helpers - Amin

"Programming with R" (parts 9-15) PM
Instructor - Amin
Helpers - Haidy

Ahmed and Frances floating about 

# Git content hiccup

* I made a typo when setting up the remote path to from the local to remote repo (hit the period when hitting the enter key to add a spurious character). Connection did not work. 
    * I ended up deleting the folder (with the files we were working in the first part of this session) and quickly re-creating it. I should have just deleted the .git file so that I could set up the remote path again. 
* Rather than pairing up participants when online it'd more difficult to see who is more active, I created a public repo on the UofTCoders github account so that participants could collaborate at the same time with me to push a file to this repo. Unfortunately, the permissions setting prevented them form pushing. I wanted to have it on the UofTCoders account so that I could have both accounts open on my side, however having a helper host this repo would solve this problem. I missed this in my testing b/c I have permissions on the UofTCoders repo.
    * Or perhaps make a dummy GitHub account. 



## First time hosting on Discord 

* We set up a channel within the UofTCoders existing discord channel 
    * We've had meetings here and were considering moving our weekly workshops here (in contrast to Zoom that we've been using for the large part of 2020)
* Set up an infographic to explain Discord to participants who were new to the platform
    * I kept an eye on my personal and UofTCoders email - we did not have any problems with people navigating the virtual workshop room. 
* A limitation of Discord was that there is a cap of 99 participants on the voice channel w/o video and 25 participants w/ video on
    * In response to this, we limited ticket sales to 20 participants to leave around 5 slots for instructors/helpers. 
    * While we were much higher than the recommended ratio of 1 helper: 8-10 learners, this worked out well since the full day online was quite taxing for everyone. 
    * Zoom would also have necessitated one person (only the host has these permissions) designated to create the breakout rooms should targeted help be needed, discord allowed everyone to move around freely and seamlessly
* On the first day, the distinction between announcements and discussion was unclear so the links and datasets on the announcements page were displaced by unrelated questions. I switched the permissions for the second day that only exec and helpers can post on announcements. However, this blocked participants from seeing posts from the last day 
    * Set this up properly from the start that exec and helpers are the only ones with posting permissions and this should not be a problem. 
    * Ahmed also explained that permissions are a little fickle on Discord and to leave as much as "/" rather than "x"-ing permissions that participants would not have had
* Reactions and discussion tab were very helpful for engaging with the participants, keeping them motivated and getting feedback. 
    * After most breaks, we asked: [Pace - 1 is too slow, 5 is too fast] and [Content - 1 is totally lost, 5 is keeping up and ready to go]. Instructors found this helpful and students gave feedback that this was good for them too. As the instructor asked this, a helper would type it in the discussion and populate the first reactions of 1:5 to make it easier for participants to just click on a number. Started with a 9pt scale, definitely the 5pt scale was much easier to set up. 
* Chat functionality is a lot better on Discord vs Zoom 
    * Having the annotation for code was nice (using `code`)
    * Participants could send screenshots of their problems that were very helpful for troubleshooting
    * Helpers could reply to specific comments and this was super helpful when there were multiple problems being tackled in the chat. 
    * The chat also does not disappear when the meeting is over. If connection is lost during a Zoom meeting, chat history is also lost. Participants also said it was very helpful that they could go over the notes at a later time. 


# Considerations for limiting access to the virtual room

* We had conversations while planning the workshop of whether we would need to restrict admission to channel within the UofTCoders event as this is a paid event. 
* Our format was slightly different from other events our group has been part of that made a designated, temporary server for the event 
    * I support having the event on our permanent event. Many people are looking for a coding community and it's more "worth it" to get to know the platform when it is not just for 2 days. 
* We had minor concerns of people attending the who had not bought tickets. More for equity (people who wanted to attend but could not purchase a ticket b/c it was sold out) than for monetary purposes. 
* Participants were asked to sign in on the etherpad with the discord handle so we could match the name to the participant. 14 participants filled it in (1 did not include their discord handle but the handle matched their name - presumably)
* Solution that we considered and are leaning towards next time is to set up a restricted channel that participants would need to be granted access to. 
    * Access would be granted through a "role". I think there are ways to automate with bots but we would probably need manual work to cross reference with the ticket holder list. 
    * Logistically, we need to know the participant's handle to grant them access. One way is to get it through the etherpad - it can be sent out in an earlier email and participants can be asked to "check-in" on the etherpad ahead of time. A helper can assign the role in advanced. 
    * Alternatively, we can have a "check-in" voice/text channel for participants to go to in the morning of the workshop to be granted the role. A helper would need to monitor this check-in channel throughout the workshop in case people are late or only attending one/some workshops. 

## Workshop survey results 

* Content knowledge improved, all respondents felt comfortable in the environment
* Major strengths 
    * Friendly and helpful helpers
    * Discussion space, permanence of the chat history, venue 
    * Format and breaks
* Places for improvement 
    * More exercises
    * Unify paces and tone between instructors 
    * More background about the application, the applied lens, why different actions were taken. 
* How instructors/helpers affected learning experience 
    * Lesson pace 
    * Targeted support in both discussion and 1:1 rooms 



## Summary

* Strengths 
    * Structure of the workshop 
        * Regular breaks 
        * Strong ratio of helpers:learners 
    * Platform 
        * Respectful and responsive discussion channel 
        * Permanence of discussion chat 
        * 1:1 help in virtual rooms 
    * Very attentive helpers, learners felt supported 
* Future improvement 
    * Set up dedicated role for restricted channel 
    * Restrict announcements for organizing team 
    * Integrate more exercises 
    * Unify approaches between instructors. 
