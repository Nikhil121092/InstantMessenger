
# About Project

This project is the current news feeds portal. We can view/read the news which are actively being updated.
The news are also categorised to get the category based news.

Source News API : https://newsapi.org/

## I am using free tier so it provides only 1000 calls in 24 hours. So, it may not update the data to store if the given quota is fnished.

## This is the React web application for a news feeds platform. 
The main focus here is to create a super fast and production-ready application.
<br>
Following are the highlights of this project:
* **React web app**: The server sends the rendered pages to the client, and then the client renders the subsequent pages on its own. This is a very important feature for SEO and it also makes the first paint super fast.
* **React Hooks**: This application uses hooks APIs from React, Redux, and other libraries. 
* **Written in Typescript**: The type safety at build time and having intellisense for it in the IDE like vscode is unparalleled to productivity. We have found production bug reduced to a significant amount since most of the code vulnerabilities are identified during the build phase itself. The Typescript was preferred over the Flow for better vscode support and much more type availability for libraries.
* **Separation of concern principle is applied**: Each component has been given a particular role. The role of the components is mutually exclusive. This makes the project easy to be unit tested.
* **Feature encapsulation is adopted**: The files or components that are related to a particular feature have been grouped unless those components are required in multiple features. This enhances the ability to share code across projects.
* **State management using Redux**: The Redux architecture is very well suited for scalable web apps. It is excellent in server side rendering for components that need data from the API server. It is also preferred over the context in the project.
* **Separate API server**: This project also has a server, having the purpose of serving only the pages for the website. Lhe logic of the application lies in a separate API server which is also opensource by us [**here**](https://github.com/janishar/nodejs-backend-architecture-typescript).
* **Boilerplate**: Utility classes have been written to reduce the application and Redux boilerplate. 
* **Latest libraries and patterns**: All the libraries used in this project are standard, concerning the latest and modern web development practices.
* **vscode tasks for templates**: For enhancing the productivity while coding on the vscode, many tasks have been written to help generate the initial working code for each component. Just execute these tasks in vscode.

## Architecture of an UI component
<p align="center">
   <img src="https://raw.githubusercontent.com/janishar/react-app-architecture/master/.templates/github_assets/ui-component-architecture.png">
</p>
<br>

## Learn the concepts used in this project
* [Create React Isomorphic App like a Pro](https://janishar.com/blog/create-react-isomorphic-app-like-a-pro)

## Node.js Backend API Project: [**Goto Repository**](https://github.com/janishar/nodejs-backend-architecture-typescript)

## How to build and run this project
* Install the API server. [**Read Instructions Here**](https://github.com/janishar/nodejs-backend-architecture-typescript)
* Install using Docker Compose [**Recommended Method For Production**] 
    * Clone this repo.
    * Make a copy of **.env.example** file to **.env**.
    * Make a copy of **tests/.env.test.example** file to **tests/.env.test**.
    * Make sure the **.env** file has the **API_BASE_URL** point to the API server.
    * Install Docker and Docker Compose. [Find Instructions Here](https://docs.docker.com/install/).
    * Execute `docker-compose up -d` in the terminal from the repo directory.
    * You will be able to access the website from http://localhost:3001
    * *If having any issue* then make sure 3001 port is not occupied else provide a different port in **.env** file.
 * Install Without Docker [**2nd Method For Development**]
    * Do steps 1 to 4 as listed above for **Install using Docker Compose**.
    * Execute `npm install`
    * Run the project:
      * Development: Execute `npm run watch`
      * Production: Execute `npm start`
    * You will be able to access the website from http://localhost:3001

## Website Pages
* Landing 
* Blog List
* Blog Page
* Writing Pad - Markdown Editor

<p float="left">
  <img width="45%" src="https://raw.githubusercontent.com/janishar/react-app-architecture/master/.templates/github_assets/screenshots/1.png">
  <img width="45%" src="https://raw.githubusercontent.com/janishar/react-app-architecture/master/.templates/github_assets/screenshots/2.png">
</p>
<p float="left">
  <img width="45%" src="https://raw.githubusercontent.com/janishar/react-app-architecture/master/.templates/github_assets/screenshots/3.png">
  <img width="45%" src="https://raw.githubusercontent.com/janishar/react-app-architecture/master/.templates/github_assets/screenshots/4.png">
</p>

 ## Project Directory Structure
 ```
 .
new_updates/
┣ public/
┃ ┣ favicon.ico
┃ ┣ index.html
┃ ┣ logo192.png
┃ ┣ logo512.png
┃ ┣ manifest.json
┃ ┗ robots.txt
┣ src/
┃ ┣ components/
┃ ┃ ┣ common/
┃ ┃ ┃ ┣ carousel.js
┃ ┃ ┃ ┣ catogies.js
┃ ┃ ┃ ┣ header.js
┃ ┃ ┃ ┣ sports.js
┃ ┃ ┃ ┗ topTech.js
┃ ┃ ┣ category.js
┃ ┃ ┣ details.js
┃ ┃ ┗ home.js
┃ ┣ images/
┃ ┣ redux/
┃ ┃ ┣ actions/
┃ ┃ ┃ ┗ newsActions.js
┃ ┃ ┣ reducers/
┃ ┃ ┃ ┗ newsReducers.js
┃ ┃ ┗ types/
┃ ┃   ┗ newsTypes.js
┃ ┣ route/
┃ ┃ ┗ route.js
┃ ┣ __testing__/
┃ ┃ ┗ newsActions.test.js
┃ ┣ App.css
┃ ┣ App.js
┃ ┣ App.test.js
┃ ┣ index.css
┃ ┣ index.js
┃ ┣ logo.svg
┃ ┣ reportWebVitals.js
┃ ┣ setupTests.js
┃ ┗ store.js
┣ .gitignore
┣ news_update.zip
┣ package-lock.json
┣ package.json
┗ README.md
 ```
