---
layout: components
title: Editor guide
intro: User guide for those who wish to edit this documentation site
nav_exclude: true
---

### Editing a page

Go to the [repository where the code for this docs site lives](https://github.com/asmithdigital/raads-digital). You will need to be logged into GitHub. Then navigate to the ['docs' directory](https://github.com/asmithdigital/raads-digital/tree/main/docs).

All the pages live in the [docs directory](https://github.com/asmithdigital/raads-digital/tree/main/docs), even this guide page. You will notice that this guide page isn't visible in the menu of the docs site, we will come back to that in a minute.

The first thing you want to do is pick a page you want to edit... Say [buttons](https://github.com/asmithdigital/raads-digital/blob/main/docs/components/buttons.md)

You will notice an `index.md` file in that same directory, I'll come back to that in a minute as well. 

  For now, just think about the buttons.md page. The `.md` extension stands for Markdown. Markdown is a very basic way to write HTML. When you hit 'commit' (another word for save), the build tools for the site will convert Markdown to HTML using Magic. Here is a [Markdown cheat sheet](https://www.markdownguide.org/cheat-sheet/).

First, you need to click the edit button pencil icons or 'Edit in place' from the dropdown. Don't click open with `github.dev` or `Github Desktop`. That's just confusing. Just edit it in place.

![alt text]({{site.url}}assets/images/edit-icon.png)

Now, make some changes... add some markdown... go crazy...

Then click the 'Commit changes' button, give your commit a title and a short description, make sure the option 'Commit directly to the main branch' is selected, and then click the 'Commit changes' button. 

![alt text]({{site.url}}assets/images/commit-button.png)

That's it! You have just edited the page. Go to the page, give it a few minutes, then refresh and it should update within 5-10 minutes.

### Now let's get more advanced

You will notice at the top of the page when you are in edit mode, there is a weird table of things, like the one below. That's called 'Front Matter'. It's just a bunch of variables that we can include into the page which will define things such as layouts, page titles, and anything we want. All you do is add the three dashes above and below and then you add the variable on the left, and the value on the right after the colon.

```markdown
---
title: Buttons
layout: components
parent: Components
---
```

Here is all the front matter that I have built into the website so far.

| Variable | Description |
|:-------------|:------------------|
| title | This is the page title and the `<h1>` element |
| intro | This is the page description that will appear below the title, and also on the summary tile seen on the category landing page (which is one of the purposes of the `index.md` file) |
| layout | This determines the page layout. When creating docs pages, use the 'components' layout. I'll describe other layouts in the more advanced section  |
| parent | This is also where the `index.md` comes in. Look at the `index.md` in the same directory as the page you are editing, and find its title. This is the title you must use (case sensitive) for your parent. This will ensure that your page shows up as a child within that section of the menu. Please don't edit the `index.md` |
| nav_order | This will determine the order in which your page appears in the menu within the category. Check the other pages in the category to find out where they are in the nav order. |
| figma | This takes a URL for your Figma file. When you add this variable a table will appear at the bottom of the page with the Figma file link |
| promo-image | This is a thumbnail image that will show up on the category landing page. It takes the file name and extension only, with no path (e.g., `file-name.png`). More on images in a minute. |
| version | Maybe this is a version that you want to display. When you add this variable you can add the version number as the value (e.g., `1.2.3`) and the version number will appear next to the title. I am working on a more advanced feature where we can add multiple versions, but that's not ready yet. |
| nav_exclude | This will hide the page from the menu. The value for this is `true` |

### Uploading images

Create your image and then navigate to [assets/images](https://github.com/asmithdigital/raads-digital/tree/main/assets/images). This is where all images can be uploaded. The `promo-image` Front matter variable knows that images will be in this directory, which is why you don't need to add the image path to the Front matter value.

Click Add file, then Upload file. Drag and drop or Add files, then commit the changes in the same way you did when editing the page. Make sure `Commit directly to the main branch.` is selected.

![alt text]({{site.url}}assets/images/upload-file.png)

That's it. Now you can start adding images to your page using the Front matter, or on the page with Markdown. 

When using images in your page Markdown, use the following URL. Note the variable ```{{site.url}}```. This is defined in the site config. This will define the repository URL and it is important to use this variable because if/when we move the site to a different repository, the images won't all become broken.

Here is an example

```
![alt text]({{site.url}}assets/images/edit-icon.png)
```

