Project files Personal Blog Website module of Udacity Nano-degree: [Font End Web Developer](https://www.udacity.com/course/front-end-web-developer-nanodegree--nd0011).

You can view live version site [here](https://74c5.github.io/ufed-blog-project/public/index.html)

# Goals

- Create a personal blog website (static) using HTML and CSS.
- Use Grid and Flexbox for CSS layout of site on multiple form factors,
- Fulfil the project rubric

# Folder Structure

- design:  briefs, colours and layouts of the website - anything used to specify the design
    - mockups:  layouts of pages
- public:  served web site folder
    - assets: any images, videos, sounds that required hosting
        - subdirectories for various parts of site
    - authors: author pages
    - css: style sheets for the web pages
    - posts: individual blog post pages

# Components and Design Decomposition

There is a base style (base.css) which contains styles common across all pages and then each page gets its own master css file which may import the following components as needed:

* cards (cards.css)
    - for posts on home page
    - mini-cards for feature section of posts page
* buttons (buttons.css)
  * 2 colours and one inverted (highlight colour)
  * on:hover changes color.
* Other authoring/styling tools
  * figure.css:
    * centred image with caption
    * will float left/right on largest screen
  * quotes.css 
* Float button (already in base.css)
  * mainly for mobile
* Colors (colors.css)
  * color scheme for site (could do with more descriptive names)


# Acknowledgements tools:

- Icons
    - [Font Awesome](https://fontawesome.com/how-to-use/on-the-web/setup/hosting-font-awesome-yourself)
for raw icons and
    - [Fontello](http://fontello.com/) to bundle them into a smaller packs.
    - Favicon generated on [gauger.io/fonticon/](https://gauger.io/fonticon/)
- Avatars
    - Template author image from [Generated](https://generated.photos/)
    - Avatar from [GetAvataaars](https://getavataaars.com)
- Colors
    - [Palleton](http://paletton.com/#uid=70j0u0kqoy79ySAf-KTyPlOEPg-
)


# Future structural Ideas/Improvements

- Bug (21/5/2020): quotes is needs more margin in center when another object is flowed to the left or right of it.
- card preview images should be styled/resized better - with classes for use in html.

Then the following would be easier, if pages were not static or could be compiled.
- post list on author page or as section on post page (would be nice if procedural).
- post tags or categories

# Fixes
a.k.a. Things to do on a production site, but would required extra work or haven't really been considered as part of this project.

- hook up all the share buttons.
- Removal of variables or at least implementation of fall backs
- if needed, vendor prefixes for styling where required (hopefully, through tooling)
- More responsive approach to styling... e.g. a little less use of fixed sizing.
- generally more consistent styling, etc.
    - this isn't a production design, just me playing with various ideas.
    - e.g heading sizes and styles are not consistent or unified across multiple pages.
- some way to order/filter cards on home screen
- post featured section has scroll function in vertical mode so that page length is not stretched by it.

# Personal "Learnings"

- Sand-boxing smaller components (e.g. cards) in simple containers before integration into main site is a good idea.
- Having a CDN for something like this would be really useful.
- A better way to use modular components (Build tools) would be nice. e.g. hard-coding the same header/footer over and over is error prone.
- I couldn't get svg icons to work the way I wanted, it required a lot more glue code and I just couldn't get the colors to apply correctly. In the end it was easier to bundle my own font.
