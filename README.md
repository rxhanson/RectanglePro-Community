# Rectangle Pro Community

Rectangle Pro is a closed source superset of the Rectangle macOS app for window management. 

Since Rectangle Pro is a separate app with much more functionality, this repository is for issues and discussions specifically related to Rectangle Pro.

## Common Issues

[FAQ/Discussions](https://github.com/rxhanson/RectanglePro-Community/discussions)

[What to do when the menu items are greyed out / disabled](https://github.com/rxhanson/RectanglePro-Community/discussions/523)

## Terminal commands

The [terminal commands for hidden settings in Rectangle](https://github.com/rxhanson/Rectangle/blob/master/TerminalCommands.md) can also be applied to Rectangle Pro, just change "com.knollsoft.Rectangle" to "com.knollsoft.Hookshot".

## Programmatically triggering window sizes & positions

You can programmatically trigger any of the Rectangle Pro actions using urls. 

Here are some examples:

* For options that already exist, like left half: 

`open -g "rectangle-pro://execute-action?name=left-half"`

<details>
  <summary>List of actions</summary>

```
left-half
right-half
maximize
maximize-height
previous-display
next-display
larger
smaller
bottom-half
top-half
center
bottom-left
bottom-right
top-left
top-right
restore
first-third
first-two-thirds
center-third
last-two-thirds
last-third
move-left
move-right
move-up
move-down
almost-maximize
fill-left
fill-right
center-half
first-fourth
second-fourth
third-fourth
last-fourth
top-left-sixth
top-center-sixth
top-right-sixth
bottom-left-sixth
bottom-center-sixth
bottom-right-sixth
first-sixth
last-sixth
fullscreen
close
minimize
quit-app
hide-app
cascade-all
cascade-app
tile2x2
tile2x3
reveal-desktop-edge
app-next-display
app-prev-display
app-left-half
app-right-half
first-three-fourths
last-three-fourths
top-left-ninth
top-center-ninth
top-right-ninth
middle-left-ninth
middle-center-ninth
middle-right-ninth
bottom-left-ninth
bottom-center-ninth
bottom-right-ninth
top-left-third
top-right-third
bottom-left-third
bottom-right-third
top-left-eighth
top-center-left-eighth
top-center-right-eighth
top-right-eighth
bottom-left-eighth
bottom-center-left-eighth
bottom-center-right-eighth
bottom-right-eighth
center-two-thirds
fill-bottom-left
fill-bottom-right
fill-top-left
fill-top-right
last
next-space
nudge-left
nudge-right
nudge-up
nudge-down
prev-space
snap-bottom-left
snap-bottom-right
snap-top-left
snap-top-right
upper-center
next-display-ratio
prev-display-ratio
stash-left
stash-right
stash-up
stash-down
unstash
cycle-stashed
toggle-stashed
unstash-all
stash-all
stash-all-but-front
reflow-pin
next-space
prev-space
  ```
</details>

### There are two available pin mode actions:

`open -g "rectangle-pro://execute-action?name=pin"`

`open -g "rectangle-pro://execute-action?name=reflow-pin"`

### For application layouts you've created, use the name you gave it

`open -g "rectangle-pro://execute-layout?name=applayout1"` 

### For custom shortcuts you've created, also use the name you gave it

`open -g "rectangle-pro://execute-custom?name=custom1"`
