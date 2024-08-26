

---

# StockChatBot Overview

**StockChatBot** is a PyQt5-based application that allows users to interact with stock market data through a chat interface. The bot provides options to view stock prices, analyze historical data, and make predictions using machine learning models. It visualizes stock data using candlestick charts and allows users to explore detailed charts with additional features.

## Installation

To set up the StockChatBot application, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone <repository-url>
   cd StockChatBot
   ```

2. **Create a Virtual Environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies:**
   Ensure you have `pip` installed and then run:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Application:**
   ```bash
   python stock_market_pred.py
   ```

## Usage

1. **Starting the Application:**
   Launch the application using the command above. The main window will display the chat interface.

2. **Interacting with the Bot:**
   - **Choose a Stock Ticker:** Click on one of the predefined ticker buttons or type a ticker symbol into the input field and press Enter or click the send button.
   - **Choose Actions:** Once a ticker is selected, choose from available actions such as viewing current prices, selecting periods for historical data, or predicting future prices.
   - **View Charts:** The application will switch to a graph view where stock prices and volumes are visualized using candlestick charts.

3. **Detailed Analysis:**
   - After viewing a chart, click the "Show Details" button to switch to a detailed analysis with additional data visualization. Click "Back to Normal" to return to the standard view.

## Dependencies

The application requires the following Python packages:

- `PyQt5`: For the GUI elements.
- `yfinance`: To fetch stock data.
- `matplotlib`: For plotting charts.
- `sklearn`: For machine learning models.
- `pandas`: For data manipulation.
- `numpy`: For numerical operations.

These dependencies are listed in the `requirements.txt` file. Make sure to install them using `pip`.

## How It Works

1. **GUI Setup:**
   - The application uses PyQt5 to create a window with two main views: a chat interface and a graph view.
   - The chat interface allows users to interact with the bot, while the graph view displays stock data charts.

2. **Stock Data Retrieval:**
   - Stock data is retrieved using the `yfinance` library, which fetches historical and current stock data based on user inputs.

3. **Data Visualization:**
   - `matplotlib` is used to create candlestick charts and other visualizations. The charts are displayed in a scrollable area to accommodate large datasets.

4. **Machine Learning Prediction:**
   - The application uses a Linear Regression model from `sklearn` to predict future stock prices based on historical data.

5. **Dynamic Updates:**
   - The application dynamically updates the chat and graph views based on user interactions and choices.

## Error Handling

- **Data Retrieval Errors:** If stock data cannot be fetched (e.g., due to an invalid ticker or network issues), the bot will display an error message in the chat interface.
- **Plotting Errors:** If there are issues with generating plots, such as missing data or incorrect formats, the bot will notify the user and handle exceptions gracefully.
- **Machine Learning Errors:** Errors in the prediction process are captured and reported, ensuring that the application does not crash unexpectedly.

In case of any issues, check the console output for detailed error messages and ensure that all dependencies are correctly installed.

---

## Working





