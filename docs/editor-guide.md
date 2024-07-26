---
layout: components
title: Editor guide
nav_exclude: true
---

## Editing your first page

Go to the [repository where the code for this docs site lives](https://github.com/asmithdigital/raads-digital). You will need to be logged into GitHub. Then navigate to the 'docs' directory.

All the pages live in the docs directory, even this guide. You will notice that this guide page isn't visible in the menu of the docs site, we will come back to that in a minute.

The first thing you want to do is pick a page you want to edit... Say [buttons](https://github.com/asmithdigital/raads-digital/blob/main/docs/components/buttons.md)

You will notice an `index.md` file in that same directory, I'll come back to that in a minute as well. 

For now, just think about the buttons.md page. The `.md` extension stands for Markdown. Markdown is a very basic way to write HTML. When you hit save, the build tools for the site will convert Markdown to HTML using Magic. Here is a [Markdown cheat sheet](https://www.markdownguide.org/cheat-sheet/).

First, you need to click the edit button pencil icons or 'Edit in place' from the dropdown. Don't click open with `github.dev` or `Github Desktop`. That's just confusing. Just edit it in place.

Now, make some changes... add some markdown... go crazy...

Then click the Commit changes button, give your commit a title and a short description, make sure the option 'Commit directly to the main branch' is selected, and then click the Commit changes button. 

That's it! You have just edited the page. Go to the page, give it a few minutes, then refresh and it should update within 5-10 minutes.

## Now lets get more advanced

You will notice at the top of the page when you are in edit mode, there is a weird table of things.

`---
title: Buttons
layout: components
parent: Components
---
`
