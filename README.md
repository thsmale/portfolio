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

### Troubleshooting

You may have to manually knit the page for the changes to reflect once you render the site.
I have noticed this in particular with the greenlake dashboard post.
```R
rmarkdown::render("_posts/2025-04-10-project-name/project-name.Rmd")
```

Using `install.packages("<pkg_name>")` may hang forever, use this as a temporary work around on a Linux system.
```
options(repos = c(CRAN = "https://packagemanager.posit.co/cran/__linux__/bookworm/latest"))
```