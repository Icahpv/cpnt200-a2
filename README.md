# CPNT200-a2 + CPNT200-a3
- **Netlify CMS Admin Panel & Collections**
- ** JAMstack Setup**

* Instructor: [Ashlyn Knox](https://github.com/lilyx13)
* Links: [Github Repo](https://github.com/Icahpv/cpnt200-a2) | [Netlify Site](https://netlify-homework.netlify.app/) + admin
* CSS Framework: [Vuetify.js](https://vuetifyjs.com/en/)

## Assignment 2 Review

- [x] Configuration (20%)
  - [x] Properly set up your netlify admin inside a nuxt project
  - [x] Deploy to Netlify
- [x] Widget (30%)
  - [x] Must have a title
  - [x] Must have a label
  - [] 1 Feature Widget
    - [] Has to be unique to the collection.
    > not sure if I understood this part correctly.
- [x] Collections (30%)
  - [x] Collections are properly defined in your admin directory
  - [x] Define two new collections
- [x] Readme (20%)
  - [x] Add links to your github repo and github pages site
    > I don't have a gh pages site, but I added my netlify site
  - [x] Code Review
    - Write briefly about anything you found interesting, difficult, or easy about coding this assignment
  - [x] Attributions

- This assignment is awesome, I didn't think a framework could do this and create a blog from the scratch. I had difficulty figuring out how to add collections, I believe the collections I added are very simple and there's more to it. I have tried adding and taking out in my collections and it all just seem to break some code, I hope I could see more of this in action. 
- What I Discovered! If I publish entries, netlify will automatically create .md files to my contents, which is crazy!

## Assingment 3 Review

- [x]Configuration (20%)
  - [x] Netlify CMS + Nuxt Deployed to Netlify
- [x] CMS Content (30%)
  - [x] Write 4 entries using two different collections. Can be sample content
  - [x] Collections should have different fields.
- [x] Nuxt-Content to Render your Collection Posts
  - [x] _slug.vue file properly set up
  - [x] Posts created in netlify cms render onto your website
- [x] Code Review & Readme

- I had a bit of difficulty getting my original repo to work so I used my 2nd assignment, I also didn't want to waste the content I added already, I hope it's okay.
- Vuetify.js, I couldn't get this CSS to work.
- Nuxt/Image - could not render images from my content to the slug files. I'm not exactly sure how to make that work, I tried v-binding but it's not working.
- This assignment was a bit difficult for me, because there's a lot of back and forth to folders and if you are bad at naming convention, it's very easy to confuse things. I'm happy I made it work.


### Attributions

- [Netlify CMS Common Widgets](https://www.netlifycms.org/docs/widgets/#file)
- [Ashlyn Knox](https://github.com/lilyx13): Code examples, specifically her [dog-blog](https://github.com/lilyx13/dog-blog) repo.


#### License
[MIT License](LICENSE) :scroll:

---

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out the [documentation](https://nuxtjs.org).

## Special Directories

You can create the following extra directories, some of which have special behaviors. Only `pages` is required; you can delete them if you don't want to use their functionality.

### `assets`

The assets directory contains your uncompiled assets such as Stylus or Sass files, images, or fonts.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/assets).

### `components`

The components directory contains your Vue.js components. Components make up the different parts of your page and can be reused and imported into your pages, layouts and even other components.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/components).

### `layouts`

Layouts are a great help when you want to change the look and feel of your Nuxt app, whether you want to include a sidebar or have distinct layouts for mobile and desktop.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/layouts).


### `pages`

This directory contains your application views and routes. Nuxt will read all the `*.vue` files inside this directory and setup Vue Router automatically.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/get-started/routing).

### `plugins`

The plugins directory contains JavaScript plugins that you want to run before instantiating the root Vue.js Application. This is the place to add Vue plugins and to inject functions or constants. Every time you need to use `Vue.use()`, you should create a file in `plugins/` and add its path to plugins in `nuxt.config.js`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/plugins).

### `static`

This directory contains your static files. Each file inside this directory is mapped to `/`.

Example: `/static/robots.txt` is mapped as `/robots.txt`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/static).

### `store`

This directory contains your Vuex store files. Creating a file in this directory automatically activates Vuex.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/store).
