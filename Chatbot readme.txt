File Question and Answer App

This is a web application that allows users to upload files and search for specific content within them. The application uses OpenAI's GPT-3.5 language model to generate answers to user queries related to the uploaded files.

Prerequisites
Before setting up and running the application, make sure you have the following:

Python 3 (version 7 to version 10) installed on your computer
An OpenAI API key
A Pinecone API key and index name
Node.js and npm installed on your computer
Installation
To install and run the application, follow these steps:

Download the source code from the GitHub repository: https://github.com/openai/openai-cookbook

Unzip the downloaded file to a directory on your computer.

Open the server directory in a PowerShell window and fill out the config.yaml file with your Pinecone API key, index name, and environment.

Install the required Python and Node.js dependencies using the following commands:

pip install openai
npm install openai
Create a virtual environment for the server by running the following commands:

python -m venv venv
.\venv\Scripts\activate
pip install -r .\requirements.txt
pip install python-dotenv
Start the Flask server by running the following command:

python .\app.py
Open a new PowerShell window and navigate to the client directory.

Install the required Node.js dependencies by running the following command:


npm install
Start the Next.js client by running the following command:


npm run dev
Open a web browser and navigate to http://localhost:3000 to access the application.
Usage
To use the application, follow these steps:

Upload a file using the "Choose File" button.

Once the file is uploaded, enter a question related to the content of the file in the search bar.

Click on the "Search" button to generate an answer to your question.

Limitations
Please note that the application may sometimes generate answers that are not in the uploaded files or provide inaccurate results.

License
This application is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
This application was developed using OpenAI's GPT-3.5 language model and Pinecone's similarity search service. Thanks to both teams for their excellent work!