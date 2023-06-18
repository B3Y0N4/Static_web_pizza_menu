# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

# Static Web App Pizza Menu Representation

This project is a React application that represents a fictional pizza restaurant called "Fast AJ Pizza Co." It provides a menu of pizzas with their names, ingredients, prices, and photos. The application also includes a header and a footer that display additional information.

The pizzaData array contains information about various pizzas offered by the restaurant. Each pizza object in the array includes properties such as name, ingredients, price, photo name, and a flag indicating if it is sold out.

The main component, App, renders the overall structure of the application. It includes the Header, Menu, and Footer components within a container.

The Header component renders the restaurant's name using a styled heading element. The style is customizable using the style object, although it is currently empty.

The Menu component displays the menu section. It starts by checking if there are pizzas available (numPizzas > 0). If there are pizzas, it renders a description of the restaurant and an unordered list (ul) of pizzas using the Pizza component. Each pizza is mapped from the pizzaData array and passed as a prop to the Pizza component.

The Pizza component represents an individual pizza item in the menu. It renders an li element containing an image of the pizza, its name, ingredients, and price. If the pizza is sold out (pizzaObj.soldOut is true), it applies a CSS class of "sold-out" to the li element.

The Footer component represents the footer section of the application. It checks the current hour and determines if the restaurant is open based on the opening and closing hours (openHour and closeHour). If the restaurant is open, it renders the Order component, which displays a message about the opening hours and an order button. Otherwise, it displays a message indicating the opening hours.

The Order component is a simple component that renders a message about the opening hours and an order button.

Finally, the ReactDOM.createRoot function is used to render the App component within the root element with the id "root" on the HTML page.

Overall, this project creates a static representation of a pizza restaurant's menu using React components and displays additional information in the header and footer sections.
