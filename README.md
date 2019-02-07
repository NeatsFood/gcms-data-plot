# gcms-data-plot
Visualizations of GCMS data from our plant samples.

This [Jupyter notebook](https://jupyter.org/) to create plots of our GCMS data was written by Manvitha Ponnapati to visualize data collected by John De La Parra.

[Example GCMS data plot](plot.html)

### What the heck is Jupyter?
- Jupyter is an interactive development system for code + data + comments. Useful for small scientific and math projects you want to analyze / visualize.
- Jupyter starts a local web server + kernel that will let you edit & run your 'document'.
- Jupyter documents are portable and easily shareable.  They are in a human readable text format (JSON).
- We use Jupyter because we frequently have to edit this bit of code to parse the data and make these plots for publication.


### Installing Jupyter
- [Install docs](https://jupyter.org/install)
- Install steps used on OSX 10.14.2 (with Python 3.6.5 already installed globally)
```
python3 -m pip install --upgrade pip
python3 -m pip install jupyter
python3 -m pip install bokeh
python3 -m pip install pandas
python3 -m pip install numpy
```

### Using Jupyter
This is how we run our notebook.  Make sure you have pre-processed the GCMS data into a `data.csv` file.
```
jupyter notebook gcms.ipynb
```
- [Using Jupyter](https://jupyter-notebook.readthedocs.io/en/stable/)
- [Examples](https://nbviewer.jupyter.org/github/jupyter/notebook/tree/master/docs/source/examples/Notebook/)
- [Bokeh charting package](https://bokeh.pydata.org/en/latest/docs/user_guide/plotting.html)

### Data pre-processing 
(Still TBD by Rob when he gets Manu's notes)

1. I have a script somewhere that automatically splits a CSV into multiple small csv files based on where the CSV file has a line With Path etc.
2. There are some cases when the samples all dont have the equal timestamps - like the last sample might be missing for some. In those cases - I do an assert and append an empty row to the dataframe if the dataframe files.
3. I recommend usually adding the indexes yourself for different samples so you know exactly what you are plotting.



