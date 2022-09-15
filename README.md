# Thuma Code Challenge

Welcome to the Thuma Take Home Interview! The purpose of this exercise is to gauge your capacity to dive into a (mostly) working system and make modifications and extentions to it. The tasks are meant to be straightforward, with most people completing the tasks in less than 30 minutes. You may take as long as needed to complete the tasks, we're not keeping track. If you have any initial questions after reading this prompt, please reach out.

## Directory Structure

The API directory contains various data fetching and utility functions. The components directory contains components shared on multiple pages. The contexts directory houses react context definitions. The hooks directory contains custom hooks for this application. The large majority of the application is housed in the pages directory. Generally, file paths from the pages directory map to url paths in the application. With two next.js specific conventions, \_app is used as the shell (all pages render into this shell) and paths with square brackets which match dynamic routes.

## The Application Now

The application currently has 3 routes (/, /products/bed, /products/mattress) which are also discoverable using the top nav bar. All routes render a nav on the top and a cart on the right side. The cart has a button that randomly generates a cart with 0-2 items in it. The product pages have a placeholder image, a form to specify the variant you want and an add to cart button. This application is clearly not designed, but it's a sufficient prototype for proving out some feature ideas and bug fixes.

## The Challenge
1. **Get the project on your computer** Create a repository on your personal github account by using this repository as a template. Make sure to make it private so nobody else can copy your work. Clone it to your local machine.
<img width="1166" alt="Screen Shot 2022-09-15 at 10 13 56 AM" src="https://user-images.githubusercontent.com/1392496/190442522-9b1398d7-61bd-45e0-9319-7a21d84fe16a.png">

***

<img width="786" alt="Screen Shot 2022-09-15 at 10 20 00 AM" src="https://user-images.githubusercontent.com/1392496/190442989-51ef80b3-ce55-4ce6-a062-be5bd6ac564d.png">

2. **Install & Run the project** Run `yarn && yarn dev` to install dependencies and run the application. The application should start up onto the cart page after this is complete.

3. **Add a remove from cart button to the cart items.** Each item in the cart should get a button to the right of it's name that, when clicked, the item is removed from the cart. Feel free to use the CloseButton component which is is in the components directory. This feature does not have a design or mock and you will not be graded on the design you come up with. The important success criteria is that if you click the button, the item is removed from the cart.

4. **Make the add to cart button on the product pages work.** Currently the product pages have a non-functional add to cart button. Please implement add to cart functionality such that when a user clicks add to cart, a variant of the product is added to the cart which matches the state of the form fields. This product should render in the cart the same way as products added via the random cart button. Remember that \_app.js is rendered on every page.

5. **Launch a nightstand product.** Extend the store's product offerings to include a nightstand. The nightstand only comes in one size, but has the same colors as the bed does. Make sure that it can be added to the cart.

6. **OPTIONAL: Make it better?** While working in this project was there something you didn't like? Maybe something about the "design" really bugs you. Maybe you don't like how the files are organized. Maybe you don't like a variable name or algorithm. Thuma's culture encourages collaboration. Be the change you want to see. Document what you did so we can discuss it (and maybe incorportate it into the default template for this interview question). Just don't make any changes that would make it harder to grade tasks 2-4.

7. **Submit your work.** Add @patrick-mcdougle as a collaborator to your private repo. **DO NOT OPEN A PR**
<img width="1369" alt="Screen Shot 2022-09-15 at 10 16 31 AM" src="https://user-images.githubusercontent.com/1392496/190442146-9fbbc3e9-b56b-4de7-88f0-805816336741.png">

**Note:** _You should not need any additional javascript dependencies to accomplish these tasks, so please do not install any._

## Documentation / Resources

- [Next Documentation](https://nextjs.org/docs/getting-started)
- [React Documentation](https://reactjs.org/docs/getting-started.html)
