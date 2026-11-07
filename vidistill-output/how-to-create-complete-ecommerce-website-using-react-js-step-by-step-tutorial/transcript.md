# Transcript

### Segment 1 — 00:00:00 - 00:10:00

**[00:00:01]** **SPEAKER_00 (GreatStack):** Hi guys. In this video, we are going to create a complete e-commerce website using MERN stack. As you can see on my computer screen, this is our website. Here we have this navigation bar, using that we can navigate to different pages.
**[00:00:19]** **SPEAKER_00 (GreatStack):** On this homepage, we have this hero element. After that, we have the products popular in the women's category. Then, we have a banner where you can display the exclusive offers. Then, we have the new collections.
**[00:00:30]** **SPEAKER_00 (GreatStack):** So when we will add a new product from our admin panel, that will be displayed in this new collection.
**[00:00:43]** **SPEAKER_00 (GreatStack):** After that, we have one newsletter subscription box. And at the end, we have the footer with some links.
**[00:00:51]** **SPEAKER_00 (GreatStack):** Let's navigate to the men's category. Here you will see the products of the men's category.
**[00:01:02]** **SPEAKER_00 (GreatStack):** Now navigate to the women's category. Here, you will get the products related to the women's category.
**[00:01:13]** **SPEAKER_00 (GreatStack):** And now let's go to the kids category, and here also you can see we have only kids product on this page.
**[00:01:24]** **SPEAKER_00 (GreatStack):** Here we have the login button. If we click here, it will open the login page. If you don't have the login ID and password, you can create one by clicking here. And in this one, we'll add one username.
**[00:01:36]** **SPEAKER_00 (GreatStack):** let's add UserOne. We'll add one email ID, let's add user1@gmail.com and we will add the password 12345678, then click on this button, so it will create a new user and we will logged in on our website.
**[00:02:02]** **SPEAKER_00 (GreatStack):** You can see we have logged in on our website, and now the user has been generated.
**[00:02:10]** **SPEAKER_00 (GreatStack):** For the database, we are using MongoDB Atlas database.
**[00:02:16]** **SPEAKER_00 (GreatStack):** On this web page, if I click on the category and open any product, and here we have the product images, then product title, price of the product, then small description of the product. And here we have the option to select the size and one add to cart button.
**[00:02:37]** **SPEAKER_00 (GreatStack):** If I click on the add to cart button, this product will be added here. You can see in the cart item this product is available. If I come back and click the cart button again, and you can see the same product has been added, and you can see the quantity two.
**[00:02:54]** **SPEAKER_00 (GreatStack):** And the total price has been increased. Now come back and let's add some more products in the cart.
**[00:03:07]** **SPEAKER_00 (GreatStack):** Now you can see the cart page. Here we have total four quantity. You can see two quantity for the first product, then other two products.
**[00:03:17]** **SPEAKER_00 (GreatStack):** This will display the total of individual product and this cart total will display the total cart value.
**[00:03:25]** **SPEAKER_00 (GreatStack):** Let's click on the logout, so this cart item will become zero, and if we login again with the same ID, we will use user1@gmail.com and password.
**[00:03:45]** **SPEAKER_00 (GreatStack):** So we are logged in, and again you can see we have the same items in this cart.
**[00:03:54]** **SPEAKER_00 (GreatStack):** If I logout again, let's try to login on this webpage with any wrong password.
**[00:04:04]** **SPEAKER_00 (GreatStack):** With any wrong password, so it will give a message, please try with correct email/password.
**[00:04:14]** **SPEAKER_00 (GreatStack):** If I click here for creating a new user with the same email ID,
**[00:04:24]** **SPEAKER_00 (GreatStack):** So, it will give a message, existing user found with this email.
**[00:04:33]** **SPEAKER_00 (GreatStack):** So we are going to create this complete e-commerce website using MERN stack, so let's start the video.
**[00:04:42]** **SPEAKER_00 (GreatStack):** First we will come to our desktop screen, and here we will create a folder.
**[00:04:49]** **SPEAKER_00 (GreatStack):** Let me add the folder name, e-commerce.
**[00:04:58]** **SPEAKER_00 (GreatStack):** Now, open this folder, and within this folder we will create another folder with the name frontend.
**[00:05:10]** **SPEAKER_00 (GreatStack):** Let's open this folder with our code editor, which is Visual Studio Code. Here we will open the terminal, open integrated terminal.
**[00:05:23]** **SPEAKER_00 (GreatStack):** We have to create the React project, so here in this terminal we will add NPX create react app dot. When we are using dot, this command will create the project in this folder, which is frontend.
**[00:05:49]** **SPEAKER_00 (GreatStack):** So, after completing it, you can see our React project has been created. Now we will install the React router dom library. For that we will add NPM install react router dom.
**[00:06:08]** **SPEAKER_00 (GreatStack):** So we have created our project and installed our React dom. Now we will run our project, so here we will add NPM start.
**[00:06:23]** **SPEAKER_00 (GreatStack):** And after that, you can see our React project is running in browser. Now we will clean the default React project.
**[00:06:28]** **SPEAKER_00 (GreatStack):** So just come back to the code editor, click here on SRC, open this app.js and from here we will remove this header tag and remove this import logo.
**[00:06:54]** **SPEAKER_00 (GreatStack):** Now in this public folder, index.html file is there. So, here we will rename our title. So, the title is E-Commerce, save this.
**[00:07:11]** **SPEAKER_00 (GreatStack):** Now you can see the project is clear. Now we can create the folder structure for our e-commerce project.
**[00:07:23]** **SPEAKER_00 (GreatStack):** Within this SRC, we will create one folder with the name components.
**[00:07:35]** **SPEAKER_00 (GreatStack):** And here, let's create another folder with the name context. We will use this context folder for context APIs and we will use this pages folder to create e-commerce pages.
**[00:08:02]** **SPEAKER_00 (GreatStack):** In this assets folder we will store the images, and in this components we will create one navbar component also, so here we'll create a new folder and write the name navbar.
**[00:08:16]** **SPEAKER_00 (GreatStack):** Within this Navbar, we will add navbar.jsx file.
**[00:08:24]** **SPEAKER_00 (GreatStack):** Next, we will convert this JSX file into component using RAFC. So write RAFC and now we will create the CSS file for this navbar.jsx. So here, we will create a new file and write the name navbar.css.
**[00:08:45]** **SPEAKER_00 (GreatStack):** Now, we have to import this CSS file in this navbar.jsx. So just add import and write the directory of the CSS file. Dot Navbar dot CSS.
**[00:09:00]** **SPEAKER_00 (GreatStack):** Next we have to mount this navbar component in app.js file. So, in this one, just remove this class name and in this one, we will mount the navbar. So just write the nav, you can see the Navbar component in this snippet.
**[00:09:14]** **SPEAKER_00 (GreatStack):** So just write the navbar, you can see the navbar component in this snippet, click here.
**[00:09:25]** **SPEAKER_00 (GreatStack):** So it will be automatically imported here. Just close this. Now the Navbar has been mounted in app.js. Now we will create the Navbar. So, in this Navbar we will create the HTML structure of the Navbar. So, within this div, we will add a class name, so let's add the class name Navbar.
**[00:09:49]** **SPEAKER_00 (GreatStack):** Now, we have to add the images. So, in this assets folder, let's right click here and select reveal in file explorer, navigate to

---

### Segment 1 — 10:00:00 - 10:20:00

**[10:00:00]** **SPEAKER_00 (GreatStack):** the images assets. So, select all the images copy and add it in the project assets folder. Paste it here. So, our assets has been inserted here in this assets folder.
**[10:16:00]** **SPEAKER_00 (GreatStack):** Now, we have all the icons, product images and product data also. In all product.js file, we have all the product data.

---

### Segment 1 — 20:00 - 30:00

**[00:20:28]** **SPEAKER_00 (GreatStack):** Just add set menu and when we will click on shop, so our menu should store shop.
**[00:20:33]** **SPEAKER_00 (GreatStack):** So, if the state is shop, then HR will be applied here.
**[00:20:38]** **SPEAKER_00 (GreatStack):** Let me remove it from here and here we will insert the ternary operator.
**[00:20:43]** **SPEAKER_00 (GreatStack):** So first we will check if our menu is shop.
**[00:20:50]** **SPEAKER_00 (GreatStack):** Then we will provide the HR tag.
**[00:20:55]** **SPEAKER_00 (GreatStack):** And if it is not shop, then it will be empty tag.
**[00:21:01]** **SPEAKER_00 (GreatStack):** Now we will use the ternary operator, copy it and add it in the another one.
**[00:21:10]** **SPEAKER_00 (GreatStack):** We will add it in all three LI.
**[00:21:14]** **SPEAKER_00 (GreatStack):** Here we will change it as mens.
**[00:21:17]** **SPEAKER_00 (GreatStack):** If the menu is mens, then here we will add HR.
**[00:21:25]** **SPEAKER_00 (GreatStack):** Then, in the third one we will add womens and in the last one we will add kids.
**[00:21:33]** **SPEAKER_00 (GreatStack):** If the menu is kids, the HR will be provided here.
**[00:21:37]** **SPEAKER_00 (GreatStack):** Save this, and now, if I click on men, you can see underline here.
**[00:21:49]** **SPEAKER_00 (GreatStack):** If I click on kids, this underline is here on this kids.
**[00:21:55]** **SPEAKER_00 (GreatStack):** Now we are going to add the Google fonts for our project.
**[00:22:00]** **SPEAKER_00 (GreatStack):** So come to the Google and search for Poppins font.
**[00:22:06]** **SPEAKER_00 (GreatStack):** Open this one, and here you can select the regular.
**[00:22:15]** **SPEAKER_00 (GreatStack):** Then click here to copy this link.
**[00:22:20]** **SPEAKER_00 (GreatStack):** In your public folder, index.html file, add it here after this link.
**[00:22:28]** **SPEAKER_00 (GreatStack):** Paste the copied URL and save it, then come to index.css file.
**[00:22:36]** **SPEAKER_00 (GreatStack):** Here we will add font family, poppins, save it.
**[00:22:45]** **SPEAKER_00 (GreatStack):** You can see the poppins font has been applied on our project.
**[00:22:53]** **SPEAKER_00 (GreatStack):** Next we will create pages for our e-commerce site.
**[00:23:02]** **SPEAKER_00 (GreatStack):** So, in this pages we will create a new file and write the file name shop.jsx.
**[00:23:13]** **SPEAKER_00 (GreatStack):** Here we will add rafc to convert it into component.
**[00:23:20]** **SPEAKER_00 (GreatStack):** Now we will create login sign up page.
**[00:23:23]** **SPEAKER_00 (GreatStack):** So create a new file and write the file name login signup.jsx.
**[00:23:37]** **SPEAKER_00 (GreatStack):** Here also we will add rafc to convert it into component.
**[00:23:41]** **SPEAKER_00 (GreatStack):** Next we will create another page for the shop category, that is shop category.
**[00:23:51]** **SPEAKER_00 (GreatStack):** Shop category.jsx.
**[00:23:54]** **SPEAKER_00 (GreatStack):** Here also rafc.
**[00:23:58]** **SPEAKER_00 (GreatStack):** Now we will create product page.
**[00:24:01]** **SPEAKER_00 (GreatStack):** Create new file and write the file name product.jsx.
**[00:24:08]** **SPEAKER_00 (GreatStack):** Here also we will add rafc.
**[00:24:12]** **SPEAKER_00 (GreatStack):** Now we will create another page for our cart.
**[00:24:17]** **SPEAKER_00 (GreatStack):** So write the file name cart.jsx.
**[00:24:24]** **SPEAKER_00 (GreatStack):** Here also rafc.
**[00:24:29]** **SPEAKER_00 (GreatStack):** Now we have created five pages, cart, login sign up, product page, shop page and shop category.
**[00:24:38]** **SPEAKER_00 (GreatStack):** Shop page will be our home page and shop category page where we will render the different categories, mens, women and kids.
**[00:24:49]** **SPEAKER_00 (GreatStack):** In the app.js file we will set up our routes.
**[00:24:54]** **SPEAKER_00 (GreatStack):** And we will link that with our navigation bar.
**[00:24:58]** **SPEAKER_00 (GreatStack):** So here, in app.js we will add import.
**[00:25:02]** **SPEAKER_00 (GreatStack):** We will import browser router from react router dom.
**[00:25:11]** **SPEAKER_00 (GreatStack):** Here we will add one more thing which is routes, then comma route.
**[00:25:17]** **SPEAKER_00 (GreatStack):** So we have imported browser router, routes and route from the react router dom.
**[00:25:25]** **SPEAKER_00 (GreatStack):** Now in this div we will add the browser router.
**[00:25:31]** **SPEAKER_00 (GreatStack):** And we have to wrap all the components using this browser router.
**[00:25:38]** **SPEAKER_00 (GreatStack):** So this navbar will be available in all the components.
**[00:25:44]** **SPEAKER_00 (GreatStack):** And after this navbar we will set up our routes.
**[00:25:47]** **SPEAKER_00 (GreatStack):** So here let's add routes.
**[00:25:52]** **SPEAKER_00 (GreatStack):** Within this routes we will add route.
**[00:26:02]** **SPEAKER_00 (GreatStack):** So the first thing is to set a path.
**[00:26:04]** **SPEAKER_00 (GreatStack):** For the home page we will add slash.
**[00:26:07]** **SPEAKER_00 (GreatStack):** Element, and in this element we will insert this shop page.
**[00:26:19]** **SPEAKER_00 (GreatStack):** Here we will add shop.
**[00:26:24]** **SPEAKER_00 (GreatStack):** And close it.
**[00:26:26]** **SPEAKER_00 (GreatStack):** Now, close this route.
**[00:26:30]** **SPEAKER_00 (GreatStack):** So if someone comes to this slash path, then this shop page will be rendered.
**[00:26:38]** **SPEAKER_00 (GreatStack):** Now, similarly we will copy it and change the path.
**[00:26:43]** **SPEAKER_00 (GreatStack):** Here we will add slash mens.
**[00:26:46]** **SPEAKER_00 (GreatStack):** If someone comes to the mens path, so then we will render shop category page.
**[00:26:54]** **SPEAKER_00 (GreatStack):** Again copy and paste and here we will add womens.
**[00:27:01]** **SPEAKER_00 (GreatStack):** Path is slash womens, so again we will use the same thing shop category page.
**[00:27:08]** **SPEAKER_00 (GreatStack):** And if someone comes on slash kids path, then also we will use the shop category page.
**[00:27:17]** **SPEAKER_00 (GreatStack):** Now here we will add some props.
**[00:27:21]** **SPEAKER_00 (GreatStack):** So if someone comes on mens, so here we will add a category.
**[00:27:30]** **SPEAKER_00 (GreatStack):** Equals mens.
**[00:27:34]** **SPEAKER_00 (GreatStack):** Just copy it and paste it in the second one.
**[00:27:38]** **SPEAKER_00 (GreatStack):** This will be woman, this will be men.
**[00:27:42]** **SPEAKER_00 (GreatStack):** And in the last one we will add category is equal to kid.
**[00:27:48]** **SPEAKER_00 (GreatStack):** Now we will set the route for our product.
**[00:27:52]** **SPEAKER_00 (GreatStack):** Here we will add route.
**[00:27:59]** **SPEAKER_00 (GreatStack):** The route path will be product.
**[00:28:07]** **SPEAKER_00 (GreatStack):** And we will use the element product element.
**[00:28:13]** **SPEAKER_00 (GreatStack):** So I am writing product slash closing tag.
**[00:28:21]** **SPEAKER_00 (GreatStack):** Now in this route we will add product ID path, so here let's add route.
**[00:28:43]** **SPEAKER_00 (GreatStack):** For this we will render element product.
**[00:28:50]** **SPEAKER_00 (GreatStack):** Close this.
**[00:28:53]** **SPEAKER_00 (GreatStack):** So we have setup the route for home, mens, womens, kids, product and product ID.
**[00:29:01]** **SPEAKER_00 (GreatStack):** Now we will set the route for our cart.
**[00:29:24]** **SPEAKER_00 (GreatStack):** Now we will set the path for our login page.
**[00:29:42]** **SPEAKER_00 (GreatStack):** Now we have set up our complete route.
**[00:29:45]** **SPEAKER_00 (GreatStack):** Now we will link this route with our navigation bar.
**[00:29:48]** **SPEAKER_00 (GreatStack):** So we will come to the navigation bar.
**[00:29:51]** **SPEAKER_00 (GreatStack):** Now we have to set the navigation menu with route.
**[00:29:56]** **SPEAKER_00 (GreatStack):** So we will use the link tag.

---

### Segment 1 — 00:30:00 - 00:40:00

**[00:30:00]** **SPEAKER_00 (GreatStack):** We will use link from React Router DOM.
**[00:30:07]** **SPEAKER_00 (GreatStack):** close it here, and insert this shop within this link.
**[00:30:14]** **SPEAKER_00 (GreatStack):** And in this link we will add two equal to.
**[00:30:19]** **SPEAKER_00 (GreatStack):** Here we will write the URL directory slash.
**[00:30:25]** **SPEAKER_00 (GreatStack):** So the shop component will be on home page.
**[00:30:29]** **SPEAKER_00 (GreatStack):** And it will be displayed on slash.
**[00:30:43]** **SPEAKER_00 (GreatStack):** Here we will add two then slash means.
**[00:31:04]** **SPEAKER_00 (GreatStack):** Similarly we will add this link tag in kids also.
**[00:31:25]** **SPEAKER_00 (GreatStack):** Now we can add the link tag for this login button.
**[00:31:37]** **SPEAKER_00 (GreatStack):** slash login, and move this button here within this link tag.
**[00:31:47]** **SPEAKER_00 (GreatStack):** Now we will wrap this cart icon.
**[00:31:52]** **SPEAKER_00 (GreatStack):** So write link to equal to slash cart.
**[00:32:07]** **SPEAKER_00 (GreatStack):** Now save it, and if I click on men, you can see the URL slash men.
**[00:32:17]** **SPEAKER_00 (GreatStack):** If I click on women, you can see the URL. We are on slash women.
**[00:32:23]** **SPEAKER_00 (GreatStack):** If I click on login, you can see their URL, it is slash login.
**[00:32:35]** **SPEAKER_00 (GreatStack):** Now, we have one more underline here that is using a link tag property.
**[00:32:42]** **SPEAKER_00 (GreatStack):** So we have to remove it.
**[00:32:48]** **SPEAKER_00 (GreatStack):** Here on this link, we will add style equal to text decoration none.
**[00:33:02]** **SPEAKER_00 (GreatStack):** And now, there is no underline effect on these text.
**[00:33:07]** **SPEAKER_00 (GreatStack):** Now we have to create the hero component for our shop page.
**[00:33:13]** **SPEAKER_00 (GreatStack):** First we will create a new folder within this components, and here we will add a name, hero.
**[00:33:29]** **SPEAKER_00 (GreatStack):** We will convert it into component using rafc.
**[00:33:34]** **SPEAKER_00 (GreatStack):** And we will add the class name for this div. So the class name is hero.
**[00:33:40]** **SPEAKER_00 (GreatStack):** Now we have to create the CSS file for this hero component, so just create a new file in this hero component and write the file name, hero.css.
**[00:33:51]** **SPEAKER_00 (GreatStack):** Next we have to import this CSS file in here.
**[00:33:55]** **SPEAKER_00 (GreatStack):** So we will add import, dot slash, hero.css.
**[00:34:04]** **SPEAKER_00 (GreatStack):** Now we have to mount this hero component in shop page.
**[00:34:12]** **SPEAKER_00 (GreatStack):** So come to pages, shop.jsx.
**[00:34:16]** **SPEAKER_00 (GreatStack):** Here we will add hero. Close it.
**[00:34:20]** **SPEAKER_00 (GreatStack):** Then save these changes. Now the shop page has this hero element.
**[00:34:27]** **SPEAKER_00 (GreatStack):** now we will create the HTML structure for this hero element for this hero component
**[00:34:33]** **SPEAKER_00 (GreatStack):** For this hero component, we have to divide in two part hero left and right.
**[00:34:37]** **SPEAKER_00 (GreatStack):** So we will add the div, dot hero left.
**[00:34:44]** **SPEAKER_00 (GreatStack):** And we will create the another div with the class name hero right.
**[00:34:50]** **SPEAKER_00 (GreatStack):** For the left part, we will add the S2 tag for the header.
**[00:34:56]** **SPEAKER_00 (GreatStack):** So in this S2 tag we will add the text new arrivals only.
**[00:35:03]** **SPEAKER_00 (GreatStack):** Next we will create another div, and within this div we will add another div.
**[00:35:09]** **SPEAKER_00 (GreatStack):** And we will provide one class name that is hero hand icon.
**[00:35:16]** **SPEAKER_00 (GreatStack):** And in this div we will add one paragraph text that is new.
**[00:35:24]** **SPEAKER_00 (GreatStack):** And we will insert one image tag and in this one we will add one image.
**[00:35:31]** **SPEAKER_00 (GreatStack):** So let's add one import tag here to import the image.
**[00:35:36]** **SPEAKER_00 (GreatStack):** Import hand icon from our asset folder, so we will add double dot slash assets.
**[00:35:52]** **SPEAKER_00 (GreatStack):** Then we can simply add hand icon in this IMG tag.
**[00:35:57]** **SPEAKER_00 (GreatStack):** After that here, we have to add one paragraph tag, where we will add collection.
**[00:36:06]** **SPEAKER_00 (GreatStack):** And after that we will add one more paragraph tag and here we will add for everyone, collections for everyone.
**[00:36:17]** **SPEAKER_00 (GreatStack):** Now after this div, we will create the latest collections button.
**[00:36:22]** **SPEAKER_00 (GreatStack):** So we will create one div with the class name hero latest button.
**[00:36:31]** **SPEAKER_00 (GreatStack):** And in this div we will create another div and we will add the text latest collection.
**[00:36:41]** **SPEAKER_00 (GreatStack):** Next we will insert one image tag and here we will add the arrow icon.
**[00:36:49]** **SPEAKER_00 (GreatStack):** So again we have to import the arrow icon, we will add import arrow icon from and asset folder.
**[00:37:02]** **SPEAKER_00 (GreatStack):** And here we will add the arrow icon.
**[00:37:09]** **SPEAKER_00 (GreatStack):** Now we will add the content in the right side.
**[00:37:13]** **SPEAKER_00 (GreatStack):** So in this hero right we will add the IMG tag and here we will add one hero image.
**[00:37:21]** **SPEAKER_00 (GreatStack):** Let's add the text hero image from assets folder.
**[00:37:30]** **SPEAKER_00 (GreatStack):** Hero image dot PNG.
**[00:37:34]** **SPEAKER_00 (GreatStack):** Here we will insert that image, hero image.
**[00:37:39]** **SPEAKER_00 (GreatStack):** Save these changes.
**[00:37:42]** **SPEAKER_00 (GreatStack):** So you can see the hero element is looking like this.
**[00:37:46]** **SPEAKER_00 (GreatStack):** Next we have to apply the CSS properties.
**[00:37:50]** **SPEAKER_00 (GreatStack):** So we will come to the hero dot CSS file.
**[00:37:55]** **SPEAKER_00 (GreatStack):** Here first we will use the class name that is hero.
**[00:38:00]** **SPEAKER_00 (GreatStack):** So for this one, we will add the height, it will be 100 before height.
**[00:38:06]** **SPEAKER_00 (GreatStack):** Then we will add the background, so in this one we have to add a linear gradient color with 180 degree rotation.
**[00:38:13]** **SPEAKER_00 (GreatStack):** Now we will add the display flex.
**[00:38:22]** **SPEAKER_00 (GreatStack):** So you can see the linear gradient color for this hero section.
**[00:38:30]** **SPEAKER_00 (GreatStack):** Next we will add the CSS properties for the hero left.
**[00:38:33]** **SPEAKER_00 (GreatStack):** Write this class name here, and here we will add flex one.
**[00:38:40]** **SPEAKER_00 (GreatStack):** Display will be flex.
**[00:38:45]** **SPEAKER_00 (GreatStack):** Flex direction will be column, and justify content will be center.
**[00:38:54]** **SPEAKER_00 (GreatStack):** Let's add the gap of 20 pixel, then padding of 180 pixel from the left side, and line height of 1.1.
**[00:39:11]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for the S2 tag.
**[00:39:15]** **SPEAKER_00 (GreatStack):** So here we will add dot hero left S2 tag.
**[00:39:20]** **SPEAKER_00 (GreatStack):** And in this one, we have to change the color.
**[00:39:30]** **SPEAKER_00 (GreatStack):** Then we will change the font size, so it will be 26 pixel.
**[00:39:40]** **SPEAKER_00 (GreatStack):** Next we will add the properties for the P tag, so here we will add hero left P tag.
**[00:39:48]** **SPEAKER_00 (GreatStack):** Here we will use the color code.
**[00:39:52]** **SPEAKER_00 (GreatStack):** Then we will add the font size of 100 pixel, font weight of 700.

---

### Segment 6 — 40:00 - 05:00

_No transcript entries for this segment._

---

### Segment 1 — 00:50:00 - 01:00:00

**[00:50:00]** **SPEAKER_00 (GreatStack):** one arrow function.
**[00:50:04]** **SPEAKER_00 (GreatStack):** And we will pass the individual item here.
**[00:50:08]** **SPEAKER_00 (GreatStack):** And in this function, we will return...
**[00:50:11]** **SPEAKER_00 (GreatStack):** we will return the item component.
**[00:50:17]** **SPEAKER_00 (GreatStack):** And we will pass the props.
**[00:50:20]** **SPEAKER_00 (GreatStack):** So first, we will pass the key.
**[00:50:26]** **SPEAKER_00 (GreatStack):** From this parameter we will get the index i and we will provide the i in the key.
**[00:50:33]** **SPEAKER_00 (GreatStack):** Next we will add the ID in the prop, so the ID will be item.ID.
**[00:50:41]** **SPEAKER_00 (GreatStack):** Next we will provide the product name in the props.
**[00:50:47]** **SPEAKER_00 (GreatStack):** So the product name will be item.name.
**[00:50:53]** **SPEAKER_00 (GreatStack):** Next we will pass the image so we will add image is equal to
**[00:50:59]** **SPEAKER_00 (GreatStack):** In this image we will insert item.image.
**[00:51:04]** **SPEAKER_00 (GreatStack):** Now we will pass the prices, so first we will pass the new price.
**[00:51:10]** **SPEAKER_00 (GreatStack):** New price equals item.new_price.
**[00:51:16]** **SPEAKER_00 (GreatStack):** Now we will pass the old price.
**[00:51:28]** **SPEAKER_00 (GreatStack):** Now we have provided all the props.
**[00:51:32]** **SPEAKER_00 (GreatStack):** Now we will mount the popular component in our shop page.
**[00:51:37]** **SPEAKER_00 (GreatStack):** So we have the shop page here and here we will mount the popular component.
**[00:51:47]** **SPEAKER_00 (GreatStack):** Save these changes.
**[00:51:49]** **SPEAKER_00 (GreatStack):** So on this web page, you can see the popular in women and these products.
**[00:51:55]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this product.
**[00:52:00]** **SPEAKER_00 (GreatStack):** So come to the popular.CSS file and here
**[00:52:05]** **SPEAKER_00 (GreatStack):** And here we have to provide the CSS properties for the popular container.
**[00:52:10]** **SPEAKER_00 (GreatStack):** So here we will add display flex.
**[00:52:13]** **SPEAKER_00 (GreatStack):** Flex direction will be column.
**[00:52:18]** **SPEAKER_00 (GreatStack):** Align items center.
**[00:52:21]** **SPEAKER_00 (GreatStack):** Gap of 10 pixel.
**[00:52:25]** **SPEAKER_00 (GreatStack):** Height of 90 view port height.
**[00:52:30]** **SPEAKER_00 (GreatStack):** Now we will add the properties for the H1 tag.
**[00:52:34]** **SPEAKER_00 (GreatStack):** So just add dot popular and H1.
**[00:52:38]** **SPEAKER_00 (GreatStack):** Here we will use color code.
**[00:52:43]** **SPEAKER_00 (GreatStack):** Then font size of 50 pixel.
**[00:52:46]** **SPEAKER_00 (GreatStack):** Font weight of 600.
**[00:52:51]** **SPEAKER_00 (GreatStack):** Save these changes. You can see it is in the center.
**[00:52:57]** **SPEAKER_00 (GreatStack):** Now we will add the properties for this HR tag.
**[00:53:01]** **SPEAKER_00 (GreatStack):** So here we will add dot popular and HR tag.
**[00:53:08]** **SPEAKER_00 (GreatStack):** So we will provide width 200 pixel.
**[00:53:14]** **SPEAKER_00 (GreatStack):** Height of 6 pixel.
**[00:53:18]** **SPEAKER_00 (GreatStack):** Border radius of 10 pixel.
**[00:53:23]** **SPEAKER_00 (GreatStack):** Then background, and add this color code.
**[00:53:28]** **SPEAKER_00 (GreatStack):** Now we will add the properties for the popular item class name.
**[00:53:34]** **SPEAKER_00 (GreatStack):** So here we will add dot popular, item.
**[00:53:39]** **SPEAKER_00 (GreatStack):** In this one, we will add the margin of top 50 pixel.
**[00:53:45]** **SPEAKER_00 (GreatStack):** Display flex.
**[00:53:49]** **SPEAKER_00 (GreatStack):** Gap of 30 pixel.
**[00:53:53]** **SPEAKER_00 (GreatStack):** Now you can see all products side-by-side.
**[00:53:56]** **SPEAKER_00 (GreatStack):** Now we will add the dollar sign in front of these prices.
**[00:53:59]** **SPEAKER_00 (GreatStack):** So come here in item dot JSX, and before this prices, we will add the dollar sign.
**[00:54:06]** **SPEAKER_00 (GreatStack):** Save these changes. You can see the dollar sign here.
**[00:54:11]** **SPEAKER_00 (GreatStack):** Now we will create the offer banner for our shop page.
**[00:54:18]** **SPEAKER_00 (GreatStack):** So first we will create a new folder in this component.
**[00:54:23]** **SPEAKER_00 (GreatStack):** Here we will provide the name offers.
**[00:54:27]** **SPEAKER_00 (GreatStack):** In this folder, we will create new file, which is offers dot JSX.
**[00:54:35]** **SPEAKER_00 (GreatStack):** Then convert it into component using RAFC.
**[00:54:43]** **SPEAKER_00 (GreatStack):** Here we will provide one class name offers.
**[00:54:50]** **SPEAKER_00 (GreatStack):** Now we will create a CSS file for this offers component.
**[00:54:55]** **SPEAKER_00 (GreatStack):** So here we will create a new file with the name offers dot CSS.
**[00:55:00]** **SPEAKER_00 (GreatStack):** Now we have to mount this CSS file in the offer dot JSX file.
**[00:55:06]** **SPEAKER_00 (GreatStack):** Here we will add import, and write the file path.
**[00:55:13]** **SPEAKER_00 (GreatStack):** Now we will mount this component in shop dot JSX file.
**[00:55:18]** **SPEAKER_00 (GreatStack):** So after this popular, we will add offers.
**[00:55:24]** **SPEAKER_00 (GreatStack):** Now we will design the HTML structure for the offers component.
**[00:55:30]** **SPEAKER_00 (GreatStack):** So here we will create two div, offers left and offers right.
**[00:55:44]** **SPEAKER_00 (GreatStack):** In the offers left, we will add h1 tag.
**[00:55:53]** **SPEAKER_00 (GreatStack):** So the text is exclusive.
**[00:55:57]** **SPEAKER_00 (GreatStack):** We will add one more H1 tag and we will add the text offers for you.
**[00:56:03]** **SPEAKER_00 (GreatStack):** Now we will insert a p tag, and in this one we will add...
**[00:56:07]** **SPEAKER_00 (GreatStack):** only on best sellers product.
**[00:56:15]** **SPEAKER_00 (GreatStack):** Now we will add a button tag.
**[00:56:22]** **SPEAKER_00 (GreatStack):** And in the right div, we will add one image tag.
**[00:56:29]** **SPEAKER_00 (GreatStack):** Here we will add one exclusive image. So first, we have to import that image.
**[00:56:37]** **SPEAKER_00 (GreatStack):** So just add import.
**[00:56:46]** **SPEAKER_00 (GreatStack):** From our asset folder slash exclusive image.png.
**[00:56:55]** **SPEAKER_00 (GreatStack):** Here we will insert exclusive image.
**[00:56:58]** **SPEAKER_00 (GreatStack):** Save these changes.
**[00:57:00]** **SPEAKER_00 (GreatStack):** Here you can see the text and image.
**[00:57:04]** **SPEAKER_00 (GreatStack):** Now we have to add the CSS properties for this image and text.
**[00:57:08]** **SPEAKER_00 (GreatStack):** So come here in offers dot CSS file, and first we will add the properties for the offers container.
**[00:57:21]** **SPEAKER_00 (GreatStack):** Here we will provide the width of 65%.
**[00:57:25]** **SPEAKER_00 (GreatStack):** Then height of 60 viewport height.
**[00:57:30]** **SPEAKER_00 (GreatStack):** Display will be flex and margin auto.
**[00:57:36]** **SPEAKER_00 (GreatStack):** Now we will provide the padding of zero pixel and 140 pixel.
**[00:57:44]** **SPEAKER_00 (GreatStack):** Then some space from the bottom, so margin bottom of 150 pixel, and background.
**[00:57:56]** **SPEAKER_00 (GreatStack):** Save these changes.
**[00:57:58]** **SPEAKER_00 (GreatStack):** You can see some changes.
**[00:58:01]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for the left part.
**[00:58:05]** **SPEAKER_00 (GreatStack):** So here we will add dot offers, left.
**[00:58:11]** **SPEAKER_00 (GreatStack):** Here we will add the flex one.
**[00:58:14]** **SPEAKER_00 (GreatStack):** Display flex.
**[00:58:20]** **SPEAKER_00 (GreatStack):** Flex direction column.
**[00:58:24]** **SPEAKER_00 (GreatStack):** Justify content center.
**[00:58:30]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties to the H1 tag.
**[00:58:36]** **SPEAKER_00 (GreatStack):** Here we will use the color code.
**[00:58:41]** **SPEAKER_00 (GreatStack):** Font size of 80 pixel.
**[00:58:45]** **SPEAKER_00 (GreatStack):** Font weight of 600.
**[00:58:53]** **SPEAKER_00 (GreatStack):** Now we will add the properties to the paragraph tag.
**[00:58:58]** **SPEAKER_00 (GreatStack):** So here we will add the color code.
**[00:59:02]** **SPEAKER_00 (GreatStack):** Font size of 22 pixel.
**[00:59:06]** **SPEAKER_00 (GreatStack):** And font weight of 600.
**[00:59:12]** **SPEAKER_00 (GreatStack):** Now we will add the style for the offer button.
**[00:59:15]** **SPEAKER_00 (GreatStack):** So just add dot offer left space, button tag.
**[00:59:22]** **SPEAKER_00 (GreatStack):** Here we will add the width 282 pixels.
**[00:59:29]** **SPEAKER_00 (GreatStack):** Height of 70 pixel.
**[00:59:33]** **SPEAKER_00 (GreatStack):** Border radius of 35 pixels.
**[00:59:39]** **SPEAKER_00 (GreatStack):** Background color.
**[00:59:44]** **SPEAKER_00 (GreatStack):** Border none.
**[00:59:49]** **SPEAKER_00 (GreatStack):** Then color white, that will be the button text color.
**[00:59:53]** **SPEAKER_00 (GreatStack):** And increase the font size, so the font size will be 22 pixel.
**[00:59:58]** **SPEAKER_00 (GreatStack):** Then we will add the font weight of 500.

---

### Segment 1 — 60:00:00 - 01:10:00

**[01:00:00]** **SPEAKER_00 (GreatStack):** and a space from the top so margin top of 30 pixel
**[01:00:00]** **SPEAKER_00 (GreatStack):** Then add cursor pointer
**[01:00:00]** **SPEAKER_00 (GreatStack):** Now, we will add the CSS properties for the right div
**[01:00:00]** **SPEAKER_00 (GreatStack):** So, just add the class name offers right
**[01:00:00]** **SPEAKER_00 (GreatStack):** Here, we will add flex one
**[01:00:00]** **SPEAKER_00 (GreatStack):** Display flex
**[01:00:00]** **SPEAKER_00 (GreatStack):** Align items center
**[01:00:00]** **SPEAKER_00 (GreatStack):** Justify content flex end
**[01:00:00]** **SPEAKER_00 (GreatStack):** Padding top will be 50 pixel
**[01:00:00]** **SPEAKER_00 (GreatStack):** Save these changes
**[01:00:00]** **SPEAKER_00 (GreatStack):** Now, our exclusive offer banner is ready
**[01:00:00]** **SPEAKER_00 (GreatStack):** Now, we will create a new collections component, where our newly added products will be displayed
**[01:00:00]** **SPEAKER_00 (GreatStack):** So first, we will create a new folder in this components
**[01:00:01]** **SPEAKER_00 (GreatStack):** Here, we will add the name new collections
**[01:00:01]** **SPEAKER_00 (GreatStack):** Within this new collections folder, we will create a file new collections.jsx
**[01:00:01]** **SPEAKER_00 (GreatStack):** Here we will use RFC
**[01:00:01]** **SPEAKER_00 (GreatStack):** Here we will provide one class name
**[01:00:01]** **SPEAKER_00 (GreatStack):** Now, we will create the CSS file for this new collections component
**[01:00:01]** **SPEAKER_00 (GreatStack):** Create a new file
**[01:00:01]** **SPEAKER_00 (GreatStack):** Now we will import the CSS file in this newcollections.jsx file
**[01:00:01]** **SPEAKER_00 (GreatStack):** Import .slash new collections.css
**[01:00:01]** **SPEAKER_00 (GreatStack):** Now we will create the HTML structure for our new collections component
**[01:00:01]** **SPEAKER_00 (GreatStack):** Here we will use H1 tag
**[01:00:01]** **SPEAKER_00 (GreatStack):** Here we will add the new collections
**[01:00:02]** **SPEAKER_00 (GreatStack):** Next, we will insert the HR tag
**[01:00:02]** **SPEAKER_00 (GreatStack):** Then, we will create one div with the class name collections
**[01:00:02]** **SPEAKER_00 (GreatStack):** We will map the new collections data within this div using item component
**[01:00:02]** **SPEAKER_00 (GreatStack):** So first we will import
**[01:00:02]** **SPEAKER_00 (GreatStack):** new collections from .slash assets folder slash new collections
**[01:00:02]** **SPEAKER_00 (GreatStack):** Here we will map new collection .map
**[01:00:02]** **SPEAKER_00 (GreatStack):** Here we will pass the arrow function
**[01:00:02]** **SPEAKER_00 (GreatStack):** Here we will pass the item and index
**[01:00:03]** **SPEAKER_00 (GreatStack):** Then we will return our item component
**[01:00:03]** **SPEAKER_00 (GreatStack):** And here also we will pass the same parameters that we have added in the popular.jsx
**[01:00:03]** **SPEAKER_00 (GreatStack):** So we will copy it from here, copy these props
**[01:00:03]** **SPEAKER_00 (GreatStack):** And add it here in this new collections item
**[01:00:03]** **SPEAKER_00 (GreatStack):** Now we will mount this component in shop page
**[01:00:03]** **SPEAKER_00 (GreatStack):** So, come here shop.jsx and after this offers we will mount new collections
**[01:00:03]** **SPEAKER_00 (GreatStack):** Now, we have new collections
**[01:00:03]** **SPEAKER_00 (GreatStack):** Now, we have to add the CSS properties
**[01:00:03]** **SPEAKER_00 (GreatStack):** So here also we will add the CSS that we have added in popular.css
**[01:00:04]** **SPEAKER_00 (GreatStack):** So just copy it from here, and come to the newcollections.css, paste it here
**[01:00:04]** **SPEAKER_00 (GreatStack):** We will replace the class name popular with the new collections
**[01:00:04]** **SPEAKER_00 (GreatStack):** Then replace all
**[01:00:04]** **SPEAKER_00 (GreatStack):** Now, remove this CSS property
**[01:00:04]** **SPEAKER_00 (GreatStack):** And here we will add .collections
**[01:00:04]** **SPEAKER_00 (GreatStack):** Here we will provide display grid
**[01:00:04]** **SPEAKER_00 (GreatStack):** Grid template column
**[01:00:04]** **SPEAKER_00 (GreatStack):** Then we will add the margin of 50 pixel from the top
**[01:00:05]** **SPEAKER_00 (GreatStack):** Gap of 30 pixel
**[01:00:05]** **SPEAKER_00 (GreatStack):** Save these changes
**[01:00:05]** **SPEAKER_00 (GreatStack):** Now our new collections component is ready
**[01:00:05]** **SPEAKER_00 (GreatStack):** Now we will create the newsletter subscription box
**[01:00:05]** **SPEAKER_00 (GreatStack):** So here we will create a new folder in the components folder
**[01:00:05]** **SPEAKER_00 (GreatStack):** Within this folder, we will create one file with the name newsletter.jsx
**[01:00:05]** **SPEAKER_00 (GreatStack):** Here we will use RFC
**[01:00:05]** **SPEAKER_00 (GreatStack):** And we will add the class name for this div
**[01:00:05]** **SPEAKER_00 (GreatStack):** So the class name is newsletter
**[01:00:05]** **SPEAKER_00 (GreatStack):** Now we will create a CSS file for this newsletter component
**[01:00:05]** **SPEAKER_00 (GreatStack):** So create a new file
**[01:00:06]** **SPEAKER_00 (GreatStack):** Now we will import this CSS file in our JSX file
**[01:00:06]** **SPEAKER_00 (GreatStack):** So here we will add import
**[01:00:06]** **SPEAKER_00 (GreatStack):** .slash newsletter.css
**[01:00:06]** **SPEAKER_00 (GreatStack):** Now we will create the HTML structure for the newsletter component
**[01:00:06]** **SPEAKER_00 (GreatStack):** So here, first we will insert the H1 tag
**[01:00:06]** **SPEAKER_00 (GreatStack):** Within this H1 tag, we will add the text that is, get exclusive offers on your email
**[01:00:06]** **SPEAKER_00 (GreatStack):** Now we will insert a paragraph tag
**[01:00:06]** **SPEAKER_00 (GreatStack):** Where we will add subscribe to our newsletter and stay updated
**[01:00:07]** **SPEAKER_00 (GreatStack):** Now we will create one div
**[01:00:07]** **SPEAKER_00 (GreatStack):** And in this div, we will insert one input tag
**[01:00:07]** **SPEAKER_00 (GreatStack):** Type will be email
**[01:00:07]** **SPEAKER_00 (GreatStack):** Your email ID
**[01:00:07]** **SPEAKER_00 (GreatStack):** Then we will use a button
**[01:00:07]** **SPEAKER_00 (GreatStack):** Within this button tag, we will add the button text subscribe
**[01:00:07]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this newsletter component
**[01:00:07]** **SPEAKER_00 (GreatStack):** So write this class name here, newsletter
**[01:00:07]** **SPEAKER_00 (GreatStack):** Here we will add the width of 65 percent
**[01:00:07]** **SPEAKER_00 (GreatStack):** Height will be 40 viewport height
**[01:00:08]** **SPEAKER_00 (GreatStack):** Display flex
**[01:00:08]** **SPEAKER_00 (GreatStack):** Flex direction will be column
**[01:00:08]** **SPEAKER_00 (GreatStack):** Align items center, justify content center
**[01:00:08]** **SPEAKER_00 (GreatStack):** Margin auto
**[01:00:08]** **SPEAKER_00 (GreatStack):** Padding zero pixel and 140 pixels
**[01:00:08]** **SPEAKER_00 (GreatStack):** Margin bottom 150 pixel
**[01:00:08]** **SPEAKER_00 (GreatStack):** Then background, and in the background we will add the linear gradient color
**[01:00:08]** **SPEAKER_00 (GreatStack):** Then we will add the gap of 30 pixel
**[01:00:08]** **SPEAKER_00 (GreatStack):** Now we will add the properties for the H1 tag
**[01:00:08]** **SPEAKER_00 (GreatStack):** So here we will add newsletter H1
**[01:00:08]** **SPEAKER_00 (GreatStack):** We will change the color
**[01:00:08]** **SPEAKER_00 (GreatStack):** Then we will increase the font size
**[01:00:09]** **SPEAKER_00 (GreatStack):** Then change the font weight
**[01:00:09]** **SPEAKER_00 (GreatStack):** Next we will add the properties for the P tag
**[01:00:09]** **SPEAKER_00 (GreatStack):** So here we will add newsletter P tag
**[01:00:09]** **SPEAKER_00 (GreatStack):** Here we will provide the color
**[01:00:09]** **SPEAKER_00 (GreatStack):** Then change the font size, it will be 20 pixel
**[01:00:09]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for the div, that is in the newsletter component
**[01:00:09]** **SPEAKER_00 (GreatStack):** So here we will add newsletter div
**[01:00:09]** **SPEAKER_00 (GreatStack):** Here we will add display flex
**[01:00:09]** **SPEAKER_00 (GreatStack):** Align items center
**[01:00:09]** **SPEAKER_00 (GreatStack):** Justify content will be space between
**[01:00:09]** **SPEAKER_00 (GreatStack):** Background will be white
**[01:00:09]** **SPEAKER_00 (GreatStack):** Width and height

---

### Segment 1 — 01:10:00 - 01:20:00

**[01:10:00]** **SPEAKER_00 (GreatStack):** The border radius will be 80 pixels.
**[01:10:08]** **SPEAKER_00 (GreatStack):** border of 1 pixel solid and one color code.
**[01:10:18]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this input tag.
**[01:10:23]** **SPEAKER_00 (GreatStack):** Here we will add .newsletter input.
**[01:10:31]** **SPEAKER_00 (GreatStack):** For this input we will provide the width of 500 pixels and margin from the left side that will be 30 pixel.
**[01:10:40]** **SPEAKER_00 (GreatStack):** Then border none, outline none.
**[01:10:46]** **SPEAKER_00 (GreatStack):** Color code.
**[01:10:51]** **SPEAKER_00 (GreatStack):** Then we will add the font family and font size of 16 pixels.
**[01:11:02]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this button.
**[01:11:09]** **SPEAKER_00 (GreatStack):** So here we will add .newsletter and div, then button tag.
**[01:11:19]** **SPEAKER_00 (GreatStack):** Here we will provide the width 210 pixel, height of 70 pixels.
**[01:11:29]** **SPEAKER_00 (GreatStack):** Border radius of 80 pixels.
**[01:11:34]** **SPEAKER_00 (GreatStack):** Background will be black and color white, that is the button text color.
**[01:11:41]** **SPEAKER_00 (GreatStack):** Then we will change the font size 16 pixel and cursor pointer.
**[01:11:48]** **SPEAKER_00 (GreatStack):** Save the changes.
**[01:11:51]** **SPEAKER_00 (GreatStack):** Now we will mount this newsletter component in shop page.
**[01:11:55]** **SPEAKER_00 (GreatStack):** So here, after this new collections we will add newsletter.
**[01:12:05]** **SPEAKER_00 (GreatStack):** Now we will come here in new collections dot CSS file and remove this height and here we will add margin bottom 100 pixels.
**[01:12:19]** **SPEAKER_00 (GreatStack):** Save the changes.
**[01:12:22]** **SPEAKER_00 (GreatStack):** Now, you can see the newsletter subscription box on this web page.
**[01:12:27]** **SPEAKER_00 (GreatStack):** Now, we will create the footer for our website.
**[01:12:33]** **SPEAKER_00 (GreatStack):** Now we will create a new folder within this component with the name footer.
**[01:12:40]** **SPEAKER_00 (GreatStack):** Within this footer folder we will create a new file with the footer dot JSX.
**[01:12:48]** **SPEAKER_00 (GreatStack):** Here we will use rafc.
**[01:12:51]** **SPEAKER_00 (GreatStack):** Here we will add a class name footer.
**[01:12:57]** **SPEAKER_00 (GreatStack):** Now we will create a CSS file for this footer component.
**[01:13:02]** **SPEAKER_00 (GreatStack):** So within this footer folder we will create a new file with the name footer dot CSS.
**[01:13:08]** **SPEAKER_00 (GreatStack):** Now import this CSS file in this footer dot JSX file.
**[01:13:14]** **SPEAKER_00 (GreatStack):** So write import dot slash footer dot CSS.
**[01:13:24]** **SPEAKER_00 (GreatStack):** Now we will create the HTML structure for this footer. So first we will create one div with the class name footer logo.
**[01:13:38]** **SPEAKER_00 (GreatStack):** In this div we will insert image tag.
**[01:13:41]** **SPEAKER_00 (GreatStack):** In this image tag we will add the footer logo, so first we will import that footer logo.
**[01:13:48]** **SPEAKER_00 (GreatStack):** So write import footer_logo from assets folder, logo_big.png.
**[01:14:03]** **SPEAKER_00 (GreatStack):** In this SRC we will add footer logo.
**[01:14:06]** **SPEAKER_00 (GreatStack):** Now we will create a P tag and here we will add the text that will be the name of our shop, that is Shopper.
**[01:14:17]** **SPEAKER_00 (GreatStack):** Now we will create a list. So here we will create a UL with the class name footer links.
**[01:14:31]** **SPEAKER_00 (GreatStack):** Within this UL, we will use LI tags.
**[01:14:37]** **SPEAKER_00 (GreatStack):** We have added five LI tags.
**[01:14:43]** **SPEAKER_00 (GreatStack):** In the first one we will add the text company, then second one is products.
**[01:14:55]** **SPEAKER_00 (GreatStack):** Then third one is Offices.
**[01:15:01]** **SPEAKER_00 (GreatStack):** Then fourth one is about, and the fifth one is contact.
**[01:15:10]** **SPEAKER_00 (GreatStack):** After this UL we will create one div with the class name, footer social icons.
**[01:15:21]** **SPEAKER_00 (GreatStack):** In this one we will create one div with the class name, footer icons container.
**[01:15:31]** **SPEAKER_00 (GreatStack):** In this container we will insert the image tag and here we will provide the Instagram icon.
**[01:15:38]** **SPEAKER_00 (GreatStack):** So first we will import that icon, so here we will add import Instagram underscore icon from our assets folder slash Instagram icon dot PNG.
**[01:15:55]** **SPEAKER_00 (GreatStack):** Next we will import the another icon.
**[01:16:01]** **SPEAKER_00 (GreatStack):** So here we will add import pinterst underscore icon from assets slash pinterst icon dot PNG.
**[01:16:17]** **SPEAKER_00 (GreatStack):** Next we will import the WhatsApp icon.
**[01:16:21]** **SPEAKER_00 (GreatStack):** So here we will add import whatsapp_icon from ./assets/whatsapp_icon.png.
**[01:16:26]** **SPEAKER_00 (GreatStack):** Now we will use these icons here.
**[01:16:28]** **SPEAKER_00 (GreatStack):** Here we will insert the Instagram icon.
**[01:16:32]** **SPEAKER_00 (GreatStack):** Now we will make the copy of this complete div.
**[01:16:41]** **SPEAKER_00 (GreatStack):** And here we will replace the icon.
**[01:16:44]** **SPEAKER_00 (GreatStack):** This will be pinterst icon.
**[01:16:49]** **SPEAKER_00 (GreatStack):** And the last one is WhatsApp icon.
**[01:16:56]** **SPEAKER_00 (GreatStack):** After this we will create one div with the class name footer-copyright.
**[01:17:13]** **SPEAKER_00 (GreatStack):** In this div we will insert one HR tag, then we will add one paragraph tag and in this paragraph tag we will add our text.
**[01:17:27]** **SPEAKER_00 (GreatStack):** Copyright at 2023 all right reserved.
**[01:17:40]** **SPEAKER_00 (GreatStack):** Our footer is ready, now we will add the CSS properties for the footer component.
**[01:17:47]** **SPEAKER_00 (GreatStack):** First we will add the properties for the footer class name.
**[01:17:53]** **SPEAKER_00 (GreatStack):** So we will add display flex.
**[01:17:58]** **SPEAKER_00 (GreatStack):** Flex direction column.
**[01:18:03]** **SPEAKER_00 (GreatStack):** Justify content center.
**[01:18:08]** **SPEAKER_00 (GreatStack):** Align items center.
**[01:18:13]** **SPEAKER_00 (GreatStack):** Then gap of 50 pixels.
**[01:18:18]** **SPEAKER_00 (GreatStack):** Next we will add the CSS properties for the footer logo.
**[01:18:24]** **SPEAKER_00 (GreatStack):** Here we will add display flex.
**[01:18:28]** **SPEAKER_00 (GreatStack):** Align items center.
**[01:18:33]** **SPEAKER_00 (GreatStack):** Then gap of 20 pixels.
**[01:18:41]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for our paragraph tag.
**[01:18:44]** **SPEAKER_00 (GreatStack):** Here we will change the color.
**[01:18:52]** **SPEAKER_00 (GreatStack):** Then increase the font size, it will be 46 pixels.
**[01:18:57]** **SPEAKER_00 (GreatStack):** Then change the font weight, it will be 700.
**[01:19:03]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for the footer links.
**[01:19:08]** **SPEAKER_00 (GreatStack):** For this footer links we will add display flex.
**[01:19:14]** **SPEAKER_00 (GreatStack):** List style none.
**[01:19:19]** **SPEAKER_00 (GreatStack):** Gap of 50 pixels.
**[01:19:23]** **SPEAKER_00 (GreatStack):** Then color and font size of 20 pixels.
**[01:19:32]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for the list items.
**[01:19:37]** **SPEAKER_00 (GreatStack):** So here we will add footer links LI.
**[01:19:42]** **SPEAKER_00 (GreatStack):** In this one we will add cursor pointer.
**[01:19:48]** **SPEAKER_00 (GreatStack):** Now we will add the CSS style for the footer social icon.
**[01:19:54]** **SPEAKER_00 (GreatStack):** So write this class name here.
**[01:19:57]** **SPEAKER_00 (GreatStack):** Here we will add display flex.

---

### Segment 1 — 01:20:00 - 01:30:00

**[01:20:00]** **SPEAKER_00 (GreatStack):** gap of 20 pixel
**[01:20:07]** **SPEAKER_00 (GreatStack):** Now we will add the properties for the footer icons container.
**[01:20:14]** **SPEAKER_00 (GreatStack):** So here we will add the padding of 10 pixels.
**[01:20:20]** **SPEAKER_00 (GreatStack):** padding bottom of 6 pixels
**[01:20:24]** **SPEAKER_00 (GreatStack):** then background this color code
**[01:20:30]** **SPEAKER_00 (GreatStack):** then border of 1 pixel solid and 1 color code.
**[01:20:40]** **SPEAKER_00 (GreatStack):** Now we will add the properties for the footer copyright.
**[01:20:50]** **SPEAKER_00 (GreatStack):** display flex
**[01:20:54]** **SPEAKER_00 (GreatStack):** flex direction column
**[01:20:59]** **SPEAKER_00 (GreatStack):** align items center
**[01:21:03]** **SPEAKER_00 (GreatStack):** gap of 30 pixels
**[01:21:07]** **SPEAKER_00 (GreatStack):** width of 100 percent
**[01:21:13]** **SPEAKER_00 (GreatStack):** then margin bottom 30 pixels
**[01:21:18]** **SPEAKER_00 (GreatStack):** then color
**[01:21:24]** **SPEAKER_00 (GreatStack):** then change the font size
**[01:21:28]** **SPEAKER_00 (GreatStack):** Now we will add the properties for this HR tag
**[01:21:36]** **SPEAKER_00 (GreatStack):** Here we will add dot footer copyright HR
**[01:21:43]** **SPEAKER_00 (GreatStack):** Here we will add width of 80 percent
**[01:21:49]** **SPEAKER_00 (GreatStack):** border none
**[01:21:54]** **SPEAKER_00 (GreatStack):** border radius 10 pixels
**[01:22:00]** **SPEAKER_00 (GreatStack):** height of 3 pixels
**[01:22:03]** **SPEAKER_00 (GreatStack):** background this color code
**[01:22:08]** **SPEAKER_00 (GreatStack):** Now save the changes
**[01:22:12]** **SPEAKER_00 (GreatStack):** Now we will mount this footer component in app.js
**[01:22:16]** **SPEAKER_00 (GreatStack):** So here we will mount the footer component
**[01:22:22]** **SPEAKER_00 (GreatStack):** Save the changes.
**[01:22:25]** **SPEAKER_00 (GreatStack):** Now, you can see this footer on our webpage.
**[01:22:31]** **SPEAKER_00 (GreatStack):** Now if I come to the mens page here also you can see this footer component
**[01:22:38]** **SPEAKER_00 (GreatStack):** because we have added this footer in app.js
**[01:22:42]** **SPEAKER_00 (GreatStack):** So finally we have created our homepage which is our shop page for our e-commerce website.
**[01:22:50]** **SPEAKER_00 (GreatStack):** Now we will create the shop categories page where we can filter the mens, womens and kids products.
**[01:23:00]** **SPEAKER_00 (GreatStack):** So first we will create one context using context API.
**[01:23:05]** **SPEAKER_00 (GreatStack):** So in this context folder we will create a new file
**[01:23:12]** **SPEAKER_00 (GreatStack):** shopcontext.jsx
**[01:23:17]** **SPEAKER_00 (GreatStack):** Here we will import the React.
**[01:23:24]** **SPEAKER_00 (GreatStack):** Then we will export const shopcontext equals create context null.
**[01:23:44]** **SPEAKER_00 (GreatStack):** So we have created one context and initialized with null.
**[01:23:48]** **SPEAKER_00 (GreatStack):** And this context is saved in shopcontext that we are exporting.
**[01:23:56]** **SPEAKER_00 (GreatStack):** Now we will create shop context provider.
**[01:24:02]** **SPEAKER_00 (GreatStack):** So here we will write const shop context provider equals one arrow function
**[01:24:16]** **SPEAKER_00 (GreatStack):** Here we will pass the props and within this function we will create a variable with the name context value equal to Here we will insert any data and functions that will be provided in the shop context provider as a value.
**[01:24:40]** **SPEAKER_00 (GreatStack):** Using that we can access these functions and values in any component.
**[01:24:47]** **SPEAKER_00 (GreatStack):** So here we will insert one data. We will use the all products data.
**[01:24:54]** **SPEAKER_00 (GreatStack):** Where we have the 36 products where we have ID category name image new price and old price.
**[01:25:01]** **SPEAKER_00 (GreatStack):** So we will import this file in this context file.
**[01:25:05]** **SPEAKER_00 (GreatStack):** So here we will add import all product
**[01:25:11]** **SPEAKER_00 (GreatStack):** All product has been imported.
**[01:25:16]** **SPEAKER_00 (GreatStack):** Now this product data will be passed in this context value.
**[01:25:21]** **SPEAKER_00 (GreatStack):** So here we will add all product.
**[01:25:26]** **SPEAKER_00 (GreatStack):** Now we will return this shop context value through shop context provider.
**[01:25:31]** **SPEAKER_00 (GreatStack):** So here we will add return shop context dot provider value equals
**[01:25:46]** **SPEAKER_00 (GreatStack):** And we will provide the value context value
**[01:25:54]** **SPEAKER_00 (GreatStack):** Within this we will pass the props dot children
**[01:26:01]** **SPEAKER_00 (GreatStack):** And here we will export it
**[01:26:13]** **SPEAKER_00 (GreatStack):** So first we have created shop context using create context.
**[01:26:49]** **SPEAKER_00 (GreatStack):** From here we are getting all products data and using context we will use it in different component.
**[01:26:58]** **SPEAKER_00 (GreatStack):** Now we will come to index.js file
**[01:27:01]** **SPEAKER_00 (GreatStack):** Wrap this app component inside this shop context provider.
**[01:27:07]** **SPEAKER_00 (GreatStack):** Using this we can provide the shop context data to all pages.
**[01:27:13]** **SPEAKER_00 (GreatStack):** Now we will create the shop category page
**[01:27:17]** **SPEAKER_00 (GreatStack):** So here we will add the class name shop category
**[01:27:24]** **SPEAKER_00 (GreatStack):** And we will create a CSS file for this shop category page.
**[01:27:30]** **SPEAKER_00 (GreatStack):** So in this pages folder we will create a new folder CSS
**[01:27:34]** **SPEAKER_00 (GreatStack):** Within this folder we will create new file
**[01:27:39]** **SPEAKER_00 (GreatStack):** shopcategory.css
**[01:27:46]** **SPEAKER_00 (GreatStack):** Now we have to import this CSS file in this shop category page.
**[01:27:50]** **SPEAKER_00 (GreatStack):** Here we will add import
**[01:28:06]** **SPEAKER_00 (GreatStack):** Here we will insert the all products data using context.
**[01:28:11]** **SPEAKER_00 (GreatStack):** So here we will write const
**[01:28:21]** **SPEAKER_00 (GreatStack):** equals use context
**[01:28:26]** **SPEAKER_00 (GreatStack):** Within this use context we will write shop context.
**[01:28:31]** **SPEAKER_00 (GreatStack):** And here we will add props.
**[01:28:36]** **SPEAKER_00 (GreatStack):** app.js
**[01:28:39]** **SPEAKER_00 (GreatStack):** And here we have passed the props category men, category women, category kid.
**[01:28:46]** **SPEAKER_00 (GreatStack):** Now we will use this props to filter our product.
**[01:28:51]** **SPEAKER_00 (GreatStack):** So come to shop category page and here we will add the HTML structure.
**[01:28:59]** **SPEAKER_00 (GreatStack):** But before that we will come to app.js and here we will import our banners.
**[01:29:09]** **SPEAKER_00 (GreatStack):** men banner
**[01:29:13]** **SPEAKER_00 (GreatStack):** from components folder assets folder
**[01:29:21]** **SPEAKER_00 (GreatStack):** banner mens.
**[01:29:24]** **SPEAKER_00 (GreatStack):** Then import
**[01:29:27]** **SPEAKER_00 (GreatStack):** women banner
**[01:29:31]** **SPEAKER_00 (GreatStack):** from and give the path
**[01:29:35]** **SPEAKER_00 (GreatStack):** components assets
**[01:29:40]** **SPEAKER_00 (GreatStack):** banner women.png.
**[01:29:42]** **SPEAKER_00 (GreatStack):** Now we will import the kids banner
**[01:29:48]** **SPEAKER_00 (GreatStack):** from
**[01:29:53]** **SPEAKER_00 (GreatStack):** components folder then assets folder

---

### Segment 1 — 90:00 - 91:30

**[01:30:00]** **SPEAKER_00 (GreatStack):** The class name will be shop category index sort.
**[01:30:02]** **SPEAKER_00 (GreatStack):** Now we will
**[01:30:04]** **SPEAKER_00 (GreatStack):** pass these banners through props.
**[01:30:07]** **SPEAKER_00 (GreatStack):** If someone comes in men's path, we will pass
**[01:30:17]** **SPEAKER_00 (GreatStack):** men banner.
**[01:30:19]** **SPEAKER_00 (GreatStack):** When someone comes on women's path, then we will pass banner equals women banner.
**[01:30:35]** **SPEAKER_00 (GreatStack):** Save these changes.
**[01:30:40]** **SPEAKER_00 (GreatStack):** Now we will come to the shop category page.
**[01:30:44]** **SPEAKER_00 (GreatStack):** Here we will create HTML structure for this shop category page.
**[01:30:50]** **SPEAKER_00 (GreatStack):** Here we will display the banner, so here we will insert one image tag and in this image SRC we will add the image.
**[01:31:01]** **SPEAKER_00 (GreatStack):** Now for the page index, we will use the paragraph tag.
**[01:31:07]** **SPEAKER_00 (GreatStack):** So if I come to the men page, you can see this banner.
**[01:31:15]** **SPEAKER_00 (GreatStack):** When we come to women, we have the women page banner, when we come on kid, we have the banner for the kid category.
**[01:31:24]** **SPEAKER_00 (GreatStack):** Now we will create a div and the class name will be shop category index sort.

---

### Segment 12 — 01:40:00 - 01:50:00

**[01:40:00]** **SPEAKER_00 (GreatStack):** Now we will add the name and ID.
**[01:40:47]** **SPEAKER_00 (GreatStack):** Then we will add one paragraph tag and here we will add the text.
**[01:41:51]** **SPEAKER_00 (GreatStack):** By continuing, I agree to the terms of use and privacy policy.
**[01:41:58]** **SPEAKER_00 (GreatStack):** Now, save the file and you can see these elements on our web page.
**[01:42:04]** **SPEAKER_00 (GreatStack):** Now, we will add the CSS properties for these components.
**[01:42:08]** **SPEAKER_00 (GreatStack):** So, in this CSS file we will create a new file: login signup dot CSS.
**[01:42:15]** **SPEAKER_00 (GreatStack):** Now, we will import this CSS file in our page.
**[01:42:20]** **SPEAKER_00 (GreatStack):** So, here we will add import. /CSS folder /Loginsignup.css.
**[01:42:31]** **SPEAKER_00 (GreatStack):** First, we will add the CSS properties to login signup class name.
**[01:42:39]** **SPEAKER_00 (GreatStack):** In this one, we will add: width of 100%, height 80 VH, background - this color code, padding from the top 100 pixel.
**[01:42:53]** **SPEAKER_00 (GreatStack):** Next, we will add the CSS properties to login signup container.
**[01:43:02]** **SPEAKER_00 (GreatStack):** Here, we will add width, height, and background, margin: auto, and padding of 40 pixel, 60 pixel.
**[01:43:16]** **SPEAKER_00 (GreatStack):** Next, we will add the CSS properties for this H1 tag.
**[01:43:22]** **SPEAKER_00 (GreatStack):** Here, we will add. Loginsignup-container H1 tag.
**[01:43:28]** **SPEAKER_00 (GreatStack):** Here we will provide the margin of 20 pixel and 0 pixel.
**[01:43:35]** **SPEAKER_00 (GreatStack):** Next, we will add the CSS properties to: login signup fields class name.
**[01:43:47]** **SPEAKER_00 (GreatStack):** Here, we will provide display flex, flex-direction column, gap of 30 pixels, margin top 30 pixels.
**[01:44:00]** **SPEAKER_00 (GreatStack):** Save these changes.
**[01:44:03]** **SPEAKER_00 (GreatStack):** Now, we will add the CSS properties for these input fields.
**[01:44:09]** **SPEAKER_00 (GreatStack):** So here, we will add. Loginsignup-fields, space input tag.
**[01:44:14]** **SPEAKER_00 (GreatStack):** Here, we will provide height of 72 pixels, width 100%, padding left 20 pixels, border of 1 pixel solid, and this color code, outline will be none, color, this color code, and the font-size of 18 pixels.
**[01:44:33]** **SPEAKER_00 (GreatStack):** Now, save these changes.
**[01:44:40]** **SPEAKER_00 (GreatStack):** So, these input fields are looking good. Next, we will add the properties for this continue button.
**[01:44:46]** **SPEAKER_00 (GreatStack):** So here, we will add. Loginsignup-container, button tag.
**[01:44:54]** **SPEAKER_00 (GreatStack):** For this button, we will provide the width, then height, then change the color, and background, then we will add the margin from the top, and border none, font-size will be 24 pixel, and font-weight of 500, cursor pointer.
**[01:45:16]** **SPEAKER_00 (GreatStack):** Now, save the file.
**[01:45:20]** **SPEAKER_00 (GreatStack):** So, this button is also looking good.
**[01:45:24]** **SPEAKER_00 (GreatStack):** Next, we will add the CSS for this text.
**[01:45:27]** **SPEAKER_00 (GreatStack):** So here, we will add. Loginsignup-login.
**[01:45:36]** **SPEAKER_00 (GreatStack):** Here, we will provide margin-top of 20 pixels, color code, then font-size, font-weight of 500.
**[01:45:49]** **SPEAKER_00 (GreatStack):** Now, we will add the CSS for this span tag.
**[01:45:57]** **SPEAKER_00 (GreatStack):** So here, we will add. Loginsignup-login, space span.
**[01:46:03]** **SPEAKER_00 (GreatStack):** Here, we will provide the color code, then font-weight of 600.
**[01:46:10]** **SPEAKER_00 (GreatStack):** Now, we will add the CSS for this text.
**[01:46:16]** **SPEAKER_00 (GreatStack):** So, we will use the class name, Loginsignup agree class name.
**[01:46:22]** **SPEAKER_00 (GreatStack):** Here, we will provide display flex, align items center, margin-top of 25 pixels, gap 20 pixels, and color this color code, then change the font-size, and font-weight.
**[01:46:44]** **SPEAKER_00 (GreatStack):** Now, save the file.
**[01:46:46]** **SPEAKER_00 (GreatStack):** Our signup page is ready now.
**[01:46:50]** **SPEAKER_00 (GreatStack):** Now, if I click on any product, it is not opening, so we have not created our product page.
**[01:47:02]** **SPEAKER_00 (GreatStack):** So, come to this product.jsx file.
**[01:47:06]** **SPEAKER_00 (GreatStack):** Here, we will grab all product's data using context.
**[01:47:11]** **SPEAKER_00 (GreatStack):** So here, we will add, const all product equals use context, within this use context, we will write shop context.
**[01:47:35]** **SPEAKER_00 (GreatStack):** As we have did in app.js, we have created routes, so we have the product, then we have product ID.
**[01:47:45]** **SPEAKER_00 (GreatStack):** So first, we will use the product ID in our product page.
**[01:47:50]** **SPEAKER_00 (GreatStack):** So, come to the product.jsx file and here we will add, const product ID equals use params.
**[01:48:08]** **SPEAKER_00 (GreatStack):** Here we have used use params to get the product ID.
**[01:48:13]** **SPEAKER_00 (GreatStack):** Using this product ID, we will find the product in all products data and we will assign that in one variables.
**[01:48:24]** **SPEAKER_00 (GreatStack):** So here, we will add, const product equals all product. find, and within this, we will pass one arrow function, e, so when e.ID equals product ID, if this condition is true, then this product will be displayed.
**[01:49:00]** **SPEAKER_00 (GreatStack):** So, we will store that product in this product variable and we will display that in our product page.
**[01:49:09]** **SPEAKER_00 (GreatStack):** So, we have the product ID in string format and e.ID is in number format.
**[01:49:15]** **SPEAKER_00 (GreatStack):** So here, we will convert the product ID in number.
**[01:49:23]** **SPEAKER_00 (GreatStack):** So here, we will add the bracket, and here we will add number.
**[01:49:29]** **SPEAKER_00 (GreatStack):** Now the product ID that is a string, is converted in number, so we got the product.
**[01:49:36]** **SPEAKER_00 (GreatStack):** Now we have to display the product in our page.
**[01:49:40]** **SPEAKER_00 (GreatStack):** So now, we will design the product page.
**[01:49:42]** **SPEAKER_00 (GreatStack):** So first, we will create the breadcrumb component.
**[01:49:50]** **SPEAKER_00 (GreatStack):** In this components folder, we will create new folder, and we will add the name, Breadcrumbs.
**[01:49:57]** **SPEAKER_00 (GreatStack):** In this folder, we will create one file.

---

### Segment 1 — 01:50:00 - 02:00:00

**[01:50:00]** **SPEAKER_00 (GreatStack):** breadcrumb.jsx
**[01:50:01]** **SPEAKER_00 (GreatStack):** dot JSX
**[01:50:06]** **SPEAKER_00 (GreatStack):** In this JSX file, we will add add FC
**[01:50:10]** **SPEAKER_00 (GreatStack):** And here, we will add the className Breadcrumb.
**[01:50:13]** **SPEAKER_00 (GreatStack):** that come
**[01:50:18]** **SPEAKER_00 (GreatStack):** For this component we will create one CSS file.
**[01:50:21]** **SPEAKER_00 (GreatStack):** Create a new file.
**[01:50:23]** **SPEAKER_00 (GreatStack):** bread crumb
**[01:50:27]** **SPEAKER_00 (GreatStack):** Now, import this CSS file in this breadcrumb dot JSX file.
**[01:50:32]** **SPEAKER_00 (GreatStack):** Here we will add import
**[01:50:36]** **SPEAKER_00 (GreatStack):** bread crumb
**[01:50:40]** **SPEAKER_00 (GreatStack):** Now save these changes, and within this component, we will use props.
**[01:50:45]** **SPEAKER_00 (GreatStack):** Using this props, we will get the product.
**[01:50:48]** **SPEAKER_00 (GreatStack):** So here, we will add const
**[01:50:57]** **SPEAKER_00 (GreatStack):** So, we got the product using props.
**[01:51:00]** **SPEAKER_00 (GreatStack):** And the product data will be used in this breadcrumb.
**[01:51:04]** **SPEAKER_00 (GreatStack):** So here we will add home.
**[01:51:07]** **SPEAKER_00 (GreatStack):** After that we will use the arrow icon.
**[01:51:11]** **SPEAKER_00 (GreatStack):** So we will import the arrow icon.
**[01:51:21]** **SPEAKER_00 (GreatStack):** breadcrumb arrow dot PNG.
**[01:51:25]** **SPEAKER_00 (GreatStack):** After this home, we will insert our image tag.
**[01:51:30]** **SPEAKER_00 (GreatStack):** In this image tag, we will add the arrow icon.
**[01:51:37]** **SPEAKER_00 (GreatStack):** After this image tag we will add shop.
**[01:51:41]** **SPEAKER_00 (GreatStack):** After that again we will add that image tag, and again we will add the same icon, arrow icon.
**[01:51:51]** **SPEAKER_00 (GreatStack):** After this image tag we will use the JavaScript variable that will be our product dot category.
**[01:52:02]** **SPEAKER_00 (GreatStack):** After this category, again we will insert that icon, using IMG tag.
**[01:52:13]** **SPEAKER_00 (GreatStack):** And after this image, we will insert the product name.
**[01:52:17]** **SPEAKER_00 (GreatStack):** Here we will add the product dot name.
**[01:52:21]** **SPEAKER_00 (GreatStack):** Then save the file.
**[01:52:23]** **SPEAKER_00 (GreatStack):** Now, we will mount this breadcrumb component in our product page.
**[01:52:31]** **SPEAKER_00 (GreatStack):** Here we will add bread crumb.
**[01:52:35]** **SPEAKER_00 (GreatStack):** And in this one we will pass the props.
**[01:52:43]** **SPEAKER_00 (GreatStack):** Now save the file.
**[01:52:46]** **SPEAKER_00 (GreatStack):** Now, we will link this product page with the product.
**[01:52:50]** **SPEAKER_00 (GreatStack):** For that we will come to the item components.
**[01:52:52]** **SPEAKER_00 (GreatStack):** Click on item dot JSX file.
**[01:52:56]** **SPEAKER_00 (GreatStack):** Now, we will link the item image with the product.
**[01:53:00]** **SPEAKER_00 (GreatStack):** So here we will use link.
**[01:53:05]** **SPEAKER_00 (GreatStack):** After that, we will wrap this image tag within this link tag.
**[01:53:10]** **SPEAKER_00 (GreatStack):** And here we will add to.
**[01:53:15]** **SPEAKER_00 (GreatStack):** In this one we will use template literal.
**[01:53:19]** **SPEAKER_00 (GreatStack):** Here we will insert the backticks, slash product, slash and here we will insert our product ID.
**[01:53:27]** **SPEAKER_00 (GreatStack):** That we will get through props.
**[01:53:30]** **SPEAKER_00 (GreatStack):** So here we will write dollar sign, curly braces, and here we will write the props dot ID.
**[01:53:40]** **SPEAKER_00 (GreatStack):** So we have wrapped the image tag using link.
**[01:53:43]** **SPEAKER_00 (GreatStack):** And in this link we have provided the product ID.
**[01:53:47]** **SPEAKER_00 (GreatStack):** Using that we can navigate to the product ID.
**[01:53:50]** **SPEAKER_00 (GreatStack):** Save these changes.
**[01:53:52]** **SPEAKER_00 (GreatStack):** If I click on this product image, we will come to the product page where you can see the product ID.
**[01:54:00]** **SPEAKER_00 (GreatStack):** Now we will create the product display component where we will get all the product images and other details.
**[01:54:10]** **SPEAKER_00 (GreatStack):** So here we will create a new folder within this component folder.
**[01:54:17]** **SPEAKER_00 (GreatStack):** So let's write the folder name, product display.
**[01:54:25]** **SPEAKER_00 (GreatStack):** Within this folder we will create a new file, product display dot JSX.
**[01:54:33]** **SPEAKER_00 (GreatStack):** Here we will use our FC.
**[01:54:38]** **SPEAKER_00 (GreatStack):** And here we will provide the class name, product display.
**[01:54:46]** **SPEAKER_00 (GreatStack):** Now we will create a CSS file for this product display component.
**[01:54:50]** **SPEAKER_00 (GreatStack):** So here we will create a new file, product display dot CSS.
**[01:54:56]** **SPEAKER_00 (GreatStack):** And now we will import this CSS file in this JSX file.
**[01:55:00]** **SPEAKER_00 (GreatStack):** So here we will add import
**[01:55:05]** **SPEAKER_00 (GreatStack):** product display dot CSS.
**[01:55:07]** **SPEAKER_00 (GreatStack):** Save these files.
**[01:55:09]** **SPEAKER_00 (GreatStack):** Now, we will mount this product display in our product page.
**[01:55:13]** **SPEAKER_00 (GreatStack):** So after this breadcrumb we will mount
**[01:55:23]** **SPEAKER_00 (GreatStack):** And here we will pass the props product.
**[01:55:31]** **SPEAKER_00 (GreatStack):** Where we will pass the product data.
**[01:55:36]** **SPEAKER_00 (GreatStack):** Using this props we will display our product image title and prices.
**[01:55:42]** **SPEAKER_00 (GreatStack):** So, we will come to the product display dot JSX file and here we will create HTML structure for our product display component.
**[01:55:51]** **SPEAKER_00 (GreatStack):** So here we will create two div
**[01:55:55]** **SPEAKER_00 (GreatStack):** that will be product display left and product display right.
**[01:56:05]** **SPEAKER_00 (GreatStack):** Now in this product display left class name we will add one div with the class name product display image list.
**[01:56:15]** **SPEAKER_00 (GreatStack):** In this div we will use four image tags.
**[01:56:20]** **SPEAKER_00 (GreatStack):** Here we will use IMG tag.
**[01:56:24]** **SPEAKER_00 (GreatStack):** And here we will provide the product image.
**[01:56:27]** **SPEAKER_00 (GreatStack):** So first, we will insert the product data using props.
**[01:56:34]** **SPEAKER_00 (GreatStack):** Here we will add const
**[01:56:45]** **SPEAKER_00 (GreatStack):** So in this image SRC we will use
**[01:56:49]** **SPEAKER_00 (GreatStack):** product dot image.
**[01:56:55]** **SPEAKER_00 (GreatStack):** And copy this image tag and paste it again.
**[01:57:00]** **SPEAKER_00 (GreatStack):** After this div we will create another div with the class name, product display image.
**[01:57:08]** **SPEAKER_00 (GreatStack):** In this div we will create one image tag.
**[01:57:12]** **SPEAKER_00 (GreatStack):** In this one we will provide the product image.
**[01:57:17]** **SPEAKER_00 (GreatStack):** So, right product dot image.
**[01:57:21]** **SPEAKER_00 (GreatStack):** In this image we will add the class name
**[01:57:34]** **SPEAKER_00 (GreatStack):** So in the left side there will be four small image and one main image.
**[01:57:38]** **SPEAKER_00 (GreatStack):** Now, we will design the right side of the product details.
**[01:57:42]** **SPEAKER_00 (GreatStack):** So here, we will display the product details.
**[01:57:46]** **SPEAKER_00 (GreatStack):** So here we will use the H1 tag.
**[01:57:51]** **SPEAKER_00 (GreatStack):** product dot name.
**[01:57:57]** **SPEAKER_00 (GreatStack):** After that we will create a div with the class name, product display right star.
**[01:58:07]** **SPEAKER_00 (GreatStack):** In this div we will use the image tag.
**[01:58:15]** **SPEAKER_00 (GreatStack):** Here we will use five image tags.
**[01:58:20]** **SPEAKER_00 (GreatStack):** And in all images, we will insert the star and star null icon.
**[01:58:24]** **SPEAKER_00 (GreatStack):** So here, we will import the images.
**[01:58:30]** **SPEAKER_00 (GreatStack):** So let's import star icon from assets folder star icon dot PNG.
**[01:58:35]** **SPEAKER_00 (GreatStack):** Similarly, we will import.
**[01:58:41]** **SPEAKER_00 (GreatStack):** star dull icon from assets folder star dull icon dot PNG.
**[01:58:49]** **SPEAKER_00 (GreatStack):** Now, we will use these images in these image tags.
**[01:58:57]** **SPEAKER_00 (GreatStack):** So here we will provide a star icon
**[01:59:02]** **SPEAKER_00 (GreatStack):** in these four IMG tags.
**[01:59:08]** **SPEAKER_00 (GreatStack):** And in the last one we will add star dull icon.
**[01:59:13]** **SPEAKER_00 (GreatStack):** After this image tag, we will insert a paragraph tag.
**[01:59:17]** **SPEAKER_00 (GreatStack):** Here we will display the number of ratings.
**[01:59:21]** **SPEAKER_00 (GreatStack):** So let's add any number, 122.
**[01:59:22]** **SPEAKER_00 (GreatStack):** Now, save this.
**[01:59:24]** **SPEAKER_00 (GreatStack):** If I open this product,
**[01:59:28]** **SPEAKER_00 (GreatStack):** and now we have product name, star ratings, number of ratings, and product images.
**[01:59:36]** **SPEAKER_00 (GreatStack):** After this div we will create another div
**[01:59:40]** **SPEAKER_00 (GreatStack):** where we will add the class name product display right prices.
**[01:59:48]** **SPEAKER_00 (GreatStack):** In this one, we will create two div
**[01:59:52]** **SPEAKER_00 (GreatStack):** that will be for old price and new price.

---

### Segment 1 — 02:00:00 - 02:10:00

**[02:00:04]** **SPEAKER_00 (GreatStack):** And in this div we will add dollar sign
**[02:00:08]** **SPEAKER_00 (GreatStack):** and insert the product.oldprice.
**[02:00:19]** **SPEAKER_00 (GreatStack):** Similarly we will create another div with a class name Product display right price new
**[02:00:28]** **SPEAKER_00 (GreatStack):** In this div we will insert the dollar sign and here we will add the product.newPrice
**[02:00:43]** **SPEAKER_00 (GreatStack):** After this div we will create one div where we will add the class name product display right description
**[02:01:01]** **SPEAKER_00 (GreatStack):** In this div we will insert the static description.
**[02:01:07]** **SPEAKER_00 (GreatStack):** After this div we will create another div with the class name product display right size
**[02:01:20]** **SPEAKER_00 (GreatStack):** In this div we will insert the h1 tag, in this h1 tag we will add the text, select size
**[02:01:32]** **SPEAKER_00 (GreatStack):** After that we will create a div with the class name product display right sizes
**[02:01:49]** **SPEAKER_00 (GreatStack):** In this div we will create five divs
**[02:01:56]** **SPEAKER_00 (GreatStack):** copy and paste it for more times, and in the first one we write the size small, then medium, large, then XL then double XL
**[02:02:21]** **SPEAKER_00 (GreatStack):** Now we will create one button and in this button we will add add to cart.
**[02:02:31]** **SPEAKER_00 (GreatStack):** After this button tag we will insert one paragraph tag and in this paragraph tag we will add the class name product display right category
**[02:02:45]** **SPEAKER_00 (GreatStack):** In this one we will insert the span tag and in this span tag we will add the category, after this span tag we will add the text that is, women, T-shirt, crop top
**[02:03:14]** **SPEAKER_00 (GreatStack):** Similarly we will copy this paragraph tag and paste it again, in this span tag we will add Tags
**[02:03:22]** **SPEAKER_00 (GreatStack):** and after this span tag we will add modern, latest.
**[02:03:38]** **SPEAKER_00 (GreatStack):** Now save the file.
**[02:03:39]** **SPEAKER_00 (GreatStack):** Now if I open any product, now we have the product images, product title, star ratings, number of ratings, old price, new price, description, size selection, add to cart button, category and tags
**[02:04:03]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for the product display component.
**[02:02:04]** **SPEAKER_00 (GreatStack):** So first we will add the CSS properties to product display class name.
**[02:02:04]** **SPEAKER_00 (GreatStack):** Here we will add display flex, margin of zero pixel and 170 pixels.
**[02:02:04]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for the product display left.
**[02:02:04]** **SPEAKER_00 (GreatStack):** Here also we will add display flex, gap will be 17 pixels.
**[02:02:04]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this product display image list.
**[02:02:04]** **SPEAKER_00 (GreatStack):** Here we will add display flex, flex direction column, gap of 16 pixels.
**[02:02:05]** **SPEAKER_00 (GreatStack):** Now we will add dot product img list IMG tag
**[02:02:05]** **SPEAKER_00 (GreatStack):** Here we will provide the height of 163 pixels.
**[02:02:05]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for the product display main image.
**[02:02:05]** **SPEAKER_00 (GreatStack):** So just copy this one, add it here and here we will add the width of 586 pixels, height of 700 pixels, save these changes
**[02:02:05]** **SPEAKER_00 (GreatStack):** Now we will design the right side of the product display component.
**[02:02:05]** **SPEAKER_00 (GreatStack):** Before that we will add the CSS properties to the breadcrumbs.
**[02:02:05]** **SPEAKER_00 (GreatStack):** So here we will come to the breadcrumbs.css, just add the class name breadcrumb.
**[02:02:06]** **SPEAKER_00 (GreatStack):** Here we will add display flex, align items center, gap of 8 pixel, and color, this color code. Then change the font size and change the font weight.
**[02:02:06]** **SPEAKER_00 (GreatStack):** Then we will add the margin and text transform will be capitalize, save these changes
**[02:02:06]** **SPEAKER_00 (GreatStack):** Now we will add the CSS for the right side of this product display components.
**[02:02:06]** **SPEAKER_00 (GreatStack):** So add this class name here, product display right.
**[02:02:06]** **SPEAKER_00 (GreatStack):** In the CSS file and here we will add margin of 0 pixel and 70 pixels. Then we will add display flex, flex direction column.
**[02:02:06]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties to our H1 tag.
**[02:02:07]** **SPEAKER_00 (GreatStack):** So here we will add dot product display right H1 tag.
**[02:02:07]** **SPEAKER_00 (GreatStack):** Here we will add the CSS properties: color, then font size, then font weight.
**[02:02:07]** **SPEAKER_00 (GreatStack):** Now save these changes. Now we will add the CSS for this star rating.
**[02:02:07]** **SPEAKER_00 (GreatStack):** So here we will add the class name product display right star.
**[02:02:07]** **SPEAKER_00 (GreatStack):** So here we will add display flex, align items center, margin top 13 pixels, gap of 5 pixels and color, then font size.
**[02:02:07]** **SPEAKER_00 (GreatStack):** Now this stars is ready.
**[02:02:07]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this product display right prices.
**[02:02:08]** **SPEAKER_00 (GreatStack):** Here we will add display flex, margin of 40 pixel and 0 pixel, gap of 30 pixels and font size of 24 pixel and font weight of 700.
**[02:02:08]** **SPEAKER_00 (GreatStack):** Now we will add the properties for product display right price old.
**[02:02:08]** **SPEAKER_00 (GreatStack):** Here we will add the color code, text decoration line through.
**[02:02:08]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties to product display right price new.
**[02:02:08]** **SPEAKER_00 (GreatStack):** Here we will use color code.
**[02:02:08]** **SPEAKER_00 (GreatStack):** Here we will add sizes.
**[02:02:08]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this product display right size, and this H1 tag.
**[02:02:09]** **SPEAKER_00 (GreatStack):** So write this class name here, then H1.
**[02:02:09]** **SPEAKER_00 (GreatStack):** Here we will provide margin of top 55 pixels, then this color code, then font size, and font weight of 600.
**[02:02:09]** **SPEAKER_00 (GreatStack):** Now we will add the properties for the product display right sizes and this div where we have a small medium large.
**[02:02:09]** **SPEAKER_00 (GreatStack):** Here we will provide display flex, margin 30 pixels, zero pixel, gap of 20 pixel.

---

### Segment 1 — 130:00 - 140:00

**[02:10:04]** **SPEAKER_00 (GreatStack):** So here we will add product display sizes div tag.
**[02:10:10]** **SPEAKER_00 (GreatStack):** Here we will add the padding of 18 pixel 24 pixel background this color code, then border one pixel solid and this color code, then border radius of three pixels and cursor pointer.
**[02:10:26]** **SPEAKER_00 (GreatStack):** Now save these files.
**[02:10:30]** **SPEAKER_00 (GreatStack):** Now we will add the CSS for the add to cart button.
**[02:10:42]** **SPEAKER_00 (GreatStack):** Here we will provide the padding of 20 pixel 40 pixel, width of 200 pixels, then font-size and font-weight, then change the color and background.
**[02:10:57]** **SPEAKER_00 (GreatStack):** Margin from the bottom, 40 pixel, border none, outline none, cursor pointer.
**[02:11:10]** **SPEAKER_00 (GreatStack):** Now we will add the CSS for these text, which is category and tag.
**[02:11:17]** **SPEAKER_00 (GreatStack):** So just copy this class name, product display right category.
**[02:11:25]** **SPEAKER_00 (GreatStack):** Here we will add margin top of 10 pixel.
**[02:11:30]** **SPEAKER_00 (GreatStack):** Now we will add the CSS for this span tag, so here we will add the same class name then a span tag.
**[02:11:37]** **SPEAKER_00 (GreatStack):** Here we will provide the font weight of 600.
**[02:11:43]** **SPEAKER_00 (GreatStack):** Now the product display component is ready.
**[02:11:47]** **SPEAKER_00 (GreatStack):** Now if I click on men category, select another product and now you can see the updated product image, product name, old price, new price.
**[02:11:59]** **SPEAKER_00 (GreatStack):** And here we have the breadcrumb with the main category and product name.
**[02:12:09]** **SPEAKER_00 (GreatStack):** Now we will create the description box for our product page.
**[02:12:15]** **SPEAKER_00 (GreatStack):** So in this components folder we will create another folder and we will add the name description box.
**[02:12:23]** **SPEAKER_00 (GreatStack):** In this folder, we will create a new file with the name description box dot JSX.
**[02:12:32]** **SPEAKER_00 (GreatStack):** Here we will use rafc.
**[02:12:37]** **SPEAKER_00 (GreatStack):** And in this div we will add one class name.
**[02:12:46]** **SPEAKER_00 (GreatStack):** Now we will create a CSS file for this component.
**[02:12:51]** **SPEAKER_00 (GreatStack):** So click here and create a new file, write the file name description box dot CSS.
**[02:12:59]** **SPEAKER_00 (GreatStack):** Now we will import this CSS file in JSX file.
**[02:13:15]** **SPEAKER_00 (GreatStack):** Now we will mount this component in our product page.
**[02:13:20]** **SPEAKER_00 (GreatStack):** Come to the pages, product dot JSX, product display component, so after that we will add this description box.
**[02:13:32]** **SPEAKER_00 (GreatStack):** Add this description box component, save the file.
**[02:13:37]** **SPEAKER_00 (GreatStack):** Now we will add the HTML structure for our description box component.
**[02:13:43]** **SPEAKER_00 (GreatStack):** So come back to the same file, which is description box dot JSX, and here we will create one div with the class name description box navigator.
**[02:13:57]** **SPEAKER_00 (GreatStack):** Within this div we will create another div with the class name description box nav box.
**[02:14:16]** **SPEAKER_00 (GreatStack):** Now we will create one copy of this div, and here we will add a class name fade, and instead of this description we will add the text reviews and here we will add 122.
**[02:14:36]** **SPEAKER_00 (GreatStack):** After this div we will create another div with the class name description box description.
**[02:14:47]** **SPEAKER_00 (GreatStack):** In this div we will create a paragraph tag, and in this paragraph we will add the static text.
**[02:15:00]** **SPEAKER_00 (GreatStack):** After this paragraph text we will create another paragraph text.
**[02:15:06]** **SPEAKER_00 (GreatStack):** Here also we will add some text.
**[02:15:10]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for these text.
**[02:15:17]** **SPEAKER_00 (GreatStack):** So first we will add the CSS properties for this description box.
**[02:15:23]** **SPEAKER_00 (GreatStack):** Write this class name here in description box dot CSS file.
**[02:15:30]** **SPEAKER_00 (GreatStack):** Here we will add the margin of 120 pixel and 170 pixel.
**[02:15:37]** **SPEAKER_00 (GreatStack):** Then we will add the CSS for this description box navigator.
**[02:15:48]** **SPEAKER_00 (GreatStack):** Here we will add display flex.
**[02:15:53]** **SPEAKER_00 (GreatStack):** Then we will add the CSS properties for description box nav box.
**[02:16:06]** **SPEAKER_00 (GreatStack):** Here we will add display flex, align items center, justify content center.
**[02:16:15]** **SPEAKER_00 (GreatStack):** Then we will change the font size and font weight, width will be 171 pixel and height 70 pixel, then border of one pixel solid and this color code.
**[02:16:34]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this fade class name.
**[02:16:42]** **SPEAKER_00 (GreatStack):** Here we will add dot description box dot nav box dot fade.
**[02:16:53]** **SPEAKER_00 (GreatStack):** Here we will add the background and this color code, then we will change the color.
**[02:17:03]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for description box description class name.
**[02:17:13]** **SPEAKER_00 (GreatStack):** For this one we will add display flex, flex direction column, gap 25 pixels, border of one pixel solid and this color code, padding of 48 pixels and padding bottom 70 pixel.
**[02:17:39]** **SPEAKER_00 (GreatStack):** Now we will create the related product component for this product page.
**[02:17:46]** **SPEAKER_00 (GreatStack):** So in this component folder we will create a new folder with the name related products.
**[02:18:03]** **SPEAKER_00 (GreatStack):** Here we will use rafc.
**[02:18:07]** **SPEAKER_00 (GreatStack):** And for this div we will add a class name related products.
**[02:18:15]** **SPEAKER_00 (GreatStack):** Now we will create a CSS file for this component.
**[02:18:19]** **SPEAKER_00 (GreatStack):** In this folder we will create a new file related products dot CSS.
**[02:18:25]** **SPEAKER_00 (GreatStack):** Now we will import this CSS file in our JSX file.
**[02:18:37]** **SPEAKER_00 (GreatStack):** Within this div we will create the HTML structure for our related product components.
**[02:18:43]** **SPEAKER_00 (GreatStack):** So here we will create one H1 tag, and in this one we will add the title related products.
**[02:18:53]** **SPEAKER_00 (GreatStack):** After that we will insert one HR tag.
**[02:18:58]** **SPEAKER_00 (GreatStack):** After this HR, we will create one div with the class name related products item.
**[02:19:07]** **SPEAKER_00 (GreatStack):** In this div we will map the product data.
**[02:19:13]** **SPEAKER_00 (GreatStack):** First we will import data product from assets data.
**[02:19:21]** **SPEAKER_00 (GreatStack):** And here we will add data product dot map method.
**[02:19:34]** **SPEAKER_00 (GreatStack):** Here we will pass the item and index number.
**[02:19:43]** **SPEAKER_00 (GreatStack):** Here we will return our item component, so we will use return item.
**[02:19:50]** **SPEAKER_00 (GreatStack):** And here we have to pass the props, as we have added in new collections, so come to new collections dot JSX file.

---

### Segment 1 — 140:00 - 150:00

**[02:20:00]** **SPEAKER_00 (GreatStack):** Now we will add the functionality that when we will click on any product, we will scroll to the top of the page. So first we will come to the item component, we will open item dot jsx file.
**[02:20:12]** **SPEAKER_00 (GreatStack):** Now, we will add the CSS properties for this Related Products component.
**[02:20:26]** **SPEAKER_00 (GreatStack):** Write this class name here, and here, we will add display flex, flex direction column, align items center, gap of 10 pixel, height 90vh.
**[02:20:43]** **SPEAKER_00 (GreatStack):** And now, if I click on any product, you can see it will open the product, and we are on the top of the page.
**[02:20:53]** **SPEAKER_00 (GreatStack):** Now, we will create the logic for the cart and add to cart button.
**[02:21:04]** **SPEAKER_00 (GreatStack):** Next, we will add the CSS properties for this HR tag.
**[02:21:14]** **SPEAKER_00 (GreatStack):** Here, we will provide width of 200 pixels, height of 6 pixels, border radius of 10 pixels, and background this color code.
**[02:21:26]** **SPEAKER_00 (GreatStack):** Now, we will add the CSS properties for related products item.
**[02:21:33]** **SPEAKER_00 (GreatStack):** So, just copy this one, add it here. Here, we will add the margin 50 pixel from the top, display flex, gap of 30 pixels.
**[02:21:47]** **SPEAKER_00 (GreatStack):** Now, we will mount this component in product page.
**[02:21:52]** **SPEAKER_00 (GreatStack):** So, come to the product.jsx files and after this description box, we will add related products.
**[02:22:06]** **SPEAKER_00 (GreatStack):** Here, we will change it related products. Save the file.
**[02:22:12]** **SPEAKER_00 (GreatStack):** Now, you can see after this description, we have the related products.
**[02:22:17]** **SPEAKER_00 (GreatStack):** Now, if I click on any product, it will open that product, but it is not scrolling to the top.
**[02:22:37]** **SPEAKER_00 (GreatStack):** We will open item.jsx file, and in this image tag, we will use on click.
**[02:22:47]** **SPEAKER_00 (GreatStack):** Within this on click, we will add window.scrollTo and here, we will pass x and y axis coordinate. So, we will add 0 and 0.
**[02:23:18]** **SPEAKER_00 (GreatStack):** Now, we will create the logic for the cart and add to cart button.
**[02:23:24]** **SPEAKER_00 (GreatStack):** So, we will come to shopcontext.jsx file.
**[02:23:28]** **SPEAKER_00 (GreatStack):** Here, first, we will create one empty cart.
**[02:23:51]** **SPEAKER_00 (GreatStack):** const getdefaultcart, and here, we will create one arrow function.
**[02:24:21]** **SPEAKER_00 (GreatStack):** So, first, we will create one for loop.
**[02:24:38]** **SPEAKER_00 (GreatStack):** Here, we will add the cart, and in this one, we will pass the index equals and initialize the product ID with 0.
**[02:24:54]** **SPEAKER_00 (GreatStack):** So here, we will add return cart.
**[02:25:04]** **SPEAKER_00 (GreatStack):** Now, we will keep this function outside of this shop context provider.
**[02:25:12]** **SPEAKER_00 (GreatStack):** And in this shop context provider, we will create one use state variable.
**[02:25:45]** **SPEAKER_00 (GreatStack):** Its size will be all product.length.
**[02:26:10]** **SPEAKER_00 (GreatStack):** Now, using the context, we can access the cart item data in any component.
**[02:26:25]** **SPEAKER_00 (GreatStack):** So, if I reload the page, you can see we have the cart data.
**[02:26:46]** **SPEAKER_00 (GreatStack):** Now, in this all product.length, we will add plus one.
**[02:27:27]** **SPEAKER_00 (GreatStack):** So, first we will send the previous value and in this function, we will use the spread operator.
**[02:28:11]** **SPEAKER_00 (GreatStack):** Instead of add to cart, we will add remove from cart.
**[02:28:44]** **SPEAKER_00 (GreatStack):** And here, we will import add to cart function through our context API.
**[02:29:11]** **SPEAKER_00 (GreatStack):** So, now we have the add to cart function.
**[02:29:16]** **SPEAKER_00 (GreatStack):** In this function, we will pass the product ID.
**[02:29:21]** **SPEAKER_00 (GreatStack):** So, first, we will link this function with add to cart button.
**[02:29:45]** **SPEAKER_00 (GreatStack):** In this shopcontext.jsx file, we will add console.log.
**[02:29:57]** **SPEAKER_00 (GreatStack):** In this one, we will pass cart item.

---

### Segment 18 — 02:40:00 - 02:50:00

**[02:40:02]** **SPEAKER_00 (GreatStack):** After that, we will add the CSS properties for the cart item format main.
**[02:40:08]** **SPEAKER_00 (GreatStack):** Here we will add display grid, grid template column 0.5 fraction, two fraction, one fraction, one fraction, one fraction and one fraction, align items center, gap 75 pixels, padding of 20 pixels, zero pixel, color, this color code, then font size 18 pixel, and font weight 600.
**[02:40:35]** **SPEAKER_00 (GreatStack):** Save these changes.
**[02:40:37]** **SPEAKER_00 (GreatStack):** Now, let's add some items in the cart. Let's click here.
**[02:40:41]** **SPEAKER_00 (GreatStack):** And we have added three different product.
**[02:40:45]** **SPEAKER_00 (GreatStack):** Now in this cart page, you can see three items.
**[02:40:50]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for these cart items.
**[02:40:55]** **SPEAKER_00 (GreatStack):** So, just use the same class name.
**[02:41:00]** **SPEAKER_00 (GreatStack):** Here we will add this class name in this cart item format.
**[02:41:05]** **SPEAKER_00 (GreatStack):** So, we will add the same class name here and save these changes.
**[02:41:10]** **SPEAKER_00 (GreatStack):** Now we have products in the same template.
**[02:41:14]** **SPEAKER_00 (GreatStack):** Now we will add the properties for the cart item format.
**[02:41:26]** **SPEAKER_00 (GreatStack):** Here we will add font size of 17 pixels, font weight of 500.
**[02:41:35]** **SPEAKER_00 (GreatStack):** Now the text is different from the title.
**[02:41:40]** **SPEAKER_00 (GreatStack):** Now we will reduce the size of this product image.
**[02:41:44]** **SPEAKER_00 (GreatStack):** So we will use this class name.
**[02:41:47]** **SPEAKER_00 (GreatStack):** Cart icon product icon.
**[02:41:51]** **SPEAKER_00 (GreatStack):** Here we will add the height of 62 pixels.
**[02:42:00]** **SPEAKER_00 (GreatStack):** Now in this image tag we will add a class name and here we will add the class name.
**[02:42:05]** **SPEAKER_00 (GreatStack):** Cart items remove icon.
**[02:42:17]** **SPEAKER_00 (GreatStack):** Width 15 pixels, margin 0 pixel, 40 pixels, cursor pointer.
**[02:42:25]** **SPEAKER_00 (GreatStack):** Now the image size has been reduced.
**[02:42:30]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this quantity button.
**[02:42:35]** **SPEAKER_00 (GreatStack):** So from here we will copy this class name.
**[02:42:42]** **SPEAKER_00 (GreatStack):** And for this class name we will add the width of 64 pixels, height 50 pixels, border of 2 pixel solid and this color code, background white.
**[02:42:56]** **SPEAKER_00 (GreatStack):** Now this quantity button is looking good.
**[02:42:59]** **SPEAKER_00 (GreatStack):** Now in this total price, we have to add the dollar sign.
**[02:43:03]** **SPEAKER_00 (GreatStack):** So let's come back and here we will add dollar.
**[02:43:08]** **SPEAKER_00 (GreatStack):** Save these changes.
**[02:43:11]** **SPEAKER_00 (GreatStack):** Now here we have the total price of the individual item, that is the price multiplied by quantity.
**[02:43:18]** **SPEAKER_00 (GreatStack):** Now we will display the total cart price, that is the cart value.
**[02:43:35]** **SPEAKER_00 (GreatStack):** And after that we will add one div with the class name cart items down.
**[02:43:46]** **SPEAKER_00 (GreatStack):** After that we will create another div with the class name cart items total.
**[02:43:56]** **SPEAKER_00 (GreatStack):** Then we will add one text in H1 tag. So let's add the text, cart totals.
**[02:44:04]** **SPEAKER_00 (GreatStack):** After this H1 tag, we will create one div.
**[02:44:10]** **SPEAKER_00 (GreatStack):** And in this div we will create another div with the class name, cart items total item.
**[02:44:21]** **SPEAKER_00 (GreatStack):** In this div we will use the paragraph text.
**[02:44:26]** **SPEAKER_00 (GreatStack):** Here we will add subtotal.
**[02:44:29]** **SPEAKER_00 (GreatStack):** And after this paragraph text we will add another paragraph text, and in this one we will insert dollar sign.
**[02:44:36]** **SPEAKER_00 (GreatStack):** And here we will use total cart value.
**[02:44:40]** **SPEAKER_00 (GreatStack):** So let me write zero for now.
**[02:44:45]** **SPEAKER_00 (GreatStack):** And we will display this data using our context.
**[02:44:48]** **SPEAKER_00 (GreatStack):** So after this div we will add one HR tag.
**[02:44:52]** **SPEAKER_00 (GreatStack):** And here we will create one div and the class name will be same, cart items total item.
**[02:45:02]** **SPEAKER_00 (GreatStack):** In this div we will create two paragraph tags.
**[02:45:07]** **SPEAKER_00 (GreatStack):** So, first one will be shipping fee.
**[02:45:13]** **SPEAKER_00 (GreatStack):** And the second paragraph tag will be free.
**[02:45:18]** **SPEAKER_00 (GreatStack):** After this div we will add one HR tag.
**[02:45:22]** **SPEAKER_00 (GreatStack):** And after that, we will insert a div with the same class name.
**[02:45:28]** **SPEAKER_00 (GreatStack):** Cart items total item.
**[02:45:41]** **SPEAKER_00 (GreatStack):** Another H3 tag and here we will display dollar sign and the total cart value. So here we will add zero for now.
**[02:45:51]** **SPEAKER_00 (GreatStack):** After this div we will create one button tag. In this one we will add the text that is proceed to checkout.
**[02:46:07]** **SPEAKER_00 (GreatStack):** Now we will create one promo code section.
**[02:46:11]** **SPEAKER_00 (GreatStack):** So here we will add div dot cart items promo code.
**[02:46:21]** **SPEAKER_00 (GreatStack):** In this div we will insert a paragraph text, and here we will add, if you have a promo code, enter it here.
**[02:46:33]** **SPEAKER_00 (GreatStack):** After that we will add one div tag with the class name cart item promo box.
**[02:46:46]** **SPEAKER_00 (GreatStack):** Now in this one we will insert one input tag.
**[02:46:51]** **SPEAKER_00 (GreatStack):** Here we will insert the placeholder, and the placeholder text will be promo code.
**[02:47:01]** **SPEAKER_00 (GreatStack):** After that, we will add one button.
**[02:47:05]** **SPEAKER_00 (GreatStack):** And in this button we will add the button text, submit.
**[02:47:10]** **SPEAKER_00 (GreatStack):** Now save the code and now you can see these things on the web page.
**[02:47:15]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for these details.
**[02:47:18]** **SPEAKER_00 (GreatStack):** First, we will add the CSS properties for the cart items down class name.
**[02:47:28]** **SPEAKER_00 (GreatStack):** So here we will add display flex, margin 100 pixel and zero pixel.
**[02:47:37]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this cart items total class name.
**[02:47:44]** **SPEAKER_00 (GreatStack):** Here we will provide flex one, display flex, flex direction column, margin right of 200 pixels, gap 40 pixels.
**[02:48:04]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this cart item total item class name.
**[02:48:16]** **SPEAKER_00 (GreatStack):** So here we will provide display flex, justify content space between, padding 15 pixels and zero pixel.
**[02:48:27]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this button tag.
**[02:48:33]** **SPEAKER_00 (GreatStack):** So here we will add dot cart items total, space button tag.
**[02:48:43]** **SPEAKER_00 (GreatStack):** Here we will provide width of 262 pixels, height of 58 pixels, outline none, border none, background this color code, color white, and font size 16 pixels, font weight of 600 and cursor pointer.
**[02:49:05]** **SPEAKER_00 (GreatStack):** Now this button looks good.
**[02:49:09]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for the promo code section.
**[02:49:13]** **SPEAKER_00 (GreatStack):** So here we have the class name, cart items promo code. Just add this class name here.
**[02:49:21]** **SPEAKER_00 (GreatStack):** For this one we will provide flex one, font size 16 pixels, font weight of 500.
**[02:49:36]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this P tag.
**[02:49:40]** **SPEAKER_00 (GreatStack):** So again write the same class name, cart items promo code, then space p.
**[02:49:48]** **SPEAKER_00 (GreatStack):** For this paragraph we will provide color this color code.

---

### Segment 1 — 02:50:00 - 02:58:57

**[02:50:00]** **SPEAKER_00 (GreatStack):** And here we will add width of 504 pixel, margin-top 15 pixels, padding-left 20 pixels, and height 58 pixels, background this color code.
**[02:50:01]** **SPEAKER_00 (GreatStack):** cart items promo box.
**[02:50:18]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this input field.
**[02:50:23]** **SPEAKER_00 (GreatStack):** So here we will add dot cart items promo box input tag.
**[02:50:34]** **SPEAKER_00 (GreatStack):** Here we will provide border none, outline none, background transparent, font size 16 pixels, width of 330 pixels, height of 50 pixels.
**[02:50:53]** **SPEAKER_00 (GreatStack):** Now we will add the CSS properties for this submit button.
**[02:50:57]** **SPEAKER_00 (GreatStack):** So here we will add cart items promo box button tag.
**[02:51:05]** **SPEAKER_00 (GreatStack):** So for this button we will provide width 170 pixels, height 58 pixels, font size 16 pixels, background black, color white, cursor pointer.
**[02:51:19]** **SPEAKER_00 (GreatStack):** Now this promobox is ready. The design for this cart is ready.
**[02:51:24]** **SPEAKER_00 (GreatStack):** Next we will insert the cart total value. So come here in ShopContext.jsx file.
**[02:51:30]** **SPEAKER_00 (GreatStack):** So come here in Shop Context dot JSX file.
**[02:51:35]** **SPEAKER_00 (GreatStack):** Here we will create one function const getTotalCartAmount = () => { First we will create one variable let totalAmount = 0; So here we will run one for loop. Here we will pass our cart items from our cart. So we will add const item in cartItems.
**[02:52:16]** **SPEAKER_00 (GreatStack):** Here we will check the quantity of that item. If it is greater than zero, so we will add if. And we will add cartItems. In this one we will pass the item. If the item quantity is greater than zero, then we will add Let we will create a variable let itemInfo = all_product. Then we will find the product using find, and in this one we will pass one arrow function, and here we will pass the individual product.
**[02:53:03]** **SPEAKER_00 (GreatStack):** And here we will check if our product.id is equal to our item. So our item is string, so we have to convert this string in number. So here we will add number. If our product.id is equal to item, then we will get that product. And using that product, we can store that product data in itemInfo. Here we will add totalAmount += Here we will access the price of that product. So we will add itemInfo.new_price then multiply with the quantity. So to access the quantity, we will add cartItems, we will pass the item.
**[02:53:59]** **SPEAKER_00 (GreatStack):** After running this function, we will get the total amount, so we will return our totalAmount.
**[02:54:12]** **SPEAKER_00 (GreatStack):** Now we will send this function through our context.
**[02:54:18]** **SPEAKER_00 (GreatStack):** So we will pass this function in context value.
**[02:54:25]** **SPEAKER_00 (GreatStack):** And now we will access this function in our cart item component.
**[02:54:29]** **SPEAKER_00 (GreatStack):** So come to the cart item component.
**[02:54:34]** **SPEAKER_00 (GreatStack):** And here, first we will get that function using context API.
**[02:54:40]** **SPEAKER_00 (GreatStack):** Now we will use this function in this cart total, so here we will add getTotalCartAmount
**[02:54:51]** **SPEAKER_00 (GreatStack):** And here we will add the same thing, getTotalCartAmount(). Now save this.
**[02:54:55]** **SPEAKER_00 (GreatStack):** Now, if I open any product and click on add to cart, let's open another product and add to cart. We have added three product. Now come to the cart page.
**[02:55:08]** **SPEAKER_00 (GreatStack):** Now we have individual prices, and here we have the total price.
**[02:55:18]** **SPEAKER_00 (GreatStack):** Now we will create a logic using that, we will count the number of item in our cart and that will be displayed in our Navbar.
**[02:55:28]** **SPEAKER_00 (GreatStack):** So here we will create one function const getTotalCartItems = () => { In this one we will create one variable let totalItem = 0. So initially the total item is zero. And here we will run a for loop. And in this one we will pass the individual item from our cart items. So here we will add const item in cartItems.
**[02:56:20]** **SPEAKER_00 (GreatStack):** In this one we will check if our quantity for that item is greater than zero, so we will add cartItems item. If it is greater than zero then we will add that product quantity in the total item variable. So we will add totalItem += cartItems[item]. And after running this loop, we will return the total item.
**[02:57:09]** **SPEAKER_00 (GreatStack):** Now we can access this function in our Navbar. So here, come to the Navbar, Navbar.jsx file, and here we will import that function using Context API.
**[02:57:24]** **SPEAKER_00 (GreatStack):** So we will add const get total cart items equal to use context.
**[02:57:32]** **SPEAKER_00 (GreatStack):** And in this one, we will pass Shop Context.
**[02:57:38]** **SPEAKER_00 (GreatStack):** Now we will show this data in our nav cart count. So here we will add function name, and save this.
**[02:57:49]** **SPEAKER_00 (GreatStack):** Now, if I add this product in the cart, if I clicked here, you can see quantity one. If I click again, you can see the quantity two in this Navbar.
**[02:58:05]** **SPEAKER_00 (GreatStack):** And you can see it is here. If I click on this cross icon, we can easily remove the product from the cart.
**[02:58:12]** **SPEAKER_00 (GreatStack):** Now if I click on this product add to cart, then another product and add to cart, added three product.
**[02:58:18]** **SPEAKER_00 (GreatStack):** Now here we have the cart total value 245 and this is the total individual item value.
**[02:58:28]** **SPEAKER_00 (GreatStack):** And here we can remove the product, so it is decreasing the total cart value and the count from this Navbar is also decreasing. If I remove it, it will become zero.
**[02:58:39]** **SPEAKER_00 (GreatStack):** So, finally we have successfully created our e-commerce website using react JS.
**[02:58:44]** **SPEAKER_00 (GreatStack):** Checkout the Link given in the description to create Backend & Login Registration system with Database.
**[02:58:46]** **SPEAKER_00 (GreatStack):** I hope this video will be helpful for you, if you have any question, you can ask me in the comment section, please like and share this video and also subscribe my channel, Great Stack.
**[02:58:53]** **SPEAKER_00 (GreatStack):** Thank you so much for watching this video.