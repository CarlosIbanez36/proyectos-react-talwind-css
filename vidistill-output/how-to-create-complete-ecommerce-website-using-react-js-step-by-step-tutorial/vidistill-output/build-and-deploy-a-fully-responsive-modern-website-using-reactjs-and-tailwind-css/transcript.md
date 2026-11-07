# Transcript

### Segment 1 — 00:00:00 - 00:10:00

**[00:00:00]** **SPEAKER_01 (PedroTech):** Most successful websites you know, have one thing in common.
**[00:00:04]** **SPEAKER_01 (PedroTech):** They have a beautiful landing page. In this video, I will be teaching you how to build the most beautiful React JS website with a modern UI UX design.
**[00:00:15]** **SPEAKER_01 (PedroTech):** We will use React JS and Tailwind CSS to build a landing page that includes a modern looking hero section, an insightful feature section, an eye catching pricing page, and a part to show the testimonials of your website.
**[00:00:30]** **SPEAKER_01 (PedroTech):** Not only will you learn how to build this incredible design, but you will be able to replicate it for your own use case.
**[00:00:38]** **SPEAKER_01 (PedroTech):** However, if you're interested in learning React JS even more in depth, check out my React JS Ultra course for beginners.
**[00:00:46]** **SPEAKER_01 (PedroTech):** The link for it will be in the description. And before we start the video, if you could leave a like and subscribe, I would massively appreciate it. So let's get into it.
**[00:00:54]** **SPEAKER_01 (PedroTech):** Okay everyone, so let's get started. I open up here a folder inside of my code editor of choice, which is VS code, and I want you guys to do the same.
**[00:01:05]** **SPEAKER_01 (PedroTech):** Now we're going to be using V to create our React project. So in order to create a V application, I'll open up the terminal, and I'm going to run npx create-vite, and I'm going to do at latest so that we get the latest version of V.
**[00:01:21]** **SPEAKER_01 (PedroTech):** Now, when we install this, it's going to ask for a project name. Since I want to create this app inside of the folder that I'm already inside of, I'm going to put a dot, but you can make another folder by putting the name of it over here as well.
**[00:01:29]** **SPEAKER_01 (PedroTech):** Then it's going to ask us for our framework. We are using React for this video, so I'm going to choose React. Then it's going to choose for a variant.
**[00:01:38]** **SPEAKER_01 (PedroTech):** They have a lot of different, uh, example projects that you can choose from, and I personally will choose for this video to create a project using JavaScript plus React Compiler.
**[00:01:52]** **SPEAKER_01 (PedroTech):** Now, if you're not familiar, React Compiler won't make any difference in the coding for this video. You can choose just normal JavaScript as well.
**[00:01:59]** **SPEAKER_01 (PedroTech):** I want to use JavaScript because I want to make it inclusive for everyone, but if you want to use TypeScript, you can use it as well.
**[00:02:04]** **SPEAKER_01 (PedroTech):** Now I'm going to put no for this option and I'm going to put yes for, uh, npm and start, and it will start installing, uh, all of the dependencies that we should have in this application.
**[00:02:14]** **SPEAKER_01 (PedroTech):** As you can see, we should have the project set up over here.
**[00:02:18]** **SPEAKER_01 (PedroTech):** So, right off the bat, we have here our project running on localhost 5173. So what I want to do is go to this URL inside of my web browser so I can see the application.
**[00:02:31]** **SPEAKER_01 (PedroTech):** Now, the first thing I want to do is I want to set up Tailwind CSS in our project.
**[00:02:37]** **SPEAKER_01 (PedroTech):** To do that, I want to run npm install and I want to install two packages. The first one is the Tailwind CSS, the second one is at Tailwind CSS but the V package for it.
**[00:02:50]** **SPEAKER_01 (PedroTech):** Now we're going to install both of them.
**[00:02:52]** **SPEAKER_01 (PedroTech):** They don't come with Vite when you set it up.
**[00:02:55]** **SPEAKER_01 (PedroTech):** As that is installing, what I want to do is I want to go to our Vite config. In our Vite config, we have to set up the Tailwind CSS plugin.
**[00:03:04]** **SPEAKER_01 (PedroTech):** So at the top over here, I'm going to import Tailwind CSS from at tailwind/vite, and in the list of plugins, I'm going to add Tailwind CSS over here. Perfect.
**[00:03:18]** **SPEAKER_01 (PedroTech):** Now, to actually get Tailwind to work in our project, we have to open up our source folder, and inside of here, we're going to start by arranging some stuff.
**[00:03:26]** **SPEAKER_01 (PedroTech):** So in our app.css, I want to delete this. We're just going to have one CSS file, which is going to be this index.css over here.
**[00:03:41]** **SPEAKER_01 (PedroTech):** Now, in here for now we're just going to delete everything that is here, but what I do want to do is I want to at the top import Tailwind CSS, just like this.
**[00:03:49]** **SPEAKER_01 (PedroTech):** And what this will do is it will now apply the different Tailwind classes that we want to use into our project.
**[00:04:03]** **SPEAKER_01 (PedroTech):** So now, let's get started. The first thing I want to do is I want to set up our app.jsx, which is the entry point component in our application.
**[00:04:14]** **SPEAKER_01 (PedroTech):** And I want to make it such that this component will serve all of the other components we're going to have in this project.
**[00:04:22]** **SPEAKER_01 (PedroTech):** To do this, I'm going to delete a bunch of the stuff that initially came with this page, and it should become just an empty website.
**[00:04:31]** **SPEAKER_01 (PedroTech):** Now, right off the bat, in our main div that is being served over here, I want to put the following class name.
**[00:04:34]** **SPEAKER_01 (PedroTech):** The background color I'll be using is called Slate.
**[00:04:38]** **SPEAKER_01 (PedroTech):** That's one of the Tailwind CSS colors, and I want to use the darkest version of it.
**[00:04:44]** **SPEAKER_01 (PedroTech):** Now, the second thing I want to do is, I want to make all of the text inside of this page to be white.
**[00:04:48]** **SPEAKER_01 (PedroTech):** Also, I want to set the overflow of this page to be hidden.
**[00:04:54]** **SPEAKER_01 (PedroTech):** Now, the first thing I want to do inside of here is, I want to set up the structure for this page.
**[00:05:13]** **SPEAKER_01 (PedroTech):** So, I want to create a navbar component that is going to contain the UI for the navbar.
**[00:05:28]** **SPEAKER_01 (PedroTech):** The second thing is we want to have a hero section, so I'm going to add a hero component that we're going to create.
**[00:05:32]** **SPEAKER_01 (PedroTech):** We're also going to have a features component which should show all the features of the website.
**[00:05:41]** **SPEAKER_01 (PedroTech):** Then a pricing section and we're going to have a list a place for us to display testimonials of our service, and in the end, we're going to show a footer.
**[00:05:52]** **SPEAKER_01 (PedroTech):** Now, the reason why we are laying them out into individual components is because it'll make it easier for us to be able to identify what UI is part of which section.
**[00:06:12]** **SPEAKER_01 (PedroTech):** So what I want to have here is I want to have the different parts of the website serving as components.
**[00:06:16]** **SPEAKER_01 (PedroTech):** So, we'll start with the navbar, we're going to create a JSX file for that.
**[00:06:21]** **SPEAKER_01 (PedroTech):** So for example, the first part of the page is going to be a navbar. So I want to create a navbar component that is going to contain the UI for the navbar.
**[00:06:29]** **SPEAKER_01 (PedroTech):** For now, I'm just going to return a div that doesn't have anything inside of it.
**[00:06:35]** **SPEAKER_01 (PedroTech):** And the reason for that is because what I want to do is, I want to create all of the different sections and the files for them first to then start writing code inside of it.
**[00:06:43]** **SPEAKER_01 (PedroTech):** We're also going to have a features component which should show all the features of the website.
**[00:06:55]** **SPEAKER_01 (PedroTech):** Then we have the features, so I'm just going to copy and paste this, create the features.jsx.
**[00:07:05]** **SPEAKER_01 (PedroTech):** And we're going to have a list of our, a place for us to display testimonials of our service.
**[00:07:11]** **SPEAKER_01 (PedroTech):** So I'll create three files.
**[00:07:12]** **SPEAKER_01 (PedroTech):** The first one, I'm going to say pricing.
**[00:07:15]** **SPEAKER_01 (PedroTech):** The second one I'm going to say testimonials and the last one I'm going to say footer.
**[00:07:22]** **SPEAKER_01 (PedroTech):** Now, in each of them, I want to make the change that we did on the other ones.
**[00:07:26]** **SPEAKER_01 (PedroTech):** So, on the pricing, I'm going to change this name to be pricing.
**[00:07:29]** **SPEAKER_01 (PedroTech):** On this one, I want to change it to say footer.
**[00:07:36]** **SPEAKER_01 (PedroTech):** Right now, we're just setting up the structure for our project.
**[00:07:40]** **SPEAKER_01 (PedroTech):** Now, what I need to do is, I need to import those components at the top here.
**[00:07:46]** **SPEAKER_01 (PedroTech):** So I'm going to import the navbar component from and then I'm going to put a dot slash and access that navbar component in our components folder.
**[00:07:56]** **SPEAKER_01 (PedroTech):** Then I can do the same thing for all of the other sections, and just change the name from navbar to hero, this will also be hero, and so on.
**[00:08:08]** **SPEAKER_01 (PedroTech):** Now, we're going to organize those sections inside of a components folder we're going to create in our source folder.
**[00:08:12]** **SPEAKER_01 (PedroTech):** So, as you can see, now the page is in white anymore and that's because this we were calling a component that didn't exist previously, but now it does because we are importing it at the top, so there's no error.
**[00:08:21]** **SPEAKER_01 (PedroTech):** And we can start building the project by starting off with the very top, the navbar.
**[00:08:27]** **SPEAKER_01 (PedroTech):** And the navbar usually does take a while to make, because not only we want to make a beautiful navbar that extends it well on web, but also a navbar that is fully responsive on mobile.
**[00:08:39]** **SPEAKER_01 (PedroTech):** So, we're going to start with the web version.
**[00:08:41]** **SPEAKER_01 (PedroTech):** And to do that, I'm going to replace this div component or this div element with a nav element.
**[00:08:47]** **SPEAKER_01 (PedroTech):** In this nav, we're going to define the classes for the navbar.
**[00:08:52]** **SPEAKER_01 (PedroTech):** We'll start by saying that the navbar is going to be fixed at the top.
**[00:08:55]** **SPEAKER_01 (PedroTech):** We're going to put it right at the top so top zero, and the width of it is going to be full so that it extends the entire width of the screen.
**[00:09:03]** **SPEAKER_01 (PedroTech):** Then, I want to make sure that the navbar is always at the top, so I'm going to put a z index to be 50.
**[00:09:09]** **SPEAKER_01 (PedroTech):** I'm setting a transition all, and that transition is going to have the duration of 300.
**[00:09:12]** **SPEAKER_01 (PedroTech):** Now, if you're not familiar with Tailwind CSS, specifically or this classes over here, you'll understand as we move on.
**[00:09:23]** **SPEAKER_01 (PedroTech):** Right now, the navbar will be very simple, but we do want it to have a some sort of animation as we scroll down through the page.
**[00:09:32]** **SPEAKER_01 (PedroTech):** Now, what I want to do is, I want to start by making this have a BG, which is exactly like the color of the background, so BG slate 950.
**[00:09:43]** **SPEAKER_01 (PedroTech):** It's the same color, but I'm going to give it a less opacity.
**[00:09:52]** **SPEAKER_01 (PedroTech):** And then I'm going to add this class name called Backdrop Blur, which allows us to put a little blur into the.

---

### Segment 1 — 00:10:00 - 00:20:00

**[00:10:00]** **SPEAKER_01 (PedroTech):** element and I'm going to give a blur with a small size.
**[00:10:03]** **SPEAKER_01 (PedroTech):** Now, none of that is visible yet, but as we add stuff into this navbar, you'll be able to see it.
**[00:10:09]** **SPEAKER_01 (PedroTech):** Now, the next thing I want to do is I want to add a div that is going to encompass the entirety of the elements inside of this navbar.
**[00:10:19]** **SPEAKER_01 (PedroTech):** We'll start by setting a maximum width that this div can have.
**[00:10:23]** **SPEAKER_01 (PedroTech):** And I'm going to give it a maximum width of 7XL, but you can make it whatever you want.
**[00:10:28]** **SPEAKER_01 (PedroTech):** Now, I'm also setting a margin in the X direction to be auto and a padding of in the X direction to be 4.
**[00:10:36]** **SPEAKER_01 (PedroTech):** And that padding should only be applied to the mobile screen.
**[00:10:40]** **SPEAKER_01 (PedroTech):** We're going to be building the responsiveness of this page as we build the app.
**[00:10:45]** **SPEAKER_01 (PedroTech):** So the way it works in Tailwind CSS is you can put styles that only apply to a certain screen size and above, similar to CSS.
**[00:10:54]** **SPEAKER_01 (PedroTech):** So we are putting here a padding X to be 4 in the smallest screen possible.
**[00:10:59]** **SPEAKER_01 (PedroTech):** But on a large screen and above, I can put this padding X to be 8.
**[00:11:04]** **SPEAKER_01 (PedroTech):** And in between these two values, I can check to see what I want to put for the padding in a small screen and above, which I want to make it be 6.
**[00:11:15]** **SPEAKER_01 (PedroTech):** So if the navigation the screen is very small, it will be a padding X of 4.
**[00:11:21]** **SPEAKER_01 (PedroTech):** If it's small to medium, it will be of 6, and if it's large and above, it will be of 8.
**[00:11:26]** **SPEAKER_01 (PedroTech):** Now, none of that right now is very visible because again the background of this navbar is the same color, but if I were to make, for example, this be red.
**[00:11:34]** **SPEAKER_01 (PedroTech):** Now, none of this is really visible in the moment because we haven't really set a height to this navbar, but that's what we want to do right now.
**[00:11:43]** **SPEAKER_01 (PedroTech):** So inside of this div, I want to add another div and this one will have a display of flex.
**[00:11:49]** **SPEAKER_01 (PedroTech):** I'm going to justify the items in between to justify between, and I'm going to center the items.
**[00:11:56]** **SPEAKER_01 (PedroTech):** Now, here it comes. I'm going to put a height for this navbar of 14.
**[00:12:01]** **SPEAKER_01 (PedroTech):** And that's only for a small screen.
**[00:12:03]** **SPEAKER_01 (PedroTech):** Between a small and a large screen, I want to make it be 16.
**[00:12:08]** **SPEAKER_01 (PedroTech):** And in a medium and above, I want to make it be 20.
**[00:12:13]** **SPEAKER_01 (PedroTech):** Now, you still don't see, now you might not see the navbar still because again, we're using the same color.
**[00:12:21]** **SPEAKER_01 (PedroTech):** But if I were to change this to red, for example, you can kind of see how it applies here.
**[00:12:25]** **SPEAKER_01 (PedroTech):** Now, why are we using the same color for the navbar?
**[00:12:27]** **SPEAKER_01 (PedroTech):** It isn't actually the same color.
**[00:12:30]** **SPEAKER_01 (PedroTech):** The thing is when you scroll down, we're going to put a border at the bottom of this section over here.
**[00:12:34]** **SPEAKER_01 (PedroTech):** We're going to do something like this, border bottom.
**[00:12:38]** **SPEAKER_01 (PedroTech):** So that it is the same color but you can clearly see where the navbar begins and where it ends.
**[00:12:43]** **SPEAKER_01 (PedroTech):** But we only want to show that border bottom when the user is scrolling, which is a functionality we don't have yet, so for now we'll have to be happy with just this.
**[00:12:52]** **SPEAKER_01 (PedroTech):** Now, below this, what I want to do is, I want to have another div and this one is going to be for the logo of this website.
**[00:13:01]** **SPEAKER_01 (PedroTech):** So inside of it, I'm going to put an image and in this image, we're going to show the logo for this website.
**[00:13:07]** **SPEAKER_01 (PedroTech):** Now, I already have a logo that I want to use for my website.
**[00:13:10]** **SPEAKER_01 (PedroTech):** If you want to copy the logo, just go ahead and get that image, it'll be in the code in the description.
**[00:13:16]** **SPEAKER_01 (PedroTech):** But I put that logo as a logo.png on the public folder.
**[00:13:20]** **SPEAKER_01 (PedroTech):** Now, what that means is that I am able to come here, say source, and access the logo.png directly.
**[00:13:29]** **SPEAKER_01 (PedroTech):** Now, obviously it's a huge image, so we do want to put some class things to it to make it smaller.
**[00:13:36]** **SPEAKER_01 (PedroTech):** Also, for accessibility reasons, we're going to put an alt.
**[00:13:40]** **SPEAKER_01 (PedroTech):** And in here, you should put the name of your website.
**[00:13:43]** **SPEAKER_01 (PedroTech):** In this example, we're making a website called CodeFlow, which is like an AI coding website, just as an example, but you can name it whatever you want.
**[00:13:51]** **SPEAKER_01 (PedroTech):** And for the class name, I want to set this logo to be a square shaped element with a width of 6 and a height of 6, so it's pretty small.
**[00:14:02]** **SPEAKER_01 (PedroTech):** I also only want to have that be the case if this is mobile.
**[00:14:08]** **SPEAKER_01 (PedroTech):** If this is web and above, we're going to put here the width to be 8 and the height to be 8 as well, so it's a little bit bigger.
**[00:14:18]** **SPEAKER_01 (PedroTech):** Now, what I want to do is I want to put the name of the website next to this logo.
**[00:14:23]** **SPEAKER_01 (PedroTech):** So right below this div, I want to add a span.
**[00:14:26]** **SPEAKER_01 (PedroTech):** And in this span, I want to add two spans.
**[00:14:29]** **SPEAKER_01 (PedroTech):** Now, why are we using span here?
**[00:14:31]** **SPEAKER_01 (PedroTech):** Because I want to apply a different color to each of the words in the logo.
**[00:14:36]** **SPEAKER_01 (PedroTech):** And a span is very good for this because a span doesn't come with any extra styling or padding in it.
**[00:14:42]** **SPEAKER_01 (PedroTech):** So the name of the website is going to be CodeFlow and you see that for now it shows over here but we're going to add some style to make it that it will appear right here.
**[00:14:50]** **SPEAKER_01 (PedroTech):** But you see that they're right next to each other because a span doesn't come with padding.
**[00:14:54]** **SPEAKER_01 (PedroTech):** So it's very easy for me to make the colors be different.
**[00:14:57]** **SPEAKER_01 (PedroTech):** For example, this one will be white and then this one is actually going to be blue.
**[00:15:05]** **SPEAKER_01 (PedroTech):** Uh, just like this, and I think it gives a good aesthetic to it.
**[00:15:08]** **SPEAKER_01 (PedroTech):** Now on this overall span over here, I want to make the text be a little bit larger, so I'm making text-lg.
**[00:15:15]** **SPEAKER_01 (PedroTech):** But on the on the web and above, we'll actually make it be XL.
**[00:15:21]** **SPEAKER_01 (PedroTech):** Then on a medium screen, we'll make it be 2XL and I'm going to make the font be medium.
**[00:15:29]** **SPEAKER_01 (PedroTech):** Now, this is the boldness, you can make it be actual bold if you were to do this.
**[00:15:33]** **SPEAKER_01 (PedroTech):** But medium is a good weight to this, it doesn't make it look too bulky and it still looks good.
**[00:15:39]** **SPEAKER_01 (PedroTech):** Now, above this two divs, two sections that we have over here, I actually want to put another div that will wrap both of them.
**[00:15:47]** **SPEAKER_01 (PedroTech):** So that we remove this space that exists in between them.
**[00:15:52]** **SPEAKER_01 (PedroTech):** That space existed because we had the justifying between which we only added because we want to have the logo and the name of the website here and the links on the right.
**[00:16:03]** **SPEAKER_01 (PedroTech):** Justifying between will put a space in between two different sections.
**[00:16:05]** **SPEAKER_01 (PedroTech):** So the logo section should be made through this div over here.
**[00:16:08]** **SPEAKER_01 (PedroTech):** And what we want to do with it is we want to set a display of flex.
**[00:16:13]** **SPEAKER_01 (PedroTech):** I want to center the items.
**[00:16:16]** **SPEAKER_01 (PedroTech):** And I also want to put a space in the X direction of one, so there's a small gap in between them.
**[00:16:23]** **SPEAKER_01 (PedroTech):** Then I want to add a group and add a cursor pointer, so when you hover it, it becomes a cursor.
**[00:16:30]** **SPEAKER_01 (PedroTech):** Now, I want to create the different links that we're going to have in this website.
**[00:16:34]** **SPEAKER_01 (PedroTech):** So I'm going to come outside of this div, right over here.
**[00:16:40]** **SPEAKER_01 (PedroTech):** And I want to add a comment here saying Nav Links.
**[00:16:45]** **SPEAKER_01 (PedroTech):** Then inside of this, I want to put a div that will have a class name which is hidden.
**[00:16:52]** **SPEAKER_01 (PedroTech):** Now, we don't want to have it hidden right now.
**[00:16:54]** **SPEAKER_01 (PedroTech):** And the reason for that is because when you get the class name hidden, it will actually hide whatever is inside of this.
**[00:17:02]** **SPEAKER_01 (PedroTech):** So if I put a text here, you clearly don't see it.
**[00:17:06]** **SPEAKER_01 (PedroTech):** If I remove this, you'll be able to see it.
**[00:17:15]** **SPEAKER_01 (PedroTech):** Now, we will eventually have it hidden, and the reason for it is because we want to hide the different menus, uh, in the navbar for depending on whether or not the user has a small screen or a big one.
**[00:17:23]** **SPEAKER_01 (PedroTech):** Because we're going to have some logic to the side, which kind of navbar we want to show.
**[00:17:28]** **SPEAKER_01 (PedroTech):** So for now, we want to remove this hidden and just set the normal styles that we have.
**[00:17:33]** **SPEAKER_01 (PedroTech):** Now, what I want to do is I want to set a display of flex.
**[00:17:36]** **SPEAKER_01 (PedroTech):** I want to center the items.
**[00:17:39]** **SPEAKER_01 (PedroTech):** Then I want to put a gap in between them of six.
**[00:17:41]** **SPEAKER_01 (PedroTech):** Now, we only have this text over here, but if we were to add all the links, each link will have a gap of six in between them.
**[00:17:47]** **SPEAKER_01 (PedroTech):** Now, if this is a large screen and above, I want to make the gap even more, so I'll put it as eight.
**[00:17:52]** **SPEAKER_01 (PedroTech):** Now, inside of here, we're going to put all of our links.
**[00:17:56]** **SPEAKER_01 (PedroTech):** We're going to start with the first one, it's going to be the features section.
**[00:18:04]** **SPEAKER_01 (PedroTech):** So I'll say features, and to make a link, we're just going to put here an href.
**[00:18:09]** **SPEAKER_01 (PedroTech):** And where are we linking to?
**[00:18:11]** **SPEAKER_01 (PedroTech):** This is a landing page.
**[00:18:14]** **SPEAKER_01 (PedroTech):** So when you click on a link, we want to be brought to a part of that landing page.
**[00:18:18]** **SPEAKER_01 (PedroTech):** So we want to scroll down to that section in this page, rather than having different URLs and different routes.
**[00:18:24]** **SPEAKER_01 (PedroTech):** So we're going to create different sections, and for each section we're going to put an ID to the section.
**[00:18:29]** **SPEAKER_01 (PedroTech):** That ID can be referenced here in the H ref through this hashtag symbol, so that when you click on the link, it will actually scroll down to that section.
**[00:18:41]** **SPEAKER_01 (PedroTech):** Now, another thing I want to do is I want to do some make some styling on this navigation link.
**[00:18:48]** **SPEAKER_01 (PedroTech):** First, I want to make the color be grey 300.
**[00:18:53]** **SPEAKER_01 (PedroTech):** Which will be just slightly more grey.
**[00:18:58]** **SPEAKER_01 (PedroTech):** And when I hover it, then it becomes white.
**[00:19:04]** **SPEAKER_01 (PedroTech):** So you see it's a bit grey, but when I hover it, it becomes white.
**[00:19:10]** **SPEAKER_01 (PedroTech):** Now, I also want to make the text be small.
**[00:19:15]** **SPEAKER_01 (PedroTech):** But if you are in a large screen and above, it's going to be base.
**[00:19:22]** **SPEAKER_01 (PedroTech):** Now, a lot whenever I put this kind of stuff, it doesn't actually apply.
**[00:19:28]** **SPEAKER_01 (PedroTech):** So we're seeing here the UI for a smaller screen, but if I open this up, you'll be able to see what it looks like in a larger screen.
**[00:19:35]** **SPEAKER_01 (PedroTech):** Even the logo on the top left is changing as well.
**[00:19:42]** **SPEAKER_00 (Pedro):** Now, what I want to do is copy this and paste it two more times.
**[00:19:48]** **SPEAKER_01 (PedroTech):** Because we want to create a link for the pricing section.
**[00:19:54]** **SPEAKER_01 (PedroTech):** So I'll say pricing, and I'll change this to say pricing.
**[00:19:58]** **SPEAKER_01 (PedroTech):** And I also want to make the test to testimonials.
**[00:20:00]** **SPEAKER_01 (PedroTech):** And I accidentally made that capitalized.

---

### Segment 1 — 20:00:00 - 20:00:00

**[00:20:00]** **SPEAKER_01 (PedroTech):** going to show up for us to open the mobile navbar when the screen is small enough. So how do we do that? Well, I'm going to add a button over here and instead of this button, we're going to use an icon that is a hamburger icon.
**[00:20:00]** **SPEAKER_01 (PedroTech):** To do that we're going to install an icon library. And there's a bunch of them out there, but I personally like to use Lucide React. It's going to give us access to a bunch of different icons that we can use. Specifically, we can use the menu icon from Lucide React.
**[00:20:00]** **SPEAKER_01 (PedroTech):** Now, right now, it's just going to show us no matter what, but you guys will see how we can change that to only show when the screen is really small.
**[00:20:00]** **SPEAKER_01 (PedroTech):** Now, the next thing I want to do is I want to set a class name over here, set the width to be five, the height to be five, in general, but also when you're a small screen, it'll become a width of six and a height of six.
**[00:20:00]** **SPEAKER_01 (PedroTech):** Perfect. Now on this button, I want to make it such that it is hidden unless we are in a small screen. The way we do that is from a medium screen and above, we're going to set the display to hidden.
**[00:20:01]** **SPEAKER_01 (PedroTech):** Now you see that this doesn't impact us at all. But if I were to open this up more, you'll see that it will disappear, because right now we are currently in a small screen.
**[00:20:01]** **SPEAKER_01 (PedroTech):** And what that also means is that now we can come up here into our nav links and do that thing that I mentioned to you guys, where if we are in a small screen, we want to set the display to hidden, so that we only have this button.
**[00:20:01]** **SPEAKER_01 (PedroTech):** But now, how do I get that back when I am in a bigger screen? What you do is in a bigger screen, you set the display to flex because you can't have a display of hidden and a display of flex. We only want to set the display of flex in a medium screen and bigger because then when we get to a smaller screen when the screen is not medium anymore, it will then become this beautiful hamburger menu.
**[00:20:02]** **SPEAKER_01 (PedroTech):** Now, in this button, I also want to center the items and now on this button, I also want to set a padding of two, I want to set the color of it to be gray 300, so it matches the color of the navbar and I'll do the same thing here, hover text white.
**[00:20:02]** **SPEAKER_01 (PedroTech):** Perfect. Now, I want to be able to click on this button and open a completely separate navbar menu that is only for mobile. How do we do that? Well, the way we do this is by keeping track of the state of whether or not a mobile menu is opened or not.
**[00:20:02]** **SPEAKER_01 (PedroTech):** And to do that, we can use the use state hook from React. So, I'm going to create a state set it equal to use state and import that from React. And a state will allow us to keep track of this boolean which we're going to call mobile menu is open, that's a boolean true or false. And we're going to have a function that we're going to use to change the value of that boolean. We're going to call it set mobile menu is open.
**[00:20:03]** **SPEAKER_01 (PedroTech):** Then initially, this boolean will be false, but when you click on this button, I want to make it such that it is hidden unless we are in a small screen.
**[00:20:03]** **SPEAKER_01 (PedroTech):** The way we do that is from a medium screen and above, we're going to set the display to hidden.
**[00:20:03]** **SPEAKER_01 (PedroTech):** Now what does that mean? It means that if I click on this button and the mobile menu is open, then I want to set it to false.
**[00:20:03]** **SPEAKER_01 (PedroTech):** So this is how it's going to look. We're going to click on this button, and we're going to alter the value of the previous value of this state to be the opposite of what it was.
**[00:20:03]** **SPEAKER_01 (PedroTech):** And now, we should see the word hello, and if I click on it again, that should disappear, because now it becomes false.
**[00:20:04]** **SPEAKER_01 (PedroTech):** Now, we don't want to show the word hello when this is true. We want to do a lot more.
**[00:20:04]** **SPEAKER_01 (PedroTech):** For example, I want to change what the icon is inside of this button depending on whether or not mobile menu is open.
**[00:20:04]** **SPEAKER_01 (PedroTech):** So I'm going to wrap this icon or the label inside of this button with some curly braces.
**[00:20:04]** **SPEAKER_01 (PedroTech):** Because if it is, we don't need to show a hamburger menu, we actually need to show something else.
**[00:20:04]** **SPEAKER_01 (PedroTech):** I want to show an X icon, because it's kind of like you want to close the menu.
**[00:20:04]** **SPEAKER_01 (PedroTech):** So I'm going to use the X icon from Lucide React, and you'll see that when I click on this, this now should become an X.
**[00:20:05]** **SPEAKER_01 (PedroTech):** And as I click, it keeps switching.
**[00:20:05]** **SPEAKER_01 (PedroTech):** Now, we also want to show the actual menu or the links appearing in a vertical manner when you open the mobile menu.
**[00:20:05]** **SPEAKER_01 (PedroTech):** And we're going to create a whole separate menu that is just for when the mobile menu is open.
**[00:20:05]** **SPEAKER_01 (PedroTech):** So what I want to do is, I want to render here a div, and this div will show another div which is going to contain the different links.
**[00:20:05]** **SPEAKER_01 (PedroTech):** So I'm going to copy all of the links we have over here, I'm going to paste them inside of this div.
**[00:20:05]** **SPEAKER_01 (PedroTech):** And you see that when I click on this, it should show the links.
**[00:20:05]** **SPEAKER_01 (PedroTech):** But they are not showing up the way that we want to. We want them to show up in the middle and also for them to be vertically stacked.
**[00:20:05]** **SPEAKER_01 (PedroTech):** So to do that, I'll go to the first div and I'm going to set a class name where if you are in a medium screen and above, I want to maintain that hidden.
**[00:20:06]** **SPEAKER_01 (PedroTech):** Now why do we want that?
**[00:20:06]** **SPEAKER_01 (PedroTech):** Because imagine this scenario, I am on a small screen, I open up the mobile menu, and I decide to open up my web browser and make it bigger.
**[00:20:06]** **SPEAKER_01 (PedroTech):** We would have two menus. See? We'd have the one over here and this one over here.
**[00:20:06]** **SPEAKER_01 (PedroTech):** By making such that no matter what, this menu will never show on a medium screen and above, this will now work.
**[00:20:06]** **SPEAKER_01 (PedroTech):** So I'm going to set this to be a BG slate 900, and I'll make the opacity be 95 instead of 90.
**[00:20:06]** **SPEAKER_01 (PedroTech):** Because imagine this scenario, I am on a small screen, I open up the mobile menu, and I decide to open up my web browser and make it bigger. We don't want that menu to still appear, because if this over here wasn't set, this is what was going to happen.
**[00:20:06]** **SPEAKER_01 (PedroTech):** Then I want to set a border to be top, so there's a clear distinction between the actual top navbar and this new mobile menu.
**[00:20:07]** **SPEAKER_01 (PedroTech):** Then I want to actually animate whenever this navbar appears.
**[00:20:07]** **SPEAKER_01 (PedroTech):** So if you look at this, when I open and close, you see it just appears out of nowhere, but I don't want it to be like that.
**[00:20:07]** **SPEAKER_01 (PedroTech):** So, what I want to do now is, I want to set the structure, are the styling for the mobile menu. So I'm going to set this to be a BG slate 900, and I'll make the opacity be 95 instead of 90.
**[00:20:07]** **SPEAKER_01 (PedroTech):** To do that, we're going to create an animation in our CSS file over here, that is going to correspond to that.
**[00:20:07]** **SPEAKER_01 (PedroTech):** To do this, I am going to come inside of here, and I'm going to create a utility class.
**[00:20:07]** **SPEAKER_01 (PedroTech):** Now, if you're not familiar with Tailwind and obviously the different layers of Tailwind that you can create, and what the utilities are, I recommend you checking out my one hour crash course on Tailwind CSS.
**[00:20:08]** **SPEAKER_01 (PedroTech):** I go over absolutely everything from the very beginning up until the end, because Tailwind is one of the best libraries out there, and it's the best way for you to style your CSS, and I highly recommend you checking that out as well.
**[00:20:08]** **SPEAKER_01 (PedroTech):** Then I want to actually animate whenever this navbar appears. So if you look at this, when I open and close, you see it just appears out of nowhere, but I don't want it to be like that. I want it to animate in and also, slide in from the top of this section.
**[00:20:08]** **SPEAKER_01 (PedroTech):** Now, this one is going to be an animation class.
**[00:20:08]** **SPEAKER_01 (PedroTech):** So I'm going to say animate in, and in the animate in, I want to set an animation fill mode to be both.
**[00:20:08]** **SPEAKER_01 (PedroTech):** Now, that only makes sense if we do have an animation.
**[00:20:08]** **SPEAKER_01 (PedroTech):** So, I want to also create here a class name called slide in from top, which is going to represent the animation that this navbar should have.
**[00:20:08]** **SPEAKER_01 (PedroTech):** Now, what we need to do is, we need to create a, oh, I just realized, a I made a misspelling here.
**[00:20:08]** **SPEAKER_01 (PedroTech):** So, I need to change this to animation.
**[00:20:09]** **SPEAKER_01 (PedroTech):** Now, what we need to do now is, we need to apply a duration to this animation.
**[00:20:09]** **SPEAKER_01 (PedroTech):** So, we want to create a duration class that can be reused whenever we want to have, for example, animations that last a certain length.
**[00:20:09]** **SPEAKER_01 (PedroTech):** Like 300 milliseconds, which is what I usually like my animations to be.
**[00:20:09]** **SPEAKER_01 (PedroTech):** So, whenever we want to set an animation to 300 milliseconds, I'll create this class and make the animation duration be equal to 300 milliseconds.
**[00:20:09]** **SPEAKER_01 (PedroTech):** So, that means that now, if we're to pass the duration to be 300 here, which it means I'm just calling this class that we created, it should have a slight delay, which makes like it's fading in.
**[00:20:10]** **SPEAKER_01 (PedroTech):** But we don't want it to just fade in, we also want it to kind of look like it's sliding in from the top.
**[00:20:10]** **SPEAKER_01 (PedroTech):** So, to do that, I am going to also pass a transform.

---

### Segment 1 — 30:00 - 00:40:00

**[00:30:00]** **SPEAKER_01 (PedroTech):** That is going to translate
**[00:30:03]** **SPEAKER_01 (PedroTech):** in the Y direction from the start, the item to be -1 rem from its original place.
**[00:30:10]** **SPEAKER_00 (Pedro):** And then when the animation is finished, it should be at its original position, which is just a translate Y of zero.
**[00:30:18]** **SPEAKER_00 (Pedro):** So you see now, if we try to animate this, it will look a bit like it's sliding in from the top.
**[00:30:24]** **SPEAKER_01 (PedroTech):** Perfect.
**[00:30:26]** **SPEAKER_01 (PedroTech):** Now, what I want to do is, again, structure this elements so that they appear stacked against each other.
**[00:30:32]** **SPEAKER_00 (Pedro):** So, I want to put some class names to this div.
**[00:30:35]** **SPEAKER_00 (Pedro):** So in this div, what I want to do is, I want to set a class name to be a padding X of 4, a padding Y of 4.
**[00:30:43]** **SPEAKER_00 (Pedro):** Now you might be wondering, why are we not just using a P of 4 in here?
**[00:30:47]** **SPEAKER_00 (Pedro):** And that's because that's only for the mobile screen, but we also want to set here in a small screen to be a padding Y of 6, and nothing for the padding of the X direction.
**[00:30:57]** **SPEAKER_00 (Pedro):** Now, between the items, I want to put a space in the Y direction to be 3.
**[00:31:02]** **SPEAKER_00 (Pedro):** Now, in a small screen and above, I'm going to make that space be 4.
**[00:31:08]** **SPEAKER_00 (Pedro):** Now, to make the items actually, each link actually, appear in a different line, we have to make it such that they are display block.
**[00:31:17]** **SPEAKER_00 (Pedro):** So, for each of these, I'm just going to pass a block value here and each of them will appear now to be stacked on top of each other.
**[00:31:26]** **SPEAKER_00 (Pedro):** Perfect.
**[00:31:27]** **SPEAKER_01 (PedroTech):** And now our navbar is almost complete.
**[00:31:30]** **SPEAKER_01 (PedroTech):** The only thing I want to do left is, I want to come up here to our nav.
**[00:31:33]** **SPEAKER_01 (PedroTech):** The only thing left that I want to do is, whenever I click any of this links, I will navigate to the place, but I also want to close the navbar in a mobile state, so that it doesn't cover half of the screen.
**[00:31:45]** **SPEAKER_00 (Pedro):** So to do that, all I have to do is, I just have to add an onClick similar to what we added for this button, so that we can manually force the navbar to close.
**[00:31:56]** **SPEAKER_00 (Pedro):** But instead of toggling it like we were doing with the button, we are literally just going to set it to false.
**[00:32:01]** **SPEAKER_00 (Pedro):** And we're going to do this for all of the links on the mobile menu.
**[00:32:06]** **SPEAKER_00 (Pedro):** So that, for example, if I were here and I wanted to go to the pricing page, I go to the pricing page, but also the navbar closes.
**[00:32:12]** **SPEAKER_01 (PedroTech):** Perfect.
**[00:32:13]** **SPEAKER_01 (PedroTech):** So now we're pretty much done with the navbar, it looks good on mobile, it looks good on web, and it's time for us to start building the hero section.
**[00:32:21]** **SPEAKER_01 (PedroTech):** So to start off with the hero section, I just want to turn this into a section element.
**[00:32:29]** **SPEAKER_00 (Pedro):** And I want to apply the groundwork for the class names that we're going to be using to structure this page.
**[00:32:34]** **SPEAKER_00 (Pedro):** So, I'm going to set the hero section to have a position of relative.
**[00:32:37]** **SPEAKER_00 (Pedro):** I'm also going to set the height of it to actually be the minimum height of the screen.
**[00:32:42]** **SPEAKER_00 (Pedro):** The reason for that is because I want the hero section to be the first thing the person sees.
**[00:32:46]** **SPEAKER_00 (Pedro):** They are not going to see any of the other sections, they have to scroll to be able to see them.
**[00:32:50]** **SPEAKER_00 (Pedro):** Then, I want to set a display flex and I want to center the items.
**[00:32:55]** **SPEAKER_00 (Pedro):** Now, I also want to justify everything from the hero section right in the center.
**[00:33:02]** **SPEAKER_00 (Pedro):** And I will put a padding on the top of the hero section to be 16, if you're in a small screen, but in a bigger screen, that padding will be even bigger, it will be 20.
**[00:33:12]** **SPEAKER_00 (Pedro):** I'm also going to set a padding in the X direction, in a small screen to be 4, and on every other screen to be 16.
**[00:33:20]** **SPEAKER_00 (Pedro):** With the exception of a large screen which we're going to make that padding be 8.
**[00:33:27]** **SPEAKER_00 (Pedro):** Now, we also just want to set an overflow to be hidden.
**[00:33:32]** **SPEAKER_00 (Pedro):** Now, none of this is going to be clear yet because we don't have anything inside of the hero section.
**[00:33:41]** **SPEAKER_01 (PedroTech):** It's going to be the effect that I had in the demo where as you hover through the elements, it's actually going to be the effect that I had in the demo, which you can see over here from the final product, where as I hover, as I move my cursor through the page, it is going to show this little glow around it.
**[00:34:00]** **SPEAKER_01 (PedroTech):** Now, to do something like this, what we need to do is, we need to keep track of the user's mouse position.
**[00:34:07]** **SPEAKER_00 (Pedro):** And to do that, we're going to create a state called mouse position, create a function called set mouse position.
**[00:34:17]** **SPEAKER_00 (Pedro):** Then, this state, it's going to be an object that is a combination of an X and a Y value.
**[00:34:24]** **SPEAKER_00 (Pedro):** Now, that X and the Y value represents the position of the cursor, and by default, this is going to be 0.
**[00:34:31]** **SPEAKER_00 (Pedro):** Then, we're going to have a use effect that is going to have an event listener that it is going to subscribe to.
**[00:34:37]** **SPEAKER_00 (Pedro):** This event listener is going to be the user moving their mouse.
**[00:34:41]** **SPEAKER_00 (Pedro):** And whenever the user moves the mouse, we're going to run this function called handle mouse move.
**[00:34:49]** **SPEAKER_00 (Pedro):** Now, to do that, we need to again, subscribe to the event listener of the user moving their mouse.
**[00:34:55]** **SPEAKER_00 (Pedro):** And to do that, you access the window, you add an event listener, you choose the event called mouseMove, and you pass the handle mouse move function here.
**[00:35:12]** **SPEAKER_01 (PedroTech):** Now, if you want to, I'll just show you, uh we can console.log the X and Y values.
**[00:35:19]** **SPEAKER_00 (Pedro):** How do you do that is, you get the X value by getting the event, and then you access the clientX, and the Y value through the event clientY.
**[00:35:31]** **SPEAKER_00 (Pedro):** If you're not familiar with use effects, it is important if you are subscribing to an event listener like this, for you to return a function in this use effect, that will remove that event listener, because what happens is, if you don't do that, then the component might unmount without actually removing the event listener, causing memory leaks.
**[00:35:55]** **SPEAKER_00 (Pedro):** So you have to do this whenever you're subscribing to an event.
**[00:36:00]** **SPEAKER_01 (PedroTech):** Now, now that we've done that, I also want to put here an empty dependency array so that we don't run this use effect infinitely.
**[00:36:12]** **SPEAKER_00 (Pedro):** So, if I open up the console log, you see as I move my mouse, it will show the different X and Y values of my mouse based on that.
**[00:36:21]** **SPEAKER_00 (Pedro):** Now, we don't want to just console log those values. We want to show a glow around the mouse.
**[00:36:27]** **SPEAKER_01 (PedroTech):** So to do that, inside of the section, I want to create this div that is going to be a self-closing div and it's going to have a class name of absolute and inset of zero and an opacity of 30.
**[00:36:42]** **SPEAKER_00 (Pedro):** Now, most of the styling for this, we're not going to be using Tailwind, just because it's a lot easier for us to manually do it with just normal CSS, through the style.
**[00:36:50]** **SPEAKER_00 (Pedro):** So, inside of here, I'm going to add a background value, so that we can build that little gro glow coming out of the mouse.
**[00:36:58]** **SPEAKER_00 (Pedro):** So, inside of here, I'm going to add a background value so that we can build that little radio gradient, which it will make a gradient out of a circle.
**[00:37:09]** **SPEAKER_01 (PedroTech):** To make a gradient a radial gradient, we have to first set its size. I'm going to make it 600 pixel, but you can make it bigger or smaller if you want.
**[00:37:13]** **SPEAKER_00 (Pedro):** You choose the say, the shape which I'm going to choose to be a circle, and you need to put the position of it.
**[00:37:24]** **SPEAKER_00 (Pedro):** So, the way you put the position is kind of interesting in CSS.
**[00:37:28]** **SPEAKER_00 (Pedro):** You put at, and then you put the X position as a pixel.
**[00:37:32]** **SPEAKER_00 (Pedro):** So what we can do is we can use that state to keep track of that position.
**[00:37:37]** **SPEAKER_00 (Pedro):** We'll use the setMousePosition function and we're going to set an object inside of here, where the X value is equal to the clientX and the Y value is equal to the clientY.
**[00:37:50]** **SPEAKER_00 (Pedro):** Now we can use that mousePosition.x in here and get the X position as a pixel for the mouse.
**[00:37:59]** **SPEAKER_00 (Pedro):** We'll do the exact same thing in the Y position for the mouse, and we should be able to get that glow.
**[00:38:05]** **SPEAKER_01 (PedroTech):** Now we're not seeing anything because we are not done yet.
**[00:38:07]** **SPEAKER_01 (PedroTech):** Now, I'm going to set the following color, which is an RGBA of a similar color to what we have in the background.
**[00:38:11]** **SPEAKER_00 (Pedro):** It's going to be the following values, 59, 130, 246, and 0.15, because I don't want to make it too visible.
**[00:38:28]** **SPEAKER_00 (Pedro):** Now, after this, I want to set this to be transparent and set 40 percent, so that we get this cool effect at the top left.
**[00:38:34]** **SPEAKER_00 (Pedro):** Now, why is it at the top left? Because, initially, the mouse is set to 0,0.
**[00:38:43]** **SPEAKER_00 (Pedro):** So you see that as I move my mouse, this should move along with me.
**[00:38:50]** **SPEAKER_00 (Pedro):** It's a really cool effect and it's really nice whenever you can add this. This won't go through the entire website because we're only adding this to the hero section, however because I also think it would look kind of weird and goofy if you added to the entire website, but for the hero section it's a really good eye-catcher.
**[00:39:04]** **SPEAKER_01 (PedroTech):** Now, on top of that, I want to add two different glows that are going to be stuck permanently on the page, and they're going to be pulsating as well.
**[00:39:13]** **SPEAKER_00 (Pedro):** Well, because even though we have this little mouse that is moving, uh sometimes if the mouse is down here, I still want to have those two glows at the top, so that it gives a nice aesthetic to this page.
**[00:39:31]** **SPEAKER_01 (PedroTech):** So to do that, I already have the two glows over here, and I'll just go over what they are.
**[00:39:33]** **SPEAKER_01 (PedroTech):** I put them on the top left and on the bottom right so that they have a good distance between them.
**[00:39:45]** **SPEAKER_05:** It's a similar glow to what we have on our mouse, but it is stuck and it's pulsating.
**[00:39:50]** **SPEAKER_05:** I put it on the top left by making the top be 20 and the left four, so it's on the top left, and then the bottom right by using the bottom and the right.

---

### Segment 6 — 00:40:00 - 00:50:00

**[00:40:00]** **SPEAKER_01 (PedroTech):** be blue and cyan so they are different kind of a different color. This one is lighter, and this one is a bit darker.
**[00:40:06]** **SPEAKER_01 (PedroTech):** To make them animate, you can just call the built-in Tailwind CSS animation called animate-pulse.
**[00:40:12]** **SPEAKER_01 (PedroTech):** So, Tailwind has some animations that are built in. Uh, we just had to create one of them for the navbar, but some of them can be reused like this one.
**[00:40:20]** **SPEAKER_01 (PedroTech):** And now we have those two uh glows around our page.
**[00:40:24]** **SPEAKER_01 (PedroTech):** Now, what I want to do is, I want to start building the skeleton for the actual content. So, I'll build this div and put another div inside of it.
**[00:40:36]** **SPEAKER_01 (PedroTech):** Then I'm going to put another div. And if you remember, the Hero section has two parts to it. It is going to have the text that is, at least in mobile is going to be appearing on top of this other section which is the code.
**[00:40:40]** **SPEAKER_01 (PedroTech):** but on web, this will appear on the left and this on the right.
**[00:40:51]** **SPEAKER_01 (PedroTech):** Now the code, we're going to have to do it all manually, so we're going to be using a lot of CSS for this and a lot of React States for this as well.
**[00:40:59]** **SPEAKER_01 (PedroTech):** Now for this part, we can do it uh by just putting the content directly in here. Now we'll start by building the code part of this, this part over here.
**[00:41:09]** **SPEAKER_01 (PedroTech):** And to do it, what I want to do is, I'll come here and I'll create this section. I'm going to call it the IDE Header. It's just the header section for the code editor that we have here.
**[00:41:20]** **SPEAKER_01 (PedroTech):** And I'm going to add another div.
**[00:41:23]** **SPEAKER_01 (PedroTech):** Now on this div, I want to set a class name of display flex, items center, justify between.
**[00:41:32]** **SPEAKER_01 (PedroTech):** And the reason for that is because this is the header. This is this part over here. And I want to have a part on the left which is those this three dots with the title of the page and then this section over here.
**[00:41:44]** **SPEAKER_01 (PedroTech):** Now the code, we're going to say justify between and I want to put a padding X of three. On a small screen and above I'm going to make a padding X of four.
**[00:41:56]** **SPEAKER_01 (PedroTech):** Then I'm going to set the padding Y to be two and the padding Y to be three on a bigger screen. The BG will be white but with only five of opacity, so you can kind of start seeing it right in the center.
**[00:42:08]** **SPEAKER_01 (PedroTech):** And I'm also going to set a backdrop blur to be small, a border at the bottom because it's a header. And that border will be white, but with only 10 of opacity, so it matches a bit more like that.
**[00:42:22]** **SPEAKER_01 (PedroTech):** Then what I want to do is, I want to actually build the class name for the, uh, part around the IDE Header. This part, I'm going to set a BG gradient to bottom right because I want to make this glassy look around the IDE.
**[00:42:40]** **SPEAKER_01 (PedroTech):** And what I do here is I'm going to make the background gradient to be from the color gray 900 divided by 20 so 20 opacity to Gray 800 divided by 20.
**[00:42:54]** **SPEAKER_01 (PedroTech):** And I'm also going to set a backdrop blur small and I'm going to make it rounded large.
**[00:43:01]** **SPEAKER_01 (PedroTech):** Now, I also want to set the overflow to be hidden, and I want to set a manual height and width for this section.
**[00:43:07]** **SPEAKER_01 (PedroTech):** Why am I doing that? Because this is a piece of code and it will look ugly like I had to manually make this UI.
**[00:43:16]** **SPEAKER_01 (PedroTech):** So it will look ugly if we were to allow this to expand and grow as the page grows.
**[00:43:25]** **SPEAKER_01 (PedroTech):** I want it to always be this size. So to do that, I'll set a height with a specific size in mind. I'm going to use pixels. I'm going to make it 280 pixels, and you'll see that this thing should grow now.
**[00:43:38]** **SPEAKER_01 (PedroTech):** And the width should be a fixed size of 350 pixels. Now, I want to do that only if this is a small screen and above, and you'll see why in a second.
**[00:43:51]** **SPEAKER_01 (PedroTech):** Now in a large screen and above, since it's going to be very large, I actually want to change the height just a bit more.
**[00:43:57]** **SPEAKER_01 (PedroTech):** So I'm going to make it be 450 pixels. This won't impact what we are seeing right now because this isn't a large screen, but it will be good.
**[00:44:03]** **SPEAKER_01 (PedroTech):** I'm also going to set a border around it and I'm setting a border color to be white, 5% so there it looks similar to what we have in the header.
**[00:44:12]** **SPEAKER_01 (PedroTech):** Now, how do we apply this to have a bigger size in a mobile? Well, in here, at this div, we're going to set the position to be relative.
**[00:44:23]** **SPEAKER_01 (PedroTech):** I'm also setting the same BG white to be 5, and I'm also setting a backdrop blur, but this time we're setting it to be Excel.
**[00:44:33]** **SPEAKER_01 (PedroTech):** Now, what I want to do is, I want to set this to be very rounded, and I also want to, in a smaller screen, to make this even more rounded because there's still a bit that I'm seeing over here.
**[00:44:48]** **SPEAKER_01 (PedroTech):** Then, I want to set a padding of 3, but on a small screen and above, I'll make that 4. I'll set a shadow around it to be 2xl, and I'm setting the border to be border white 10.
**[00:45:01]** **SPEAKER_01 (PedroTech):** So we're building the outer layer, which you could see over here, right? We have this outer layer, we have the inner layer and the header. That's the three things we've made so far.
**[00:45:12]** **SPEAKER_01 (PedroTech):** But on top of all of that, we have this div which we have to set a position relative, the order to be two, and most importantly, the width to be full.
**[00:45:25]** **SPEAKER_01 (PedroTech):** Now, we get this beautiful uh code editor appearing in our screen. Now, it doesn't fully look like a code editor yet, but it will in a second.
**[00:45:34]** **SPEAKER_01 (PedroTech):** The first thing to make this look like a code editor is add the little close, minimize, and open buttons.
**[00:45:40]** **SPEAKER_01 (PedroTech):** To do that, it's actually easier than you might imagine, because if you think about it, it's just three circles with different colors.
**[00:45:47]** **SPEAKER_01 (PedroTech):** So, that's literally what we have to do. Inside of here, I want to add a div that is going to encompass the three little dots, and each dot will look like this. We're just going to create the dot, make it be a circle so it will have the same width and height.
**[00:45:56]** **SPEAKER_01 (PedroTech):** I'm going to make it 2, and it will be rounded full and it will have a color which will be red 500, at least for the close one.
**[00:46:12]** **SPEAKER_01 (PedroTech):** Now, I also want to change the size if it's a bigger screen, so in a bigger screen, the width will be 3, and in a bigger screen the height will be 3.
**[00:46:21]** **SPEAKER_01 (PedroTech):** Now, I'm also going to copy this and paste it two more times, and the reason for that is because this one is going to be yellow, and this one is going to be green.
**[00:46:33]** **SPEAKER_01 (PedroTech):** Now they're stacked on top of each other. To put them next to each other, we have to have this be a display flex.
**[00:46:40]** **SPEAKER_01 (PedroTech):** And we also want to put a gap in between them, because they're all closed up together since this is the display gap where this is just one row, then I want to set the space X to be 2.
**[00:47:00]** **SPEAKER_01 (PedroTech):** Now I do think this gap is a bit bigger. I think we want to do this only in bigger screens. In smaller screens, let's make this be 1.
**[00:47:11]** **SPEAKER_01 (PedroTech):** Now, I want to put a span with the name of the website. So, CodeFlow AI, that's the title of the website.
**[00:47:18]** **SPEAKER_01 (PedroTech):** I don't want it to appear here. It's appearing here because of the justify-between from this. So, I want to wrap this section and the new span that I created with this div.
**[00:47:28]** **SPEAKER_01 (PedroTech):** Now this div, to be honest, will keep it exactly the same, but I'm just going to remove this space X 1, because I think space X of 2 makes sense between this section and this one.
**[00:47:41]** **SPEAKER_01 (PedroTech):** Now, in the title here, I want to make it definitely a lot smaller, so I'm going to say text XS. On a small screen and above, we'll make it be just small. The color will be gray 300, so it blends in.
**[00:47:53]** **SPEAKER_01 (PedroTech):** Now, what we want to do is just add this last section over here. I'm not going to make it exactly the same. I don't think I'm going to add this AI thing over here, because looking back now, I think it looks a bit goofy.
**[00:48:07]** **SPEAKER_01 (PedroTech):** But the thing is this, I'm going to add this section over here just for UI purposes. To do that, it's pretty simple. Below this div over here, whatever we put is already going to appear on the, uh, like top right.
**[00:48:16]** **SPEAKER_01 (PedroTech):** So, all we have to do is just add this Chevron down icon, which is an icon from Lucide, which is just an arrow and an arrow pointing down.
**[00:48:26]** **SPEAKER_01 (PedroTech):** Now, I'm going to make this have a class name of width 3 and height of 3, so it's a lot smaller. And I also want to make it such that in a small screen and above, we'll make it a little bit bigger so it looks better.
**[00:48:42]** **SPEAKER_01 (PedroTech):** And we'll make the height as well, and I'm also making the color be gray 400 so it's not very white.
**[00:48:46]** **SPEAKER_01 (PedroTech):** Now, we want to make the code inside of it. And more importantly, we want to make it such that you can move through the different tabs so that you can see the code changing.
**[00:48:56]** **SPEAKER_01 (PedroTech):** How do we do that? Well, to do that, we need to create a variable that is going to keep track of the different pieces of code, whatever is written in here for whatever tab we are in.
**[00:49:10]** **SPEAKER_01 (PedroTech):** So we have three tabs and I I just made whatever the names are but you can change it as you want. But we have three tabs in this code editor. We have the app JSX, we have the hero JSX and the navbar JSX.
**[00:49:21]** **SPEAKER_01 (PedroTech):** Now each of them has a code associated with it. And that looks even better if you are looking in web.
**[00:49:25]** **SPEAKER_01 (PedroTech):** Now, how do we make that? Well, we'll create a variable. I'll create here a folder called data and in here I'll create a file and I'll call this codeExample.js.
**[00:49:43]** **SPEAKER_01 (PedroTech):** It's going to be a JavaScript file because we're not going to return a component in here and what I want to do is, I want to export const an object called codeExamples.
**[00:49:57]** **SPEAKER_01 (PedroTech):** Now this object will take in a key and a

---

### Segment 1 — 00:50:00 - 01:00:00

**[00:50:00]** **SPEAKER_01 (PedroTech):** e-value, like every other object, right? But the key, I'm going to actually make it kind of look like JSON. The key is going to be the name that we show up over here. So the name of the file like App.jsx. And the value is going to be actual code that you put here.
**[00:50:16]** **SPEAKER_01 (PedroTech):** Now to write the code, we need to take into account, for example, spaces, like positioning of everything. So to do that, I'm going to use backticks and directly write the code inside of here. I already have the code written for this. It is uh this code over here.
**[00:50:30]** **SPEAKER_01 (PedroTech):** Now don't worry about positioning or anything like that, because we're going to be using a library that is going to format all of that to make it look good for us. Now you can copy the code that I have, it's going to be in the description.
**[00:50:41]** **SPEAKER_01 (PedroTech):** None of this makes any sense, it's just for uh like demonstration purposes, but you should make it applicable to your own website. Now we're going to copy this and paste it two more times.
**[00:50:55]** **SPEAKER_01 (PedroTech):** And we're going to make one for the Hero.jsx and we're also making one for the Navbar.jsx. Now like I said, I already have the code written for them, so I'm just going to copy and paste from the uh code that I already wrote, but you can play around with the values and write whatever code you want.
**[00:51:16]** **SPEAKER_01 (PedroTech):** So I'll be back in a second when I finish pasting it. Perfect. Now we have this value and we can access it inside of here.
**[00:51:23]** **SPEAKER_01 (PedroTech):** But before we even use that, I want to set up the UI for the header, so the different tabs over here, and the code. So to do that, I'm going to create a div over here with another div. The first section is the uh file tabs and I'm going to create a button for each of the tabs.
**[00:51:47]** **SPEAKER_01 (PedroTech):** Now it should appear down here, and this button should have the label of App.jsx. Now we're going to have three of them. So App.jsx, then we're going to have one for the Hero and one for the Navbar.
**[00:52:04]** **SPEAKER_01 (PedroTech):** Now like I said, this definitely shouldn't be appearing here. This should appear inside of this, so we made a mistake, we need to put this right over here so that it's this is the outer div.
**[00:52:15]** **SPEAKER_01 (PedroTech):** And we want to make it such that we style this to look like the actual tabs here. So for each of these buttons, I'm going to add a class name and it's going to be a padding x of 3, a padding y of 2. Then we're setting a backdrop blur to be small, the text will be extra small, and on a bigger screen we're also going to make that be small.
**[00:52:45]** **SPEAKER_01 (PedroTech):** We're also going to rounded it at the top as large, not at the bottom because you look how it's only rounded at the top. And finally to make it look like a tab, we're going to add a border, a rounded, we're also going to add a BG of white 5 and the text will be gray 300.
**[00:53:09]** **SPEAKER_01 (PedroTech):** Now I also want to set a transition to be all, a duration to be 200. Now we don't have this duration to be 200, we'll create it down here from similar to what we did with the duration here. We want to have a simple animation for this as well, but we're going to be using 200 because it will make the animation faster, and we'll change this to 200 milliseconds.
**[00:53:32]** **SPEAKER_01 (PedroTech):** Now I also want to add a class name called whitespace no wrap, and we should be good with this. I'm going to copy this, and I'm going to paste it two more times.
**[00:53:50]** **SPEAKER_01 (PedroTech):** Now, obviously there should be some space in between them. So, in this top div over here, I'm setting a flex and a space x of one.
**[00:54:03]** **SPEAKER_01 (PedroTech):** Perfect.
**[00:54:19]** **SPEAKER_01 (PedroTech):** Then on the top here, we're going to give some space. I'm going to add a padding of 3, and on a bigger screen that will be 4, position will be relative and the height will be full.
**[00:54:27]** **SPEAKER_01 (PedroTech):** Now this doesn't really look like this, right? I know. Just wait a second, because what we need to do is we need to find a way to keep track of which tab we're in, because if you notice the UI clearly changes based on which one we're in.
**[00:54:34]** **SPEAKER_01 (PedroTech):** So in this case, it's for the Hero, so we change this to be Hero, and on this case, we change it to be Navbar.
**[00:54:43]** **SPEAKER_01 (PedroTech):** So to do that, we're going to create a state up here that is going to keep track of the active tab. We're going to also call this set active tab and this state will be a string that will just be the key of whatever values we have here. So you know we have App.jsx as one of them, Hero.jsx is the other, and Navbar.jsx as the other. By default, it should start as App.jsx.
**[00:54:45]** **SPEAKER_01 (PedroTech):** But I want to be able to switch between the different tabs.
**[00:54:48]** **SPEAKER_01 (PedroTech):** So to do that, for each of this buttons, we're going to add an onClick, that when you click on it, we're going to set the active tab to be whatever this is.
**[00:54:57]** **SPEAKER_01 (PedroTech):** So in this case, it will be the App.jsx,
**[00:55:01]** **SPEAKER_01 (PedroTech):** and on the other ones, such as this one over here, it's going to be the Hero, and on this one, it's going to be the Navbar.
**[00:55:11]** **SPEAKER_01 (PedroTech):** Then, what I do is if the class name, if this is the active tab for each of the buttons, I want to change a bit the styling in it. Now, how do I do that? Well, I am going to change the quotation marks on this from just normal quotation marks, to be backticks because this is going to be dynamic, meaning we're going to insert JavaScript inside of here, to change the UI based on some sort of behavior, which in this case is, if this is the active tab.
**[00:55:17]** **SPEAKER_01 (PedroTech):** Now, this should also change the code that is displayed below.
**[00:55:25]** **SPEAKER_01 (PedroTech):** So, I feel like now it's a good time for us to do that.
**[00:55:28]** **SPEAKER_01 (PedroTech):** If we go below this file tabs over here, we're going to create the section for the code content.
**[00:55:35]** **SPEAKER_01 (PedroTech):** Now, to do that, like I said, we need to install a library that is going to help us format code into actual code, like our actual text that looks like code.
**[00:55:45]** **SPEAKER_01 (PedroTech):** The name of this library is react-syntax-highlighter.
**[00:55:50]** **SPEAKER_01 (PedroTech):** I've used this library so many times in the past, and I think it's awesome for this kind of stuff.
**[00:55:55]** **SPEAKER_01 (PedroTech):** We're just going to install react-syntax-highlighter.
**[00:56:01]** **SPEAKER_01 (PedroTech):** Now, if that's true, I want to do something, like apply some style and if not, I want to apply some other style. Now, if it's not the active tab, I want to make it be BG white, the same way we did over here. I also want to apply the text to be gray. It's going to be white and the border is also going to be blue, but it's going to be 400 at a 20 percent opacity.
**[00:56:03]** **SPEAKER_01 (PedroTech):** What we do is inside of this code content section, we're going to add a div that is going to encompass the section.
**[00:56:09]** **SPEAKER_01 (PedroTech):** All I'm doing to this div is just setting it to be have a position relative and overflow hidden, and I want to grow the flex.
**[00:56:16]** **SPEAKER_01 (PedroTech):** Then on this div, I'm going to call the SyntaxHighlighter component from react-syntax-highlighter.
**[00:56:23]** **SPEAKER_01 (PedroTech):** Now this component is a wrapper component, meaning you have to put something inside of it.
**[00:56:29]** **SPEAKER_01 (PedroTech):** Now, what do we want to put inside of it?
**[00:56:31]** **SPEAKER_01 (PedroTech):** Well, we want to put the code snippets that we put on this object.
**[00:56:37]** **SPEAKER_01 (PedroTech):** So we're going to import that object over here.
**[00:56:40]** **SPEAKER_01 (PedroTech):** CodeExamples, we can just import it like that.
**[00:56:45]** **SPEAKER_01 (PedroTech):** Now, if it is the active tab, then I actually want to make it be blue. I'll make it blue 500 and give it 30 opacity, the text won't be gray, it's going to be white, and the border is also going to be blue, but it's going to be 400 at a 20 percent opacity.
**[00:56:48]** **SPEAKER_01 (PedroTech):** We want to show them depending on what the active tab is.
**[00:56:52]** **SPEAKER_01 (PedroTech):** And we know what the active tab is, so we can access it by just putting activeTab inside of here.
**[00:56:59]** **SPEAKER_01 (PedroTech):** What this will look now is, you see that because App.jsx is the selected one, it has a completely different style than the other ones. And I'll apply this exact same styling functionality to all of the different buttons.

---

### Segment 1 — 01:00:00 - 01:10:00

**[01:00:00]** **SPEAKER_01 (PedroTech):** more to do inside of this SyntaxHighlighter component.
**[01:00:04]** **SPEAKER_01 (PedroTech):** The first thing is, we have to specify a language, because it needs to know what language it is in order to properly format.
**[01:00:10]** **SPEAKER_01 (PedroTech):** Since we're using JavaScript, I'll put JavaScript in here.
**[01:00:12]** **SPEAKER_01 (PedroTech):** Now, I realized that it's causing an error, and the error is actually because we are installing the version 16 plus of react-syntax-highlighter.
**[01:00:22]** **SPEAKER_01 (PedroTech):** I don't recommend installing that one because it's not compatible with the latest version.
**[01:00:25]** **SPEAKER_01 (PedroTech):** I recommend you to, instead, install this version over here, 15.6.6.
**[01:00:29]** **SPEAKER_01 (PedroTech):** That's not a big deal to have a low, not the latest version.
**[01:00:33]** **SPEAKER_01 (PedroTech):** This is just the React syntax highlighter library, it's totally fine.
**[01:00:36]** **SPEAKER_01 (PedroTech):** Now, to, to get that to to that version, we actually need to uninstall React syntax highlighter.
**[01:00:45]** **SPEAKER_01 (PedroTech):** And after uninstalling it, I want you guys to instead install the version 15.6.6.
**[01:00:50]** **SPEAKER_01 (PedroTech):** There's two ways of doing this, you can do it through the command, or you can just paste the version like this on the package.json, then running npm install.
**[01:01:00]** **SPEAKER_01 (PedroTech):** And it should have that version now.
**[01:01:03]** **SPEAKER_01 (PedroTech):** Now let me rerun our, uh, development server, so npm run dev.
**[01:01:08]** **SPEAKER_01 (PedroTech):** And if I refresh this, we should be able to see code.
**[01:01:11]** **SPEAKER_01 (PedroTech):** Perfect. We are being able to see code.
**[01:01:14]** **SPEAKER_01 (PedroTech):** Not only that, but we are able to move through the different code and the code will appear perfectly formatted.
**[01:01:21]** **SPEAKER_01 (PedroTech):** Now, it it's obviously really ugly, so we do want to change that.
**[01:01:25]** **SPEAKER_01 (PedroTech):** Now, to make this look not ugly, we're going to apply a style.
**[01:01:30]** **SPEAKER_01 (PedroTech):** Now, there's a bunch of different styles you can choose.
**[01:01:32]** **SPEAKER_01 (PedroTech):** I'm going to use a different one from the one I have here. The one I have here is from Visual Studio Code.
**[01:01:37]** **SPEAKER_01 (PedroTech):** I'm going to be using the night Owl style.
**[01:01:40]** **SPEAKER_01 (PedroTech):** Now what this is going to do is it's going to make the code look exactly like this.
**[01:01:44]** **SPEAKER_01 (PedroTech):** It's like choosing a VS Code theme for the code in your website.
**[01:01:49]** **SPEAKER_01 (PedroTech):** Now, I also want to apply some custom styles and that's because, uh, I don't like how it looks right now where it's like kind of the edges are not rounded.
**[01:01:58]** **SPEAKER_01 (PedroTech):** So, what we're going to do is, first, we're going to set a margin to be zero.
**[01:02:04]** **SPEAKER_01 (PedroTech):** We don't want any margin on it.
**[01:02:06]** **SPEAKER_01 (PedroTech):** We also want to set the border radius to be equal to 8 pixels.
**[01:02:11]** **SPEAKER_01 (PedroTech):** Then I want to set the font size inside of it, font size to be equal to 11 pixels because I do think it's a bit too big right now.
**[01:02:21]** **SPEAKER_01 (PedroTech):** Then I want to set the line height to be equal to 1.4.
**[01:02:28]** **SPEAKER_01 (PedroTech):** I also want to set the height to be 100%.
**[01:02:37]** **SPEAKER_01 (PedroTech):** And then what I'm going to do is I'm going to set a border.
**[01:02:40]** **SPEAKER_01 (PedroTech):** This border is going to be of 1 pixel, solid, and I'm setting the following color, 3c3c3c.
**[01:02:48]** **SPEAKER_01 (PedroTech):** Perfect, now I can move around the different pieces of code and you can see that it shows the different options appearing in our screen.
**[01:03:00]** **SPEAKER_01 (PedroTech):** Great, and it looks even better when you are, uh, opened up like this.
**[01:03:05]** **SPEAKER_01 (PedroTech):** Obviously, we have to fix this, because, uh, it shouldn't be filling up this whole screen, but it won't because there's going to be a whole different column here on the left.
**[01:03:13]** **SPEAKER_01 (PedroTech):** Now, this is pretty much it for the code content.
**[01:03:17]** **SPEAKER_01 (PedroTech):** What we want to do now is actually show the different floating cards.
**[01:03:22]** **SPEAKER_01 (PedroTech):** This is actually hidden on mobile, so we'll have to open up her screen a bit.
**[01:03:28]** **SPEAKER_01 (PedroTech):** But if I were to open this up, you see that we have this, uh, cards that appear down here that change depending on which, uh, version of this you are.
**[01:03:37]** **SPEAKER_01 (PedroTech):** Now, to have a floating card associated with each, uh, uh, tab, we want to do something similar to what we did here for the code examples.
**[01:03:46]** **SPEAKER_01 (PedroTech):** So, we're going to create a variable here, probably in the same file.
**[01:03:49]** **SPEAKER_01 (PedroTech):** We're going to export constant, call it floating cards.
**[01:03:57]** **SPEAKER_01 (PedroTech):** And I'll make an object inside of here with everything that we need to specify for the floating card.
**[01:04:10]** **SPEAKER_01 (PedroTech):** Now, here you're supposed to like just describe a couple features that your website has.
**[01:04:15]** **SPEAKER_01 (PedroTech):** So, you just put whatever you want. I'm just putting like slop in here like this isn't really anything that makes any sense, but you can put whatever you want in yours.
**[01:04:26]** **SPEAKER_01 (PedroTech):** And there is a couple things that we need to keep track of, because they change on each of them.
**[01:04:30]** **SPEAKER_01 (PedroTech):** First is obviously the title, so this part over here.
**[01:04:34]** **SPEAKER_01 (PedroTech):** Then is the icon that we have here, right? We have a different icon.
**[01:04:38]** **SPEAKER_01 (PedroTech):** Then the description, and then the color of everything.
**[01:04:42]** **SPEAKER_01 (PedroTech):** So in this object, for each of the different tabs, we need to set a bg color, which at least for the first one is going to be bg-blue-500 with 20% opacity.
**[01:04:54]** **SPEAKER_01 (PedroTech):** Then an icon color, which is going to be text-blue-400.
**[01:05:03]** **SPEAKER_01 (PedroTech):** Then we need to put a text color, I'm going to set that to be text-blue-200.
**[01:05:10]** **SPEAKER_01 (PedroTech):** A content color, which is the content that we're highlighting right now, like the actual content inside of it, and that should be text-blue-300.
**[01:05:21]** **SPEAKER_01 (PedroTech):** You can change the colors to whatever you want. I this is just what I chose.
**[01:05:27]** **SPEAKER_01 (PedroTech):** So the icon, uh, for this first one, since we're talking about AI, I just put AI. It's not an actual emoji, but that's fine.
**[01:05:34]** **SPEAKER_01 (PedroTech):** The second one is the title. Uh, I'll put something like this: smart completion.
**[01:05:39]** **SPEAKER_01 (PedroTech):** And then the third one is the content. I'm going to put something generic like AI-powered code suggestions in real-time.
**[01:05:54]** **SPEAKER_01 (PedroTech):** Now, we do this for all of the other tabs, so one for the hero and one for the navbar.
**[01:05:59]** **SPEAKER_01 (PedroTech):** I obviously already did this, so I'll just paste the ones that I already did.
**[01:06:03]** **SPEAKER_01 (PedroTech):** And it should look a bit like this, you change the color and the content for each of them.
**[01:06:07]** **SPEAKER_01 (PedroTech):** And in the end, you should have a specific value for each specific type.
**[01:06:12]** **SPEAKER_01 (PedroTech):** Now, I want to go back to our hero.jsx, I'll close that up.
**[01:06:16]** **SPEAKER_01 (PedroTech):** And for the floating cards, I want to add a div that is going to be actually a div that has a class name that is dynamic.
**[01:06:28]** **SPEAKER_01 (PedroTech):** First, I want to make sure that it doesn't appear in mobile, so I'm going to make it hidden.
**[01:06:33]** **SPEAKER_01 (PedroTech):** Uh, I only show it in a large screen and in our large screen the display is going to be block so that it shows.
**[01:06:39]** **SPEAKER_01 (PedroTech):** Then I'm going to make it absolute.
**[01:06:41]** **SPEAKER_01 (PedroTech):** I'll open the actual content here so we can see, it will be absolute.
**[01:06:45]** **SPEAKER_01 (PedroTech):** It will be absolute, then it's going to have a bottom 4 and a right 4, so it's in the bottom right.
**[01:06:53]** **SPEAKER_01 (PedroTech):** I'm also going to set this to transform and I'm going to translate it on the X direction, eight.
**[01:07:00]** **SPEAKER_01 (PedroTech):** Now, we can't really see anything right now, but you'll be able to see it when we actually add the color of it.
**[01:07:07]** **SPEAKER_01 (PedroTech):** I'm also translating on the Y direction to be 8.
**[01:07:13]** **SPEAKER_01 (PedroTech):** And what I want to do is I want to put a specific width to it, I'm setting the width to be 72.
**[01:07:18]** **SPEAKER_01 (PedroTech):** Now, the thing that changes is the color of it.
**[01:07:22]** **SPEAKER_01 (PedroTech):** So I'm going to add here a variable, and I'm going to access the bg color of this card by getting the floating cards object that we just created, accessing the value through the current active tab and getting the BG color.
**[01:07:41]** **SPEAKER_01 (PedroTech):** So, so we currently can't see it, but when we do, it's going to have the accurate color.
**[01:07:45]** **SPEAKER_01 (PedroTech):** Then inside of this, I'm going to put a div with a class name of flex and an items center with a space in the X direction of two and a margin bottom of two.
**[01:07:57]** **SPEAKER_01 (PedroTech):** You can start seeing it appearing now, since we have some content.
**[01:08:01]** **SPEAKER_01 (PedroTech):** Then, instead of this, I'll put the first div with the icon.
**[01:08:04]** **SPEAKER_01 (PedroTech):** So in here I'll put the floating cards and get the active tab and just say dot icon.
**[01:08:18]** **SPEAKER_01 (PedroTech):** Then below this, I'm going to get a span, which, by the way, it one thing that we can make be easier is instead of always accessing the floating cards.activeTab, we can just make a variable up here called current floating card, I don't know, and then set it equal to this.
**[01:08:42]** **SPEAKER_01 (PedroTech):** Then I can get this, and just reuse it how many times I want without having to always access the active tab.
**[01:08:49]** **SPEAKER_01 (PedroTech):** Now, if I go here, I want to add the span, and I want to add the current floating card, and access the title.
**[01:09:02]** **SPEAKER_01 (PedroTech):** Then I'll do the same thing with, then I'm going to get below this div that we just created and I'm going to create another div which inside of it is just going to include the content.
**[01:09:12]** **SPEAKER_01 (PedroTech):** So I'm going to say current floating card dot content.
**[01:09:16]** **SPEAKER_01 (PedroTech):** Now, we just have to style that.
**[01:09:19]** **SPEAKER_01 (PedroTech):** So on this div over here, I'm going to set a class name, where for the icon, I'm going to say it is going to have a width of six and a height of six.
**[01:09:32]** **SPEAKER_01 (PedroTech):** So in here, I'm going to get the current floating card dot icon color.
**[01:09:41]** **SPEAKER_01 (PedroTech):** Then in here, I'm going to set a display flex, items center, justify center, text to be small, font to be bold.
**[01:09:51]** **SPEAKER_01 (PedroTech):** Then on the span, I'll set a class name where the text is small, the font is medium, and we need to change the color, which means we have

---

### Segment 9 — 01:10:00 - 01:20:00

**[01:10:00]** **SPEAKER_01 (PedroTech):** to make this dynamic as well, and I'll just wrap this entire thing with back ticks, and in here, I'm going to insert the currentFloatingCard.textColor.
**[01:10:13]** **SPEAKER_01 (PedroTech):** Now, what we do after this is, I'm going to copy this class name, I'm going to apply it over here. But, where we want to actually don't use the text color, we want to use the content color, because that's different.
**[01:10:25]** **SPEAKER_01 (PedroTech):** And we also don't want to make the content be font medium, and we want to align the contact the the content to the left, just like this. Perfect.
**[01:10:36]** **SPEAKER_01 (PedroTech):** Now, we see the card appearing over here, and it changes as we move. Now, it is ugly, right? We still have to edit it to make it look cool like this, but that's pretty simple because it's just a bunch of stuff that we have to put in addition to what we already put over here.
**[01:10:51]** **SPEAKER_01 (PedroTech):** So, what I want to do is, I want to add a backdrop blur XL. I'm going to make it rounded large, so it has some border radius. Then, I want to make it such that the padding on it is four, so there's some space. I'm going to set a border to it, and that border is going to be colored white with 20% opacity.
**[01:11:18]** **SPEAKER_01 (PedroTech):** Then, I'm setting a shadow to be large, so 2XL. And that should be enough. So, we'll be able to move through the different items and you should be able to see this moving as well, and it looks pretty good.
**[01:11:32]** **SPEAKER_01 (PedroTech):** Now, the next thing we want to do is, we want to be able to put this on the right over here, right? Because this isn't how it's supposed to be, and have all this text over here. So, I wanted to build the code first, just because I know a lot of you guys came for the video for that, but what we're going to do now is build the left side of this page and it will look a thousand times better.
**[01:11:51]** **SPEAKER_01 (PedroTech):** Okay, everyone. Now it's time for us to add the section that is going to go on the left on web and on top on mobile. So, to do that, I'm going to come back here to our Hero.jsx. We're going to go up to right below this two glows that we put over here, and I actually want to wrap this entire section with two new divs.
**[01:12:15]** **SPEAKER_01 (PedroTech):** This will help us with organization, I'm going to bring the end of this divs to below everything else that we have.
**[01:12:23]** **SPEAKER_01 (PedroTech):** You'll see that now that section will stay smaller and not expand, and we'll go up here and for each of this div, we want to define the following structure.
**[01:12:33]** **SPEAKER_01 (PedroTech):** First of all, I want to set a max width for the whole page, and I'm going to set it to be 7xl, then a margin X of auto, a text center, position will be relative, and the width will be full.
**[01:12:51]** **SPEAKER_01 (PedroTech):** Then, inside of this div I want to set a max width to be also 7xl, then the margin will be auto as well, and I'm going to say a display flex, flex-col, but that depends, because if we are in a small screen, we want to make it into a column, so that we put the text above and then we have this column over here.
**[01:13:13]** **SPEAKER_01 (PedroTech):** But if not, then we want to make it into a grid with two different separate columns. You'll see what I mean by this. If I were to add here, for example, a p tag that says this, and we are in mobile, this will appear on top of this.
**[01:13:26]** **SPEAKER_01 (PedroTech):** But if I were to open this up, we want to change it such that this now appears here. To do that, we come to this second div that we have over here, and we make it such that in a large screen, the display is not even going to be flex. It's going to be grid, and also in our large screen, we're going to make it grid cols 2, so there's two columns.
**[01:13:48]** **SPEAKER_01 (PedroTech):** So now this appears on the left and this on the right, when previously, when you go to mobile, it becomes a single column.
**[01:13:58]** **SPEAKER_01 (PedroTech):** Perfect. Now, I also want to put a gap of six, no matter which kind we are. So, if we are in a single column, this should have a space. And then I want to change this such that if it is a small screen and above, we're going to have a gap of eight, and in a large screen and above, that gap will be 12.
**[01:14:16]** **SPEAKER_01 (PedroTech):** I'm also going to center the items, and set the position to be relative.
**[01:14:24]** **SPEAKER_01 (PedroTech):** Now, inside of this, we don't want to put this random text. We want to put a whole section full of information. We want to put a like a tagline for the the website, this little thing at the top, and then a description together with two actionable buttons.
**[01:14:39]** **SPEAKER_01 (PedroTech):** So first, we'll build the section above, that first little tag that we have.
**[01:14:44]** **SPEAKER_01 (PedroTech):** To do that, I'll add two divs and I'm going to add an icon called sparkle, or sparkles, this one over here. It's an icon from Lucide React, which builds this little thing over here.
**[01:14:58]** **SPEAKER_01 (PedroTech):** Then below this, I want to add a span that will have the name of the website. So, I'm going to say, "Introducing CodeFlow AI," just like that.
**[01:15:11]** **SPEAKER_01 (PedroTech):** Now, we have a lot of work to make this look good. The first thing is building the pill. So, what I want to do is, I want to make it such that this has an a class name of inline flex, so they're next to each other. Then I'm going to just center the items. I'm going to put a gap of two in between them, then I'm setting a padding of X of three in a small screen.
**[01:15:26]** **SPEAKER_08:** but a padding of X of four in a bigger screen.
**[01:15:42]** **SPEAKER_01 (PedroTech):** And then, we can apply the actual coloring and all the styling to the pill.
**[01:15:47]** **SPEAKER_01 (PedroTech):** So, what I can do is I can put a padding of Y of two and put a BG blue of 500. Now that's way too blue, so we're only going to get a 10% opacity in that, so it actually looks like a transparent pill. I'm also setting a border and a color to be border blue 500, but just slightly more less opaque, so 20%.
**[01:16:11]** **SPEAKER_01 (PedroTech):** Then, I want to set this to have full rounded corners. I also want to make it such that this will have a space from the bottom, so margin bottom of four. And in a small screen and above we'll set that to be six.
**[01:16:25]** **SPEAKER_01 (PedroTech):** Then, I want to use the animations that we have created so far, the animate in and the slide in from, but in this case, we don't want to slide in from the top like we have for this. We want to slide in from the bottom. So, we kind of want to have an animation here called slide in from bottom.
**[01:16:47]** **SPEAKER_01 (PedroTech):** Now, we don't have that yet, so we do have to create it. So, we're going to come over here, we're just going to copy the keyframes that we have here, going to paste it here. We're going to change it to say, "Slide in from bottom," instead of top.
**[01:17:01]** **SPEAKER_01 (PedroTech):** And the transformation is kind of going to be the opposite, instead of going from negative one to zero, it's going to go from one to zero.
**[01:17:07]** **SPEAKER_01 (PedroTech):** Then, I'm going to come up here, and I'm going to copy this, and I'm going to change this to say, "Slide in from bottom," and pass this animation name into here.
**[01:17:18]** **SPEAKER_01 (PedroTech):** Now, we can go over here, and we can just use this animation, and you see that when I refresh this, now we should have the animation, but it's not really showing up because there isn't a delay to it. So there's no time set for this animation to work in.
**[01:17:34]** **SPEAKER_01 (PedroTech):** So, what I want to do is, I want to add a duration here. But I want it to not be very quick. I don't want it to be 300 seconds because if you look at how it looks, it's pretty fast, right?
**[01:17:43]** **SPEAKER_01 (PedroTech):** I want it to actually be 700 milliseconds. But we don't have that animation yet, so we do have to create it. So, I'm going to come here and I'm going to change this to have a class name called duration 700, and it will apply the 700 millisecond animation duration.
**[01:18:01]** **SPEAKER_01 (PedroTech):** You see that now, it takes a little bit more, but it makes it look a lot better. Perfect. Now, we just want to style the individual items inside of it. We're going to start with the sparkles.
**[01:18:14]** **SPEAKER_01 (PedroTech):** I'm going to set the width to four and the height to four. I also want to set the color to be blue 400.
**[01:18:17]** **SPEAKER_01 (PedroTech):** We're going to make it be extra small so it's a lot smaller.
**[01:18:25]** **SPEAKER_01 (PedroTech):** Then I want to set for the span, the same thing. We're going to make it be extra small so it's a lot smaller. We want to make it such that on a small screen and above, we need to make it a little bit bigger, and the color is also going to be blue, but it's going to be blue 300.
**[01:18:30]** **SPEAKER_01 (PedroTech):** Perfect.
**[01:18:31]** **SPEAKER_01 (PedroTech):** Now the next thing we want to do is add the tagline that this page is going to have.
**[01:18:35]** **SPEAKER_01 (PedroTech):** So we're going to come down one div here and we want to add an H1 tag that is going to encompass the entire title section.
**[01:18:42]** **SPEAKER_01 (PedroTech):** Now this H1 tag is going to have three spans, because we will be the three different words that we have here.
**[01:18:56]** **SPEAKER_01 (PedroTech):** The second one is going to say something like Build Better, and the last one is just the name of the website.
**[01:19:14]** **SPEAKER_01 (PedroTech):** Now to style them to appear one on top of each other, we're going to come to this H1 over here.
**[01:19:19]** **SPEAKER_01 (PedroTech):** The first one is going to say, "Code Faster". The second one is going to say something like, "Build Better", and the last one is just the name of the website.
**[01:19:27]** **SPEAKER_01 (PedroTech):** But on a small screen and above we're going to set it to be 3xl, on a medium screen we're going to set it to be 4xl and on a large screen we're going to set it to 5xl.

---

### Segment 1 — 80:00 - 01:20:00

**[01:20:00]** **SPEAKER_00 (Pedro):** and then we can see it's basically the same thing that we have for the previous buttons, which is we have an ArrowRight and we have a span, and we also have to pass the correct text, which is "Watch Demo".

---

### Segment 1 — 01:30:00 - 01:40:00

**[01:30:00]** **SPEAKER_01 (PedroTech):** so we're hovering the button, the button becomes bigger. But the inner icon, when we hover it, also expands a bit to the right.
**[01:30:07]** **SPEAKER_01 (PedroTech):** That's what the translate x-1 does. Now, the next thing we want to do is go to this button.
**[01:30:13]** **SPEAKER_01 (PedroTech):** I'm going to copy the class names from this button and just paste it here. Not that we're going to have an exact replica, because we won't, but I want to just save time with not writing a bunch of stuff again.
**[01:30:26]** **SPEAKER_01 (PedroTech):** The main difference here is the background, because we're not going to have a gradient on this one. We're actually going to have a BG that is white and it's only 5% opacity, just like that.
**[01:30:39]** **SPEAKER_01 (PedroTech):** Then a backdrop blur that is going to be small, and we're adding a border around it, and that border will be white, but with 10% opacity.
**[01:30:53]** **SPEAKER_01 (PedroTech):** Now when you hover it, we don't want to scale it. We just want to change the color.
**[01:30:58]** **SPEAKER_01 (PedroTech):** So, I'm going to go to where we have the hover effect, which is over here, and when we hover it, I'm just going to set the BG to become slightly more opaque, so 10. Perfect.
**[01:31:08]** **SPEAKER_01 (PedroTech):** Now inside of this, we have this div which is a bit different, and it's before the text, which is different from above. And in this div, I just want to set a padding of two, a BG that is white, 10. I'm going to set this to be rounded-full, and when we group hover it, the BG will become white 20. So, this is how it's going to look like.
**[01:31:27]** **SPEAKER_01 (PedroTech):** And when we group hover it, the BG will become white 20.
**[01:31:32]** **SPEAKER_01 (PedroTech):** You see how there's an effect to it? Perfect. I'm also adding a duration of 300 and a transition to the colors. Perfect.
**[01:31:45]** **SPEAKER_01 (PedroTech):** Now we'll go to the icon, which is the play button over here. We're adding a class name, same thing as we did over here. I might even just copy this and paste it here, but I don't like this icon without a fill to it.
**[01:31:59]** **SPEAKER_01 (PedroTech):** You see that the one we have over here has a white fill to it.
**[01:32:06]** **SPEAKER_01 (PedroTech):** and you can actually add a fill to an icon in Tailwind by just using the fill, and then giving it a color, like white. I think it looks a lot better. Perfect.
**[01:32:12]** **SPEAKER_01 (PedroTech):** So this is how it looks. It looks pretty good. There are still some things we need to do, but as of right now, this looks really good.
**[01:32:22]** **SPEAKER_01 (PedroTech):** This is how it should look, and this is how it looks right now.
**[01:32:25]** **SPEAKER_01 (PedroTech):** Now, to fix that, what we want to do is, we want to go to the overall section over here, and where we have the large grid calls too, this section over here.
**[01:32:35]** **SPEAKER_01 (PedroTech):** We also want to add a text to be center if this is mobile, and a text to be allowed allowed to the left, if it's a large screen and above.
**[01:32:44]** **SPEAKER_01 (PedroTech):** This will make it such that the text will then become aligned to the left in this big screen. Now, this is not actually the one we're writing. This is the one we're writing, but it should look exactly how it looks over here.
**[01:32:56]** **SPEAKER_01 (PedroTech):** Also the text is slightly smaller, so we do need to apply a bigger height to this h1. So you see how in here we have 5xls, small, medium, large, and so on. We actually want to apply one to XL, and in that case, we want to make it be 6xl, which is slightly bigger, so it actually matches that.
**[01:33:17]** **SPEAKER_01 (PedroTech):** Now we're almost there. There's just some small differences. The main difference is obviously this part over here where the code editor here isn't expanding to the full width.
**[01:33:27]** **SPEAKER_01 (PedroTech):** So to do that, now that is actually because of a bug that we introduced. If you look over here, we are applying the responsiveness of the height, and for some reason I put a width over here, so you want to change that to be a height. You'll see that now it will look perfectly fine just like how it does over here.
**[01:33:47]** **SPEAKER_01 (PedroTech):** Perfect. So, we're pretty much done with this section.
**[01:33:52]** **SPEAKER_01 (PedroTech):** So now it's time for us to start building the next section in this website. The next section is going to come below, and it's going to be the section for the features, where you're able to see the different features being displayed in an alternating order.
**[01:34:06]** **SPEAKER_01 (PedroTech):** Now you can put whatever features you want here, but I like to use code as the example. But in your website you might want to put images instead of the code. But if you want to follow what I'm doing, then I'm going to show you how to do that.
**[01:34:19]** **SPEAKER_01 (PedroTech):** So to do that, we're going to come to our features file over here. I'm going to close this off, and in the features, we want to start by defining what the features are going to be.
**[01:34:31]** **SPEAKER_01 (PedroTech):** So, I'm going to make an array over here called features and we're going to use it.
**[01:34:36]** **SPEAKER_01 (PedroTech):** Now this array is going to be an array of objects, and each feature is going to have a title. For example, the first one, I'm going to say that you can code complete using this product. So AI code completion.
**[01:34:48]** **SPEAKER_01 (PedroTech):** Then we're going to have a description. I'm going to say something like this, like, intelligent code suggestions powered by AI.
**[01:34:56]** **SPEAKER_01 (PedroTech):** Now below this, I want to put an image that is associated with this. Now again, if you want to use real images like a PNG, you put that image over here. But in our case, we're going to be using code, and to do that, we're going to be using the same functionality that we've done over here, but this time we're going to not put the code directly here, but rather use a name for whatever code this is.
**[01:35:22]** **SPEAKER_01 (PedroTech):** So what I'm going to do is, I'm going to give it a name, let's call it code-completion for this one, and we're going to create a code snippet associated with this code completion name.
**[01:35:32]** **SPEAKER_01 (PedroTech):** Then we're going to choose the image position, because they're going to alternate. And one is going to be left, one is going to be right. We can do it whatever you want, but in a big screen you see that the first one is on the left, the second one is on the right, and then the third one is on the left as well.
**[01:35:50]** **SPEAKER_01 (PedroTech):** You can again, change that however you want or even maintain all of them in the same side if you want to.
**[01:36:00]** **SPEAKER_01 (PedroTech):** Now, to do that, I will create one feature, one object like this for each feature. I obviously already created all my features, so I'll just copy and paste the ones, but you want to fill in for all of those.
**[01:36:20]** **SPEAKER_01 (PedroTech):** Now, inside of this features component, I want to return a section. And this is the first section where we do want to put an ID, and the reason we do that is so we can navigate to the feature section when we click on the navbar. So you see that if I were to click over here and go to features, it should scroll me down a bit.
**[01:36:25]** **SPEAKER_01 (PedroTech):** Now since we don't have any content here, it just barely scrolled me down, but it should take me to that section.
**[01:36:31]** **SPEAKER_01 (PedroTech):** I'm also putting a padding and Y of 20, and a padding X of 10 in mobile, and a padding X of 6 in a small screen to medium, and in a large screen and above, we'll set that to be 8.
**[01:36:46]** **SPEAKER_01 (PedroTech):** Then inside of this section, I want to add the first part, which is going to be a div that is going to encompass the entire section.
**[01:36:59]** **SPEAKER_01 (PedroTech):** So we're making a div with an H2, which is going to include a span, and it will say something like this.
**[01:37:10]** **SPEAKER_01 (PedroTech):** It's just a tag phrase for you to be able to display your features.
**[01:37:13]** **SPEAKER_01 (PedroTech):** Now below this, we're adding a line break, and then we're adding another span that should have another type of catch phrase or word that is associated to your product, like workflow.
**[01:37:32]** **SPEAKER_01 (PedroTech):** I'll make this div center the items, and margin bottom of 12, so there's a lot more space.
**[01:37:51]** **SPEAKER_01 (PedroTech):** Now inside of this, on the H2, I want to set the class name to be text 5XL, but then on a small screen and above, we'll make that 4XL.
**[01:38:09]** **SPEAKER_01 (PedroTech):** Also the font is going to be bold, the margin bottom will be four, and we'll set that to be six.
**[01:38:18]** **SPEAKER_01 (PedroTech):** Now, what I want to do is, I want to display the different code pieces together with a text associated with it.
**[01:38:21]** **SPEAKER_01 (PedroTech):** Now what I want to do is, on this first span, we're going to add a BG gradient to it.
**[01:38:26]** **SPEAKER_01 (PedroTech):** Now, inside of this, on the H2, I want to set the class name to be text-5xl, but then on a small screen and above, we'll make that 4xl, then 5xl, then on a large screen we'll make that even bigger, 6xl.
**[01:38:36]** **SPEAKER_01 (PedroTech):** Then we want to clip the text like we did before so the gradient applies to the text.
**[01:38:42]** **SPEAKER_01 (PedroTech):** So in a very large screen, we're going to make that even 32.
**[01:38:50]** **SPEAKER_01 (PedroTech):** Now, we'll do this for this one, and for the bottom one, we're actually going to just apply the a different color.
**[01:38:57]** **SPEAKER_01 (PedroTech):** We're going to make it blue instead. So from blue 400 to cyan 400.
**[01:39:07]** **SPEAKER_01 (PedroTech):** Now, we do want to set a div, uh, class name for this overall section.
**[01:39:13]** **SPEAKER_01 (PedroTech):** It's going to be pretty simple. We're just setting the maximum width of this entire section to be 6XL and the margin in the X direction to always auto.
**[01:39:21]** **SPEAKER_01 (PedroTech):** Then we want to clip the text like we did before, so the gradient applies to the text, and we'll make the text be transparent.
**[01:39:32]** **SPEAKER_01 (PedroTech):** We're going to start by going below this div, and adding a div that is going to encompass the section.
**[01:39:41]** **SPEAKER_01 (PedroTech):** That we're going to space in the Y direction with 16, and put an even bigger gap in between the the different features in a larger screen.
**[01:39:58]** **SPEAKER_01 (PedroTech):** Then inside of this div, we want to loop through our features.

---

### Segment 1 — 01:40:00 - 01:50:00

**[01:40:00]** **SPEAKER_01 (PedroTech):** Now in this div I want to a apply a key directly into it
**[01:40:06]** **SPEAKER_01 (PedroTech):** and a class name.
**[01:40:09]** **SPEAKER_01 (PedroTech):** Now for now we are not going to touch this class name just because I want to put the content inside of it so you guys can at least see what the class names are doing to it.
**[01:40:17]** **SPEAKER_01 (PedroTech):** So the first is going to be the image section
**[01:40:21]** **SPEAKER_01 (PedroTech):** or the code section actually.
**[01:40:24]** **SPEAKER_01 (PedroTech):** I will just say that. I called it image just because I don't know if you guys would rather just make it into an image instead of code.
**[01:40:31]** **SPEAKER_01 (PedroTech):** But yeah.
**[01:40:32]** **SPEAKER_01 (PedroTech):** Now, inside of here I want to have a div and I will put another div to close it.
**[01:40:41]** **SPEAKER_01 (PedroTech):** And I hate that I have to self close all the divs inside of a map but that is just part of developing.
**[01:40:47]** **SPEAKER_01 (PedroTech):** Then I want to start building the structure for this.
**[01:40:50]** **SPEAKER_01 (PedroTech):** It is similar to what we build in the above section with this code.
**[01:40:53]** **SPEAKER_01 (PedroTech):** We are going to start by adding a IDE interface.
**[01:40:58]** **SPEAKER_01 (PedroTech):** And in here we are going to add a div which will contain the header.
**[01:41:06]** **SPEAKER_01 (PedroTech):** I am aware we are adding a bunch of divs but it is going to make sense.
**[01:41:10]** **SPEAKER_01 (PedroTech):** So in the first section it is the header.
**[01:41:12]** **SPEAKER_01 (PedroTech):** We are going to add another div and this one is going to have three divs inside of it.
**[01:41:17]** **SPEAKER_01 (PedroTech):** But this we have already done before so I am going to copy from the hero.
**[01:41:20]** **SPEAKER_01 (PedroTech):** It is just this section over here.
**[01:41:23]** **SPEAKER_01 (PedroTech):** We can actually just copy this, actually I will just copy this over here, not the whole section.
**[01:41:28]** **SPEAKER_01 (PedroTech):** And we can paste it over here.
**[01:41:31]** **SPEAKER_01 (PedroTech):** Now you see, it will make three of those little dots that apply to the code editor header.
**[01:41:38]** **SPEAKER_01 (PedroTech):** Then we do want to put a span in here with the feature title.
**[01:41:42]** **SPEAKER_01 (PedroTech):** So we'll say feature dot title and it should appear right below it.
**[01:41:48]** **SPEAKER_01 (PedroTech):** Now I want to make it such that it is a lot smaller so I am going to say text gray 400 a margin left of two
**[01:41:56]** **SPEAKER_01 (PedroTech):** and I will set that to be even more in a bigger screen and I make it be extra small, so it is a lot smaller, but then on a small screen we are going to make it be small.
**[01:42:06]** **SPEAKER_01 (PedroTech):** Perfect.
**[01:42:07]** **SPEAKER_01 (PedroTech):** Now below this div we are going to add another div and this is for the code highlighting.
**[01:42:13]** **SPEAKER_01 (PedroTech):** So I am going to add here a section where I want to add the syntax highlighter.
**[01:42:21]** **SPEAKER_01 (PedroTech):** So I can actually copy it from here.
**[01:42:23]** **SPEAKER_01 (PedroTech):** I am just going to copy this component.
**[01:42:26]** **SPEAKER_01 (PedroTech):** And I am going to put it directly inside of here.
**[01:42:29]** **SPEAKER_01 (PedroTech):** Now the difference is that in here we don't have the code examples active tab thing.
**[01:42:35]** **SPEAKER_01 (PedroTech):** What we do have though is actually what I think I might just do is you should just instead of putting image name you should make this be the code.
**[01:42:43]** **SPEAKER_01 (PedroTech):** So I am going to say code snippet
**[01:42:50]** **SPEAKER_01 (PedroTech):** and I am just going to insert the code snippet directly in here.
**[01:42:53]** **SPEAKER_01 (PedroTech):** So for example, for the first one it should be something like this.
**[01:42:57]** **SPEAKER_01 (PedroTech):** And then I will copy this and I will put it here and here as well.
**[01:43:02]** **SPEAKER_01 (PedroTech):** And then what we can do is instead of just getting like this we can just say that this is going to be the features object and get the current feature.
**[01:43:14]** **SPEAKER_01 (PedroTech):** Actually I can just say feature dot code snippet and then we should be able to see the code snippet appearing.
**[01:43:22]** **SPEAKER_01 (PedroTech):** Now we do get an error and I think it is because we didn't import this syntax highlighter component.
**[01:43:28]** **SPEAKER_01 (PedroTech):** So I will just do this.
**[01:43:30]** **SPEAKER_01 (PedroTech):** I will just write it again syntax highlighter and it should import.
**[01:43:32]** **SPEAKER_01 (PedroTech):** Also the night owl needs to be imported as well.
**[01:43:36]** **SPEAKER_01 (PedroTech):** Now it should work and you should see all three of them appearing.

---

### Segment 13 — 01:50:00 - 02:00:00

**[01:50:00]** **SPEAKER_01 (PedroTech):** l
**[01:50:00]** **SPEAKER_01 (PedroTech):** but on bigger screens we're going to make that large and I'm going to set the leading to be relaxed so there's more gap in between the texts. Perfect. Now if we go over here the text in itself looks great. Obviously there's a lot to be done around this over here. So what do we want to do? Well first of all let me just pull this over here. There are some changes we need to make to the code itself because it doesn't look like it does over here.
**[01:50:26]** **SPEAKER_01 (PedroTech):** So the first thing is that we made it such that the color of this background actually applies to the color of the VS code code editor here. So here we're using Night Owl but we might want to change it such that it applies the same background color as what we set for this the header section around.
**[01:50:46]** **SPEAKER_01 (PedroTech):** And what we can do is instead of setting the background instead of just letting the background be set by this we can set the background actually in the custom styles, yeah, we are inside of the custom styles, the background here to be transparent and then whatever the background of this section is it will apply to the code editor. You see that now it looks like it's integrated to it but there is a border and we want to remove that. We had that on the other one but on this one we don't want it.
**[01:51:14]** **SPEAKER_01 (PedroTech):** So now it already looks a lot similar to this but there are still some things. For example where is this cool little color around this, this gradient? To add that gradient here is what we need to do. We're going to come above this IDE interface section over here and we have this div but above this div we're going to add a self-closing div that is going to just set this background. It is a self-closing, it doesn't need to wrap anything so make sure it doesn't and it only applies to the background of this section. In my opinion it makes it look a lot better but you can change the colors to whatever you want. You can even make this be green or whatever you want. But I like it going from blue to purple because it matches the theme of the website.
**[01:51:59]** **SPEAKER_01 (PedroTech):** Now we have to address the fact that when I make this into a bigger screen this isn't working. This should appear, this code should appear on the left similar to how this one appears on the right. So the way we fix this is the following way.
**[01:52:08]** **SPEAKER_01 (PedroTech):** Now right off the bat, I can see that there's a bug over here. We set on a large screen for this to be flex grow when in reality it should be flex row. And just like that this fixes the issue. Sorry about that obviously when I'm typing sometimes it might be hard to recognize that I made a misspelling but if you notice that then that's good because yours didn't end up having any issues. So we're pretty much done with the section for the features, and it looks pretty good. You can obviously play around with it if you want to. You can add other things to the text. Like for example I added here a bunch of thing over here for, for this section specifically you can add that for yours as well but it looks totally fine in my opinion. Now we want to add the next section which is going to be the pricing section. This one is pretty interesting because it actually applies to every single landing pages you see out there because you do have to have a pricing section so people can purchase your product.
**[01:53:05]** **SPEAKER_01 (PedroTech):** Okay so now it's time for us to build the pricing section so I'm going to open this up and I'm going to restructure this so we can see how it will look immediately as we're writing the code. So right off the bat we need to do something similar to what we did with the features. We're going to come over here and create an array which is going to define the different plans that we're going to have on this website. So for each plan we're going to have an object with a name, so this is the starter plan, then we have to have a price. For example the starter plan is going to be 29.99 then we're going to have a description, something like perfect for individuals and small teams, then a features section which you should list up whatever you want, usually people make it such that the beginner one has a couple of features and the other ones has all the same features as the ones before plus a couple more. I'm going to add some features here that I already wrote, but you should add whatever makes sense to your website.
**[01:54:11]** **SPEAKER_01 (PedroTech):** And finally, we want to add a Boolean that is going to determine if this is the most popular or not. So there's going to be three of them, right, and one of them is going to be the most popular, which is the middle one, but we need to identify which one is which. Now you do this for all of the plans, again, I already have that so I'm just going to copy and paste and I'll be back in a second. Perfect. So I just added here an option for a professional plan and an option for an enterprise plan. I'm also going to add .99, I always like doing that because I think it looks better. And now what we want to do is, we want to define this section, so I'm going to replace this here with a section tag then on the section I want to put an ID of pricing then for the class name, we're going to put the same stuff that we did for the, for the features section. So we're going to go up here and we'll just copy this entire class name here and then just add it directly here.
**[01:55:12]** **SPEAKER_01 (PedroTech):** Perfect. Now in this section what I want to do is I want to start by just adding the title. We can actually copy the same thing we did here for this, is just this part over here, plus the overall div that will encompass everything, so we need to self close this div over here. One thing I want to do though is, I want to make this be 7 XL just because the pricing section might be a bit bigger. Then inside of this I want to make it such that it says something like this. It should say simple transparent pricing plans and there should be a little description below it. So to do that I'm going to, first on this first one over here, I'm going to say Simple, Transparent, then I'm adding a line break, and then on this one I'm adding Pricing Plans. Then we're closing the H2 and we're adding a paragraph tag which is something we didn't have on the other one. On this one we're just going to add something like this, choose the perfect plan for your needs, all plans include a 14 day free trial. Then I'm going to add a class name here, set it to text gray 400, text base, text XL, and on a small screen and above I'm going to set that to be text large, setting a max width to be 2 XL and a margin X to be auto.
**[01:56:34]** **SPEAKER_01 (PedroTech):** Perfect. Now we're finished with the header section and we can go ahead and build the cards. So I'm adding this div over here and on this div I'm adding a class name of display grid, grid columns of one, but on a medium screen and above we'll make that be two columns, and on a large one we'll make that be three columns. That will make it such that the pricing plan over here in one, like in a mobile screen, it should just fall all of them in one column. In a slightly bigger one it should show two columns and on a bigger one it should show three. Now we're also setting a gap of six in a small screen, we're going to set that gap to be eight and a large screen we'll put it back to be six. Now inside of this div we want to loop through the pricing plans. So for each of the plans we want to map and get the plan plus the key. Then I want to render a div that is going to show each individual card. I'll assign the key to the key field on the div and I'll start by adding the structure of this card. Now this class name is going to be dynamic and the reason for that is because we want to add a different type of style depending on if this is the most popular or not or just the normal ones.
**[01:58:01]** **SPEAKER_01 (PedroTech):** Now to start this off, I'm setting this to be a position relative, a BG slate of 900 but only 50 percent, and a backdrop of blur small. Then we're setting a border, we're setting a rounded XL so you starting to see the three different cards appearing here and we're setting on a small screen and above for it to be rounded 2 XL and we need to set some heights to it. So I'm starting with a padding general padding of six and on a bigger screen that will become eight. Now we want to add a transition all, and a duration of 300. I'm going to make the overflow be visible and I'm going to add a group and a display flex. Now we're setting the flex to be column and the height to be the full length of this. What we want is we want to change this structure depending if the plan is popular. So if the plan dot is dot most popular is true, then I want to add the following class. If not I want to add something else. Now what class do we want to add for the most popular? I want to make it such that the border is going to be blue 500, so the middle one should become like that. Now did we put a most popular? Oh, for some reason here it says popular instead of most popular. Perfect. So the middle one should be like that.
**[01:59:34]** **SPEAKER_01 (PedroTech):** Now, what I want to do is, I want to also set a shadow to be 2 XL on the middle one. I want to set that shadow to be blue, so blue 500 and only put a 20 percent opacity. Then I want to make it such that in a large screen I want to make it even bigger. So you'll see that in a large screen when I open this up, we're going to have the three, but the middle one is going to be slightly bigger. Perfect.

---

### Segment 1 — 120:00 - 130:00

**[02:00:00]** **SPEAKER_01 (PedroTech):** on a smaller on a non-popular one, we want to set the border to have a color of Slate 800.
**[02:00:08]** **SPEAKER_01 (PedroTech):** Then, I also want to make it such that when you hover it, the border will become slate 700.
**[02:00:15]** **SPEAKER_01 (PedroTech):** And this should be good to go. You see, as I hover this stuff, it does affect it.
**[02:00:20]** **SPEAKER_01 (PedroTech):** Now, instead of this, I want to start by adding the most popular tag.
**[02:00:25]** **SPEAKER_01 (PedroTech):** So if the plan is most popular, then I want to add this little tag at the top.
**[02:00:32]** **SPEAKER_01 (PedroTech):** We are adding a div over here that is going to have a another div inside of it.
**[02:00:39]** **SPEAKER_01 (PedroTech):** And inside of the second div, we are going to have a star component which is an icon from Lucide React.
**[02:00:45]** **SPEAKER_01 (PedroTech):** Now, below this, we're also adding a span that says 'Most Popular'.
**[02:00:51]** **SPEAKER_01 (PedroTech):** Now I do want to make it such that it doesn't appear inside, but rather at the top.
**[02:00:55]** **SPEAKER_01 (PedroTech):** So in this div, we're going to set this to have a position absolute, and also it is going to be at the top
**[02:01:03]** **SPEAKER_01 (PedroTech):** like two above the thing, so it's slightly up, that's why it's negative.
**[02:01:07]** **SPEAKER_01 (PedroTech):** And in bigger screens, it will even be more. So, negative top three.
**[02:01:14]** **SPEAKER_01 (PedroTech):** The left is going to be a half, so it's right in the middle, and we're setting this to transform, negative translate x 1 half, and then we're setting the z index to be 10 just to make sure it's above.
**[02:01:28]** **SPEAKER_01 (PedroTech):** Now this div over here, we're going to set the display to flex, items to center, a space in the x direction to be 1, and then we're setting a padding of x of 3, and a bigger padding if it's bigger, a padding of y of 1, same thing, we're just slightly increasing the padding in the y direction if it's a bigger screen.
**[02:01:50]** **SPEAKER_01 (PedroTech):** And we're going to set a bg gradient to the bottom, where it's going to go from blue 500 to cyan 500. So it's the same color we've been using kind of for the different texts.
**[02:02:04]** **SPEAKER_01 (PedroTech):** Then I'm going to make this be rounded full so it's a pill, and I want to make the text be extra small, so that's a lot smaller, and we'll make it small in a bigger screen. The font will be semi-bold and a shadow is going to be large.
**[02:02:23]** **SPEAKER_01 (PedroTech):** Then inside of this, we want to apply some styles to this, this star. We're going to put a width of 3 and a height of 3.
**[02:02:40]** **SPEAKER_01 (PedroTech):** Perfect. And then what I want to do is, next to this, I want to make it such that this will also have a fill white.
**[02:02:52]** **SPEAKER_01 (PedroTech):** And now we have this pill appearing at the top. Perfect.
**[02:02:56]** **SPEAKER_01 (PedroTech):** So now it's time for us to add the first part of this card, which is the plan name, description, and price.
**[02:03:03]** **SPEAKER_01 (PedroTech):** So, I'll add this div over here that should encompass all of that.
**[02:03:08]** **SPEAKER_01 (PedroTech):** In the first section, we'll add the plan name. So, we'll add an H3 that says 'plan.name'.
**[02:03:11]** **SPEAKER_01 (PedroTech):** We'll then add a plan description, so this will become a paragraph tag and it will say 'plan.description'.
**[02:03:24]** **SPEAKER_01 (PedroTech):** Then I want to add a div that is going to encompass this whole thing, and it's going to include the price of this through a span.
**[02:03:41]** **SPEAKER_01 (PedroTech):** Now, I also want to add a span right next to it that is going to say that this is a monthly subscription, so 29.99 per month.
**[02:03:49]** **SPEAKER_01 (PedroTech):** And this should be enough for the section.
**[02:03:52]** **SPEAKER_01 (PedroTech):** Now, above here, we want to make this have a text that is centered, and a margin bottom of 6, with a margin bottom of 8 in bigger screens.
**[02:04:01]** **SPEAKER_01 (PedroTech):** Then for the plan name, I want to set the text to be XL and 2XL in bigger ones, and the font to be bold with a margin bottom of 2.
**[02:04:11]** **SPEAKER_01 (PedroTech):** Then for the paragraph, we'll make the color be gray 400, a text that is extra small, and a text that is small in bigger screens with a margin bottom of 3 and a margin bottom of 4.
**[02:04:26]** **SPEAKER_01 (PedroTech):** Now, on this section, the reason why we made it into a div, is because there's the whole part over here where it's two spans connected.
**[02:04:34]** **SPEAKER_01 (PedroTech):** So, what we want to do is, we want to say display flex so it's in the side, and then we're going to set the items to actually be aligned to the baseline, and then, next to it, we're going to justify everything to the center.
**[02:04:51]** **SPEAKER_01 (PedroTech):** Now, after that, we want to change this span to have a text that is way bigger, so 3XL.
**[02:04:58]** **SPEAKER_01 (PedroTech):** We're then going to make it even bigger on bigger screens, and 5XL as well.
**[02:05:05]** **SPEAKER_01 (PedroTech):** The font is going to be bold, and we want to make it such that it has a gradient color to it.
**[02:05:12]** **SPEAKER_01 (PedroTech):** So what I'm going to do is I'm going to apply this gradient to the right that we've been using, where you can clip the text and make it be a gradient from blue to cyan.
**[02:05:23]** **SPEAKER_01 (PedroTech):** Then, what I want to do is, on this div over on this span, I want to make the text be gray 400, margin left of 1, margin left of 2, the text is small, and the text is base when it's bigger.
**[02:05:37]** **SPEAKER_01 (PedroTech):** Perfect. So now, we have a similar card to the rest of this.
**[02:05:41]** **SPEAKER_01 (PedroTech):** Now there's a bit more that we need to add, we need to add the features for this section, and also the button at the bottom.
**[02:05:47]** **SPEAKER_01 (PedroTech):** Now for the features, here's what we want to do.
**[02:05:50]** **SPEAKER_01 (PedroTech):** We'll get this div, we'll go below here and we'll create an unordered list that will loop through the plan.features.
**[02:06:01]** **SPEAKER_01 (PedroTech):** We'll loop through each feature, get them, get the, since we are inside of a map already that has a key, we need to name this key feature key.
**[02:06:13]** **SPEAKER_01 (PedroTech):** Then instead of this, we want to create a list item and in this list item, I'm going to set the key to be equal to the feature key.
**[02:06:22]** **SPEAKER_01 (PedroTech):** And for each item in this list item, I want to render a check mark on the left, since this is a, it's this, the features over here.
**[02:06:33]** **SPEAKER_01 (PedroTech):** So I'm going to use the check mark icon, it's called check from Lucide React.
**[02:06:40]** **SPEAKER_01 (PedroTech):** Then, I want to have a span below this that will just show the name of the feature.
**[02:06:47]** **SPEAKER_01 (PedroTech):** Now, let's obviously style this. For this list item, what I want to do is I want to set a display flex, I want to set them to the left, so item start, and I want to put a space, a gap in the x direction of 2, and on a bigger screen that should be a bit more.
**[02:07:04]** **SPEAKER_01 (PedroTech):** Then for the check mark, what I want to do is, I want to set a width of 2.5 and a height of 2.5.
**[02:07:12]** **SPEAKER_01 (PedroTech):** And also I want to make it have a width of 4, a height of 4, and I'll make that be different on a bigger screen, and I'll make it be rounded full, so there's a circle around the icon.
**[02:07:26]** **SPEAKER_01 (PedroTech):** But for that, we need to put a background, so you can see that it's a circle. So we'll make it be 500 divided by 20.
**[02:07:34]** **SPEAKER_01 (PedroTech):** Then we want to center the check marks inside of that, so I'm going to say display flex, items center, and justify center.
**[02:08:04]** **SPEAKER_01 (PedroTech):** Then, I want to make it such that it is going to have a text blue of 400.
**[02:08:10]** **SPEAKER_01 (PedroTech):** But since we're also applying a different height, uh, for the overall circle when it's a bigger screen, we'll do the same thing here, but the height and width is going to be 3.
**[02:08:20]** **SPEAKER_01 (PedroTech):** Now, you can see that when I expand this it becomes bigger, and it already looks pretty nice.
**[02:08:26]** **SPEAKER_01 (PedroTech):** Now, we do want to change the text for the feature, I want to add a text gray 300, so we change the color.
**[02:08:34]** **SPEAKER_01 (PedroTech):** Then I want to set the text to be small, and a text to be base when it's bigger.
**[02:08:41]** **SPEAKER_01 (PedroTech):** I'm just going to put a gap so that spaces this out a bit in the Y direction and we're going to set it to 3.
**[02:08:53]** **SPEAKER_01 (PedroTech):** Then, in bigger screens we're going to set that to be 4, a margin bottom of 6 and a margin bottom of 8, and we're setting the flex to be row.
**[02:09:05]** **SPEAKER_01 (PedroTech):** Perfect. Now, you see that we can expand and it looks pretty good.
**[02:09:12]** **SPEAKER_01 (PedroTech):** Now, we just have to add the action button at the bottom.
**[02:09:17]** **SPEAKER_01 (PedroTech):** So, since we've added this action button before, it's going to be very similar to this action button from the top up here.
**[02:09:25]** **SPEAKER_01 (PedroTech):** So, what I want to do is, I want to come here and I want to add this button. This button will change, depending on if this is the popular plan or not.
**[02:09:33]** **SPEAKER_01 (PedroTech):** If it's the popular plan, then it should show a gradient around the button.
**[02:09:40]** **SPEAKER_01 (PedroTech):** If not, it should just show this generic button, which has a background color of white with 5% of opacity.
**[02:09:48]** **SPEAKER_01 (PedroTech):** Now, below this section over here, so right over here, we want to add a little text that allows the user to be able to contact us if they need a custom plan.
**[02:10:00]** **SPEAKER_01 (PedroTech):** This is done whenever a business.

---

### Segment 1 — 02:10:00 - 02:20:00

**[02:10:00]** **SPEAKER_01 (PedroTech):** or something one wants to purchase your product for a lot of people so you can make a custom plan so that you earn more from providing more of your service to more people
**[02:10:11]** **SPEAKER_01 (PedroTech):** Now in here, I'm going to add a text saying, "Need a custom plan?"
**[02:10:17]** **SPEAKER_01 (PedroTech):** And I want to add an A tag that is right next to it, not an A P tag, an A tag, that will have a link to you being able to contact you.
**[02:10:29]** **SPEAKER_01 (PedroTech):** So, I'm going to say "Contact our sales team."
**[02:10:32]** **SPEAKER_01 (PedroTech):** Now, what I want to do is in this div, I'm going to add a margin top of eight, and we'll make that 12 in a bigger one, and I want to center this right in the middle.
**[02:10:42]** **SPEAKER_01 (PedroTech):** Then, I want to come to this paragraph tag, I'll make the color of it be "text-gray-400", "text-base", and a "text-xl".
**[02:10:56]** **SPEAKER_01 (PedroTech):** Then to make this look blue because it's a link, we just have to pass an href here.
**[02:11:00]** **SPEAKER_01 (PedroTech):** Now, you'll pass the href you want. This is also a this is obviously a fake website, but if you want, you can put a link to your email or a link to a different part of your page where someone can contact your team.
**[02:11:13]** **SPEAKER_01 (PedroTech):** Now, for the styling, I want to make this be blue, so blue-400 so it looks like a link, and I want to make this such that when you hover it, it just becomes "text-blue-300".
**[02:11:24]** **SPEAKER_01 (PedroTech):** Perfect. And now we have this beautiful pricing section that has the most popular plan is the one in the middle with different UI for them, and it looks really nice.
**[02:11:35]** **SPEAKER_01 (PedroTech):** There's just one minor thing I want to change, which is this over here. I added this thing. I love adding this, which is a glassy effect when you hover something.
**[02:11:42]** **SPEAKER_01 (PedroTech):** I think this gives a good aesthetic to it, and if you want to do something like this, it's actually pretty simple.
**[02:11:57]** **SPEAKER_01 (PedroTech):** I add this a bunch of times into my different projects, it's pretty big.
**[02:12:01]** **SPEAKER_01 (PedroTech):** But basically, it just has an absolute positioning at the top, and when you hover it, it expands a gradient from the top left to the bottom right.
**[02:12:13]** **SPEAKER_01 (PedroTech):** Now, it looks really good when you hover it, but one thing I just noticed is there's a small gap in here, so I think what we need to do is we need to add here a rounded-full, so that that doesn't happen.
**[02:12:24]** **SPEAKER_01 (PedroTech):** But then that happens, so let's just make it be rounded-large. Yes, it fits perfectly now.
**[02:12:33]** **SPEAKER_01 (PedroTech):** So, if you want to add this, either get the code from the description where we're going to have this, or you can just try to pause here and look at the code, but this is how it looks.
**[02:12:43]** **SPEAKER_01 (PedroTech):** It has some hover effects, some translation, and a duration, and a gradient.
**[02:12:50]** **SPEAKER_01 (PedroTech):** Perfect, so we're pretty much done with our project.
**[02:12:53]** **SPEAKER_01 (PedroTech):** We just have to do one more section, which is the section, oh this is interesting. Why did that disappear? I don't know, but it's back.
**[02:13:02]** **SPEAKER_01 (PedroTech):** So, we want to make the section for the testimonials, and then add a simple footer.
**[02:13:10]** **SPEAKER_01 (PedroTech):** So, for the testimonials, we're going to come back to our section over here, testimonials.
**[02:13:17]** **SPEAKER_01 (PedroTech):** And, similar to everything we've been doing so far with the last two sections, the testimonials is going to have an array which we are going to use to loop through.
**[02:13:25]** **SPEAKER_01 (PedroTech):** Now, you can add as many testimonials as you want. I added three. I think that's perfectly fine.
**[02:13:31]** **SPEAKER_01 (PedroTech):** So, testimonials. And obviously you want to make sure to get real testimonials, okay? I know it's tempting to put fake ones, but if you're going to have a real website, you put real testimonials.
**[02:13:41]** **SPEAKER_01 (PedroTech):** Just add fake ones in this example like I have, because it's just for the experience of building the website.
**[02:13:48]** **SPEAKER_01 (PedroTech):** Now, for the testimonials, each testimonial requires the name of the person who created the testimonial.
**[02:13:59]** **SPEAKER_01 (PedroTech):** Then, you put their role, so their job, like a Senior Developer.
**[02:14:06]** **SPEAKER_01 (PedroTech):** Then, we're going to have an image. Now, an image is the image of the person.
**[02:14:12]** **SPEAKER_01 (PedroTech):** Since this is like fake, this is a mock data. I'm using an a URL from Pexels, which is a free copyright website where you can get pictures of people or other things as well.
**[02:14:22]** **SPEAKER_01 (PedroTech):** Now, we're also going to put a content, which is just what the person said about your platform.
**[02:14:27]** **SPEAKER_01 (PedroTech):** So, I have this fake data here. It's just some silent, uh it's just some simple, uh quotes saying that like this platform makes me, I don't know, work a thousand times more efficiently.
**[02:14:40]** **SPEAKER_01 (PedroTech):** Now, it's time for you to add the other ones. I already have them over here. I created two more.
**[02:14:49]** **SPEAKER_01 (PedroTech):** I usually like to put different roles and different kinds of people, but we have three people to show up.
**[02:14:52]** **SPEAKER_01 (PedroTech):** Great. Now it's time for us to build the beginning infrastructure of this section.
**[02:14:57]** **SPEAKER_01 (PedroTech):** Now to do that, it's going to be very similar to the previous one as well.
**[02:15:00]** **SPEAKER_01 (PedroTech):** So, I'm going to copy this logic over here, even the header, and I'm just going to paste it over here.
**[02:15:07]** **SPEAKER_01 (PedroTech):** Now, we have to fix some stuff, like I have to add a self-closing div and a self-closing section.
**[02:15:13]** **SPEAKER_01 (PedroTech):** But we should have a header with a section appearing at the bottom.
**[02:15:16]** **SPEAKER_01 (PedroTech):** We'll change this to say testimonials.
**[02:15:21]** **SPEAKER_01 (PedroTech):** And also I feel like, oh here over here we want to change this instead of saying, instead of having a span, we actually want to just have an H2 tag that will say, "What developers are saying about us".
**[02:15:39]** **SPEAKER_01 (PedroTech):** And then, what I want to do is, for the speed tag, I'll add something else, like, uh just more promotion for your website.
**[02:15:47]** **SPEAKER_01 (PedroTech):** Now, there's a bit of styling that we want to do here, like I don't like how this title is set up. It should be like this.
**[02:15:52]** **SPEAKER_01 (PedroTech):** So, what I want to do is, this section, this title should be particularly different from the other ones because in a larger screen this section has a title on the left and the content on the right.
**[02:16:02]** **SPEAKER_01 (PedroTech):** And on the other ones, it just has a title in the middle.
**[02:16:06]** **SPEAKER_01 (PedroTech):** So, to address this, I'm going to open this up and here's what we want to do.
**[02:16:10]** **SPEAKER_01 (PedroTech):** We're going to start by setting here a thing that says left side, which is the header.
**[02:16:17]** **SPEAKER_01 (PedroTech):** Then we want to wrap this entire thing around with a div that will wrap even the section below.
**[02:16:24]** **SPEAKER_01 (PedroTech):** And this div is going to have a class name of display flex, flex column.
**[02:16:30]** **SPEAKER_01 (PedroTech):** In a large screen is going to become a flex row.
**[02:16:36]** **SPEAKER_01 (PedroTech):** And I'm going to set the items to the start, a gap between them of eight, make that gap bigger in bigger screens and even bigger later on, so gap 16.
**[02:16:47]** **SPEAKER_01 (PedroTech):** Then on the left side over here, I want to remove this, and what I want to do instead is I want to make it such that it has a on a large screen, the width is going to be one half of the screen.
**[02:16:58]** **SPEAKER_01 (PedroTech):** So on a large screen it should only be on the left and it should fit in half of the screen.
**[02:17:04]** **SPEAKER_01 (PedroTech):** The other, the other thing I want to do is I want to make the width be full if it's not a large screen, which is the case if it's mobile because then you'll see when it's mobile, it actually goes and stays the full length and puts the other stuff in the middle.
**[02:17:21]** **SPEAKER_01 (PedroTech):** Now, after that, I want to center the items and on a large screen I'll just set them to the left.
**[02:17:28]** **SPEAKER_01 (PedroTech):** Now this looks fine both on the large screen and on a small screen.
**[02:17:34]** **SPEAKER_01 (PedroTech):** So, so now what I want to do is I want to create the right side, which is the Testimonials.
**[02:17:45]** **SPEAKER_01 (PedroTech):** So to do that, I'll create here a div that is going to have a class name of display flex and items start.
**[02:18:03]** **SPEAKER_01 (PedroTech):** And a space in the x direction of three, with a bigger space when it's bigger.
**[02:18:18]** **SPEAKER_01 (PedroTech):** Now inside of this div, I want to add the two parts of, uh, the testimonial card.
**[02:18:32]** **SPEAKER_01 (PedroTech):** It's going to have this part over here, which is the quotation mark, and the second part is the actual testimonial.
**[02:18:45]** **SPEAKER_01 (PedroTech):** So, to do that, what I want to do is I want to, first create the left part by creating this div.

---

### Segment 1 — 140:00 - 150:00

**[02:20:00]** **SPEAKER_00 (Pedro):** that is going to have a flex shrink
**[02:20:03]** **SPEAKER_13:** of zero.
**[02:20:07]** **SPEAKER_13:** then in this div, I want to add a div with the quotation mark.
**[02:20:14]** **SPEAKER_13:** Now, we do want to make the quotation mark a lot bigger and have a gradient.
**[02:20:30]** **SPEAKER_13:** Then below this, we'll go down two divs. We'll make the right side, and the right side is going to be the actual testimonial with the user image and everything else.
**[02:20:38]** **SPEAKER_13:** So, I'm going to set this to be flex grow.
**[02:20:42]** **SPEAKER_13:** And inside of this div, I want to add a p tag that is going to list the testimonial.
**[02:20:51]** **SPEAKER_13:** Now, we also want to put the image of the user.
**[02:20:55]** **SPEAKER_13:** So below this P tag, I'm going to add a div that is going to have an image that shows the profile image of the user by using the source.
**[02:21:11]** **SPEAKER_13:** Now we want to specify an alt as well for accessibility reasons.
**[02:21:20]** **SPEAKER_13:** Uh, actually, no. Let's put the name of the user as the alt.
**[02:21:25]** **SPEAKER_13:** Then in the class name here to make the image uh look like a circle, I'm going to make this have a width and a height that is exactly the same.
**[02:21:35]** **SPEAKER_13:** And then, it looks kind of smashed, but you you'll see it will look good.
**[02:21:38]** **SPEAKER_13:** We're going to make the width be 12 and the height be 12 in bigger sizes.
**[02:21:43]** **SPEAKER_13:** And then I'll make this into a full circle.
**[02:21:48]** **SPEAKER_13:** Then I want to make the object cover, which then what this makes is, it makes it such that it doesn't squish. It just clips around the image.
**[02:21:59]** **SPEAKER_13:** Now, I will come to the testimonial over here, I'm adding a class name. Make this text white, we're then going to set this to text base. On a small screen, this will become text large, and we're going to have a leading that is relaxed and a margin bottom of three with a margin bottom of four when it's small.
**[02:22:18]** **SPEAKER_13:** Now, for this div over here, we're going to add a class name where we say display flex. We're going to center the items.
**[02:22:25]** **SPEAKER_13:** There's going to be a space in the x direction of two, and you'll see, because we'll have to put the name of the user as well next to their profile image.
**[02:22:32]** **SPEAKER_13:** So that's the gap for that, and we'll make it bigger as well.
**[02:22:36]** **SPEAKER_13:** Now below this image, I want to add a div to put the name and the role of the user.
**[02:22:43]** **SPEAKER_13:** So in here, I'm going to add a an H4 tag, I feel like H4 makes sense.
**[02:22:51]** **SPEAKER_13:** Then below this, we'll add a paragraph tag for the role.
**[02:22:59]** **SPEAKER_13:** Now, we want to make the H4 have a font that is semibold, a text that is white, and I also want to make the text be small, but on a small screen, we'll make the weight be base.
**[02:23:14]** **SPEAKER_13:** Then I'm going to copy this, and I'm going to paste it over here.
**[02:23:19]** **SPEAKER_13:** Now we want to change just a bit. We want to make it, actually, we're just going to change everything.
**[02:23:24]** **SPEAKER_13:** We're going to make the text be extra small, and it will be small on bigger screens and then the color won't be white, it'll actually be gray 400.
**[02:23:35]** **SPEAKER_13:** And now we are pretty much done with the section.
**[02:23:39]** **SPEAKER_13:** Yeah, the only thing that we need to do is put a gap in between these different items over here.
**[02:23:45]** **SPEAKER_13:** And to do that, we can come here to where we're looping. We have this div over here, and we have to add a space Y of six.
**[02:23:56]** **SPEAKER_13:** This should be good, but on a bigger screens, we want to make that gap be even bigger so I'll make it eight.
**[02:24:03]** **SPEAKER_13:** And now we have this beautiful testimonial section that adapts fully responsive, in whatever kind of screen we're in.
**[02:24:09]** **SPEAKER_13:** Now we're almost done with the website. We just want to add the footer.
**[02:24:12]** **SPEAKER_13:** For the footer, I'll be honest, I don't think it matters that much, especially if you're building a website like this.
**[02:24:19]** **SPEAKER_13:** Like we don't have any of these links in this website, we're just building the the landing page.
**[02:24:24]** **SPEAKER_13:** So for the footer, I'm actually going to go a little bit faster than what we were in the other pages.
**[02:24:29]** **SPEAKER_13:** So for the footer, what I want to do is I'll close all of this, we'll come here to the footer section. So, where's the footer? It's uh here.
**[02:24:39]** **SPEAKER_13:** And I'm just going to copy and paste the entire code for the section and go over everything that we do.
**[02:24:44]** **SPEAKER_13:** So, first of all, we are seeing that the footer is now here.
**[02:24:47]** **SPEAKER_13:** You can clearly see it works, and it works in mobile as well.
**[02:24:54]** **SPEAKER_13:** If you come over here, it actually in mobile, I made it such that the footer becomes way smaller, just because it would look kind of weird to show off the different links in a mobile setting.
**[02:25:02]** **SPEAKER_13:** Now, this is what this code looks like.
**[02:25:04]** **SPEAKER_13:** First of all, we choose the links that we want to have.
**[02:25:07]** **SPEAKER_13:** So, footers usually have a bunch of links depending on what kind of company you have.
**[02:25:12]** **SPEAKER_13:** So you divided into different sections.
**[02:25:14]** **SPEAKER_13:** Then in here, we create a section normally like we would before.
**[02:25:17]** **SPEAKER_13:** We put the logo and the name like we did on the Navbar, and a little bit of a tagline for the company.
**[02:25:23]** **SPEAKER_13:** Then we list out all of our social media platforms, this part over here.
**[02:25:28]** **SPEAKER_13:** And if you have a company and you have a profile in those, you go ahead and put the Href to link to that.
**[02:25:34]** **SPEAKER_13:** Now, we used the icon from Lucide React for each of them.
**[02:25:38]** **SPEAKER_13:** And then we loop through the footer links through this object.entries.map, because object.entries will make a list out of an object, and it loops through all of them and makes a link for each individual section.
**[02:25:53]** **SPEAKER_13:** Now this is pretty much it.
**[02:25:54]** **SPEAKER_13:** There is one more thing I do want to do though, which is if you've noticed on this one over here, it has a border bottom to the Navbar when we are scrolling.
**[02:26:04]** **SPEAKER_13:** But when we get to the top, that border bottom disappears.
**[02:26:08]** **SPEAKER_13:** In this case, it just never has that border bottom.
**[02:26:11]** **SPEAKER_13:** Now some people might like it like this, might like it without the border bottom, with the glass morphism, uh because of the backdrop blur that we added.
**[02:26:21]** **SPEAKER_13:** However, I like this and this is what I promised, so this is how we do it.
**[02:26:26]** **SPEAKER_13:** So, we're going to come bit back here to our App.jsx, and we're going to have to create a variable called scrolled, which detects if the user has scrolled or not, and we're going to pass this as a boolean to the Navbar component.
**[02:26:39]** **SPEAKER_13:** Now to detect if the user has scrolled or not, it's similar to what we did with the other sections.
**[02:26:45]** **SPEAKER_13:** So, we're going to come here and we're going to create a state called scrolled and a function called setScrolled. Set this equal to a use state, which will be false.
**[02:26:57]** **SPEAKER_13:** And then I'm going to pass a use effect that is going to subscribe to a scroll listening event.
**[02:27:08]** **SPEAKER_13:** So, I'm going to come here and add an empty dependency array and then in here, I am going to add a window.addEventListener, and we're going to subscribe to the scroll event.
**[02:27:20]** **SPEAKER_13:** And when we subscribe to that, we're going to call this function we're going to create called handleScroll.
**[02:27:25]** **SPEAKER_13:** Now, we'll create that function up here. We'll say function handleScroll.
**[02:27:33]** **SPEAKER_13:** And this is exactly like what we did for the mouse, but it's for the scroll.
**[02:27:37]** **SPEAKER_13:** And we can set the value of the scrolled boolean to be true if the user has a scroll positioning in the Y direction to be greater than 50, which is, I believe the height of the navbar.
**[02:28:00]** **SPEAKER_13:** So, we need to now return something here because we need to clean this up, so there's no memory leaks.
**[02:28:07]** **SPEAKER_13:** So we're just going to copy this, and I'm going to say removeEventListener for the scroll event.
**[02:28:15]** **SPEAKER_13:** Then we pass this value to the navbar, now in this navbar we need to get that, so I'm going to say scrolled as one of the options here.
**[02:28:21]** **SPEAKER_13:** And all I want to do is in our navbar over here, this should become a dynamic navbar.
**[02:28:28]** **SPEAKER_13:** So I'll close this up, make it into a dynamic class name.
**[02:28:32]** **SPEAKER_13:** And you know where we put the background color over here, with the back blur and the background color over here, we're just going to wrap this around with a variable.
**[02:28:41]** **SPEAKER_13:** And we're going to check to see if the user has scrolled. We want to do something, if not, we want to leave it how it was.
**[02:28:49]** **SPEAKER_13:** Now, what do we want to do if the user scrolled? Well, I'm going to copy this, paste it over here.
**[02:28:54]** **SPEAKER_13:** And I want to change it a bit. I want to make the actual opacity be a lot bigger.
**[02:29:00]** **SPEAKER_13:** Because I do like the glass morphism, but I want to be able to have more opacity on the navbar when we're scrolling.
**[02:29:09]** **SPEAKER_13:** But most importantly, I want to make the blur be large and set a border to the bottom.
**[02:29:15]** **SPEAKER_13:** That border will have a color of slate 800, so it blends in with the color.
**[02:29:22]** **SPEAKER_13:** Now you see when I scroll down, it should now have a border which it didn't have before.
**[02:29:29]** **SPEAKER_13:** Now, we just have to fix one more thing.
**[02:29:32]** **SPEAKER_13:** So, obviously, there is two issues here with the code.
**[02:29:36]** **SPEAKER_13:** The first one is that it's still kind of not filling the entire section, and the second one is that if you go into a smaller screen, it does work and feel up the section, but then the code inside of it is centered, which doesn't make sense because who codes in a code editor where the code is centered?
**[02:29:46]** **SPEAKER_13:** Now to fix that, we're going to go here to our hero.
**[02:29:49]** **SPEAKER_13:** And we're going to go to, uh, let's take a look to see what it could be.
**[02:29:54]** **SPEAKER_13:** Okay, it seems like I remember fixing this, maybe we have two of these, but, uh, you see how we're, setting the class names

---

### Segment 1 — 150:00 - 153:01

**[02:30:00]** **SPEAKER_00 (Pedro):** not 150:00 for this but I remember fixing this. We changed this to become a height instead of a width.
**[02:30:05]** **SPEAKER_00 (Pedro):** And I believe now this will fix this.
**[02:30:07]** **SPEAKER_00 (Pedro):** I clearly remember us fixing this, maybe I command-Z for some reason, but now it works.
**[02:30:13]** **SPEAKER_00 (Pedro):** Now, what we want to fix is the alignment of this, because this shouldn't be aligned to the center.
**[02:30:18]** **SPEAKER_00 (Pedro):** Now, to fix that, I'm going to go to our syntax highlighter, and I want to add some minor things that we haven't added so far.
**[02:30:27]** **SPEAKER_00 (Pedro):** So let me just expand this more like this. What I want to do is I want to set the wordWrap to break-word.
**[02:30:35]** **SPEAKER_00 (Pedro):** This is just a minor thing in case there's an issue with that, and I want to make the white space be pre-wrap.
**[02:30:43]** **SPEAKER_00 (Pedro):** Now, we need to go to where we set the text positioning, so let me go to where I say text-left.
**[02:30:54]** **SPEAKER_00 (Pedro):** No. Actually, I can just come to the code editor over here and I can pass a textAlign and set this to be aligned to the left.
**[02:31:07]** **SPEAKER_00 (Pedro):** That works better. Perfect. So, now we're pretty much done with the website.
**[02:31:13]** **SPEAKER_00 (Pedro):** If you don't want to deploy this, then you're pretty much done, but now what we're going to do is be able to deploy this very easily by using Vercel as our host.
**[02:31:23]** **SPEAKER_00 (Pedro):** So, if you don't have an account, I recommend going to Vercel and creating one.
**[02:31:26]** **SPEAKER_00 (Pedro):** I already have one, so I'm just going to come here and add, uh, add project.
**[02:31:31]** **SPEAKER_00 (Pedro):** And what's going to happen is it's going to import our Git repositories. The reason for that is because I created a Vercel.com account by using my GitHub account as the link.
**[02:31:43]** **SPEAKER_00 (Pedro):** So I recommend you doing that as well. So we're going to go to GitHub, just like this, and we're going to create a new repository.
**[02:31:49]** **SPEAKER_00 (Pedro):** I'm going to call this the modern-ux-ui website, something like that.
**[02:31:58]** **SPEAKER_00 (Pedro):** And I'm going to click on create repository. Then I'm going to copy all of this. I'm going to come back to our code over here, and I want to open up our terminal and run the command git init, git add dot, and then paste all of that.
**[02:32:19]** **SPEAKER_00 (Pedro):** Now our code should be in the GitHub repo. And by the way, this is the code that you guys have been looking at ever since the beginning of this video.
**[02:32:27]** **SPEAKER_00 (Pedro):** But most importantly, now that repository should appear here in our Vercel account to be able to deploy.
**[02:32:32]** **SPEAKER_00 (Pedro):** I'm going to click on import, and it's going to detect that the framework is Vite.
**[02:32:37]** **SPEAKER_00 (Pedro):** If you for some reason used a, an environment variable in this project, which I didn't because it wasn't necessary, you can add them right over here.
**[02:32:45]** **SPEAKER_00 (Pedro):** But we don't need to. So I'm just going to click on deploy.
**[02:32:48]** **SPEAKER_00 (Pedro):** And hopefully, if everything is right, in less than a minute we should see our website deployed live.
**[02:32:52]** **SPEAKER_00 (Pedro):** Great. As you can see, again, took less than a minute. I'll click on continue to dashboard and I'll click visit, and as you can see our website is live and ready to be used.