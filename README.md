# portfolio

My little portfolio site. It is one HTML file with the CSS inside it, so there is
nothing to install and nothing to build.

## Pages

- **Home** - a short welcome and a link to the other two pages
- **About Me** - who I am and what I am into
- **Task Dashboard** - a few task counters plus a search and filter row

The pages are switched with CSS only. There are three hidden radio buttons at the
top of the file, and clicking a label checks one of them. The CSS then shows the
matching page. No JavaScript is used.

## Making it fit the screen

The main thing I had to fix was the About page. I had set the two columns with
percent widths (35% and 65%) and then added a gap between them. That is always
100% of the parent plus the gap, so it pushed the page wider than the screen and
gave me a sideways scrollbar.

The fix was to use `flex: 1 1 220px` instead of percent widths, and to add
`flex-wrap: wrap` so the columns stack on a narrow screen.

## Viewing it

Just open `gideon_portfolio_task_dashboard.html` in a browser.