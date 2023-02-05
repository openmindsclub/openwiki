# Adding a Pizza Recipe

1. Add the `pizza-recipe.md` file of the article in `/content/en/posts` or `/content/fr/posts` depending on the language of the article.

2. Add headers to the `/content/{en|fr}/posts/pizza-recipe.md` like so:

```
---
author: "Lilia Mehamli"
title: "Pizza Recipe A to Z"
date: 2023-02-05
description: "Learn how to make a pizza recipe the open source way!"
tags: ["pizza", "recipe", "cooking"]
thumbnail: "/pizza-recipe/thumbnail.jpg"
---
```

3. Add the thumbnail of the Pizza Recipe in `/static/pizza-recipe/thumbnail.jpg`

PS: Keep in mind that the path of the thumbnail is declared in the headers (step 2) without specifying the parent folder `/static/`

4. For the sake of conformity, we will upload all the images/media files in `pizza-recipe.md` to the folder `/static/pizza-recipe/`. And they will be referenced as such:

```
![Screenshot](/pizza-recipe/tomato.png)
```

PS: Again, without specifying the parent folder `/static/`
