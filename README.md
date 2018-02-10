# stock-watch
MERN Stack Single-Page-Application with Web Sockets to display graphic representations of stock data

This application is a visual representation of historical as well as near-real-time data from the Investors Exhange.
[IEX API](https://iextrading.com/). 

User can search from over 8500 stock listings to view a particular stock's performance over the past 12 months and compare it to any other number of stocks.

## Features

#### Stock Ticker
The page has a running ticker that cycles through the stock prices of the previous trading period at the close of business.

#### Stock Chart 
Add stocks using the Stock Search and hover over the chart to get a readout of the stock value at the close of business on a given day.

#### Stock Search 
Autofilled Search Bar of all the listings in the IEX database. Works best when searching by Company Name. You can search by Stock Symbol, but be prepared to have to scroll to find the particular symbol.

#### Stock Cards 
Color-coded cards to match the chart, includes the most recent trading price (within the hour, or day, if after hours), the name of the CEO, description of the company and a link to their website.

## Technology

* React - the front-end was built with `create-react-app`, `react-chartjs-2` for the chart, `moment` for representing time, `isomorphic-fetch` for making front-end api calls, `redux` for state management, and `socket.io` for managing state across instances.

* MongoDB - the backend is only used for persisting state over time across instances. Using Node.js api.

* Node + Express + Socket.io - keeping it real on the back end with node.


