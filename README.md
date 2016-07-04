# Slack-esque Landing Page
## by Robin Jayaswal

This project, Homework 1 of CS52, sought to make a static landing page resembling that of *slack.com* using pure HTML and CSS. 

### Description
I implemented the overall structure using almost exclusively flexboxes, and was able to recreate the structure of Slack's homepage.
After styling it to my liking using pure CSS, I then added in screen size responsiveness with media query, creating one mobile version.
Finally, I added in some responsiveness using the "CSS Checkbox Hack", allowing the user to open up the top level menu when the screen 
was narrow, as well as expanding the link headers to show links, and added a nice transition to when the top level menu appeared.

**What worked:** I found most things to work remarkably well.

**What did not work:** Though the CSS Checkbox Hack did work, it certainly offers limited capability in some situations. The situation
where I had trouble getting it to work as I wanted in this assignment was expanding the link headers at the bottom of mobile view. 
Unlike with the top level menu, I was hoping that the link box that would appear upon clicking would not be absolutely positioned, but would
make everything below it slide down. However, because I wanted the link header to look like this:

![Alt text](https://s31.postimg.org/o8ajk0z63/Screen_Shot_2016_07_04_at_9_32_07_AM.png)

And had to use labels as the checkbox pseudo buttons, I needed to make this container have ```flex-direction: row```,
with ```justify-content: space-between```. However, because the checkbox hack requires the checkbox, label, and element to be edited all
to be within the same div, it was now not easy to position the box of links that should appear since I wanted it below, not in a row. I ended
up positioning the link box to appear absolutely, 60 pixels below the link header it came from, and just covering everything below it
(the limited capability of checkbox hack also made it so I could not figure out how to make bottom elements slide down). The end result of this, 
that opening a link header looks like this:

![Alt text](https://s32.postimg.org/5w43otfnp/Screen_Shot_2016_07_04_at_9_37_53_AM.png)

was not quite what I had wanted. But, at least it is a box of links that appears when you click the link header. I guess if I ever decide to 
start a billion dollar messaging app like Slack I'll have to use some javascript. 


### Layout Stage Screencaps




