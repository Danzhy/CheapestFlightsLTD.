# Flight Finder Application

## Overview
This application allows users to find the cheapest flight options departing from their chosen origin city or airport. Users input their desired origin using the IATA code, and the program fetches data on the five most affordable flights from that location. Additionally, users can input their preferred currency, and the program will convert the flight prices into that currency using real-time exchange rates. This feature is designed to provide budget-conscious travelers with an easy way to explore flight options while ensuring prices are displayed in the currency of their choice.

## APIs Used
The application integrates two APIs: the [Amadeus API](https://developers.amadeus.com/) for flight ticket data and the [Currencybeacon API](https://currencybeacon.com/) for currency conversion. The Amadeus API was chosen for its ability to provide detailed flight information, including destination, price, and departure and return dates. The Currencybeacon API was incorporated to offer users the flexibility of viewing flight prices in their preferred currency, ensuring a user-friendly experience. These two APIs complement each other, allowing the app to deliver both flight and currency conversion information seamlessly.

## Instructions for Use
1. Upon running the application, the user is prompted to input their desired currency (e.g., USD, EUR, AED).
2. After selecting the currency, the user will enter the IATA code of their origin city or airport.
3. The application will retrieve and display the five cheapest flights from that location, with prices converted into the selected currency.
4. If an invalid IATA code or non-existent currency is entered, the user will be prompted to try again, ensuring smooth and error-free execution.

## Setup
To use this application, you need to have valid API keys for both the Amadeus API and the Currencybeacon API. These keys are required to authenticate your requests and access the respective services. For the Amadeus API, you must obtain an API key and API secret, which are then used to generate an access_token by making a POST request to the Amadeus OAuth endpoint. This access_token is necessary for making subsequent requests to fetch flight data. 
 The Currencybeacon API key is used to authenticate your requests for currency conversion. Make sure to securely store these keys, as they are required to access the API services in the program. Before running the application, ensure that both API keys are set up and available in your environment.
