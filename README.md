# Rader-Chart

## Overview
This repository contains a practice project replicating an existing Matplotlib dashboard to understand data visualization techniques.
For this example, I reproduced a Radar Chart (Spider Chart) using sample subject-course data to learn how to plot polar graphs in Python and customize axes, colors, and labels.
The purpose of this exercise is skill-building only, not presenting original data and all credits for the original design go to its creator.

# Objective
The radar chart visualizes the relevance of various subjects across multiple courses. It was created in Python using Matplotlib as a practice exercise to replicate and understand someone else’s work. The goal was to learn how to build, customize, and save radar charts for future data visualization projects.

<img width="352" height="342" alt="Screenshot 2025-10-05 205505" src="https://github.com/user-attachments/assets/7d4da2d5-7a74-47a2-bcfa-6128cae980b4" />

## Table of Content 
- [Project Overview](#project-overview)
- [Objective](#objectives)
- [Key Questions](#key-questions)
- [Tools and Methodologies](#tools-and-methodologies)
- [Data Processing ](#data-processing)
- [Data Modeling](#data-modeling)
- [Key Insights](#key-insights)
- [Summary & Recommendations](#summary-&-recommendations)
- [References](#references)

## Key Business Questions
- Which subjects are most relevant or required for each course (Medicine, Law, Engineering, etc.)?
- How do the subject requirements compare across different courses?
- Which courses emphasize sciences versus arts/humanities the most?
- Are there subjects that are universally important across all courses?
- Which courses show the greatest variability in subject emphasis?

# Tools and Methodologies
## Tools Used:
- Python (for data handling and visualization)
- Matplotlib (for creating and customizing the radar/spider chart)
- NumPy (for angle and data array calculations)
- Jupyter Notebook (to run and document the code interactively)
  
  ![imports](https://github.com/user-attachments/assets/2a42c288-add0-4ad8-87c2-480d3bdbba81)


## Method Used:
- Created sample data for courses vs. subjects on a 0–20 scale.
- Used NumPy to calculate angles for each variable around the circle.
- Built and customized a radar (polar) chart using Matplotlib.
- Applied different colors, titles, and labels for clarity.
- Documented and saved the chart image for sharing and GitHub publishing.

  ![Subjects](https://github.com/user-attachments/assets/334501e2-2138-4ec2-b87d-1b77e6710a6e)
  ![Data](https://github.com/user-attachments/assets/c1c5114c-90ed-4d35-be79-2f8701b01eac)



# Data Processing
## Data Preparation
- Created a simple dataset linking courses/roles (Medicine, Law, Engineering, etc.) to subject relevance (Mathematics, Chemistry, Biology, etc.) on a 0–20 scale.
- Converted the data into a Python dictionary so it could be easily plotted.
- Defined the subjects list and ensured the first value was repeated at the end of each array to “close” the radar chart shape.
## Transformation
- Used NumPy to calculate equal angles for each subject around the radar chart.
- Normalized the data so that all courses had scores within the same 0–20 scale for fair comparison.
## Visualization Setup
- Built a radar chart using Matplotlib with one polygon per course.
- Assigned distinct colors to each course for easy visual separation.
- Added axis labels, ticks, and a title for context.

  ![labelling](https://github.com/user-attachments/assets/af92afe7-4aad-4709-ab18-0366326dd5da)


# Data Modeling
Although this project uses a small, custom dataset, a simple model was created to structure the information before visualization:
Fact Table: Subject Relevance Scores (numerical values 0–20 for each course/role).
### Dimension Table:
- Courses/data – Medicine, Law, Business Admin, Engineering, etc.
- Subjects – Mathematics, Chemistry, Biology, Literature, etc.

  <img width="650" height="570" alt="raderchart" src="https://github.com/user-attachments/assets/c0d81ce2-d42d-45d4-8ffb-5ee0f8d7de8d" />

# Key Insights
Based on the sample data plotted on the radar chart:
- Science-Focused Courses:
  Medicine, Chemical Engineering, Mechanical Engineering, and Microbiology show very high scores in Chemistry, Physics, and Biology, reflecting their heavy science    requirements.
- Business and Social Science Focus:
  Business Administration shows stronger emphasis on Economics, Statistics, and Mathematics but low emphasis on pure sciences.
- Humanities-Focused Courses:
  Law and Mass Communication score high in Literature-in-English, History, Government, and Foreign Languages, but much lower in sciences.
- Common Ground:
  Mathematics and Statistics appear moderately across almost all courses, showing they’re fairly universal.
- Variability:
Science-related courses have the steepest differences between science and arts subjects, while Business Admin and Mass Communication have a more balanced profile across non-science subjects.

# Summary & Recommendations
## Summary of Key Findings
- Science-oriented courses (Medicine, Chemical & Mechanical Engineering, Microbiology) score highest in Chemistry, Physics, and Biology.
- Business and social science–oriented courses show strong emphasis on Economics, Statistics, Government, and Mathematics.
- Humanities-oriented courses (Law and Mass Communication) rank highest in Literature-in-English, History, Government, and Foreign Languages.
- Mathematics and Statistics appear moderately across all courses, making them universally important subjects.

## Recommendations
- Curriculum Planning: Use radar charts to identify gaps in subject preparation for students entering each course and adjust pre-requisites accordingly.
- Career Guidance: Educators or career counselors can use similar charts to visually communicate subject requirements to students considering different courses.
- Visualization Practice: Experiment with colors, grid lines, and labels to make charts more readable when presenting to non-technical audiences.

# References
- Original radar chart example used for practice and learning: [https://drive.google.com/file/d/1r26aS9B-CnUXf1l_tDY1nzI4TMOne_3d/view?usp=drive_link]
- Matplotlib Documentation
- -Polar/Axes : https://matplotlib.org/stable/gallery/specialty_plots/radar_chart.html
- -Spines : https://matplotlib.org/stable/api/spines_api.html#module-matplotlib.spines
- NumPy Documentation (for angle calculations): https://numpy.org/doc/
Note: This radar chart was created as a practice exercise to learn how to build and customize spider/radar charts in Python. The design was inspired by an existing example and not created from original data.
