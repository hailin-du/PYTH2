![icon](assets/pycon.png?raw=true)
# PYTH2: Python Programming

*🎉🎈🎂🍾🎊🍻💃*

*A hands on and practical introduction
 to programming and python development.*

## Table of Contents

### [WELCOME](src/README.md)
### [GETTING STARTED](src/Intro/README.md)
* **[Tools and Resources](src/Intro/tools.md)**
* **[Setting Up Our Environment](src/Intro/environment.md)**
* **[Running Python Locally](src/Intro/running_py_locally.md)**
* **[Jupyter Notebooks](src/Intro/jupyter_notebooks.md)**
### [LECTURES](src/Lectures_class2/README.md)
* **[Intro to GA & Python - 5/21](src/Lectures_class2/Lecture1.md)**
* **[Conditionals - 5/23](src/Lectures_class2/Lecture2.md)**
* **[Lists, Tuples, & Sets - 5/28](src/Lectures_class2/Lecture3.md)**
* **[Dicts - 5/30](src/Lectures_class2/Lecture4.md)**
* **[Loops & Iterators - 6/4](src/Lectures_class2/Lecture5.md)**
* **[Modules & Functions Intro - 6/6](src/Lectures_class2/Lecture6.md)**
* **[Functions - 6/11](src/Lectures_class2/Lecture7.md)**
* **[Intro to OOP & Classes - 6/13](src/Lectures_class2/Lecture8.md)**
* **[Classes - 6/18](src/Lectures_class2/Lecture9.md)**
* **[Intro to Data Science - 6/20](src/Lectures_class2/Lecture10.md)**
* **[Intro to Pandas Objects - 6/25](src/Lectures_class2/Lecture11.md)**
* **[Pandas Data Processing I - 6/27](src/Lectures_class2/Lecture12.md)**
* **[Pandas Data Processing II - 7/2](src/Lectures_class2/Lecture13.md)**
* **[Pandas EDA I - 7/9](src/Lectures_class2/Lecture14.md)**
* **[Pandas EDA II - 7/11](src/Lectures_class2/Lecture15.md)**
* **[Pandas Data Analysis Lab - 7/16](src/Lectures_class2/Lecture16.md)**
* **[Data Visualization - 7/18](src/Lectures_class2/Lecture17.md)**
* **[Data Visualization Lab - 7/23](src/Lectures_class2/Lecture18.md)**
* **[In-Class Project Work - 7/25](src/Lectures_class2/Lecture19.md)**
* **[Project Presentations! - 7/30](src/Lectures_class2/Lecture20.md)**
### [TOPICS](src/Topics/README.md)
* **[Essential Terminology](src/src/Topics/nb/essential_terminology.ipynb)**
* **[Basic Data Types](src/src/Topics/nb/basic_data_types.ipynb)**
* **[Conditionals](src/src/Topics/nb/conditionals.ipynb)**
* **[Lists](src/src/Topics/nb/lists.ipynb)**
* **[Dicts](src/src/Topics/nb/dicts.ipynb)**
* **[Loops](src/src/Topics/nb/loops.ipynb)**
* **[Modules & Packages](src/src/Topics/nb/modules.ipynb)**
* **[Functions](src/src/Topics/nb/functions.ipynb)**
* **[List Comprehensions](src/src/Topics/nb/list_comprehensions.ipynb)**
* **[Classes](src/src/Topics/nb/classes.ipynb)**
* **[Data Science](src/src/Topics/nb/data_science.ipynb)**
* **[Intro to Pandas Objects](src/src/Topics/nb/intro_pandas.ipynb)**
* **[Exploratory Data Analysis w. 🐼](src/src/Topics/nb/preprocessing.ipynb)**
* **[Pandas Analysis II](src/src/Topics/nb/eda.ipynb)**
* **[Data Visualization](src/src/Topics/nb/data_viz.ipynb)**
* **[Course Review](src/src/Topics/nb/course_review.ipynb)**
* **[Python Project Ideas](src/src/Topics/nb/project_ideas.ipynb)**
### [HOMEWORK](src/Homework/README.md)
* **[Homework 1](src/Homework/hwk1.md)**
* **[Homework 2](src/Homework/hwk2.md)**
* **[Homework 3](src/Homework/hwk3.md)**
* **[Homework 4](src/Homework/hwk4.md)**
* **[Homework 5](src/Homework/hwk5.md)**
* **[Final Project Reqs](src/Homework/final.md)**
### [RESOURCES](src/Resources/README.md)
* **[Python Glossary](src/Resources/python_glossary.md)**
* **[Basic Statistics](src/Resources/basic_stats.md)**
* **[Pandas Glossary](src/Resources/pandas_glossary.md)**
* **[General Reference Guides](src/Resources/genref.md)**
* **[Libraries, Packages, & Other Tools](src/Resources/tools_libs.md)**
* **[Cheat Sheets](src/Resources/cheat_sheets.md)**
* **[Helpful Articles/Tutorials](src/Resources/articles.md)**
* **[Open Source Datasets](src/Resources/datasets.md)**
### [ABOUT](src/About/README.md)
## Building and Deploying

The `scripts` folder contains a few py scripts that help transform the content from markdown to jupyter notebooks and regenerate the README. On deploy, travis CI runs these tasks and generates output content.

### Build Env and Install Reqs 

Create a virtual env:

```
python3 -m venv .env
source .env/bin/activate
pip install -r requirements.txt
```

### Converting Markdown to Jupyter Notebooks

In `scripts/conf.py`, set the `IPYTHON_DIRS` to include whichever directories that must be converted. Then:

```python
python scripts/convert_to_nb.py
```

The dirs in `IPYTHON_DIRS` will now have a `nb` folder with jupyter notebooks.

### Regenerating README

Each `.md` file has something like:

```
<!---
{"next":"Lectures_class2/Lecture2.md","title":"Intro to GA & Python - 5/21"}
-->
```

This is parsed by the `scripts/build_summary.py` script and a list is created where each subsequent file is denoted in `next`. Files that are part of `IPYTHON_DIRS` automatically link to the jupyter notebook vs the markdown. To run:

```python
python scripts/build_summary.py
```

## Taq Karim

<img src="https://github.com/mottaquikarim/JavascriptBootcamp/blob/master/assets/taq.jpg?raw=true" style="width: 100px; height: auto;" width="100" align="left"> 

[Hello, Wrold!](https://medium.com/@the_taqquikarim/console-log-hello-wrold-3e3abeb44396) I'm Taq, Tech Lead of the Demand Side (DSP) team at Place Exchange, a programmatic advertising exchange platform for Out of Home media. I'm also a lecturer, leading workshops and courses on a wide variety of topics (frontend / backend) in institutions such as Coalition 4 Queens (now Pursuit), The Startup Institute, NYCDA, OneMonth, The King's College and Columbia Splash. [I've taught Front-end Web Development at GA 14x](https://medium.com/@the_taqquikarim/10-lessons-learned-from-100-weeks-of-teaching-fewd-12c43db14f6b) (so far). When I'm not working I am usually [thinking about math](https://medium.com/math-musings/why-does-25-25-2-2-1-100-25-an-explanation-6c7e7b283d41), [building](https://medium.com/@the_taqquikarim/a-technique-for-saving-content-from-a-data-text-html-uri-10f045a8876d) [software](https://medium.com/@the_taqquikarim/introducing-bonfire-2c0e437895e2), [working](https://photos.app.goo.gl/w1crzgI7DqCgGR373) [on](https://photos.app.goo.gl/EaFkp5SmyO0opkg32) [hardware](https://photos.app.goo.gl/tvxPl2zbIMl7FEnK2) [hacks](https://www.instagram.com/p/8rARZNND_t/?taken-by=taqqui.karim) or hanging out with my cat, Layla Karim.

## Julianna Garreffa

*bio here*
