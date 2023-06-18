# Parsume

## A faster way to sift through hundreds of resumes

Are you a recruiting manager that is sick and tired of having to look through thousands, even millions of resumes? Do you wish there was an easier way to sift through all the applicants to find the perfect one? That is where Parsume comes in.

* Quick and effective parsing of resumes based on desired traits and keywords
* Simple and effective ranking system, which puts the best applicants on top
* Robust user authentication, ensuring that none of your data ever gets breached

Check out the site here: https://resume-parser-project.vercel.app/signin

## Technologies used:
* React (Javascript)
* Flask (Python)
* NLTK
* MongoDB

## How to use

Coming soon

## How to tweak this project for yourself

1. Download the frontend and backend repositories (backend repo linked above).
2. Slot in the required environment variables for their respective repositories. Make sure you use a .env file for the backend and a .env.local file for the frontend.
3. Run pip install requirements.txt in the backend and npm install in the frontend to install all project dependencies
4. Run python run.py in the backend and npm start in the frontend

For database access, you can either create your own mongodb database and plug in your connection URI or you can manipulate the project files so you can use your database of choice. 

### Environment Variables Needed:

Backend:

* ```PORT``` = Your port number of choice (anything but 3000)
* ```MONGODB_URI``` = The connection URI to your MongoDB database
* ```JWT_SECRET_KEY``` = You can go to an online password generator and slot your value in here

Frontend:

* ```REACT_APP_API_URL``` = your server link, whether it's deployed or on localhost

## Find a bug?
If you found an issue or would like to submit an improvement to this project, please submit an issue using the issues tab above. If you would like to submit a Pull Request with a fix, reference the issue that you created.

## Q & A

### Why does logging in for the first time take a very long time?

The deployed server shuts down whenever the page is not being used by anyone. It takes a bit of time for the server to reboot for the first time. The server is also based in Ohio and is on a free plan, so the connection may not be optimal and the CPU is a bit limited at the moment. Also worth nothing that the backend was coded in Python, so it will take much longer than if it was coded in any other language.
