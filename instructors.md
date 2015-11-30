---
layout: page
title: swirl | Instructors
active: teach
---


# You're an instructor!

swirl is a platform for teaching R programming and data science. However, an educational platform is only as good as the content it delivers to students. Although we have contributed [some content](https://github.com/swirldev/swirl_courses#swirl-courses){:target="_blank"} ourselves, swirl is designed in such a way that you can create your own interactive content and share it freely with students in your classroom or around the world.

The [swirlify](https://github.com/swirldev/swirlify){:target="_blank"} R package provides a comprehensive toolbox for swirl instructors. Our authoring tools will guide you effortlessly through the process of creating interactive content, so that you can focus on the message you want to convey to students. The instructions that follow will have you writing your own interactive content with swirlify in just minutes! For more complete instructions about writing swirl courses please see [our wiki](https://github.com/swirldev/swirlify/wiki).

## Step 1: Get R

In order to run swirl and swirlify, you must have R 3.0.2 or later installed on your computer. If you are on a Linux operating system, please visit our [Installing swirl on Linux](https://github.com/swirldev/swirl/wiki/Installing-swirl-on-Linux){:target="_blank"} page.

If you need to install R, you can do so [here](http://cran.rstudio.com/){:target="_blank"}.

For help installing R, check out one of the following videos (courtesy of Roger Peng at Johns Hopkins Biostatistics):

- [Installing R on Windows](http://youtu.be/mfGFv-iB724){:target="_blank"}
- [Installing R on Mac](http://youtu.be/Icawuhf0Yqo){:target="_blank"}

## Step 2 (recommended): Get RStudio

In addition to R, it's highly recommended that you install RStudio, which will make your experience with R much more enjoyable.
	
If you need to install RStudio, you can do so [here](http://www.rstudio.com/products/rstudio/download/){:target="_blank"}. Select the appropriate installer for your operating system.

## Step 3: Install swirl and swirlify

Open RStudio (or just plain R if you don't have RStudio) and copy and paste the following commands into the console to install everything you need:

```
install.packages(c("swirl", "swirlify"))
```

## Step 4: Start swirlify

Type `library(swirlify)` at the R prompt to load the package. You'll have to repeat this step every time you restart R or RStudio.

## Step 5: Create a new lesson or edit an existing one

swirl courses are collections of individual lessons. It's up to you how long you'd like each lesson to be, but we think it's better to have many short, focused lessons than a few long, very general ones.

To create a new lesson:

```
new_lesson("My Lesson", "My Course")
```

This will create a course directory in your current working directory that looks like this (notice the underscores):

```
─ My_Course
  └─ My_Lesson
     ├─ lesson.yaml
     ├─ initLesson.R
     ├─ dependson.txt
     └─ customTests.R
```

To start working on an existing lesson:

```
set_lesson() # Set the lesson interactively

## OR...

set_lesson("path/to/My_Course/My_Lesson/lesson.yaml") # Set the lesson directly
```

Regardless of whether you use `new_lesson()` to create a new lesson or `set_lesson()` to open an existing one, swirlify should open the lesson file automatically for you to start editing.

## Step 6: Create your interactive content!

For more complete information see the [swirlify wiki](https://github.com/swirldev/swirlify/wiki), but here some helpful hints to get you on your way:

- Save your lesson file often as you edit it!
- To test your lesson in swirl, save the lesson file, then type `testit()` at the prompt. You may wish to use the `from` and `to` arguments with `testit()` for testing specific portions of your lesson. Check out `?testit` for more information.
- Use <a href="http://git-scm.com/" target="_blank">Git</a> and <a href="https://github.com/" target="_blank">GitHub</a>! If you're new to version control, GitHub provides <a href="https://help.github.com/articles/set-up-git" target="_blank">excellent tutorials</a> for beginners. swirl even has a built-in function (`install_course_github()`) that allows students to download a course directly from your GitHub repository!
- A great way to get comfortable with authoring your own content is by <a href="https://guides.github.com/activities/forking/" target="_blank">forking</a> our <a href="https://github.com/swirldev/swirl_courses" target="_blank">course repository</a> on GitHub and loading one of our R Programming lessons into swirlify (using `set_lesson()`). Experiment by making changes to the lesson, then use `testit()` to run the lesson in swirl with your changes.
- Read <code>?AnswerTests</code> for more information on how answer testing works.
- Keep your answer tests simple at first (e.g. `omnitest('x <- rnorm(10)')`), so that you can focus on writing content. You can always go back and make them more sophisticated later.
- Any variables you define in initLesson.R will appear in the user's workspace upon starting the lesson.
- For examples of how to include data in a lesson, install and run the <em>Including Data</em> lesson from our <a href="https://github.com/swirldev/swirl_misc" target="_blank">development repository</a> via <code>install_from_swirl("Including Data", dev = TRUE)</code>.
- swirl lessons are written in <a href="http://www.yaml.org/" target="_blank">YAML</a>. If you haven't used YAML before, have no fear! We chose it for its simplicity and ease of use. However, if you want to use certain special characters like `:`, you need to surround your text with single or double quotes. Here's a simple example:

```
- Class: text
Output: "The following command assigns the mean of x to y: y <- mean(x)."
```

- If you are using RStudio to edit lesson.yaml, set the file type to <em>Text File</em> in the bottom righthand corner of the editor. This will enable text wrapping.




## Step 7: Ask questions and get involved

To ask and answer questions about authoring swirl content, check out our <a href="https://groups.google.com/group/swirl-discuss" target="_blank">swirl discussion group</a>. Don't hesitate to <a href="mailto:info@swirlstats.com" target="_blank">send us an email</a> if you can't find the answer you're looking for.