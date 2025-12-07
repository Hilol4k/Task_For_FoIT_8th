# Task_For_FoIT_8th
This is a repository made for 8th task of Fundamentals of IT and will be connected to "render dot com"
# How to run the project locally (on your own computer)
1. Install Python
Download Python (version 3.10+) if you don't have it.

During installation, check the box "Add Python to PATH".

2. Clone your repository

Open the terminal (or PowerShell/Command Prompt) and type:

\```Bash
git clone https://github.com/<your-username>/<repository-name>.git
cd <repository-name>
\```

3. Create a virtual environment

\```Bash
python -m venv venv
\```

Activate it:

Windows:

\```Bash
venv\Scripts\activate
\```

macOS/Linux:

\```Bash
source venv/bin/activate
\```

4. Install dependencies

\```Bash
pip install -r requirements.txt
\```

5. Run the application

\```Bash
python app.py
\```

Now open your browser and go to http://localhost:5000.

You will see your page.

# How to deploy on Render.com

1. Prepare the repository

Make sure you have:

\```
app.py (the main file)
\```
\```
requirements.txt (list of dependencies)
\```
\```
README.md
\```

2. Go to Render.com

Visit Render.com.

Sign up (you can do it through GitHub).

3. Create a new service

Click New + → Web Service.

Select your GitHub repository.

Set parameters

Environment: Python 3.

Build Command:

\```
pip install -r requirements.txt
\```

Start Command:

\```
gunicorn app:app
\```

(if your Flask application is called app inside app.py).

5. Run the deployment

Click Create Web Service.

Wait while Render builds the project.

At the end, a link will appear like:

\```
https://service-name.onrender.com
\```

Check  

Follow the Render link.  

Make sure the form works (for example, enter a number and get a result).

Link for the website: https://task-for-foit-8th.onrender.com/
