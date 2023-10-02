# datafun-07-ml-predictive


### Author: [Adrian Vega](https://github.com/adriacv17) <br >Respository: [datafun-07-ml-predictive](https://github.com/adriacv17/datafun-07-ml-predictive) <br> Data: 09/28/2023


### Focus of Module

In this final module, you'll employ machine learning (ML). At a high-level, there are three general categories of ML: supervised, unsupervised, and reinforcement learning. We'll employ a type of supervised learning, simple linear regression, to train a model using all available data and use the resulting model (a best-fit straight line) to make predictions. 

Tasks for this module at the end of README.md


### Chapters

1. Work through the book and examples from Chapter 10 refreshing especially your work on 10.16 on Time Series and Simple Linear Regression.
2. Read through the book and examples from Chapter 15 on Machine Learning, focusing on 15.4 Simple Linear Regression and Predictions.



### Set up a Virtual Environment

Next, we'll create and activate a virtual environment specifically for this project. We'll also install additional packages required for this project.




### Create a Virtual Environment

1. Open the terminal in VS Code. (View / Terminal)
2. Run the following command to **create** a virtual environment for this project.

```shell
python -m venv .venv
```

Verify that a new `.venv` folder was created. It may take a while for the command to complete.

🚀 Rocket Tip: When VS Code Python Extension offers to select the Environment, say Yes.




### Activate the Virtual Environment

Wait for the creation to finish, then **activate** the virtual environment:

- For PowerShell: `.\.venv\Scripts\Activate`
- For macOS/Linux:  `source .venv/bin/`

🚀 Rocket Tip: Notice the terminal changes to reflect the active virtual environment.




### Install Dependencies to the Active Virtual Environment

Install additional project dependencies into the active virtual environment.
The packages ipykernel and jupyterlab are required to run a notebook.
The packages pandas, matplotlib, and seaborn are used to work with data and charts.

```shell
python -m pip install --upgrade pip ipykernel jupyterlab
python -m pip install --upgrade pandas matplotlib seaborn
python -m pip install --upgrade voila
```

Alternatively, you can install all the packages listed in the requirements.txt file.

```shell
python -m pip install --upgrade -r requirements.txt
```

Note: The `--upgrade` parameter gets the latest version of each package.


### Task 1 - Prepare Your Module Repository <br>
1. GitHub<br>
a. Create a new repository named datafun-07-ml-predictive on GitHub.<br>
b. Initialize it with the default README.md.<br>
2. Local Machine<br>
a. In VS Code, clone your new repo into your Documents folder.<br>
3. Repository Essentials<br>
a. Add a .gitignore file from a previous Python project.<br>
b. Add a requirements.txt file to hold external dependencies for Jupyter notebooks and others as you need them. <br>
4. Update README.md<br>
a. Modify the README.md to include your name, the link to your repo, and the focus of this project repository. <br>
b. Include instructions with the exact commands to: <br>
1. Create and activate your virtual environment.<br>
2. Install all required external dependencies.<br>
3. Execute your Python files.<br>
5. Create your local virtual environment (hint: use venv to create a .venv folder)<br>
6. Activate your local virtual environment (hint: call a command in the .venv subfolder)<br>
7. Install any external dependencies you need (hint: use requirements.txt and all the files needed for Jupyter notebooks, pandas, etc.)<br>
8. Push to GitHub <br>
a. Add and commit all your changes with a commit message "Initialized repo"<br>
b. Push your changes to GitHub
 

#### Task 1 - Verify Repository
1. Take a screenshot of your GitHub project repository after you've pushed these changes to GitHub.
2. Display the screenshot as evidence of task completion.
 

### Task 2 - Work Through Chapter 10 <br>
Read and work through Chapter 10 - Object-Oriented Programming - and understand the examples. <br>

10.1 Introduction<br>
10.2 Custom Class Account<br>
10.3 Controlling Access to Attributes<br>
10.4 Properties for Data Access<br>
10.5 Simulating “Private” Attributes<br>
10.6 Case Study: Card Shuffling and Dealing Simulation<br>
10.7 Inheritance: Base Classes and Subclasses<br>
10.8 Building an Inheritance Hierarchy; Introducing Polymorphism<br>
10.9 Duck Typing and Polymorphism<br>
10.10 Operator Overloading<br>
10.11 Exception Class Hierarchy and Custom Exceptions<br>
10.12 Named Tuples<br>
10.13 A Brief Intro to Python 3.7’s New Data Classes<br>
10.14 Unit Testing with Docstrings and doctest<br>
10.15 Namespaces and Scopes<br>
10.16 ★ Intro to Data Science: Time Series and Simple Linear Regression<br>
 

#### Task 2 - Verify Ch 10<br>
1. Take a screenshot of one of the Chapter 10 examples running in your VS Code environment on your machine.<br>
2. Tell us why you chose that part of your work. <br>
 

### Task 3 - Work Through Chapter 15<br>
Read and work through Chapter 15 - Machine Learning - and understand the examples. <br>

15.1 Introduction to Machine Learning<br>
15.1.1 ★ Scikit-Learn<br>
15.1.2 ★ Types of Machine Learning<br>
15.1.3 Datasets Bundled with Scikit-Learn<br>
15.1.4 Steps in a Typical Data Science Study<br>
15.2 Case Study: Classification with k-Nearest Neighbors and the Digits Dataset, Part 1<br>
15.3 Case Study: Classification with k-Nearest Neighbors and the Digits Dataset, Part 2<br>
15.4 ★ Case Study: Time Series and Simple Linear Regression<br>
Suggestion: Specify data file paths as Python raw strings. See FAQ for more.<br>

#### Task 3 - Verify Ch 15
1. Take a screenshot of one of the Chapter 15 examples running in your VS Code environment on your machine.
2. Tell us why you chose that part of your work.
 

### Task 4 - Implement 10.16 and 15.4 <br>
Add a notebook to your project repository and follow the process provided in the text. <br>

1. Use a notebook (rather than interactive mode). 
2. Create a new notebook in your repository with an appropriate file name and extension. 
3. Add all external dependencies to your requirements.txt and install them into your active virtual environment as needed using the command in your README.md. 
4. In a Markdown cell at the top of the notebook, add:<br>
a. The Notebook Title<br>
b. Your Name as Author<br>
c. A Clickable Link to your Project Repository<br>
<br>
Part 1<br>
<br>

1. Add a Markdown heading for Part 1 - Linear Regression.
2. Follow the instructions from 10.16 (starting page 414).
3. Use Markdown cells to create section headings as you work. 
4. Use pandas DataFrames to plot Celsius vs Fahrenheit 
5. Note: The data is for the average (daily) high temperature in January over many years.
6. For example, in 1895, the average high temperature in January was 34.2.
7. We only care about this one series of data: the "average high temp in Jan".
8. There's a lot of stats in the title, and it has confused students. Just think of each value as "the temperature" for that year.
9. We'll use all of the data available to build a best-fit line (supervised learning). 
10. We'll use the slope and intercept of the best-fit line to estimate a point out in the future.
11. Refresh your understanding of the equation for a line (y=mx +b)
12. Section 1 - Load: Follow the instructions to load NY City January high temperature from a csv file into a DataFrame.
13. Section 2 - View: Follow the instructions to view head and tail of the file. 
14. Section 3 - Clean: Follow the instructions to clean the data.
15. Section 4 - Describe: Use describe() to calculate basic descriptive statistics for the dataset. 
16. Section 5 - Calculate Line: Use the SciPy stats module linregress function to calculate slope and intercept for the best fit line through the data.
17. Section 6 - Predict: Use your results to predict the "average high temp in Jan" for the year 2026. 
18. Section 7 - Plot: Follow the instructions and use Seaborn to generate a scatter plot with a best fit line. Set the axes and y limit as instructed.
<br>
Part 2<br>
<br>

1. In the same notebook, add a Markdown heading for Part 2 - Machine Learning.
2. Continue with 15.4 (staring page 620). 
3. This time, we'll use scikit-learn estimator, and we'll practice splitting data for training (to build a model) and testing (testing our model against known values). 
4. Follow the instructions all the way though charting it again with the specified axes.
5. Add Section Headings as you work. 
6. At the end of your notebook, add a final section with some remarks comparing the two methods.<br>
<br>
Excellent analytical skills need professional communication skills to be of maximum benefit. <br>
<br>
 

#### Task 4 - Push to GitHub
1. Execute the completed notebook
2. Add, commit, and push your changes to GitHub. You can use incremental commits as you work - provide useful commit messages.
3. At the end, use a commit message like "Task 4 complete".
4. Verify your GitHub notebook appears complete and well-presented. 
 

#### Task 4 - Verify
1. Capture a screenshot of your completed notebook as viewed in GitHub at the conclusion of this task.
2. Display the screenshot as evidence of task completion.


### Optional Bonus
1. Practice more machine learning skills by working through 15.5 with the California Housing Dataset.
2. In the same notebook, add a Markdown heading for Part 3 - Bonus.
3. Follow the instructions all the way though loading the data, training and testing the data, visualizing the data, and choosing the best model from the 4 listed. 
4. Use appropriate Markdown Section headings to present your work. 
5. Customize your presentation and include helpful remarks to "tell a story with data".
 

#### Optional Bonus - Push to GitHub
1. Execute the completed notebook
2. Add, commit, and push your changes to GitHub. You can use incremental commits as you work - provide useful commit messages.
3. At the end, use a commit message like "Part 3 Bonus complete".
4. Verify your GitHub notebook appears complete and well-presented. 
 

#### Optional Bonus - Verify
1. Capture a screenshot of your completed notebook as viewed in GitHub at the conclusion of this task.
2. Disply the screenshot as evidence of task completion.