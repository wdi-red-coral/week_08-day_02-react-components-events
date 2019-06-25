# React Events

React documention is great, so let's not forget that we can use React documenation as a resource.

- [Handling Events](https://reactjs.org/docs/handling-events.html)
- [Forms](https://reactjs.org/docs/forms.html)

## Code along

To learn more about React events, we are going to build an application that will 
1.  Hide and show memes when the meme title is clicked
2.  Add a meme to our list when a form is submitted

### The images should start as hidden
<img src="https://github.com/wdi-infinity/lesson-week_05-day_04-react-events/raw/master/images/notClicked.png" width="400px" height="auto" />


### And show when a user clicks on the title show the meme
<img src="https://github.com/wdi-infinity/lesson-week_05-day_04-react-events/raw/master/images/clicked.png" width="400px" height="auto" />

## Let's plan out our steps!

### Set Up Application

1.  Use create react app to generate a new react application
2.  Start the application and view on localhost
3.  Add memes array to the application's state
```js
[
    {
    "title": "Angry",
    "image": "http://imgur.com/kH6o0mN.png"
    },
    {
    "title": "Aww Yeah",
    "image": "http://imgur.com/vTSZ6CG.png"
    },
    {
    "title": "Cereal Guy",
    "image": "http://imgur.com/SjnMMhd.png"
    },
    {
    "title": "Cereal Spitting",
    "image": "http://imgur.com/rdw32yx.png"
    },
    {
    "title": "Challenge Accepted",
    "image": "http://imgur.com/xHcS2LF.png"
    },
    {
    "title": "Heck Yea",
    "image": "http://imgur.com/DRd0yKE.png"
    },
    {
    "title": "Concentrated",
    "image": "http://imgur.com/t9uwvai.png"
    },
    {
    "title": "Derrrp",
    "image": "http://imgur.com/kBSZgbG.png"
    },
    {
    "title": "Determined",
    "image": "http://imgur.com/CATjyHj.png"
    },
    {
    "title": "Dude Come On",
    "image": "http://imgur.com/8Tkr6ld.png"
    },
    {
    "title": "EWBTE",
    "image": "http://imgur.com/ZaSaYAK.png"
    },
    {
    "title": "Excited Troll",
    "image": "http://imgur.com/CFLPW9U.png"
    },
    {
    "title": "Fap Fap",
    "image": "http://imgur.com/NImikb7.png"
    },
    {
    "title": "Forever Alone",
    "image": "http://imgur.com/4L89AMP.png"
    },
    {
    "title": "Forever Alone Excited",
    "image": "http://imgur.com/NyEoz2g.png"
    },
    {
    "title": "Oh Yea Female",
    "image": "http://imgur.com/WMgvwaq.png"
    },
    {
    "title": "Full Panel",
    "image": "http://imgur.com/iN5P0r4.png"
    },
    {
    "title": "Happy",
    "image": "http://imgur.com/JqhcMU4.png"
    },
    {
    "title": "Hehehe",
    "image": "http://imgur.com/U9GK6jL.png"
    },
    {
    "title": "Laughing",
    "image": "http://imgur.com/wJUtNXR.png"
    },
    {
    "title": "Me Gusta",
    "image": "http://imgur.com/6otWkQZ.png"
    },
    {
    "title": "Milk",
    "image": "http://imgur.com/bxMhEKZ.png"
    },
    {
    "title": "Newspaper Guy",
    "image": "http://imgur.com/MhbPTSQ.png"
    },
    {
    "title": "Okay",
    "image": "http://imgur.com/X6niVYQ.png"
    },
    {
    "title": "Original Rage",
    "image": "http://imgur.com/CD0nLh8.png"
    },
    {
    "title": "Original Troll",
    "image": "http://imgur.com/sV4AReH.png"
    },
    {
    "title": "Poker Face",
    "image": "http://imgur.com/EFHsGkJ.png"
    },
    {
    "title": "Prrrr",
    "image": "http://imgur.com/gXmsig6.png"
    },
    {
    "title": "Smile",
    "image": "http://imgur.com/Bp2y4zT.png"
    },
    {
    "title": "Thoughtful",
    "image": "http://imgur.com/HdmBrwX.png"
    },
    {
    "title": "Troll Dad Full",
    "image": "http://imgur.com/Mgyz87x.png"
    },
    {
    "title": "Troll Dad Jump",
    "image": "http://imgur.com/PFzOfO7.png"
    },
    {
    "title": "Wait A Minute",
    "image": "http://imgur.com/rxlv8TX.png"
    },
    {
    "title": "What",
    "image": "http://imgur.com/0JmUzko.png"
    },
    {
    "title": "Why With Hands",
    "image": "http://imgur.com/gEZW60M.png"
    },
    {
    "title": "YUNO",
    "image": "http://imgur.com/uXKy3RJ.png"
    }
] 
```
4.  In render, iterate through memes array and display title and meme as image.
5.  Move title and image tag into a Meme component and pass each meme object into the Meme component as a prop.

### Add Click Event

6.  Create a CSS class named `hidden` and class named `show`.
7.  Add `memeStyle` to Meme component state and default the value to `hidden`.
8.  Apply `memeStyle` from state as `className` to `img` tag.
9.  Add click event to meme title.
10.  Make click event update state of `memeStyle` to `hidden` or `show`.

### Add Submit Event

11.  Add form and inputs to render
12.  Add form object to state
13.  Update inputs `name` attribute to match form object
14.  Bind inputs `value` to form object property
15.  Write `onChange` function to update form object property
16.  Write `onSubmit` function to add form object to meme array in state and reset form object to clear form. 
