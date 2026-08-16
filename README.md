# recipe-collection

1. **Website Creation**
    For this project, I created a recipe website showcasing five recipes I put together. Each recipe is presented as its own section containing a title, an image of the finished dish, a list of ingredients, step-by-step cooking instructions, and a nutrition breakdown. The site is
    structured with a header and navigation menu at the top linking to each recipe, and a footer
    at the bottom. My goal was to create a clean, easy-to-navigate page where each recipe is clearly organized and simple to follow.

2. **HTML Elements**
    - '<nav>' and '<a href="#id">' : Understanding how a link’s href=”#pasta” matches an
     element’s id=“pasta” took some getting used to, along with learning what the title attribute
     does as a hover tooltip. 
    - '<figure>' / '<figcaption>' : I initially didn’t see why this was needed
     over a plain image and caption, until I understood it groups them as one related unit. •
    - '<time>' : The most confusing, since it adds no visible change to the page. I learned the
    datetime attribute stores a machine-readable value behind the scenes. 
    - '<p>' vs. heading tags : I first assumed the difference was just font size, before realizing headings represent structural importance, not just styling. 
    - '<table>' : Getting '<tr>', '<th>', and '<td>' properly nested and closed took some trial and error.

    - I used '<header>' for the site title and navigation, '<main>' to wrap all the recipe content,
'<article>' for each individual recipe as a self-contained unit, '<section>' for the nutrition
overview, and '<footer>' for the copyright notice at the bottom.
iii. '<article>' was the most useful, since it let me treat each recipe as its own independent
block of content with a consistent internal structure (heading, image, ingredients, steps),
making the page easy to navigate and extend.

3. **HTML Attributes**
    - href - without it, my navigation links wouldn’t be able to jump to each recipe section. 
    - id- needed to give each recipe a unique target for the navigation links to point to.
    - src -required for each <img> to actually display an image on the page.

   - I used id to give each recipe a unique identifier so navigation links could jump to that
   specific section. I used class=“recipe” on all five <article> elements to mark them as the
   same type of content since a class can be reused across multiple elements while an id must
   stay unique to one.

   - alt was the most useful for user experience, since it describes each image for people
   using screen readers or in cases where an image fails to load, making the site more accessible.

4. **Development Process**
    - I decided on a recipe website as my topic, then planned out the content I wanted to include. I mapped out the structure before writing code.. a header with navigation, a main section containing each recipe as its own article with a consistent format (image,ingredients, steps) and a footer.

    - I regularly saved my file and opened it in the browser to check that changes displayed as
expected. When something looked wrong, I checked for unclosed or mismatched tags,
which was especially useful when I built the nutrition table and figure elements since a
missing closing tag caused a formatting issue.

   - One of my biggest challenges was pushing my project to GitHub for the first time. I ran
into an authentication issue, then a merge conflict because my repository had a README
file created directly on GitHub that didn’t exist in my local project. I resolved this by pulling
the remote changes with –allow-unrelated-histories, resolving the merge, and completing
the merge commit before pushing again successfully.

5. **Git & GitHub Implementation**
    - I used git init to start the repository, git add and git commit to stage and save changes, git
push origin main to upload to GitHub, and git pull origin main –allow-unrelated-histories to
resolve a merge conflict. I also used git status, git log –oneline, git remote -v, and git ls-files
to check the state of my repository while troubleshooting.

   - I made 7 commits total. My strategy was to write short, lowercase, present-tense
messages describing what changed in that commit e.g. “add pasta recipe”, “add nutrition
table”.

   - Version control keeps a full history of changes, so mistakes can be traced or reverted if
needed. It also makes collaboration possible since multiple people can work on the same
project and safely combine their changes.

6. **Code Quality & Best Practices**
    - I regularly opened my file in the browser to check it rendered correctly, and checked for
common mistakes like unclosed tags or mismatched opening/closing tags when something
didn’t display as expected.

- I used consistent indentation, gave elements meaningful id and class names (e.g.
id=“pasta”, class=“recipe”), used semantic elements to reflect the actual structure of the
content, and kept each recipe formatted the same way for consistency.

- I would add more detailed content such as serving sizes, and possibly restructure the
nutrition information to appear within each recipe individually rather than as a separate
summary table.