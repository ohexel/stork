# Stork: a color theme for `beamer`
This color theme uses the colors suggested in `Colors.pptx`.
 
I do not give any guarantees that all colors defined by all themes are covered
in this themes or that they work together harmoniously. I defined the major
colors (`structure`, `palette {primary,secondary,tertiary,quaternary}`, 
`sidebar`, `palette sidebar {primary,secondary,tertiary,quaternary}`, `alerted
text`) but there are many more specific ones and I only did some cursory checks
against the default theme, one theme with a footer (Boadilla), one theme with a
sidebar (Bergen), and one theme with a sidebar talk outline (Berkeley).

## How to use it
Add the file `beamercolorthemestork.sty` to the directory of your `beamer` 
presentation or to the directory where your other `beamer` themes live.

Add `\usecolortheme{stork}` to your preamble to activate it.

## Where in the preamble should I load the color theme?
In `beamer`, changes to themes are cumulative. This means that themes that are
loaded later in the preamble add to or override themes loaded earlier. If you
would like to change a specific element of your presentation to a specific
color, you can load another color theme in which that that color is defined
first and load the `stork` color theme afterwards. Or you can define the color
and the element in the `sty` file. Look through some of the color themes that
come with `beamer` to get an idea of which elements can be changed. 

## Why `stork`?
Till Landau named his color themes after flying animals. I wanted to follow his
example. The symbol of the Max Planck Society is the owl, but I was trying to
find something more specific to our institute. My first idea was "seagull" but
sadly that was already taken. Then I thought about demography's themes
mortality, fertility, and migration. Mortality seemed a bit morbid as an
inspiration and everyone knows that babies are delivered by storks, so `stork`.
Also, there is the [Rostocker Pfeilstorch](https://en.wikipedia.org/wiki/Pfeilstorch)
which adds another link to Rostock and to migration too.

## What about the logo?
`\logo{\includegraphics[<options>]{<path_to_the_logo_file>}}`

See section 8.2.5 of the `beamer` user guide (p. 72).

The outer theme defines where the logo goes. If the logo does not show up, use
a different (outer) theme. 		
