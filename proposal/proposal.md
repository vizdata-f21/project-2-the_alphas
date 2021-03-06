The Alphas Project \#2 Proposal
================

# Project Goal

We intend to create a `Shiny` Application wherein the user inputs an
image and the application outputs a simplified version of this image as
well as a custom color palette based on the image which can then be used
in `ggplot2` visualizations and/or in a paint by numbers.

# Project Motivation and Focus

We’ve been inspired to create this application by the prospect of
automating the “paint-by-numbers” (PBN) process. Limitations in current
R packages make the prospect of generating blank, uncolored PBN
templates untenable, but we instead intend to take an image, bin its
most common colors, then return it with a simplified color palette. The
number of colors in the palette can be controlled by the user using a
sliding bar to indicate a more complex or more simple color palette.
Further, we’ll show some simple visualizations to break down the
frequency of colors in the modified image. Additionally, we will return
the outlines of the image without color using the function we’ve created
for possible printing purposes. We have decided to accomplish these
goals within a shiny app in order to make the application user friendly
and accessible to non-R users, for example.

Here is what we have so far:

![RShiny app](../data/app-screenshot.png)

We’ve chosen to organize our project repository in a similar manner to
our first project. There are four primary folders - data, exploration,
project, and proposal - as well as an overall project `README.md`. Test
images will reside in the data folder while the exploration folder
contains R scripts of our custom functions. The project folder will hold
the final self-contained `Shiny` app and final versions of the functions
in exploration. The final goal is that the user may upload their own
images and thus eliminating a need for the data or exploration folders.

# Weekly Plan Outline

Week of 11/8: all 4 team members will go through peer review of the
proposal and make any necessary edits to the project/proposal. Resubmit
if necessary. Margaret can perfect the function that draws the
boundaries of the colors. Evan will work on integrating the back-end
image parsing with image upload capabilities for `Shiny`. Emely and
Andrew will explore the features of the colordistance package and aid
other team members where necessary.

Week of 11/15: The basic part of the project should be solidified at
this point (ie: drawing boundaries, extracting color, etc) At this point
we can start working on the `Shiny` app which will be the user’s
interface for uploading their image. All 4 team members should
contribute to this, and Evan can spearhead the efforts with his previous
experience working with interactivity and `Shiny`. Simultaneously, we
should explore the other facets of the project and see which of the
ideas we came up with is going to be the most feasible and interesting.

Week of 11/22: Continue developing the `Shiny` app, incorporate the
aspects of the project that we decide on the previous week (ie:
interactive paint by numbers, the different visualizations, etc). Begin
presentation slides and write up. Emely and Margaret will take the lead
on the write up and Andrew and Evan will work on the presentation
slides.

Week of 11/29: Finalize all aspects of the `Shiny` app and project in
general. Have other people test out the `Shiny` app to ensure it is
working and user friendly.

# Package Documentation

<https://hiweller.github.io/colordistance/>

<https://cran.r-project.org/web/packages/magick/vignettes/intro.html>
