# Writing Your First R Package
Repository for the 2025 ICA Pre-Conference Hackathon Breakout Session

## Prerequisites 
- You can code in R
- You know (more or less) how to define a function

## Reading
Wickham, H., & Bryan, J. (2023). _R Packages: Organize, Document, and Share Your Code._ O'Reilly Media. Link: https://r-pkgs.org/

## What you need to do
### Install the life-saving packages
```
install.packages(devtools)
install.packages(usethis)
```

### Create a R Project
```
usethis::create_package("myfirstpkg")
```

### Have at least one function
```
get_sd <- function(x){
  stats::sd(x)
}
```

### Documentations
Heres are some useful functions to have, I will explain it later...
```
usethis::use_mit_license()
usethis::use_package("stats")
devtools::document()
```

### Setup a Git Repository
Again, some useful functions:
```
usethis::use_git()
usethis::gh_token_help()
usethis::create_github_token()
gitcreds::gitcreds_set()
```

### Create first release
```
usethis::use_release_issue()
```

### Install your package
If you follow the steps, you would have your first package ready to be installed. Seriously, it is that simple. You could use the follow code to install (before putting it on CRAN)
```
devtools::install_github("justinchuntingho/myfirstpkg")
```

### What's next?
- Readme
- Vignette
- Unit tests
- Get good at Git (optional, but seriously you would thank yourself in the future)
- Bug reports
- Write a software paper (for example, Journal of Open Source Software)
