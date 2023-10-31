** Travel Time Predictor - Travelia **
```markdown
# Travel Time Predictor - Travelia

## Overview

Travelia is a web application that predicts travel time between two cities based on distance, utilizing a probabilistic model. The application employs a custom API for distance information and includes a unique API key for secure access.

## Features

- **Travel Time Prediction:** Predict travel time by considering the distance and adjusting it using a probabilistic model.

- **Traffic Conditions:** Account for traffic conditions by adjusting travel time based on the desired departure time, considering traffic fluctuations throughout the day.

- **Custom API Key:** Secure access to the distance information API with a custom API key, ensuring controlled usage.

## How to Use

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/akshit2941/travel-time-predictor.git
   cd travel-time-predictor
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application:**
   ```bash
   python main.py
   ```

   The application will be accessible at http://127.0.0.1:5000.

4. **Access Travel Time Prediction:**
   Open a web browser and navigate to http://127.0.0.1:5000. Enter the starting city, destination city, and desired departure time to get the predicted travel time.

5. **API Documentation:**
   The application provides a simple API for travel time prediction. Use the following endpoint:

   - **Endpoint:** /time
   - **Method:** GET
   - **Parameters:**
     - city1 (Starting city)
     - city2 (Destination city)
     - desired_time (Desired departure time in the format %H:%M)

   **Example Request:**
   ```http
   GET http://127.0.0.1:5000/time?city1=CityA&city2=CityB&desired_time=08:30
   ```

   **Example Response:**
   ```json
   {
     "city1": "CityA",
     "city2": "CityB",
     "distance": 200,  
     "predicted_time": 2.5  
   }
   ```

   **API Key:**
   To use the API, include the custom API key in the request headers:

   ```http
   GET http://127.0.0.1:5000/time?city1=CityA&city2=CityB&desired_time=08:30
   ```

## License
This project is licensed under the MIT License.
```

Feel free to use this as your README file for the Travel Time Predictor - Travelia project on GitHub.
