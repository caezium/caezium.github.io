---
draft: false
---
usage ex.
```
> [!sticky|blue float left s-45]
> > Comment #1 
> > As long as you listen in Dr. Neto's class, you don't need any extra classes after school
```
#### how to use
params:
 - colors such as blue, purple, yellow, green
 - left, center, right
 - s-30 to 3-95, percentage of screen coverage
 - markdown works in the callout

#### new and expanded features
- Floating cue section
	- `| float` metadata/parameter to make a sticky note float to the left side of your note. ex. `> [!sticky | blue float s-40]`
	- this placement mirrors the cue section of the *Cornell note-taking system*.
	- why not right side? we read from left to right, so the cue stickies will gain more attention.
	- In editing mode, floating stickies will return to the normal margins but with a more transparent look, indicating that it is a floating/cue sticky. Note: don't space floating sticky notes closely in line numbers or else they would overlap. Why would you even need multiple cue stickies that close? you should have floating notes at s-30, you can make it larger, but it will overlap to the main notes section, if you still want it to be that large but not overlap, you can use `<br>` tags.
- Zoom on hover - self-explanatory
- Collapsible stickies 
	- add a `+` or `-` sign after `[!sticky|metadata]` to make it collapsible with the default state of open and close correspondently. ex. `> [!sticky | yellow]-`
	- clicking on the arrow`>` or header on top of the sticky note will expand/collapse it.
- more sticky widths, up to 95%
- standardized all markdown colors in sticky note.
- slightly changed color system, should be natural for both dark and light mode
- removed default titles and callout icons.

- *Optimized Sub-optimal*



> [!STICKY| blue title right s-80] 
> > Comment #1 
> > [[CSS stickynotes3.7]]
> > As long as you listen in Dr. Neto's class, you don't need any extra classes after school

test test test test 
test test test test 
test test test test 
test test test test 
test test test test 
test test test test 










> [!sticky | left yellow]+
>  **Comment #1** 
> As long as you listen in Dr. Neto's class, you don't need any extra classes after school
> this is a collapsible note, defaulted as open.

eeeee


>[!sticky | float right blue s-30]
>this is a floating/cue note
>hello
>hello
>hello






aa
a
a
a
a

> [!sticky | ctr s-30]- title
> hello
> [[CSS stickynotes3.7]]
a

						^ this is a collapsible note, defaulted to closed
>[!sticky | float left s-30]+
>hello
>hello
>another one! collapsible too

e
text text text
text text text
text text text
text text text
text text text
>[!sticky | float purple s-90]
>loooooong
>

<br><br>
text ^there was one `<br>` tag for no overlap