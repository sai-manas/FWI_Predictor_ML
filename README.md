# Fire Weather Index (FWI) Prediction for Algerian Forest Fires using Multiple Linear Regression

## Description
FWI predictor application will predict the Fire Weather Index 


## Screen Recording of FWI predictor application deployed on aws
https://github.com/sai-manas/FWI_predictor_WebApp_ML/assets/106865226/92900578-282b-458f-8e9d-954a5a0ffcb0

## How to use
> This web application can be hosted using Flask or deployed on AWS
### Flask
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

### AWS (ELastic Beanstalk,Code Pipeline)
1. **Fork the GitHub Repository:**
   - Click the "Fork" button in the top-right corner of this repository's page.
   - This action will create a copy of my repository under your GitHub account.
   - Use this as a source for deploying application in AWS

2. **Deploy application using ELastic Beanstalk and Code Pipeline in AWS**
   - Follow the steps in this Article for deploying Web application in AWS. URL - https://dev.to/wardaliaqat01/cicd-pipeline-hands-on-aws-code-pipeline-elastic-beanstalk-github-35n3
