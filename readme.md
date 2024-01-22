Website is hosted at https://tomportfolio.netlify.app. 

## Creating a new blog post

The following commands into the R console.

This creates a new directory in `_posts/` with the template code.

```R
library(distill)
create_post("Project Name")
```

Then add the directory created in `_posts/` to `index.Rmd`.

Then to build the website fun the following command in R console.

```R
rmarkdown::render_site()
```
