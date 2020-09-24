# Prosjekt 2
[![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-Ready--to--Code-blue?logo=gitpod)](https://gitpod.idi.ntnu.no/#https://gitlab.stud.idi.ntnu.no/it2810-h20/team-07/prosjekt-2) 


# Solution on the webpage as a whole
Chose to use 9 installations, where about half of them where programmed in SVG and the other in HTML canvas. There you could find different combinations of animation, sound and text, where the sound is from different audio files and the text is retrieved dynamically from a poetry database. The site as a whole is parameterized, where a user can choose different themes for the page. This is a choice that is saved so that the page will open with this preference. Since the page contains nine different installations, a user can choose three favorite ones that are displayed on top of the page and can be viewed in a slideshow format. This is a choice that was made to make the webpage intuitive and sensible. By doing so a user can easily access their favorites, while still having the possibility to view all the artworks with a scroll of a page.

## Technology that was used in the process

### React

Our webpage is written in TypeScript which bases itself on react which is a JavaScript library that is built for building interfaces. There has been use for both class and functions, where functions have been more widely used throughout the programming phase. To make the programming phase as swift as possible, the structure of the components of the page was divided into useful groups. This made is easier to get the correct information when a file is needed for a specific reason. Props, state and the use of context API was used to keep control over specific states of items and the different props. The use of props in the installation files helps by not having to repeat the same lines of code for every installation. The thought behind the page was to have a single page application, where the user can get all the information by scrolling on the page they are on. This was a good way to explore different methods of showing the artworks. As stated earlier the functions where made using both Canvas and SVG. This was to show the ability to use different solutions for the same type of problem. When the artwork is clicked, a modal opens displaying the full artwork with animation, poem and sound playing simultaneously. This is the solution we chose as we did not see a reason to always lead to a new page, when all the information is already there. All the UI components have been programmed from scratch, including modal, installations, layout and so on.

### AJAX

As stated earlier, we used a pre-made poetry database to get the text for our artworks. This was done using AJAX. AJAX is a build in HTTP request object, this was used to receive data from the poetry serve while the page loading and already loaded. In the code there is a file called Poem that uses fetch, which is a method that logically fetches resources. Audio was implemented using the regular HTML audio tag with autoplay.

### HTML Web Storage

On our webpage a user will see a favorite button when opening the different artworks, by pressing this it will use HTML web storage and save this option for a user on their browser. This is achieved by using local storage and session storage, by doing this, every user can have their own unique webpage that they can customize to a degree.

### Web design

To make the website accessible to as many people as possible on as many devices as possible, the attribute @media was used so that the items on the screen would fit different screen sizes. When opening the project on a computer a user will see that the space is utilized well so that the artwork is not cramped on top of each other. When the screen gets smaller this can be an issue, so by using @media and a max screen size, the layout of the page changes so that it is still user friendly. This indicates a transformative and flexible layout. The images themselves have a max size of 750 by 450, but when this size is not possible it will transform to fit the screen size without distorting the image. This is done by using CSS element viewbox.

-   Viewport???

### Testing

The testing for this project was done using Jest. Jest is a JavaScript testing framework, that works well with projects using React, such as this one. The initial test is a snapshot test that keeps track of large objects. This makes sure that the different objects on the webpage do not suddenly change. It does this by rendering a component and comparing the snapshot of it to a reference snapshot. To make sure that the webpage works on different devices and screen sizes the testing was done both manually, but also with the use of the inspection tool in google chrome. By using the inspection tool, we as the programmers can see how the webpage will work on different screen sizes that we cannot manually test. When doing the testing it was important make sure that all the different features worked regardless of what device they were used on. Here we could also change the direction of the screen, put the screen vertically, and see how the page interacted in that direction. When doing this type of testing there were some bugs that were found on the smaller screens, but this was fixed, because of the testing that was done. The manual testing was done using three of the most popular browsers; Chrome, Firefox and Safari. This ensures that the code works just as well for most of the users out there.

### Node.js and NPM, Git and coding

In the start phase of this project it was decided that we would download Node.js to our own computers instead of using GitPod. By doing this we based our project on Node Package Manager (NPM) to get things running. We used the package *_npx create-react-app prosjekt-2 --template_* typescript to create a project with the initial configurations. To track project development, we used issues and milestones in GitLab. This helped keep the programmers on track so that the project was completed on time.