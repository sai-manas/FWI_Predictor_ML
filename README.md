# Fire Weather Index (FWI) Web App Predictor: Algerian Forest Fires dataset

## Overview

FWI predictor web application predicts the Fire Weather Index (FWI) for Algerian forest fires using various regression models, including Ridge Regression, Lasso Regression, Linear Regression, and ElasticNet. The model selection process involved thorough comparison and cross-validation, ultimately determining Ridge Regression as the optimal choice due to its superior accuracy. 

The model is trained on a dataset encompassing two regions of Algeria—Bejaia in the northeast and Sidi Bel-abbes in the northwest. The dataset spans from June to September 2012 and includes various weather-related attributes such as temperature, relative humidity, wind speed, rain, and components of the FWI system.

## Jupyter Notebook

The detailed analysis and code implementation are available in the [Jupyter notebook](https://github.com/sai-manas/FWI_Predictor_ML/blob/main/notebook/Algerian_forest_ML_project.ipynb).

## Screen Recording of FWI predictor application deployed on aws
https://github.com/sai-manas/FWI_Predictor_ML/assets/106865226/13fbea64-b82c-47c8-a82f-062f80e9422d

## Dataset Information

- **Instances:** 244 (122 for each region)
- **Attributes:** 11 weather-related attributes and 1 output attribute (FWI)

## Technologies Used

- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn , Pickle, Warnings
- **Web Framework:** Flask
- **Frontend:** HTML, CSS
- **Deployment:** AWS Elastic Beanstalk, AWS CodePipeline

## Data Cleaning and Preprocessing

The dataset underwent rigorous cleaning, addressing missing values, mispaced entries, and data type conversions. Regions were added as a new column, and unnecessary features were dropped. Categorical values were cleaned, and the dataset was saved as a cleaned CSV file.

## Exploratory Data Analysis (EDA)

EDA was performed to analyze the distribution of fires across different months and regions. August emerged as the month with the highest number of fires in both regions. Visualization tools like box plots, count plots, and correlation matrices were employed to derive insights.

## Feature Engineering and Model Development

Feature selection based on correlation was conducted to identify highly correlated features, and multicollinearity was addressed by dropping correlated columns. The data was split into training and testing sets, and features were standardized using StandardScaler. Various regression models, including Ridge, Lasso, Linear Regression, and ElasticNet, were compared, and Ridge Regression was selected based on superior accuracy and generalization.

## Model Evaluation

The model's performance was evaluated using metrics such as Mean Absolute Error (MAE) and R2 Score. The Ridge Regression model exhibited promising results, providing valuable insights into FWI prediction for forest fire risk assessment.

## Web App Deployment

To make the model accessible, I developed a web application using Flask, a Python web framework. 

The application is deployed on AWS Elastic Beanstalk, with continuous integration and deployment facilitated by AWS CodePipeline.

## How to use

### I. Notebook Usage
   - Explore notebook to understand the implementation and evaluation of different regression models, along with data visualization

> Hosted this web application using Flask and deployed on AWS
### II. Flask
1. **Clone the GitHub Repository:**
   - Open your terminal or command prompt.
   - Navigate to the directory where you want to clone the repository.
   - Run the following command to clone my GitHub repository:
     ```
     git clone https://github.com/my-username/my-repo.git
     ```
   - Replace `my-username` with my GitHub username and `my-repo` with the name of my repository.
     
2. **Install Python:**
   - If you haven't already, make sure you have Python installed on your system. You can download it from the official Python website (https://www.python.org/downloads/) and follow the installation instructions for your operating system.
     
3. **Create a Virtual Environment (Optional but recommended):**
   - It's a good practice to create a virtual environment to isolate the dependencies of your project. You can create a virtual environment using the following command:
     ```
     python -m venv venv
     ```
4. **Activate the Virtual Environment (Optional but recommended):**
   - Activate the virtual environment using the appropriate command based on your operating system:
     - On Windows:
       ```
       venv\Scripts\activate
       ```
     - On macOS and Linux:
       ```
       source venv/bin/activate
       ```
5. **Install Required Packages:**
   - Navigate to the root folder of your cloned repository.
   - Run the following command to install the required Python packages listed in the `requirements.txt` file:
     ```
     pip install -r requirements.txt
     ```
6. **Run the Flask Application:**
   - Once the packages are installed, you can start your Flask application. In your repository's root folder, you should typically have a file named `application.py`, which is the main Flask application file.
   - Run the application with the following command:
     ```
     python application.py
     ```
7. **Access the Application:**
   - Your Flask application should now be running. You can access it in your web browser by navigating to `http://localhost:5000` or the URL provided by your application.

### III. AWS (ELastic Beanstalk,Code Pipeline)
1. **Fork the GitHub Repository:**
   - Click the "Fork" button in the top-right corner of this repository's page.
   - This action will create a copy of my repository under your GitHub account.
   - Use this as a source for deploying application in AWS
     
2. **Deploy application using ELastic Beanstalk and Code Pipeline in AWS**
   - Follow the steps in this Article for deploying Web application in AWS. URL - https://dev.to/wardaliaqat01/cicd-pipeline-hands-on-aws-code-pipeline-elastic-beanstalk-github-35n3
