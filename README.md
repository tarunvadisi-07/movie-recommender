# 🎬 movie-recommender
A Simple and interactive movie recommendation website that helps users discover movies similar to the ones they enjoy.
## About the Project
Finding a good movie to watch can sometimes be difficult when there are so many options available.This project makes that process easier by suggesting movies based on the movie selected by the user.
The Movie Recommender System is devloped using Python and Machine Learning Concepts.It follows a Content-Based Filtering approach to find movies with similar characteristics.
Users simply enter a movie name, and the sysytem displays five similar movies through a user-driendly web interfaces.
## Features
- Search for movies using thier titles.
- Get five similar movie recommendations.
- Content-based movie recommendations.
- Uses generes,keywords,overview,cast and director.
- simple and user-friendly interface.
- FastAPI backened for handling requests.
- Displays messages when a movie is not found or the server is unavailable.

## Technologies Used
Python - Main Programming language<br>
Pandas - Loading and processing movie datasets<br>
NumPy - Numerical operations<br>
Scikit-learn - Text vectorization and similarity calculation<br>
FastAPI - Devloping the backend API<br>
HTML - Creating the webpage structure<br>
CSS- Styling the website<br>
JavaScript - Handling search and communicating eith the backend<br>

## How it works
1.Dataset Loading - Movie informaton and credits are loaded from CSV files.
2.Data preprocessing - Unnecessary information is removed and useful details are extracted.
3.Feature Extraction - Selected movie information is combined into a single text feature called tags.
4.Text Vectorization - CountVectorizer converts the text information into numerical vectors.
5.Similarity Calculation - Cosine Similarity compares the movie vectors.
6.Recommendations - The system finds and displays the five most similar movies.

## Requirments
- python 3.9
- Git
- VS code
- A Web browser
The movie dataset CSV files must also be available inside the public folder.

## How to Run the Project
Follow these steps to run the project on your local computer.
### Step 1: Clone the Repository
Open PowerShell or the VS Code terminal and run:
```bash
git clone https://github.com/tarunvadisi-07/movie-recommender.git
```
Move into the project directory:
```bash
cd movie-recommender
```
### Step 2: Open the Project in VS Code
```bash
code .
```

### Step 3: Create a Virtual Environment
Create a virtual environment to manage the Python libraries required by the project.
```powershell
python -m venv venv
```
### Step 4: Activate the Virtual Environment
For Windows PowerShell, run:
```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```
- Then activate the environmet:
```powershell
.\venv\Scripts\Activate.ps1
```
For Windows Command Prompt (CMD), use:
```cmd
venv\Scripts\activate.bat
```
For macOS or Linux, use:
```bash
source venv/bin/activate
```
After successful activation, you should see (venv) at the beginning of your terminal line.
### Step 5: Install Required Libraries
Install all the dependencies listed in `requirements.txt`:
```bash
python -m pip install --upgrade pip
```
Wait until the installation is complete.
### Step 6: Check the Project Structure
Make sure your project contains the following files and folders:

```text
movie-recommender/
│
├── api/
│   └── main.py
│
├── public/
│   ├── tmdb_500_movies_subset.csv
│   └── tmdb_500_credits_subset.csv
│
├── index.html
├── server.py
├── requirements.txt
└── README.md
```
### Step 7: Run the Application
Make sure you are in the main project directory and execute:
```bash
pip install -r requirements.txt
```
### Step 8: Open the Website
Open your web browser and visit:
```text
http://localhost:10000
```
The Movie Recommender System homepage should now appear.

### Step 9: Search for Movies
1. Enter a movie title in the search box.
2. Click the **Search** button.
3. The system processes the selected movie.
4. Five similar movie recommendations will be displayed on the webpage.
You can try titles such as `Avatar`, `Titanic` or `The Dark Knight`, provided they are available in the dataset.

### Step 10: Access API Documentation
The project uses FastAPI for backend operations.
You can access the API documentation at:
```text
http://localhost:10000/api/docs
```
### Step 11: Stop the Application

To stop the server, return to the terminal and press:

```text
CTRL + C
```

## Common Issues
**1. Python is not recognized**
Check whether Python is installed:
```bash
python --version
```
**2. Module not found error**
Install the required packages again:
```bash
pip install -r requirements.txt
```
**3. Dataset not found**
Make sure both CSV files are present inside the `public` folder and their filenames match the names used in the Python code.
**4. Website is not opening**
Check whether the server is running successfully in the terminal. Then open:
```text
http://localhost:10000
```
**5. Movie not found**
The current system uses an exact movie title match. Make sure the entered movie title is available in the dataset.

## Future Improvements
Some features that can be added in future versions include:
- Movie posters and ratings.
- Autocomplete for movie search.
- A larger movie database.
- Personalized recommendations based on user preferences.
- Improved recommendation techniques.
- Additional movie details such as release year and description.

## Learning Outcomes
Developing this project helped us understand how recommendation systems work in real-world applications. We gained practical experience in dataset handling, data preprocessing, feature extraction, text vectorization and similarity calculation.


