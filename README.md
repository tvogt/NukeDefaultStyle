# NukeDefaultStyle
a USS file to undo the Unity default theme styling, while keeping the layout

## What is this?
This file exists because someone at Unity had the brilliant idea of doing five things that boggle the mind:
1. the default theme is compiled at runtime and not available as a file anywhere for inspection and editing
2. it mixes styling (like background colors) with layout (like spacing, flex directions, etc.)
3. the layout parts are essential if you don't want to spend hours re-creating them from scratch
4. the specificity rules will fuck over your style because the defaults are often more specific than your styling unless you manually debug everything to overwrite sometimes arcane nested selectors
5. there is no **!important** or other way to tell the engine "resolve any conflicts in favor of this rule"

This file tries to take care of that by replacing all styling with the closest approximation of "nothing", i.e. transparent colors.

For all I can tell, applying a FONT at the root level works, btw.

    
## Who is this for?
Anyone who uses sprites for their UI elements.
    
## If someone at Unity reads this:
Please buy the person responsible a big bag of coffee, they are obviously in severe caffein withdrawl.
Also, you could fix any of the 5 items above and the entire problem would disappear.
    
## Note:
This uss contains a bunch of selectors that for all I've seen do nothing at all. I'm including them because some joker on the Unity forum insisted that they would work. They don't. But here they are, just so I don't have to hear that again.

## Contributions:
If you found a selector I missed, fork and send a merge request.

If you want to help out otherwise, no I don't need coffee money - go and bug Unity about the default theme so they fix it. I'd much prefer to not having to maintain this file ad infinitum.

## You think some of these are not needed?
Maybe. But it's called "nuke" for a reason. I want to make absolutely certain that I never, ever, ever see that stupid grey background behind a sprite again. Ever. So, if you get the reference, take off and nuke the site from orbit, it's the only way to be sure.
