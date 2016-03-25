---
layout: post
title: Introducing swirl 2.4
active: blog
date: 2016-03-25 14:00:00
---

# Introducing swirl 2.4.0

The first major swirl release in over a year comes with some big changes. First
we would like to thank all of the translators that 
[answered the call](http://swirlstats.com/blog/polyglot.html) when we started
looking for volunteers to translate swirl's menus. Because of their efforts 
swirl's menus are now available
in Spanish, French, German, Turkish, Simplified Chinese, and Korean in addition
to English. You can select the language you prefer with the new `select_language()`
function. There have also been several amazing courses created for swirl in 
non-English languages including [ConoceR](https://github.com/dhduncan/ConoceR)
by David Duncan, [Programando en R](https://github.com/josersosa/Programando_en_R)
by José Sosa, [Programación Estadística con R](https://github.com/ifunam/programacion-estadistica-r)
by Ismael Martínez, and [Data Science and R (R語言翻轉教室)](https://github.com/wush978/DataScienceAndR/tree/course) by Wush Wu.

Courses created with the latest version of swirlify can be distributed as `.swc`
files, and these files can be installed with the new `install_course()`
function. This function also aims to replace `install_from_swirl()`.
Providing just the name of the course you want to install -  for example
`install_course("R Programming")` - will install the course up to ten times faster
than `install_from_swirl("R Programming")`. We do not have to plans to remove any of 
swirl's old course installation functions, however moving forward `install_course()`
will receive the most attention from developers.

We've also added an interface for `options()` called `swirl_options()` which
allows you to change where courses are installed on your computer, where swirl
user data is stored on your computer, and whether or not swirl should log your
progress during lessons. We'll be releasing details on how you can use logging
in swirl courses in order to evaluate how your students are using swirl.

From this release on we expect to have regular updates every one or two months, 
with new features and menu translations. If you have any questions, comments, or
suggestions please send us an email, a tweet, or a pull request!

**- Team swirl**