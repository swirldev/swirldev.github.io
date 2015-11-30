---
layout: page
title: swirl | FAQ
active: faq
---

<h1>You have (frequently asked) questions!</h1>

<p>If you don't find an answer to your question on this page, please check our <a href="help.html">Help page</a> for more options.</p>

<p class="question">What is swirl?</p>
<p class="answer">swirl is a software package for the R programming language that turns the R console into an interactive learning environment. Users receive immediate feedback as they are guided through self-paced lessons in data science and R programming.</p>
<p class="answer">For a more technical discussion of swirl's inner workings, please visit our <a href="https://github.com/swirldev/swirl" target="_blank">GitHub repository</a>. The project is entirely open source, so you're only limited by your own curiosity.</p>

<p class="question">Who is swirl's intended audience?</p>
<p class="answer">Most of the original swirl content was developed with beginners in mind. We have added more advanced topics over time and will continue to do so in the future. For the most up-to-date course information, check out our <a href="https://github.com/swirldev/swirl_courses#swirl-courses" target="_blank">course repository</a>.</p>

<p class="question">What do I need to use swirl?</p>
<p class="answer">Check out our <a href="students.html">Students page</a> for step-by-step instructions on getting started with swirl. Most importantly, you'll need a computer with an internet connection and a recent version of R installed. We highly recommend you get RStudio as well.</p>

<p class="question">Is RStudio required to run swirl?</p>
<p class="answer">No, but we highly recommend it. The main reason for this is that it will make your life as an R programmer a whole lot easier, particularly if you're new to R. It's possible that at some point in the future we will add functionality to swirl that makes special use of RStudio's graphical user interface (GUI).</p>

<p class="question">How long will it take me to work through a typical swirl lesson?</p>
<p class="answer">Although swirl lessons vary in length, we aim to keep them around 10-20 minutes a piece. We find that this is generally long enough to convey a meaningful amount of information, but not so long that you'll get bored or overwhelmed. A key feature of the swirl learning environment is that it is totally self-paced, meaning that you can take as much (or as little) time as you need to fully understand the material.</p>

<p class="question">How did swirl begin and who is behind it?</p>
<p class="answer">The idea for swirl grew out of a conversation between a graduate student at <a href="http://www.jhsph.edu/departments/biostatistics/" target="_blank">Johns Hopkins Biostatistics</a>, <a href="http://nickcarchedi.com/" target="_blank">Nick Carchedi</a>, and his mentor, <a href="http://www.bcaffo.com/" target="_blank">Brian Caffo</a>, during the summer of 2013. At the time, Nick was looking for a summer project to keep him out of trouble. Fed up with the lack of existing tools for learning R and data science interactively, he wondered whether he could create an interactive learning environment within the R console. Brian challenged him to try.</p>
<p class="answer">Over the next several weeks, with sage advice from Brian, Jeff Leek, and Roger Peng, a prototype for swirl emerged. With the gracious help of two summer interns, Lauren Williams and Ethan Schwartz, Nick created some preliminary instructional content. In September 2013, the release of <a href="http://simplystatistics.org/2013/09/27/announcing-statistics-with-interactive-r-learning-software-environment/" target="_blank">swirl 1.0 was announced</a> on Simply Statistics.</p>
<p class="answer">This news caught the attention of a couple, Bill Bauer and Gina Grdina, who had a strong interest in education, math, and software development. Bill and Gina reached out to Nick and have since been instrumental in transitioning swirl from a quirky prototype to a serious learning tool. Many others have contributed along the way to swirl's success and are credited in Nick's <a href="http://simplystatistics.org/2014/01/28/swirl-2/" target="_blank">follow-up post</a> on Simply Statistics.</p>
<p>In 2015 <a href="http://seankross.com" target="_blank">Sean Kross</a> took over as the maintainer and lead developer of swirl. Sean and Nick met in the summer of 2013 during their work in the <a href="http://jhudatascience.org/">Johns Hopkins Data Science Lab</a>.</p>

<p class="question">Will swirl always be free and open source?</p>
<p class="answer">The swirl R package and its core content will ALWAYS be free and open source. This is something we take very seriously.</p>
<p class="answer">While we may offer customized content or advanced features/add-ons to enterprise customers, this will NEVER impact individual users. Furthermore, we will NEVER attempt to profit from content contributed by independent instructors without explicit consent.</p>

<p class="question">Does any content I contribute to swirl remain my property?</p>
<p class="answer">Yes! If you share content via the swirl platform, it remains 100% in your control. In fact, we're currently working on a better way to give instructors credit for their contributed content. swirl is a platform of the people, by the people, and for the people!</p>

<p class="question">How do I get the most recent version of swirl?</p>
<p class="answer">As we are constantly adding new features and content to swirl, we will make the most recent version of the software available on <a href="http://cran.r-project.org/" target="_blank">CRAN</a> every 1-2 months. Standard installation instructions can be found on our <a href="students.html">Students page</a>.</p>
<p>If you want all of the latest features and content, but don't feeling like waiting around for the official updates to be released, you can always access the development version of swirl via our <a href="https://github.com/swirldev/swirl" target="_blank">GitHub repository</a>. Here's the process for installing and running the development version of swirl directly from the R console:</p>
<pre>> install.packages("devtools")
> library(devtools)
> install_github("swirldev/swirl")
> library(swirl)
> swirl()</pre>
