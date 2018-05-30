<!-- markdownlint-disable MD022 MD032 -->
# James Priest

## 100 Days Of Code

| Log 1 | Log 2 | Log 3 |
| --- | --- | --- |
| [100 Days Round 1](https://james-priest.github.io/100-days-of-code-log/) | [100 Days Round 2](https://james-priest.github.io/100-days-of-code-log-r2/) | this log |

## Challenge & Commitment
This is part of Alexander Kallaway's [100DaysOfCode](https://github.com/Kallaway/100-days-of-code "the official repo") challenge. More details about the challenge can be found here: [100daysofcode.com](http://100daysofcode.com/ "100daysofcode.com").

**Commitment:** *I will code daily for the next 100 days.*

|  Start Date   | End Date     |
| ------------- | ------------ |
| May 9, 2018   | - - - |

## Goals

- [x] Code daily
- [x] Complete Udacity's [Grow with Google Challenge Scholarship](https://www.udacity.com/grow-with-google) - Mobile Web Specialist
- [x] Get accepted to the Google Udacity [Mobile Web Specialist Nanodegree](https://www.udacity.com/course/mobile-web-specialist-nanodegree--nd024) program
- [ ] Successfully complete the Google Udacity [Mobile Web Specialist Nanodegree](https://www.udacity.com/course/mobile-web-specialist-nanodegree--nd024) program
- [ ] Pass the Microsoft Programming in HTML5 with JavaScript & CSS3 Cert - [Exam 70-480](https://www.microsoft.com/en-us/learning/exam-70-480.aspx "Exam 70-480: Programming in HTML5 with JavaScript and CSS3")
- [ ] Pass the Google [Mobile Web Specialist Certification](https://developers.google.com/training/certification/mobile-web-specialist/) exam for Mobile Web Development

# Code Log
<!--

## 1.
### Day 1: January,10 2018 - Saturday

**Project:** Mobile Web trackS

**Progress:**

**Thoughts:**

**Link to Work:**
---

## 1. Create New Codelog
### Day 1: May 9, 2018 - Wednesday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![tables](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_rwdf5-23.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/rwdf5-23.png)

**Progress:** Completed *Lesson 5: Optimizations* from the Udacity course: [Responsive Web Design Fundamentals](https://www.udacity.com/course/responsive-web-design-fundamentals--ud893).

This lesson dealt with how to adapt:

- Responsive tables for mobile (hidden columns, contained scrolling, block elements)
- Font sizing across different viewports
- Images resolution based on device pixel density
- Minor breakpoints

Read more: [Notes - Responsive Web Design Lesson 5: Optimizations](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-web-design-fundamentals.html#lesson-5-optimizations)

**Links:**
- My Course Notes - [Responsive Web Design Fundamentals](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-web-design-fundamentals.html)
- Udacity's [Responsive Web Design Fundamentals by Google](https://www.udacity.com/course/responsive-web-design-fundamentals--ud893) (free 2 week course)

---

-->
---

## 18. The Picture Element
### Day 18: May 28, 2018 - Monday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![9-21](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri9-21.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri9-21.jpg)
[![9-18](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri9-18.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri9-18.jpg)

**Progress:** Continued *Lesson 9: Full Responsiveness* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

This lesson covered the `<picture>` element and how it's used in **art direction**.

- **art direction** is the process of using different images for different viewport sizes

Here's an example of what the code looks like for the kitty above:

```html
<picture>
    <source media="(min-width: 650px)" srcset="kitten-large.png">
    <source media="(min-width: 465px)" srcset="kitten-medium.png">
    <img src="kitten-small.png" alt="Cute kitten">
</picture>
```

The browser chooses the first matching media query.

This markup says:
- Use 'kitten-large.png' when the viewport is 650px or larger
- Otherwise, use 'kitten-medium.jpg' if the viewport is 465px or larger.
- Otherwise fallback to 'kitten-small.png' if none of the conditions are met or if the browser doesn't support the `<picture>` element.

Read more: [Notes - Responsive Images - Lesson 9 - Full Responsiveness - The Picture Element](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#96-the-picture-element)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 17. Using sizes with srcset
### Day 17: May 27, 2018 - Sunday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![9-2](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri9-9.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri9-9.jpg)

**Progress:** Continued *Lesson 9: Full Responsiveness* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

This lesson covered the combination of `srcset` and `sizes` attributes.

- **srcset** - tells the browser which images and their widths it has available to choose from.
- **sizes** - tells the browser what the display size will be on the page given the size of the viewport

Here's an example:

```html
<img src="small.jpg"
  srcset="small.jpg 500w,
          medium.jpg 1000w,
          large.jpg 1500w"
  sizes="(max-width: 250px) 100vw,
         50vw"
  alt="Wallaby">
```

This says we have three images sized at 500px, 1000px, & 1500px, respectively, and that the display size will be 100% the viewport width for viewport widths under 250px and will be 50% the viewport width for viewport widths over 250px.

The following items were covered

- Use of `srcset` with `sizes` attribute
- Necessity to still set image size through proper media queries
- How Chrome determines what the optimal sized image resource is to download

Read more: [Notes - Responsive Images - Lesson 9 - Full Responsiveness - Sizes Attribute](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#93-sizes-attribute)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 16. Pixel Density Descriptors
### Day 16: May 26, 2018 - Saturday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![9-2](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri9-2.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri9-2.jpg)

**Progress:** Started *Lesson 9: Full Responsiveness* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

This lesson discussed the limitations of using media queries to determine which image size to download. Instead the lesson discusses the following:

- Use of `srcset` attribute
- specifying pixel density descriptors for each listed image
- Using DevTools to test and verify

Read more: [Notes - Responsive Images - Lesson 9 - Full Responsiveness](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#9-full-responsiveness)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 15. Project Part 2 Solution
### Day 15: May 25, 2018 - Friday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![project part 2](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri8-32.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri8-32.jpg)

**Progress:** Finished *Lesson 8: Images with Markup* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

This lesson gave the requirements to complete part 2 of this responsive blog project:

- Use unicode symbols in place of symbol graphics
- Replace fixed graphics with CSS stylings
- Add social media icons
- Add a responsive logo

Read more: [Notes - Responsive Images - Lesson 8 - Images with Markup: Project Part 2](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#814-project-part-2)

**Links:**
- Course Project - [Responsive Blog Project Part 2](https://rawgit.com/james-priest/udacity-nanodegree-mws/master/exercises/ri-8-14-project-part-2/build/index.html)
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 14. Icon Fonts & Inlining SVG/data URI Images
### Day 14: May 23, 2018 - Wednesday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![character symbols](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri8-27.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri8-27.jpg)

**Progress:** Continued *Lesson 8: Images with Markup* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

This lesson talked about:

- Icon Fonts
- Inlining SVG & data URI
- When to use raster vs. vector
- When to use inlining vs. external images

Read more: [Notes - Responsive Images - Lesson 8 - Images with Markup: Icon Fonts](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#88-icon-fonts)

**Links:**
- List of various icon fonts - [WeLoveIconFonts.com](http://weloveiconfonts.com/)
- Dynamically adjust CSS stylings on icons - [Icon fonts on CSS-Tricks](https://css-tricks.com/examples/IconFont/)
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 13. Unicode Character Sets
### Day 13: May 22, 2018 - Tuesday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![character symbols](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri8-19.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri8-19.jpg)

**Progress:** Continued *Lesson 8: Images with Markup* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

This lesson talked about:

- Character symbols
- Unicode tables
- Use of symbols & CSS effects as an alternative to images

Read more: [Notes - Responsive Images - Lesson 8 - Images with Markup: Symbol Characters](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#86-symbol-characters)

**Links:**
- Unicode Tables - [Character sets](http://unicode-table.com/en/sets/)
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 12. CSS Background Images
### Day 12: May 22, 2018 - Tuesday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![responsive images example](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri8-9.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri8-9.jpg)

**Progress:** Started *Lesson 8: Images with Markup* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

This lesson talked about the following:

- Latency as a barrier to performance (need to reduce number of resource requests)
- Proper use of CSS text and fonts (use separate text over images)
- Using CSS effects in place of images (when possible, opt for CSS effects; gradients, shadows, etc.)
- Use of CSS background images for responsiveness (various techniques covered)

Read more: [Notes - Responsive Images Course - Lesson 8 Images with Markup](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#lesson-8-images-with-markup)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 11. Grunt Automation for Responsive Images
### Day 11: May 21, 2018 - Monday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![Chrome Logos](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri7-42.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri7-42.jpg)

**Progress:** Continued *Lesson 7: Units, Formats, Environments* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

The course material was great at exposing me to new concepts of how to responsively serve images based on viewport size or device pixel density.

But it only scratched the surface on how to fully implement these responsive image techniques. I devoted some time to additional online resources to accomplish the following:

1. Understand how to fully implement **responsive image technologies**.
2. Implement **resolution switching** with `srcset` and `sizes` attributes of `<img>` tag.
    - **Resolution switching** serves the same image at a different size or resolution based on screen pixel density and/or viewport constraints.
3. Understand **art direction** through use of `<picture>` & `<source>` elements.
    - **Art direction** involves serving a different image based on space allocation.
4. Develop a sensible breakpoint system and use it to come up with ideal compression & dimension settings for image processing.
5. Implement Grunt (a task runner) to automate the process of creating multi-sized images.
6. Configure Grunt to update the HTML based on the set of images generated for each `<img>` element.

Those links are in my notes but I've included them below as well

Read more: [Notes - Responsive Images Course - Resources & Links](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#-resources--links)

**Links:**
- Using Responsive Image Techniques (what they are and how they work)
  - [MDN Responsive Images - MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)
  - [Native Responsive Images - Dev.Opera](https://dev.opera.com/articles/native-responsive-images/)
  - [The anatomy of responsive images - Jake Archibald](https://jakearchibald.com/2015/anatomy-of-responsive-images/)
- Responsive Breakpoints (how to make an informed decision)
  - [The 100% correct way to do CSS breakpoints - freeCodeCamp Medium](https://medium.freecodecamp.org/the-100-correct-way-to-do-css-breakpoints-88d6a5ba1862)<br>
    I used the breakpoints defined in this article to determine target sizes for groups of responsive images rather than using those breakpoints for responsive layout. I base my responsive layout breakpoints on the content and how that content flows.<br>
    The target sizes I settled on were (400px, 600px, 900px, and 1600px)
- Grunt (what it is and how to set it up)
  - [Grunt Homepage](https://gruntjs.com/)
  - [Getting Started](https://gruntjs.com/getting-started)
  - [Configuring Tasks](https://gruntjs.com/configuring-tasks)
  - [Plugins](https://gruntjs.com/plugins)
- Image Optimization with Grunt (How-to articles)
  - [Tools for image optimization - Addy Osmani](https://addyosmani.com/blog/image-optimization-tools/)
  - [Generate Multi-resolution images for srcset with Grunt - Addy Osmani](https://addyosmani.com/blog/generate-multi-resolution-images-for-srcset-with-grunt/)
- Essential Grunt packages (what's required to set up this automation)
  - [grunt-responsive-images](https://www.npmjs.com/package/grunt-responsive-images) - npm
  - [grunt-responsive-images](https://github.com/andismith/grunt-responsive-images) - GitHub
  - [grunt-responsive-images-extender](https://www.npmjs.com/package/grunt-responsive-images-extender) - npm
  - [grunt-responsive-images-extender (test html)](https://github.com/stephanmax/grunt-responsive-images-extender/blob/master/test/fixtures/testing.html) - GitHub
  - [grunt-responsive-images-extender (Gruntfile.js)](https://github.com/stephanmax/grunt-responsive-images-extender/blob/master/Gruntfile.js) - GitHub

- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 10. My Build Environment
### Day 10: May 20, 2018 - Sunday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![Chrome Logos](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri7-40.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri7-40.jpg)

**Progress:** Continued *Lesson 7: Units, Formats, Environments* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

Created a Build Environment for my Responsive Images Blog Project. This includes:

- Enabled Windows Subsystem for Linux (WSL) & installed Ubuntu terminal on Windows 10
- Installed many linux packages on Ubuntu (Node.js, npm, GraphicsMagick, ImageMagick)
- Updated Visual Studio Code to use Ubuntu as terminal
- Installed Grunt (grunt-cli) and a host of grunt packages

I also spent the last 5 days learning how to use Grunt and properly configure a Gruntfile. I learned how to
- concat & minify a js application
- automate image compression
- update html & css as part of a build operation
- build a distribution from source

Read more: [Notes - Responsive Images Course - My Build Environment](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#-my-build-environment)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 9. Project Part 1 Solution
### Day 9: May 17, 2018 - Thursday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![Chrome Logos](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri7-44.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri7-44.jpg)

**Progress:** Continued *Lesson 7: Units, Formats, Environments* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

Lesson 7.16 Project Solution covered

- Ensuring images fit the viewport with `max-width: 100%`
- Setting the article width to a reasonable `50em` (800px) width
- Creating a set of images targeting a range of sizes

Read more: [Notes - Responsive Images Lesson - 7.16 Project Solution](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#716-project-solution)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 8. Responsive Images Blog Project Part 1
### Day 8: May 16, 2018 - Wednesday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![Chrome Logos](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri7-35.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri7-35.jpg)

**Progress:** Continued *Lesson 7: Units, Formats, Environments* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

Lesson 7.16 covered

- Requirements necessary to complete part 1 of the Responsive Images Blog project
- Introduction to task runners and build processes with Grunt
- CLI based image compression tools such as ImageMagick and GraphicsMagick
- GUI based tools such as ImageOptim, Trimage, & ImageAlpha

Read more: [Notes - Responsive Images Lesson - 7.16 Project Part 1](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#716-project-part-1)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 7. Raster/Vector, File Formats & Image Compression
### Day 7: May 15, 2018 - Tuesday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![Chrome Logos](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri7-31.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri7-31.jpg)

**Progress:** Continued *Lesson 7: Units, Formats, Environments* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

Lessons 7.9-7.15 covered

- Difference between Raster(bitmaps) & Vector(paths) images
- Working with file formats such as SVG, PNG, and JPEG
- Importance of image compression & optimization
- Introduction to Google's [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/?url=simpl.info%2Fcssfilters) for page analysis and optimization tips

Read more: [Notes - Responsive Images Lesson - 7.9 Raster and Vector](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#79-raster-and-vector)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Google's [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/?url=simpl.info%2Fcssfilters)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 6. Orientation & Alignment
### Day 6: May 14, 2018 - Monday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![Landscape & Portrait](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri7-18.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri7-18.jpg)

**Progress:** Continued *Lesson 7: Units, Formats, Environments* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

Lessons 7.6-7.8 covered

- More use of `calc()` for alignment of images that includes padding & margin
- Targeting both **portrait** & **landscape** orientation modes
- Use of viewport units and measurements (vh, vw, vmin, & vmax)

Read more: [Notes - Responsive Images Lesson - 7.6 Quiz: calc()](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#76-quiz-calc)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 5. Use of Relative Sizing
### Day 5: May 13, 2018 - Sunday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![Relative sizing 1](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri7-10.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri7-10.jpg)

**Progress:** Continued *Lesson 7: Units, Formats, Environments* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

Lessons 7.2-7.5 dealt with

- Saving images for a wide range of devices starting with lowest quality first
- Page requests and response times related to revenue
- Use of percentages with relative sizing
- Proper use of relative sizing with `max-width: 100%` so an image doesn't expand beyond its natural width
- Use of `calc()` function to properly size images by combining absolute and relative values. For example, combining a percentage width with a fixed margin

Read more: [Notes - Responsive Images Lesson 7.2 - All About Bits & Pixels](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#72-all-about-bits-and-pixels)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 4. DevTools Image Analysis
### Day 4: May 12, 2018 - Saturday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![DevTools screenshot 1](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri7-5.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri7-5.jpg)

**Progress:** Started *Lesson 7: Units, Formats, Environments* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

This lesson shows how to use Chrome DevTools to determine:

- bandwidth used for each resource
- relative download times
- image size (both in-browser and natural)
- inferred relative compression rate

[![DevTools screenshot 2](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri7-2.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri7-2.jpg)

[![DevTools screenshot](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri7-4.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri7-4.jpg)

Read more: [Notes - Responsive Images Lesson 7.1](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html#71-quiz-sizing-intro)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 3. Responsive Images Intro
### Day 3: May 11, 2018 - Friday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![responsive images](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_ri6-4.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/ri6-4.jpg)

**Progress:** Completed *Lesson 6: Up & Running* from the Udacity course: [Responsive Images](https://www.udacity.com/course/responsive-images--ud882).

This lesson introduces the concepts of responsive image design. The main take-aways were:

- Create highest quality images with fewest bytes possible
- Design for mobile; Great products are created, never ported
- Art direction is an art and not a science

Read more: [Notes - Responsive Images Lesson 6](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)

**Links:**
- My Course Notes - [Responsive Images](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-images.html)
- Udacity's [Responsive Images by Google](https://www.udacity.com/course/responsive-images--ud882) (free 2 week course)

---

## 2. Adapt Site for Mobile
### Day 2: May 10, 2018 - Thursday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![mobile1](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/sm_mobile1.jpg)](https://james-priest.github.io/udacity-nanodegree-mws/assets/images/full-size/mobile1.jpg)

**Progress:** Completed the Home Town App for *Lesson 5: Optimizations* from the Udacity course: [Responsive Web Design Fundamentals](https://www.udacity.com/course/responsive-web-design-fundamentals--ud893).

The assignment was to take an existing app designed for desktop and modify it to be completely responsive across multiple devices.

This required:

- Combining various responsive design patterns adapted to the content
- Starting adaptation with a the smallest viewport
- Using media queries & breakpoints at various sizes
- Implementing minor breakpoints
- Increase base font size & line height for readability on small devices
- Font sizing across different viewports
- Responsive tables for mobile (hidden columns, contained scrolling, block elements)
- Images resolution based on device pixel density

Read more: [Notes - Responsive Web Design Lesson 5.11 Wrap Up](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-web-design-fundamentals.html#511-wrap-up)

**Links:**
- My Course Notes - [Responsive Web Design Fundamentals](https://james-priest.github.io/udacity-nanodegree-mws/course-notes/responsive-web-design-fundamentals.html)
- CodePen - [The Brighton Times](https://codepen.io/james-priest/pen/ZovQQp) - Responsive design exercise
- Udacity's [Responsive Web Design Fundamentals by Google](https://www.udacity.com/course/responsive-web-design-fundamentals--ud893) (free 2 week course)

---

## 1. Created Round 3 Code Log
### Day 1: May 9, 2018 - Wednesday

**Project:** Google Udacity Nanodegree (Mobile Web Specialist)

[![new code log](assets/images/sm_code-log-1.jpg)](assets/images/full-size/code-log-1.png)

**Progress:** Created a new GitHub repo for my Round 3 code log.

This now uses a purple theme and has an updated nav which I've migrated over to my previous two logs.

Other updates for today include:

- Upgrade to Windows 10 Insider Build
  - Now has tabbed console
  - Better Linux Subsystem integration
  - Built-in screen capture with Screen Sketch integration
- Updated Jekyll dependencies on other logs
- Practiced remote debugging of web pages on my Android phone

**Links:** My GitHub repo [https://github.com/james-priest/100-days-of-code-log-r3](https://github.com/james-priest/100-days-of-code-log-r3)