# masonry-vanilla

This theme applies the Masonry layout to a Vanilla / Plain Roam Graph (i.e., no other CSS).

## How to Install

Simply add a CSS code block onto your roam/css page and copy the following into it (you can choose whether to include Optional-2 and 3):

```
/* MAIN CSS - Required */
@import url('https://gitmurf.github.io/masonry-vanilla/masonry-main.css');

/* OPTIONAL 1 - Some additional options on top of Vanilla that Murf uses */
@import url('https://gitmurf.github.io/masonry-vanilla/masonry-optional-1.css');

/* OPTIONAL 2 - More customized formatting to Murf's liking (still Roam Vanilla base though) */
@import url('https://gitmurf.github.io/masonry-vanilla/masonry-optional-2.css');
```

If you'd like to customize any of the main settings / colors / widths / heights you can add the following into your roam/css and customize accordingly:

```
:root {
    --main-left-bg: white;
    --right-sidebar-bg: rgb(247 248 249);
    --right-sidebar-drag-bg: #337ac6;
    --masonry-bg: white;
    --masonry-scrollbar-bg: lightgrey;
    --masonry-resizer-color: lightgrey;
    --masonry-startWidth: 550px; /* DEFAULT: 550px; Change this to "unset" if you DON'T want the sidebar pages to be reset in grid like format each time */
    --masonry-minWidth: 440px;
    --masonry-maxWidth: 1200px;
    --masonry-startHeight: 234px; /* DEFAULT: 243px; Change this to "unset" if you DON'T want the sidebar pages to be reset in grid like format each time */
    --masonry-minHeight: 200px;
    --masonry-border: 1px solid lightgrey;
    --closed-bullet-color: 4px solid #CED9E0;
    --code-color: crimson;
}
```

### FULL DEMO

https://user-images.githubusercontent.com/64155612/106953016-bf202c00-66e6-11eb-8345-9958fc719abd.mp4

## OPTIONAL roam/js Scripts

**Toggle sidebar full page width scrolling**

```
var tfps = document.createElement("script");
tfps.type = "text/javascript";
tfps.src = "https://gitmurf.github.io/masonry-vanilla/JS/toggleFullPageScroll.js";
document.getElementsByTagName("head")[0].appendChild(tfps);
```

![Toggle left window](https://user-images.githubusercontent.com/64155612/106884097-ba7f5780-6695-11eb-9812-3a6ce5869678.gif)

**Andy Matuschak mode with full height and toggles different sidebar widths with page widths**

```
var mms = document.createElement("script");
mms.type = "text/javascript";
mms.src = "https://gitmurf.github.io/masonry-vanilla/JS/matuschakModeSizer.js";
document.getElementsByTagName("head")[0].appendChild(mms);
```

![Andy Matuschak mode](https://user-images.githubusercontent.com/64155612/106884646-73459680-6696-11eb-838e-4b378e74839b.gif)

**Cycle through different block widths to make wider on page**

```
var cbw = document.createElement("script");
cbw.type = "text/javascript";
cbw.src = "https://gitmurf.github.io/masonry-vanilla/JS/cycleBlockWidth.js";
document.getElementsByTagName("head")[0].appendChild(cbw);
```

![Cycle Block Widths](https://user-images.githubusercontent.com/64155612/106885194-1f877d00-6697-11eb-9d96-273f6b76b52a.gif)

## Contributions / Inspiration

First and foremost I must give credit where credit is due (inspiration for Vanilla Masonry):

- Abhay (@abhayprasanna) for all his hardwork and collaboration on this. See his AMAZING Dracula Pro theme at: https://github.com/abhayprasanna/abhayprasanna.github.io
- Daniel van der Merwe (@vandermerwed) created the first Masonry layout that I know of. See his stuff at: https://github.com/vandermerwed/Roam-Research-Dark
- Azlen Elza (@azlen) for Zenith: https://github.com/azlen/roam-themes
- Viktor Tabori (@thesved) for his updates / fixes for Zenith: https://github.com/thesved/thesved.github.io
- Rob Haisfield (@classicrob) for his port of previous Masonry to Dracula Pro: https://github.com/classicrob/Current-themes/blob/master/Abhay-Dracula-Masonry
