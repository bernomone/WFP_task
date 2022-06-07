# WFP_task

World food program Data Science Assignemnt task. To make this repository work, be sure to have Docker installed. In the main folder run **docker build . --tag wfp:task** to build the image.

Then **docker run -p 8888:8888 --rm -v $(pwd):/app/ wfp:task** to run the container on port 8888 (please be sure this port available first). **localhost:8888** will show the notebooks for the analysis. 

This project is developed using Jupyter Notebooks. Please refer to {this page}[https://jupyter.org/] for more information. The notebooks are number in the order they should be run. The data they produce is saved in the **data_out/** folder; ML models for imputation are stored in the **models/** folder; all the figures produced are saved in the **figures/** folder.

- *01_merging_datasets.ipynb* merges all the datasets into a single one, which is saved in the pickle file **/data_out/source_of_truth.pkl**
- *02_data_analysis.ipynb* analyses the data and produces the figures present in the report
- *03_fit_imputation_model.ipynb* generate an imputation model using a Gradient Boosting Regression algorithm. 
- *04_imputation.ipynb* uses the generated model to impute the missing Food Security Index time seriesgi