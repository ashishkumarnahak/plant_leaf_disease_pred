# plant_leaf_disease_pred
A web-based deep learning system to detect and classify diseases in plant leaves using image data. This tool allows users to upload an image of a leaf and returns a diagnosis (healthy vs diseased), helping farmers, gardeners, and researchers monitor crop health and take timely action.

🔍 Features
Trained convolutional neural network model for classifying plant leaf images into disease or healthy categories
Image preprocessing, normalization, and augmentation to improve model robustness
Web interface built using Flask (or your framework) for real-time image upload and disease prediction
Model persistence with saved architecture (.json) and weights (.h5) files
Easy to setup and deploy; requirements specified via requirements.txt
🛠️ Technologies Used
Technology	Purpose
Python	Core language for model development and backend logic
TensorFlow / Keras	Building, training, and evaluating the deep learning model
Flask	Web backend for serving the model and handling user image uploads
HTML/CSS/JavaScript	Frontend for the upload + result display pages
Image Processing	Resizing, normalization, augmentation to improve model generalization
📁 Project Structure
├── Dataset/ # Images used to train and validate the model ├── static/ # Static files (CSS, JS, images) for web interface ├── templates/ # HTML templates for the web pages ├── Training.py # Script to train the deep learning model ├── Example.py # Example usage / demo of model inference ├── leaf.py # Main script for running predictions on input images ├── model.h5 # Trained model weights file ├── model1.json # Model architecture in JSON format ├── my_model_weights.h5 # Alternative / latest weights file ├── requirements.txt # Python dependencies

⚙️ Setup & Installation
Clone the repository:
git clone https://github.com/ashishkumarnahak/Plant-Leaf-Disease-Prediction.git
cd Plant-Leaf-Disease-Prediction

Create a virtual environment and activate it (optional but recommended):
---bash python3 -m venv venv source venv/bin/activate #on windows: venv\scripts\activate
Install dependencies: bash pip install -r requirements.txt
4.Run the model training (if needed): bash python Training.py 5.To start the web app and test prediction: bash python leaf.py 6. Open your browser and go to:

http://localhost:5000
