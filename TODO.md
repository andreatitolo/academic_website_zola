# Website basic structure

## Initial stage

- [x] Create basic homepage and subpages
  - [x] publication, courses, talks, projects, teaching, contact, CV, Search, More.., Blog
  - [x] header (manual lists)
  - [x] footer (manual lists)
  - [x] homepage (all text)
  - [x] Create _index.md of all subpages
  - [x] Create two placeholder markdown files for each subpage
  - [x] Create contact page
    - [x] Need to add a page.html template to render single pages
  - [x] Privacy
  - [x] Colophon
  - [x] Credits
  - [x] More

## Middle stage

- [ ] Implement basic CSS for homepage
  - [x] Only the visible stuff
  - [x] Flexbox for homepage (try to avoid all the classes)
  - [ ] header links animation
  - [ ] header background
  - [ ] header shadow?
  - [ ] buttons are too big
    - [ ] shadows under button
- [x] Try image
- [x] Replace footers and headers lists using zola syntax and TOML config
  - [x] Image path in config
  - [x] Menu items
  - [x] institution
  - [x] role
  - [x] email
  - [x] social buttons
  - [x] interest items
  - [x] education
  - [x] See others from kodama theme
  - [x] bio
  - [/] footer?
  - [x] favicon
- [x] Aria current to navbar
- [x] Apply a proper templates 
  - [x] pubs
    - [x] css
      - [x] links are not underlined
      - [x] Add to zotero button in publication page?
      - [x] unify publishers website and pdf
      - [x] Add preprint button
  - [x] courses
    - [x] css
  - [x] talks
    - [x] css
      - [x] notice class
  - [x] teaching
    - [x] css
  - [x] Publist
    - [x] css
    - [x] test local files (bib and pdf)
  - [x] Talkslist
  - [x] Teachinglist
- [x] Add datetime to publication page
- [x] cv
- [x] search
- [x] contact page
- [x] Style aria current page
- [x] 404 page
- [x] More page
- [x] prev next link from duckquill https://daudix.codeberg.page/duckquill/blog/

## Late stage

- [x] Link underline animation (even theme) only in header
- [x] Color change of links in text - leave underline? add accent-hover as variable
- [x] Put links in homepage bio
- [x] Privacy
- [x] Colophon
- [x] Credits
- [x] Import data
  - [x] publications
  - [x] talks
    - [x] Fix slides location in list page
    - [x] Add nav footer to talk like pub
  - [x] teaching
    - [x] same as above
- [x] cv
- [x] See how everything look 
- [x] Fix publications list pdf
- [x] make pub_container larger on larger screens
- [x] change color scheme
  - [x] Dark mode
- [x] change fonts
- [x] links footer
- [/] push search to the right?
- [/] style archaeoring with classes?
- [x] Test classless css
  - [x] Mostly font-weight, lists and similar
- [x] Year in parenthesis after the authors in publication list
- [x] Change "list of" to just the name
- [x] add conditional bold if the author is the same as config.author
- [x] remove useless classes from pages and page footer nav
- [/] Use something like author in toml frontmatter and convert it to author using something like {{ item.link | replace(from='$EMAIL_ADDRESS', to=config.extra.email)}}
- [/] same with the publication types?
- [/] Author institution as with hugo and css tooltip in template?
- [x] Add comma separator to Authors in page and lists
- [/] Use a shortcode or a macro for author bold - not working
- [x] Safari favicon is broken
- [x] Favicons not present in subpages
- [x] More space between tags
- [ ] Create taxonomy for tags
  - [ ] Style tag list and single page
- [ ] Do the same for authors?
- [/] Remove cite button on the publication page and use the rendering of the bibtex as with Kodama?
- [ ] Add a README
- [ ] See if some taxonomies tags can be removed

# Style

# Publish

- [ ] redirects needed?
  - [ ] For talks, yes -> see docs for zola aliases at https://www.getzola.org/documentation/content/section/ https://www.getzola.org/documentation/content/page/
- [ ] robots.txt
- [ ] fix atom feed, see: https://github.com/getzola/zola/issues/2404
- [ ] security headers
- [ ] netlify.toml with zola version
- [ ] Update site metrics
- [ ] Mobile spacing, fonts, and stuff

# Future

- [ ] Make all margins the same across the pages (no layout change when switching pages)