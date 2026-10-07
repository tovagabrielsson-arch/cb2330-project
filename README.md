# cb2330-project
This project is based on the paper Gut Microbiota from Twins Discordant for Obesity Modulate Metabolism in Mice: https://www.science.org/doi/10.1126/science.1241214 

The pipeline models the change in adiposity in germ-free mice, measured in percentage points of increased fat mass during the 15 days after transplantation of microbiota from adult female twins discordant for obesity. 

Initially, the difference in fat mass gain, theta, is roughly estimated from Figure 1D in the paper. This figure shows the average gain in fat mass after 15 days, in mice receiving lean- and obese-donor microbiota, respectively. Subsequently, we use data from Figure 1E to implement a grid search method to determine the best fitting value of theta. This dataset was made by visually estimating five data points between days 8 and 35, in one of the twin pairs.

From our model, we found that mice with obese-donor microbiota gained on average 0.413 percentage points of fat mass per day, compared to mice with lean-donor microbiota, who gained 0.020 percentage points of fat mass per day. This gives a difference of 0.393 percentage points per day. This value differs substantially from our original estimate of theta, 10/15, because they are based on different data. 

The bootstrap showed a great uncertainty in the result, largely because of the small number of data points. We can conclude that our model is not strongly supported by the limited data. 

The pipeline should be run directly from top to bottom. The data is stored in the file called 'data' under the folder 'data file'. The data does not need to be downloaded, since the pipeline can access it through the url. If downloaded, the pipeline can instead use the local data file if the file path is updated in the cell under the heading “Backwards”.

### Generative Ai use
Used for consulting on possible projects, debugging and to help with bootstrap and code to read data. Generative AI was also used to find spelling errors and to format and edit figures. 
