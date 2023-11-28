---
title: "Papermod"
date: 2023-11-14T12:49:20-05:00
author: "Ney Perea"
draft: false
---

## hugo file system

![treeFileStruc.png](img\treeFileStruc.png)
###  content folder
Post, articles, pages all we work should be store in here.
###  layout folder
for theme override, if you want to modify themes layout just copy layout theme´s folder in here then modify.
### static
for images and static files

---
to add a new content:

```
hugo new posts/newfile.md

```


### markdown sintax

```
hugo  server

```

```
![coverimage](img/coverImage.png)
```

to render an image the picture should be inside **static** folder
![coverimage](img/coverImage.png)
this is an example to link an image to out article in papermod theme.


## making menus

![coverimage](img/makingMenu.png)

**weight** identifies the order of de menu position

if there is no page that represent the menu you want to display it will send you a 404 alert

![there isnt page](img/noPage.png)

in here there is no archieve page.

![there isnt page](img/createApage.png)

must be an page that represent the view inside layout theme.

![archieve in laytou](img/archieveInlayout.png)

![overide a theme page](img/overideAthemePage.png)


in the frontmatter you can add "tag" tags of your post 
or "categories" tags

![more options](img/configFileMoreOptions.png)

you can overide everything just read the layout theme pages. so you can modify both a parametrer either html code.











