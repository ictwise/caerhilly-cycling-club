# PCSwimming
PC Swimming E-commerce App - Stream 4 Project

This is a **fictional** ecommerce site, for the nature of this project, for a swim team where swimmers can collaborate and pay team fees, and the community can view upcoming events. Alumni can also post photos of their memories from being on the team. This project is based off a swim team coached by my father in Michigan. 
# Demo
A live demo of this project can be found [here](https://pcswimming-project.herokuapp.com/). This application is hosted on Heroku using a Postgres (MySQL Database)
![Desktop Demo](https://raw.githubusercontent.com/hschafer2017/PCSwimming/master/README_Resources/Swimming.gif "Desktop Demo")
# UX
This site is intended for use by Swimmers and Alumni to allow them further ease of access into what's happening at team events, who is organizing them, a meet schedule, and a place to buy team gear for the season. By paying online, it makes it easier for the coach to keep track of who paid and what they ordered, rather than having to keep track of checks or multiple spreadsheets. 
No template was used to build this site. There were some specific UX and UI designs that were taken into consideration when styling this site. The footer was left off the desktop view to present a cleaner, more minimalistic approach to the design. By adding a footer in the desktop view, I would have risked an awkward contrast in colors to follow the transparent theme of the navbar. However, you can see the footer implemented on pages in the mobile and tablet view, since the background here is off-white. I also did not include it on any pages that are viewed to be 'an extension' of another. This was to create a continuous flow of the website, instead of making it constantly seem like you're going to a new page each time you click. 
There are two types of users- Swimmers and Alumni. The swimmers are able to see the discussion board, the shop section, and the events section, while the Alumni only have permission to see the Alumni posts and the events sections. 
When you click to see detail on a product or a swimmer/alumni post, you'll be able to also see all of the other posts or products in the desktop view. I chose this route to stay consistent with the background color scheme throughout the desktop view, and to allow users to toggle back and forth between multiple posts or multiple products without having to constantly go back to a seperate HTML. 
This did pose a bit of an issue with the positioning, however. Since the navy blue size is position:relative and the off-white side is position:fixed, this initially posed a problem when scrolling, especially in the mobile and tablet views. I managed to get around this, however, by altering the height of the panel-body class and adding some extra space at the bottom. I wanted to keep these in a panel to be consistent with the panels used to show events, posts, and products. I chose this 'panel' look because it created a contrast with the navy blue in the desktop, while also creating a nice contrast with the mobile/tablet background via the box shadow. 
With the discussion board for Swimmers, it allows them to discuss team dinners, volunteer opportunities, and other team events. This strives for team inclusivity as all members of the swim team could register for an account. All posts and comments can be monitored by the Coach (a superuser). 
The swimmer on certain desktop pages was a minimalistic way to fill the off-white space on the right half when there was nothing selected. 
I wanted to implement an ease of access with this site, to make it as simple and obvious as possible for both swimmers and alumni to navigate through the site while maintaining consistency throughout the design. 
# Technologies 
1. Django (2.0)
2. Heroku
3. Postgres Database (mySQL)
4. Stripe Payment 
5. JavaScript/jQuery
6. HTML
7. CSS
8. Bootstrap (3.3.7)
# Development Process 
The backend was done first, with the styling added after. As the styling was progressing, and after it was mostly finished, there were some back-end additions that needed to be made for testing and bug fixes. 
Once the styling was looking the way I wanted, I then realized that I had so much CSS that it was becoming unmanageable, and I knew that there were repeat property values declared for the same element. So, I copied the CSS I had here into a blank workspace, and moved it back to this one bit by bit with a mobile-first approach, significantly reducing my CSS repetition. There is minimal difference in styling. 
Initially, I created a separate repository for the static and styling and then hooked it up to the backend, prior to changing the initial styling layout for the project. That repository can be found [here](https://github.com/hschafer2017/PC-Static/commits/master), note that this is not the styling that the site currently has. I played around with different styling options to create the best look and feel for the site and user. The styling redesign that is the current styling was done in this workspace.
