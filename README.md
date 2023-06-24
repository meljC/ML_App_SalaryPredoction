# ML Web App for Salary Prediction With Streamlit

We're building a Machine Learning web application from scratch in Python with Streamlit, using real world data (from nearly 65,000 developers). 

## Data
The 2020 Developer Survey from Stack Overflow

Check it out here, there are interesting insights:
https://insights.stackoverflow.com/survey/2020#overview

## Workflow
In the jupyter notebook we analyze the data and build our model (clean the data, create a model, train and save the model). Then we use it to write the python scripts to build the Web app using Streamlit.

## Model
For the model we took only 5 columns, and kept only data for full-time employment, and used the country, education level and years of experience for the prediction. We also cleaned up the data and removed the outlier salaries amd countries with a small number of data points (less than the cutoff). 

Since the countries and education level are strings, and our model only understands numbers - we need to transform them into numbers. For this we use the label encoder from sklearn.

## Project Setup: 
1. Create & Activate a virtual environment (conda or python)
```
conda create -n ml python=3.10
conda activate ml
```

2. Install packages

```
pip install streamlit
```

and you'll need 
numpy pandas matplotlib scikit-learn sklearn

3. Install a kernel for this virtual environment
 ipython kernel install --user --name=ml

## Run the App: 
streamlit run app.py

## References
[YT Tutorial by Patrick Loeber](https://youtu.be/xl0N7tHiwlw)
