# Decision Tree Classifier

This project was developed for the "Artificial Intelligence" course and aims to **creating a Decision Tree Classifier using ID3 (entropy based)**. Second Semester of the Second Year of the Bachelor's Degree in Artificial Intelligence and Data Science.

<br>

## Programming Language:

<div style = "display: inline_block"><br/>
  <img align="center" alt="python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
</div><br/>

<br>

## The Decision Tree
In order to create this decision tree, there were a few things we had to take into account:
- The Decision Tree **input needs to be in a CSV (Comma Separated Value) format**, each column is an attribute, being the **last one the variable of interest for classification**;
- The program needs to be able to **read any dataset and learn the appropriate decision tree**;
- The program must also be prepared to **accept as input a file with test examples** (after generating the tree, it must be able to apply it to new examples and be able to **classify them appropriately**);
- Not allowed to use scikit-learn or other libraries to automatically define and train the decision trees
- The print of the decision tree created must be in the following format:

<p align="center">
  <img width="460" height="300" src="https://github.com/user-attachments/assets/c5980ad5-af00-4e48-b32a-4c289161fd15">
</p>

**Attribute:** the root of each subtree;
**Value:** is one of the values of the attribute (one of the branches of the tree);
**Class:** is the class value assigned to that branch in the tree (and corresponds to a leaf);
**Counter:** is a counter of the number of examples corresponding to that tree branch

<br>

## The Datasets and its Problems:
In this task, we were asked to consider 4 different data sets to test the decision tree implementations, each of which has specific characteristics that we must take into account to improve our decision tree:

- **reataurant:** Its a <u>simple dataset</u> that contains information about customers and restaurants (type of food, waiting time, price etc). Only has <u>two options for classification</u> ("Yes", "No") and the <u>data type is "Object" (string)</u>.
- **weather:** This dataset has some issues and contains information about weather conditions for playing tennis. In addition to this dataset containing **continuous values**, it also presents some **imbalance between classes**.
- **iris:** This dataset contains numerical information about plants from **three classes**: iris setosa, iris virginica and iris versicolor, so we are faced with a non-binary classification (more than one class).
- **connect4:** This dataset is a board configuration of the connect four game that classifies each entrance as "win", "loss" or "draw". After analyzing the dataset, we realized that we wouldn't need to make any further changes to our decision tree.

To address the issues detected in each dataset, we developed the following features in our decision tree to deal with them:

| Problem | Solution |
| :- | :- |
|Unbalanced Classes | SMOTE |
| Continuous Values | Binning |
| Multiclasses | One VS All |


<br>

## About the repository:

- ds ➡️ Folder with the used datasets;
- report_PL3_6.ipynb ➡️ Is the work developed in detail and all its code;
- IA_2324_Trab2.pdf ➡️Project statement

<br>

## Link to the course: 

This course is part of the **<u>second semester</u>** of the **<u>second year</u>** of the **<u>Bachelor's Degree in Artificial Intelligence and Data Science</u>** at **<u>FCUP</u>** and **<u>FEUP</u>** in the academic year 2023/2024. You can find more information about this course at the following link:

<div style="display: flex; flex-direction: column; align-items: center; gap: 10px;">
  <a href="https://sigarra.up.pt/fcup/pt/UCURR_GERAL.FICHA_UC_VIEW?pv_ocorrencia_id=529859">
    <img alt="Link to Course" src="https://img.shields.io/badge/Link_to_Course-0077B5?style=for-the-badge&logo=logoColor=white" />
  </a>

  <div style="display: flex; gap: 10px; justify-content: center;">
    <a href="https://sigarra.up.pt/fcup/pt/web_page.inicial">
      <img alt="FCUP" src="https://img.shields.io/badge/FCUP-808080?style=for-the-badge&logo=logoColor=grey" />
    </a>
    <a href="https://sigarra.up.pt/feup/pt/web_page.inicial">
      <img alt="FEUP" src="https://img.shields.io/badge/FEUP-808080?style=for-the-badge&logo=logoColor=grey" />
    </a>
  </div>
</div>
