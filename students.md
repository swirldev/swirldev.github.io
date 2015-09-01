---
layout: page
title: swirl | Students
active: learn
---

# You're a student!

The swirl R package makes it fun and easy to learn R programming and data science. If you are new to R, have no fear. On this page, we'll walk you through each of the steps required to begin using swirl today!

## Step 1: Get R

In order to run swirl, you must have R 3.0.2 or later installed on your computer. If you are on a Linux operating system, please visit our [Installing swirl on Linux](https://github.com/swirldev/swirl/wiki/Installing-swirl-on-Linux){:target="_blank"} page.

If you need to install R, you can do so [here](http://cran.rstudio.com/){:target="_blank"}.

For help installing R, check out one of the following videos (courtesy of Roger Peng at Johns Hopkins Biostatistics):

- [Installing R on Windows](http://youtu.be/mfGFv-iB724){:target="_blank"}
- [Installing R on Mac](http://youtu.be/Icawuhf0Yqo){:target="_blank"}

## Step 2 (recommended): Get RStudio
In addition to R, it's highly recommended that you install RStudio, which will make your experience with R much more enjoyable.
	
If you need to install RStudio, you can do so [here](http://www.rstudio.com/products/rstudio/download/){:target="_blank"}. Select the appropriate installer for your operating system.

<h2>Step 3: Install swirl</h2>
<p>Open RStudio (or just plain R if you don't have RStudio) and type the following into the console:</p>
<p><code>> install.packages("swirl")</code></p>
<p>Note that the <code>></code> symbol at the beginning of the line is R's prompt for you type something into the console. We include it here so you know that this command is to be typed into the console and not elsewhere. The part you type begins after <code>></code>.</p>

<h2>Step 4: Start swirl</h2>
<p>This is the only step that you will repeat every time you want to run swirl. First, you will load the package using the <code>library()</code> function. Then you will call the function that starts the magic! Type the following, pressing Enter after each line:</p>
<pre>> library("swirl")
> swirl()</pre>

<h2>Step 5: Install an interactive course</h2>
<p>The first time you start swirl, you'll be prompted to install a course. You can either install one of the recommended courses or visit our <a href="https://github.com/swirldev/swirl_courses#swirl-courses" target="_blank">course repository</a> for more options.</p>
<p>If you'd like to install a course that is not part of our course repository, type <code>?InstallCourses</code> at the R prompt for a list of functions that will help you do so.</p>

<h2>Step 6: Have fun!</h2>

<p>Please visit our <a href="help.html">Help page</a> if you have trouble completing any of these steps.</p>