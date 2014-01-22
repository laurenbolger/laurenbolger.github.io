---
layout: blog
title: Super Fun Game
---

I'm always looking for fun ways to get better at coding, so I wanted to make something a little different using CSS. The best way to get good at CSS is to write a lot of CSS, but sometimes it gets boring writing the same kinds of code over and over again. I thought it would be cool to use CSS to make a game. Transforms and transitions are pretty much the coolest things ever, and I really wanted an excuse to use a bunch of them for something. I got the idea to make this game (ok, its not really a game, but its still fun!) when I started learning more about transforms. I like the interactive aspects of CSS so I came up with the idea of clicking tiles to reveal a picture. 

To make the game, I initially thought that I could use the pseudo-class `:visited` as a way to make the tiles disappear after they were clicked. The tiles would be links, and when you clicked one and it became visited, it would disappear. However, due to security concerns, only a few (mostly color based) properties can be applied to :visited. Thus, applying `:visited` to the tiles didn’t make them disappear, it actually didn't do anything. If you’re the kind of person who is super fascinated by the `:visited` pseudo class’s security concerns (you weirdo), go [here](https://developer.mozilla.org/en-US/docs/Web/CSS/Privacy_and_the_:visited_selector?redirectlocale=en-US&redirectslug=CSS%2FPrivacy_and_the_%3Avisited_selector).

After doing some more research, I came to the conclusion that I was going to have to use checkboxes. I knew that using checkboxes,the pseudo-class `:checked`, and a sibling selector to select the checkbox's label, you can make change styles on click without JavaScript. I took this basic idea, and camouflaged my checkbox labels so that they appear as the tiles. Clicking the label checks the checkbox, so I was able to have activate transitions when the tiles are clicked on. 

Check out my game here:

[Super Fun Game!](/projects/super-fun-game)

**Spoiler alert: All the pictures are of my dog. Yes, I’m THAT person.**

I would like to to re-do this game in JavaScript, hopefully within the next month, as a learning exercise. However, I need to up my J-script skillz a bit before I can successfully rebuild it. Next time it wll be an actual game!
