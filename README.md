## Capstone Project: Predicting NYC Restaurant Demand
------------------------------------------------------------------------------

### Executive Summary

#### Problem Definition:
FoodHub, an online food delivery platform, faces challenges in understanding customer demand, optimizing delivery times, and improving restaurant performance. With increasing competition, it's crucial to enhance customer satisfaction and streamline operations to remain competitive.

#### Data Science Opportunity:
Using FoodHub's historical order data, we can predict restaurant demand, optimize delivery efficiency, and provide personalized restaurant recommendations. By leveraging machine learning models and data analysis, this project identifies patterns in customer behavior, order trends, and operational bottlenecks. These insights enable targeted marketing strategies, improved delivery routes, and better restaurant partnerships.

#### Affected Parties:
- **Restaurant Owners**: Struggle to meet fluctuating demand and maintain high-quality service.
- **Delivery Personnel**: Face delays and inefficiencies in delivery routing.
- **Customers**: Experience inconsistent delivery times and limited personalized recommendations, impacting their satisfaction.
  
#### Key Takeaways:
- **Predictive Demand Models**: Accurately forecast restaurant demand to enhance preparation and delivery times.
- **Personalized Recommendations**: Tailor restaurant suggestions to improve customer experience.
- **Operational Efficiency**: Optimize delivery routes and resource allocation to reduce delivery times.
- **Business Growth**: Data-driven insights support targeted marketing and partnerships, leading to increased customer satisfaction and revenue growth.

#### Dataset Description:
The dataset includes detailed information about customer orders, such as:
- **Order ID**: Unique identifier for each order.
- **Customer ID**: Unique identifier for each customer.
- **Restaurant Name**: Name of the restaurant fulfilling the order.
- **Cuisine Type**: Type of cuisine ordered.
- **Cost of the Order**: Total cost of the order.
- **Day of the Week**: Whether the order was placed on a weekday or weekend.
- **Rating**: Customer rating of the order (out of 5).
- **Food Preparation Time**: Time taken by the restaurant to prepare the food.
- **Delivery Time**: Time taken by the delivery person to deliver the food after pickup.

  
This project provides actionable solutions to drive operational improvements and customer engagement, ensuring sustained success for FoodHub.




------------------------------------------------------------------------------
# BrainStation Data Science Capstone Project

This is a template repository for setting up your capstone project: it includes a simple folder structure and placeholder files for the most important assets you will be creating.

## Usage

1. Start a new GitHub repo using this template.
2. Update your `LICENSE` file with date and owner.
3. Update your `README.md` file to reflect the project - see a sample structure below and please refer to Synapse on what needs to be included here. 
4. Set up and activate your conda environment:
    - Create a new `conda` environment for your capstone project.
    - Activate the environment and export:
        ```bash
        conda env export > conda.yml
        ```
    - Make sure re-export every time after you update the environment.
    - You can reset your conda environment by running:
        ```bash
        conda env create -f conda.yml
        conda activate <your-env-name>
        ```
5. Add your own notebooks in `./notebooks/` and remove placeholders.
6. Add your own data in `./data/` and remove placeholder. Note: `.gitignore` will ignore the data folder when you push to github, save a copy of your raw and processed data, pickled models in a Google Drive folder and add the link in the `data_links.md` file.
7. Add your project documents, figures, reports, presentation pdf's in the `./docs` and remove placeholders.
8. Add your references (tutorials, papers, books etc.) in `./references`. 
9. Add your own scripts in `./src/` and remove unnecessary folders.

Feel free to rename the folder and customize the project structure to best fit your work - this template is just the starting point.

------------------------------------------------------------------------------


### Demo

... Show your work:
...     Data visualizations
...     Interactive demo (e.g., `streamlit` app)
...     Short video of users trying out the solution


### Methodology

... High-level diagrams of entire process:
...     various data processing steps
...     various modelling directions
...     various prototyping directions


### Organization

#### Repository 

* `data` 
    - contains link to copy of the dataset (stored in a publicly accessible cloud storage)
    - saved copy of aggregated / processed data as long as those are not too large (> 10 MB)

* `model`
    - `joblib` dump of final model(s)

* `notebooks`
    - contains all final notebooks involved in the project

* `docs`
    - contains final report, presentations which summarize the project

* `references`
    - contains papers / tutorials used in the project

* `src`
    - Contains the project source code (refactored from the notebooks)

* `.gitignore`
    - Part of Git, includes files and folders to be ignored by Git version control

* `conda.yml`
    - Conda environment specification

* `README.md`
    - Project landing page (this page)

* `LICENSE`
    - Project license

#### Dataset

... Google Drive links to datasets and pickled models

### Credits & References

... Include any personal learning

------------------------------------------------------------------------------
Data set: https://www.kaggle.com/datasets/ahsan81/food-ordering-and-delivery-app-dataset/data
Analysis 1: https://www.kaggle.com/code/xinningzhang1/notebookc236a99686/edit
Analysis 2: https://www.kaggle.com/code/nonnyman1/nyc-restaurant-food-order-data/notebook

