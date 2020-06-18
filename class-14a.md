# Class 14a reading notes

[What Google Learned From Its Quest to Build the Perfect Team](https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html)  
***same notes in [class-14b notes](class-14b.md)!***

[What Google Learned From Its Quest to Build the Perfect Team](https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html)

Google put some analytical research behind why some teams thrive, while others falter... a few key highlights:

> "Norms can be unspoken or openly acknowledged, but their influence is often profound."

"The right norms, in other words, could raise a group’s collective intelligence, whereas the wrong norms could hobble a team, even if, individually, all the members were exceptionally bright."

"As the researchers studied the groups, however, they noticed two behaviors that all the good teams generally shared. First, on the good teams, members spoke in roughly the same proportion, a phenomenon the researchers referred to as ‘‘equality in distribution of conversational turn-taking.’"  
"Second, the good teams all had high ‘‘average social sensitivity’’ — a fancy way of saying they were skilled at intuiting how others felt based on their tone of voice, their expressions and other nonverbal cues."

***"Within psychology, researchers sometimes colloquially refer to traits like ‘‘conversational turn-taking’’ and ‘‘average social sensitivity’’ as aspects of what’s known as psychological safety..."***

Advice: "We must be able to talk about what is messy or sad, to have hard conversations with colleagues who are driving us crazy. We can’t be focused just on efficiency."

Successful teams don't usually just 'happen.' Each group member (and this goes doubly for a group leader/manager/authority figure) needs to do their part to establish norms that create psychological safety. This includes parameters - if you will - to ensure that team members' needs are being met, that they're being heard, that they aren't afraid to be their authentic selves. With norms that embrace authenticity, you can diffuse tension, avoid groupthink, and innovate further and faster than teams that don't enjoy such freedoms. In short, **psychological safety** is key to any group's success!

<hr />

[Read this article on CSS Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

The `transform` property provides alternative ways to size, position, and change elements. Of note, browser support isn’t great yet, but "it is getting better every day."  

*Syntax*
```
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```
The above "includes multiple vendor prefixes to gain the best support across all browsers. The un-prefixed declaration comes last to overwrite the prefixed versions, should a browser fully support the transform property."

The transform ability really allows a website to give immediate 'feedback' and interactivity to the user, a much more engaging experience than a more static site (topic appropriate, of course). Create and "move" shapes! I imagine this will come in quite handy for game/app development...

[Read this article on CSS Transitions & Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

"With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted." I love features like this! It seems like an easy way to give positive user feedback and make your site feel interactive!

Pseudo-classes are:  `:hover`, `:focus`, `:active`, and `:target`.

**Transition related properties** 
1. `transition-property`
2. `transition-duration`
3. `transition-timing-function`
4. `transition-delay`

> **"Not all properties may be transitioned**, only properties that have an identifiable halfway point.

The `transition-duration` controls how long the transition takes, and you can set multiple durations (for different properties). The ```transition-timing-function``` can provide options like ease-in and then speed up. You can also set up a delay between activation of transition and when it actually begins.

When more control is required, animations can pick up where transitions leave off... introducing `@keyframes`.

By default, animations run their cycle once from beginning to end and then stop, however, you can set them in an infinite loop or set a number of times to execute.

"Animations, just like transitions, can be written out in a shorthand format. This is accomplished with one `animation` property."

[8 simple CSS3 transitions that will wow your users](http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)  

7 out of the 8 transitions below are quite straightforward, 1 involves a bit more...

1. Fade in
2. Change color
3. Grow & shrink
4. Rotate
5. Square to circle
6. 3D Shadow
7. Swing <-- this is the more complicated one involving `@keyframes`
8. Inset border

[6 Buttons animated](https://codepen.io/retyui/pen/ByoaXV)

Oh buttons! (but I only saw 3?)

[CSS3 Animations: Keyframes](https://codepen.io/akshaychauhan/pen/oAfae)

Not much to write about this one, but I like it!

[404](https://codepen.io/kieranfivestars/pen/MYdQxX)

Oh love this! I can see some fun applications for this with a game high-score type number?

[Pure CSS Bounce Animation](https://codepen.io/dp_lewis/pen/gCfBv)

Super interesting... trying to think of a good use-case scenario for this (though I imagine I'll find/think of one). Definitely some interesting graphic possibilities for apps/games.

<hr />

[Previous - Class 13 reading notes](class-13.md)  
[Next - Class 14b reading notes](class-14b.md) 

[Return to Table of Contents](README.md)