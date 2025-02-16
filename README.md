HARVESTIFY 🌿 
A simple ML and DL based website which recommends the best crop to grow, fertilizers to use and the diseases caught by your crops.
This project is featured on Krish Naik's YouTube Channel => Check it out here
DISCLAIMER ⚠️
This is a POC(Proof of concept) kind-of project. The data used here comes up with no guarantee from the creator. So, don't use it for making farming decisions. If you do so, the creator is not responsible for anything. However, this project presents the idea that how we can use ML/DL into precision farming if developed at large scale and with authentic and verified data.

MOTIVATION 💪
Farming is one of the major sectors that influences a country’s economic growth.

In country like India, majority of the population is dependent on agriculture for their livelihood. Many new technologies, such as Machine Learning and Deep Learning, are being implemented into agriculture so that it is easier for farmers to grow and maximize their yield.

In this project, I present a website in which the following applications are implemented; Crop recommendation, Fertilizer recommendation and Plant disease prediction, respectively.

In the crop recommendation application, the user can provide the soil data from their side and the application will predict which crop should the user grow.

For the fertilizer recommendation application, the user can input the soil data and the type of crop they are growing, and the application will predict what the soil lacks or has excess of and will recommend improvements.

For the last application, that is the plant disease prediction application, the user can input an image of a diseased plant leaf, and the application will predict what disease it is and will also give a little background about the disease and suggestions to cure it.

DATA SOURCE 📊
Crop recommendation dataset (custom built dataset)
Fertilizer suggestion dataset (custom built dataset)
Disease detection dataset
Notebooks 📓
I have also published the corresponding code on Kaggle Notebooks.
Crop Recommendation
Disease Detection
Built with 🛠️
       

    

DEPLOYMENT 🚀
Deployment is done using deploy branch
This website is deployed at Heroku
You can access it here
Note: The website may take a minute to load sometimes, as the server may be in hibernate state
How to use 💻
Crop Recommendation system ==> enter the corresponding nutrient values of your soil, state and city. Note that, the N-P-K (Nitrogen-Phosphorous-Pottasium) values to be entered should be the ratio between them. Refer this website for more information. Note: When you enter the city name, make sure to enter mostly common city names. Remote cities/towns may not be available in the Weather API from where humidity, temperature data is fetched.

Fertilizer suggestion system ==> Enter the nutrient contents of your soil and the crop you want to grow. The algorithm will tell which nutrient the soil has excess of or lacks. Accordingly, it will give suggestions for buying fertilizers.

Disease Detection System ==> Upload an image of leaf of your plant. The algorithm will tell the crop type and whether it is diseased or healthy. If it is diseased, it will tell you the cause of the disease and suggest you how to prevent/cure the disease accordingly. Note that, for now it only supports following crops

Supported crops
How to run locally 🛠️
Before the following steps make sure you have git, Anaconda or miniconda installed on your system
Clone the complete project with git clone https://github.com/Gladiator07/Harvestify.git or you can just download the code and unzip it
Note: The master branch doesn't have the updated code used for deployment, to download the updated code used for deployment you can use the following command
❯ git clone -b deploy https://github.com/Gladiator07/Harvestify.git 
deploy branch has only the code required for deploying the app (rest of the code that was used for training the models, data preparation can be accessed on master branch)
It is highly recommended to clone the deploy branch for running the project locally (the further steps apply only if you have the deploy branch cloned)
Once the project is cloned, open anaconda prompt in the directory where the project was cloned and paste the following block
conda create -n harvestify python=3.6.12
conda activate harvestify
pip install -r requirements.txt
And finally run the project with
python app.py
Open the localhost url provided after running app.py and now you can use the project locally in your web browser.
