# Welcome to Maitretech Solution Coding Challenge:

> Best of Luck for Challenge!!!
> Challenge Compltion Time : 9 hours

## Overview:

To complete this codding challenge, you will need to write a simple React web app using create-react-app (CRA), and provide us buildable the source code files along with the build files. The project should be built and installed without any errors. Please read completely, this README before proceeding.

The purpose of this challenge is to assess your **skills and approach to composing a simple react based web app** given a set of screens and an API feed. We will also review the **written JSX, CSS and JS** output along with the final output.

This challenge is expected to be completed in 9 hours.

## The Challenge:

It's pretty simple. Using the provided screens in the screens directory as a reference, you'll need to build a set of React components to render the app. You'll also need to fetch the data in JSON format and save the data by invoking the API. The images which you may require is already available in the assets directory. 

Although this is a basic exercise, we'll be looking for **simple, well-designed, performant, and error free code** in the submission.

Please update this `README` with any tests or other documentation you created as part of your solution.

## Details:

You will need to build the following 4 pages with React:
  - **Sign Up** page
  - **Login** page
  - **GoTo Menu** page
  - **Food Items** page
  - **Order Summary** page
  - **Thank You** page

The deployable solution should be built in a folder named **`dist`** with an entry point file of **`index.html`**.

Please create components for each part of the page (eg. header, content, footer, etc).
Assets are provided in the `assets` folder. Data is provided in `data` folder in the form of JSON file.

The pages should also be responsive and viewable on mobile and tablet devices with decent look and feel. Each page is accessible by different URL.

### "Sign Up" page
Create a Sign-up Page that allows the user to Sign Up (Register) for the Application. These credentials will be used for logging into the application. The fields for signing up are Full Name, email, and password. The password should be at least 6 characters long. The email should be in the proper format. The Fields should be appropriately validated. 

You will develop an API that stores data in the file. The data will be stored in a JSON file as with the name `credentials.json` as a datastore. 

### "Login" page
Create a Login Page that allows the user to log into the Application. If a user tries to access **GoTo Menu**, **Food Items**, **Order Summary**, or **Thank You** page without entering valid credentials, he should be redirected to the **Login Page** page. You can use `credentials.json` file created earlier to validate the user's credentials. After validation of user credentials, the user details must be stored in the local storage. 

### "GoTo Menu" Page

Refer to the [screens/Screen1.png](./screens/Screen1.png) screen.

This will be your `index.html` screen.

You will need to display a welcome message with a button to `Go To The Next Page`, which link to the "Food Items" page.

### "Food Items" page

Refer to the [screens/Screen2.png](./screens/Screen2.png) for Food Items Page.

For this page, you will need to fetch data from URI `./data/feeds.json` using fetch API. The data will be in JSON format containing the name, price, and image of the food items. The data us ibkt fetched when the user details are already present in the local storage. Please pass 'Content-Type': 'application/json' and 'Accept': 'application/json' as headers :

Then do the following:

- Display the name and the price of `entries` as shown in the [screens/Screen2.png](./screens/Screen2.png)
- Where the `+` of the entry is clicked, the Total and Cost should be updated as shown in [screens/Screen2.1.png](./screens/Screen2.1.png).
- When `Cart` icon is clicked, [screens/Screen2.2.png](./screens/Screen2.2.png) is shown, where order can be manupulated by clicking `+` and `-` buttons. IT should also reflect the current quantity. If the item is less than `1`, the item should be removed from the list.
- When the `SAVE AND CHECKOUT` is clicked, the user should be redirected to the the screen [screens/Screen3.png](./screens/Screen3.png)

You will also need to handle the loading and error states of fetching the JSON feeds:

**NOTE** You can use any State Management Library or Context API to accoplish it. 

## Getting Started:

- Please clone this repo.
- Create CRA project within this repo.
- Move assets to your `public` folder for your CRA.
- Please copy `feeds.json` where you can access it from the source.
- Start coding yoru app.

## Code Submission process:

Please only submit error free working code, otherwise you will be disqualified from the coding challenge. In order to submit your working code, please do the following:

- Update this `README` with necessary information.
- Create a new git branch in the format `<your-name>_challenge` for example if your name is `John`, the branch should be `john_challenge`.
- Push the branch for review.

## FAQ:

### What language, framework, build tool... should I use?

You must use React to built using [React](https://reactjs.org/).

We perfer you use Context API for State management. Apart from state management, you can either use redux, redux-toolkit or reoil. Please don't use any other state management library.

Youare are not allowed to use any third party CSS frameworks other then `Tailwind CSS`. If you are not confortable in using `TailwindCSS`, please use plain CSS. However, you can use `scss/sass` if you are aware. 

We also prefer the use of minimal dependencies.

## Other Notes

Please send through any other code or projects that you're proud of and would like to share with us.

Any feedback on the coding challenge once you're done is also appreciated!
