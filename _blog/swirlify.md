---
layout: post
title: Getting Started with swirlify
active: blog
date: 2015-11-30 15:10:00
---

# Introducing swirlify!

Have you ever wanted to write your own swirl course? Now it's easier than ever! Team swirl is proud to announce swirlify, an R package for writing swirl courses. The swirlify package includes functions for adding question templates, sharing your course, testing your course, and even licensing your course. We've designed swirlify to be used with the latest version of RStudio, which you can download [here](https://www.rstudio.com/products/rstudio/download/). Now for a quick demo of how you can use swirlify:

```r
# We're on CRAN! 😍
install.packages("swirlify")

library(swirlify)

# Create a new lesson and a new course
new_lesson("My Lesson", "My Course")

# Start editing your new lesson
file.edit(lp())

# Add some questions! These functions are specially designed to be used with
# autocompletion on western English keyboards. Just type: `W` -> `Q` ->`Tab`
# for a list of functions for adding types of questions.
wq_message()
wq_multiple()
wq_numerical()

# Add your lesson to the MANIFEST so you can distribute and test your new lesson
add_to_manifest()

# After filling in the question templates make sure your lesson is formatted
# correctly.
test_lesson()

# Test your lesson in swirl
testit()

# Add a permissive license (because we love open source)
add_license()

# If you're satisfied you can pack your new swirl course into a single file
# and share it with the world!
pack_course()
```

You can find extensive documentation for swirlify in our [wiki](https://github.com/swirldev/swirlify/wiki). If you have any questions about using swirlify we encourage you to contact us at [info@swirlstats.com](mailto:info@swirlstats.com).

**-Team swirl**