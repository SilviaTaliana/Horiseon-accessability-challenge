# Horiseon-accessibility-challenge
## Homework assignment week 1

### Introduction

This project is about ensuring this website has good accessibility for people who rely on screen readers to navigate websites. The layout of the website was not changed in any way, but with a few changes, it is now easier for screen readers to read and I also made some changes to ensure the site was in full working order. To do this, I made the following changes. 

### Changes

First I fixed the link that was broken at the top of the page called “search engine optimization”. This link was not working because it was trying to go to an id attribute that was missing. I added the id “search-engine-optimization” to the relevant div in the content below and then the link worked. I then proceeded to add comments throughout the html file so it is easier for the other developers to find and understand what the different sections are. Next I added an alt attribute for each image on the page so screen readers are able to read these and the user can understand what is in the image without seeing it. I also added a figure element surrounding each image so screen readers and search-engines can easily identify images on this web page. 

I changed the first div containing the company logo and the 3 links into a header element so screen readers understand what this section of the page is. Then I changed the div surrounding the three links into a nav element so screen readers understand that these links take you to different sections of the page. As per my research, I found that it is perfectly fine to have a nav element inside of a header element as long as these links only take you to different sections of the current page and not an external site Because I changed the names of these elements, I had to change the names in the linked css file so the layout of the page would not change. This was good because it also allowed me to tidy up the css file. 

Then I added a main and footer element around the main content and footer by replacing the div elements that were there. I could not include the benefits section (located on the right) in the main section however because it changed the layout of the page so I had to come back to this. The footer was easily changed and tidied up in the css file. Changing the divs into header/nav/main/footer also allowed me to remove some of the classes that were applied when these were divs, which is good in three main ways: 
1. it helps screen readers to understand what the different sections are and where to navigate to
1. it helps other coders read the code and know which sections are being referred to
1. it helps tidy up the css file because some of the css elements can be combined under the one heading rather than referring to so many different classes 

In the main content, I decided to change the classes of the images to give them more meaningful names so that when developers looked at the css file, they knew exactly what element they were referring to i.e. instead of class=”float-right” I turned it into class=”seo-img”. I also changed the div class="hero" to div class="background-img" so that other developers know what this specific div refers to. 

Then I worked on the flow for the css document so that it was easier to read. To do this, I changed around the order of the elements so that tags referencing the same element were all grouped together e.g. instead of having multiple tags to reference all of the h2 headings, I regrouped them all in to one h2 tag. I had to change the h2 tag in the footer to a h4 tag so that the footer would not also change. I chose the h4 tag because it is not as important as the other headings and there were already h3 tags in the benefits section of the page. I also grouped together the different style elements that were referring to the same image to tidy this up. As with the h2 tag in css, I grouped together all the h3 tags as well. 

Lastly, I changed the title from “website” to “Horiseon main web page” to give it a more meaningful title.

### Challenges I faced

As I mentioned previously, I struggled to put the main element outside both the main information and the benefits sections. I finally figured out that I had to put another section element with a class=”main-info” that I could tag in the css file so that the layout of the page did not change. This also helps because the benefits section now has a meaningful place on the page according to a screen reader. The reason I did not want to leave the benefits section outside of the main element is because it was not a section that made sense on its own so it needed to be a part of the main information for context. 

### Conclusion 

My main motivation for this assignment was to make this website accessible to all users, particularly those who require screen readers for accessiblity. I also wanted to neaten up the code so other web developers understood what each section reffered to on the web page. I believe I achieved this goal without too many problems and still maintaining the original layout of the page. One thing I hope to learn in the near future is how to make sure all the different sections of the page stay in the correct place when the browser size is changed by the user. This is because I noticed that the text overflowed when I changed my browser size. 
