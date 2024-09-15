# Currency-Convertor-Application
This is a simple currency converter app built using Python and Streamlit. It allows you to convert from one currency to another with real-time exchange rates.The currency converter app is built using the Streamlit framework and the forex_python library, which allows the app to retrieve exchange rates between various currencies.
The app starts by creating a currency converter object using the CurrencyRates() class. Then,
it defines a function called convert_currency() that takes three arguments - the amount to
convert, the currency to convert from, and the currency to convert to. This function uses the
get_rate() method of the currency converter object to retrieve the exchange rate between the
two currencies, and then multiplies the amount to convert by this exchange rate to calculate the
converted amount.
If there is an error retrieving the exchange rate (for example, if one of the specified currencies
is not supported), the function returns None and displays an error message using the write()
method of the Streamlit framework.
The Streamlit app defines a UI with two dropdown menus to select the currencies to convert
from and to, and a text input to specify the amount to convert. When the "Convert" button is
clicked, the app calls the convert_currency() function with the specified inputs and displays the
result using the write() method.
Finally, the name variable is checked to ensure that the app is being run directly (as opposed to
being imported as a module), and if so, the app() function is called to run the Streamlit app.
