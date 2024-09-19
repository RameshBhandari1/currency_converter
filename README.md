**Currency Converter Project Documentation**

Overview

The Currency Converter is a web application that allows users to convert amounts between different currencies using real-time exchange rates from the Free Currency API. The application features a user-friendly interface, enabling easy selection of currencies and displaying conversion rates dynamically.


**Table of Contents**

Features

Technologies Used

Installation

Usage

Code Structure

API Integration

Event Flow

Styling




**Features**

User can select base and target currencies.
Real-time conversion rates are displayed.
Currency list can be filtered for easier selection.
Swapping between base and target currencies is straightforward.
Responsive design suitable for various devices.



**Technologies Used**

HTML5: Structure of the web application.
CSS3: Styling of the application using modern design principles.
JavaScript: Functionality and interactivity.
API: Integration with the Free Currency API for fetching currency data and exchange rates.

**Installation**

Clone the repository:

bash

Copy code

git clone https://github.com/RameshBhandari1/currency_converter.git

cd currency-converter

Open the index.html file in your preferred web browser.




**Usage**

Enter an amount in the base currency input field.

Select the desired base currency by clicking the corresponding button.

Open the currency drawer to search for and select the target currency.

The converted amount will be displayed in the target currency input field, along with the current exchange rate.




**Code Structure**

index.html: Main HTML file containing the app structure.

style.css: Stylesheet for the application, defining layout and design.

script.js: JavaScript file containing logic for fetching data, handling user interactions, and updating the UI.

Key JavaScript Functions

initApp: Initializes the application, fetching currency data and exchange rates.

showDrawer: Displays the currency selection drawer.

hideDrawer: Hides the currency selection drawer.

filterCurrency: Filters the currency list based on user input.

calculateRate: Calculates the conversion rate based on user input.

fetchCurrencies: Fetches the list of available currencies from the API.

fetchExchangeRate: Fetches current exchange rates for the selected base currency.




**API Integration**

The application utilizes the Free Currency API for fetching currency information and exchange rates. The API key is required for authentication. Replace const key = "your_api_key"; with your actual API key.



**API Endpoints**

Get Currencies:

GET https://api.freecurrencyapi.com/v1/currencies?apikey={key}

Get Exchange Rates:

GET https://api.freecurrencyapi.com/v1/latest?apikey={key}&currencies=&base_currency={baseCurrency}




**Event Flow**

The app initializes and fetches currency data and exchange rates.

User interacts with the UI:

Clicks to open the currency drawer.

Types to filter currencies.

Selects a currency pair.

Enters an amount to convert.

The app updates the displayed conversion rates based on user input.




**Styling**

The application uses CSS variables for easy theme management. The layout is responsive, with a clean, modern design that enhances user experience. Material icons are used for interactive elements like buttons.
