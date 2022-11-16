# [Window Shopping Website]([https://hackmd.io/c/tutorials](https://iwp-assign1.herokuapp.com/products))

## Description
This website platform serves as a medium to share your opinion on any product. Can be used by product designers to host their product online and get reviews from people who read about it. The main idea is to get reviews from potential-customers and critics about the product right from the designing stage.

## Frameworks and Tools used:
* HTML
* CSS
* Javascript
* Mongodb
* Nodejs
* Express
* Express Body-Parser
* Express Sanitizer
* EJS

## Database

### Collections
* Brands: list of the brands and their corresponding image sources.
* Category: list of the categories and their correspoding image sources.
* Products: All the products added to the database are stored here.

### Products-Collection
* Contains brand-name, category, title, image-source, description and array of ratings
* The products reviews array are accessed in the product page with most recent review appearing first
* The recently added review is inserted in the 0-th index using unshift function
* product is uniquely identified using the \_id attribute which is randomly initialized

## Modules

### Models:
Contains modules in javascript that create or load the collection into a variable.

### Public
Contains CSS and Javascript files for website body.
### Routes
Calls specific controller to handle a request from the client.
### Controllers
Contains function processing the request and then either rendering the new page or redirecting the request to other page.
### Views
Contains EJS scripts which load the data from the database and display on the website in a ordered manner. Also contains a Partials folder which has ejs script for reusable peice of code like the header and the footer.

## Website-Design

### Homepage:
1. Homepage has fixed navigation bar with links to home, all new, and about.
2. Slideshow which changes the slide when next or prev button is clicked.
3. Subsequently followed by rows that contain upto 6 product cards.
4. Ends with the footer.

:::info
Show by brand, show by category, show by sorted order, and show all use the same EJS and css file. This is achieved by passing relavant product like from the controller.
:::
### All Page:
Shows all the products present in the database.
### Show by Brand
Loads all the products from the specific brand.
### Show by Category
Loads all the products from the specific category.
### Product Page
Loads the details of the product along with the review about the product. There is also a div to add review to the product. The review is automatically saved to the database of the product that the review was written.
### New Product
Lets the client add product to the database. the product is instantly added and can be viewed in the latest for the brand list on Homepage.
### About
Contains information about the website.
## Contributors
* Aditya Jivoji
* Khushi Dave
