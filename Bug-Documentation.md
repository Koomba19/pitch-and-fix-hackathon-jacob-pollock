# Bug Squashing Time

## Immediate Steps

- Check for `!Important` on any CSS. Not a bug, I just don't like them.
- Examine every page for comments and immediate vscode errors
- index.html has 16 errors through w3c validator
- cart.html has 2 " "
- product-detail.html has 10 " "
- product-detail has comments left in where bugs were inserted, after fixing those, we'll see if anything remains.
- There are so many comments in the .js files. Not an issue *per se,* but it feels unnecessary when the name of the function is the actual comment. For example, the comment of *//Setup Event Listeners* on the function `setupEventListeners()`.
- All CSS files pass w3c validation, which shocks me. responsive.css has an empty ruleset but that's fine.

## Thursday 4/24  
Apparently that's all I did was the Immediate Steps.  

## Friday 4/25  
I saved the thing to commit it. Which I forgot to do before.  
- styles.css L 78 changed nav-item and nav-items to class form ID in order to fix the index.html L 15
- Added /div to index.html L168 to resolve that sections validation errors of missing a closing tag on the top div.
- index.html L177 input tag had mismatched double to single quotes. Changed to all double quotes.
- index.html L217 first list item had an anchor tag that was left open, facebook should now have a proper anchor tag after closing it.  
It's off to work for me unfortunately. Hopefully I keep at this after my shift.

## Sunday 4/27
**Skipped Saturday because I chose to sleep and work at my day job in one day. Today we don't sleep, work on this, and go to my day job. Yes, the rest of my life does take up the remaining hours that my job leaves me.**  
- Added bold to the extensions section. Style choice I saw that makes sense for readability. Might do that to more sections, but likely not.  
- Closed div tag in cart.html on L 169. cart.html clears validation.
- I've been thinking that a file called "cat.css" was a bizarre choice, but I didn't want to judge. Found a link tag in cart.html that links to cart.css. -_- 
- cat.css renamed to cart.css
- product-detail.html; comment left states that viewport tags are missing. I likely wouldn't have noticed, since the doctype boilerplate always adds them in for me. Added the viewport tags to index.html, cart.html, and product-detail.html.
- That's not even funny. Ctrl + clicking the font-awesome link **will** take you to the cloudflare website. Copy pasting it directly into the browser will also just bring you to the cloudflare homepage. However, a google search with the link text will illuminate that the 'cloudfare' typo exists. I might not have found that nearly as quickly if not for the product-detail.html comment help.  
  1. Google searched the link. Found Font Awesome with the latest version of 6.7.2 for all.min.css  
  2. Saw there was an option for "copy link tag" next to copy URL. Clicked that.  
  3. Pasted it into index.html over top the old, broken link.  
  4. Got scared. Spent the last 20 minutes learning about CDNs and basic security on the web when linking through them.  
  5. Fixed the link in cart.html and product-detail.html.  
- Fixed the logo icon in product-detail.html and cart.html with correct relative pathing, *and* to correct image file. index.html works since it's in the root and points to the right file.  
- Fixed without understanding. product-details L 167 added data-tab attribute for reviews. That might make sense once I go through js files,
- product-detail.html L 178 says there should be a bug with having no /table tag. But there is one? So I'll mark it fixed in the comment, hopefully it is.
- product-detail.html L 284 added /div tag.
- product-detail.html L 395 added /a tag. I'm confused though as to the empty `<i>` tags. If I'm putting classes on it anyways, can't I just use text-decoration?
- Looking at main.js there is a lot of **comment bloat** happening here. 130 lines of code and 24 of them are comments that are copies of the following line. like L 10 and 11  
  1. **Line 10** // Setup event listeners  
  2. **Line 11** setupEventListeners();  
  That's unnecessary and I'll be removing comments like that as I move through.  

## Thursday 5/1  
How in the heck did this happen! Need to get back to work  
- After a lot of misunderstanding. I added a favicon to cart, product-detail, and index.html.  
- For some reason the subscribe thing works fine on index.html. Must investigate further to see if there's anything janky in the code.  
- Added Todo List.md, realized that I put a space in it like a jerk, fixed it to say todo-list.md
- Made the 4 pages that are listed in the nav bar inside the heading.  
- Discovered that the subscribe bar on homepage works, mostly. And is called the newsletter, which is cute.

### Misc

- Took a peek at the text editor for that .svg, that's neat how tidy it was made and I'm curious as to what program you used Eric.

## Extensions Installed

- **W3C Web Validator** - Celian Riboulet
- **Better Comments** - Aaron Bond
- **Error Lens** - Alexander
- **HTML Boilerplate** - sidthesloth
- **JavaScript (ES6) code snippets** - charalampos karypidis
- **WSL** - Microsoft
- **Live Server** - Ritwick Dey
- **'Prettier - Code formatter'** - Prettier