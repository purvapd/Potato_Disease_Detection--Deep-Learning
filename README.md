# Potato_Disease_Detection--Deep-Learning

## Problem statement 

**The project aims to develop a deep learning model to classify potato crops into three categories: 'Potato___Early_blight',
'Potato___Late_blight', and 'Potato___healthy'. Early and late blights are common diseases that cause significant crop 
yield and quality losses.**
	
Clone my Github repository on your local system :- https://github.com/purvapd/Potato_Disease_Detection--Deep-Learning

### To create a deep learning model, follow these steps:

Step 1: Install Anaconda
https://docs.anaconda.com/anaconda/install/windows/

Step 2: Launch Jupyter Notebook

Step-3: Open the potato_disease_detection\training\training_model.ipynb notebook 

Step-4:	Run each cell

At the end of this step you will get the CNN model  version 1 in the folder 
potato_disease_detection\saved_models\1

### Create Fast API

1. Open the "potato_disease_detection\api" directory.

2. Install the necessary packages by running the command 
	
		pip install -r requirements.txt

3. Open Visual Studio Code and make sure the terminal path is set to "potato_disease_detection\api".

4. Install the uvicorn package and Run the Fast API by running the command 

		pip install uvicorn

		uvicorn main:app --reload

5. To check if the API is working or not, you can use Postman by installing it from the link provided
(https://learning.postman.com/docs/getting-started/installation-and-updates/).

6. In Postman, use the following credentials to test the API:
	
		URL: http://localhost:8000/predict

		Type: POST

		Body:

		Key: file (select file type only)

		Value: Select an image of a potato leaf as a file.

		You will receive a response as follows:

		{

		"class": "Late_blight",

		"confidence": 0.9994027614593506

		}
	
###  Run website:-
1. Install nodejs 
https://nodejs.org/en/download

2. make sure the terminal path is set to "potato_disease_detection\frontend".

		Install the packages 

		pip install npm

		npm install --from-lock-json

		npm audit fix

3. Make sure FAST API is running. Now to run the website 
npm run start
	
