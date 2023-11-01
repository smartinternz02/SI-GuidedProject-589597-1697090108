# SI-GuidedProject-589596-1697090072

# Machine Learning Model for Occupancy Rates and Demand Prediction

## Overview
This project is aimed at building a machine learning model to predict occupancy rates and demand in the hospitality industry. The model takes into account various environmental and temporal features to make predictions.

## Dataset
The dataset used for this project includes the following attributes:
- Temperature
- Humidity
- CO2 (Carbon Dioxide levels)
- Light
- Humidity Ratio
- Year
- Month
- Day

## Project Structure
The project is organized as follows:
- `data/`: Contains the dataset used for training and testing the model.
- `static/`: Includes static files like images for the web application.
- `templates/`: Contains HTML templates for the web application.
- `app.py`: The Flask application that integrates the machine learning model with a web interface.
- `ML-occupancy-rates.pkl`: A pre-trained machine learning model (Decision Tree) saved as a pickle file.
- `index.html`: The HTML form for user input.
- `home.html`: The HTML page for displaying predictions.

## Model Building
The machine learning model is built using the scikit-learn library. We use a Decision Tree classifier for this project. The model is trained using the features (temperature, humidity, CO2, light, humidity ratio) and the target variable (occupancy).

## Web Integration
The model is integrated into a web application using Flask. Users can input values for the attributes mentioned above, and the model will predict whether the space is occupied or not.

## Usage
1. Clone the repository to your local machine.
2. Install the required Python packages using `pip install -r requirements.txt`.
3. Run the Flask application: `python app.py`.
4. Access the web application in your browser by visiting `http://localhost:5000`.

## Web Interface
- The web interface, accessible at the root URL, provides an input form for users to enter attribute values.
- Upon form submission, the model predicts occupancy and displays the result on the web page.

## Acknowledgments
- Special thanks to the scikit-learn and Flask communities for their excellent documentation and resources.

## License
This project is open-source and available under the [MIT License](LICENSE).

