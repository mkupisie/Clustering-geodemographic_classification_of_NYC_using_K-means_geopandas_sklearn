## Clustering: geodemographic classification of NYC using K-means algorithm
Many questions related to spatial observations are complex phenomena that involves several dimensions, what make it hard to summarize them into a single variable. It is especially visible when trying to map distribution of people taking into account e.g. their nationality, education level, age etc. It's uncommon for a geographic region to be exclusively populated by individuals of identical heritage, particularly in the context of urban areas. 

**Clustering** can be used to reduce the dimensionality - the number of variables the analyst needs to look at - and converting it into a more intuitive set of classes.
The fundamental concept behind statistical clustering is to condense the information from multiple variables into a relatively small number of categories. Subsequently, each entry in the dataset is assigned exclusively to one category, based on its values for the initially considered variables.**

**K-means** is one of the most popular clustering algorithm and it can be run in python using sklearn.cluster module in scikit-learn (a popular machine learning library in Python).

### Data
For the purpose of classification the data available in pysal library in examples package were used (https://pysal.org/notebooks/lib/libpysal/Example_Datasets.html).

**NYC Socio-Demographics data** contains the information of total population of the following groups:
- **european:** Total Population White
- **asian:** Total Population Asian American
- **american:** Total Population American Indian
- **african:** Total Population African American
- **hispanic:** Total Population Hispanic
- **mixed:** Total Population Mixed race
- **pacific:** Total Population Pacific Islander

### **Results**
### **1.1. Classification on the map**

![NYC_results](https://github.com/mkupisie/Clustering_geodemographic_classification_of_NYC_using_K-means_geopandas_sklearn/assets/130785524/9f307b2a-5c22-4f63-a682-891dd581ff8d)

### **1.2. The mean of total population for each ethnic group within the class**

![table_results](https://github.com/mkupisie/Clustering_geodemographic_classification_of_NYC_using_K-means_geopandas_sklearn/assets/130785524/358dd91b-85b4-4677-9385-5a05e6c0e3d5)


**Based on the results above it can be noticed that within each group there is a strong majority of one, two and sometimes three ethnic groups:**
- **class 0:** hispanic and african
- **class 1:** european
- **class 2:** african
- **class 3:** hispanic and european
- **class 4:** european and asian
- **class 5:** asian
- **class 6:** african, european and hispanic
- **class 7:** no population
- **class 8:** european
- **class 9:** african and hispanic




