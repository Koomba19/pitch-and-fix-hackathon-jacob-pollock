# Bug Squashing Time

## Immediate Steps

- Check for `!Important` on any CSS. Not a bug, I just don't like them.
- Examine every page for comments and immediate vscode errors
- index.html has 16 errors through w3c validator
- cart.html has 2 " "
- product-detail.html has 10 " "
- product-detail has comments left in where bugs were inserted, after fixing those, we'll see if anything remains.
- There are so many commments in the .js files. Not an issue *per se,* but it feels unnecessary when the name of the function is the actual comment. For example, the comment of *//Setup Event Listeners* on the function `setupEventListeners()`.
- All CSS files pass w3c validation, which shocks me. responsive.css has an empty ruleset but that's fine.

## Thursday 4/24  
Apparently I that's all I did was the Immediate Steps.  

## Friday 4/25  
I saved the thing to commit it. Which I forgot to do before.  
- styles.css L 78 changed nav-item and nav-items to class form ID in order to fix the index.html L 15
- Added /div to index.html L168 to resolve that sections validation errors of missing a closing tag on the top div.
- index.html L177 input tag had mismatched double to single qoutes. Changed to all double qoutes.
- index.html L217 first list item had an anchor tag that was left open, facebook should now have a proper anchor tag after closing it.  
It's off to work for me unfortunately. Hopefully I keep at this after my shift.

### Misc

- Took a peek at the text editor for that .svg, that's neat how tidy it was made and I'm curious as to what program you used Eric.

## Extensions Installed

- W3C Web Validator - Celian Riboulet
- Better Comments - Aaron Bond
- Error Lens - Alexander
- HTML Boilerplate - sidthesloth
- JavaScript (ES6) code snippets - charalampos karypidis
- WSL - Microsoft
- Live Server - Ritwick Dey
- 'Prettier - Code formatter' - Prettier