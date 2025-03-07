Demonstration of PCA on Iris data
Information on the iris data here: https://en.wikipedia.org/wiki/Iris_flower_data_set

Information on the sklearn machine learning library here: http://scikit-learn.org/

Some information on plotly can be found here:

3D scatter plots
2D scatter plots and annotations
Line charts
Reference
We will put our data in a pandas Data Frame, described here: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html

Data Frames are useful as they store information about the data (e.g. row, column meanings) along with the data itself. Sometimes you need to get the raw data into a numpy array to run algorithms in scikit-learn and we show how to do that in the tSNE example in the last section of the notebook below.



Visualisation of flow cytometry data using PCA
In this lab we will use PCA to visualise a dataset from a flow cytometry experiment. We have taken one flow cytometry dataset from a healthy control sample, from the paper "Longitudinal immune profiling reveals key myeloid signatures associated with COVID-19" (available from https://www.science.org/doi/full/10.1126/sciimmunol.abd6197).

Flow cytometry can be used to quantify the level of cell surface markers on a large number of individual cells in a sample. These markers provide useful information about the cell-type and cell function for many single cells in a sample, e.g. a blood sample. The panel of markers used in this experiment was chosen to help distinguish different immune cells in the blood such as T-cells, monocytes and neutrophils. In the above paper it was shown that the number and activity of these cells differs between patients with mild and severe covid, suggesting how differences in the patient immune response can play an important role in determining the disease severity.

Below we show how to get the data into your notebook. We use a random subset of 2500 cells in this lab, although the full dataset includes around 100,000 cells for each flow cytometry experiment.
