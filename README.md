# cb2330-project
This project is based on the paper Gut Microbiota from Twins Discordant for Obesity Modulate Metabolism in Mice: https://www.science.org/doi/10.1126/science.1241214 

The pipeline models the change in adiposity in germ-free mice, measured in percentage points of increased fat mass for 15 days after transplantation of microbiota from adult female twins discordant for obesity. 

Initially, the difference in fat mass gain, theta, is roughly estimated from Figure 1D in the paper. This figure shows the average gain in fat mass after 15 days, in lean mice and obese mice, respectively. Subsequently, we use data from Figure 1E to implement a grid search method to determine the best fitting value of theta. This dataset was made by visually estimating the total of five data points over 8 to 35 days, in one of the twin pairs.

From our model, we found that the mouse with obese microbiota gained on average 0.413 percentage points of fat mass per day, compared to the mouse with lean microbiota, who gained 0,020 percentage points of fat mass per day. This makes the difference to 0,393 percentage points per day. This value varies greatly from our original theta, 10/15, because they are based on different data. 

The bootstrap showed a great uncertainty in the result, largely because of the small number of data points. We can conclude that our model does not show good statistical support. 

The pipeline should be run directly from top to bottom. The data is stored in the file called 'data' under the folder 'datafile'. The data does not need to be downloaded, since the pipeline can access it through the url. 

### Generative Ai use
Used for consulting on possible projects, debugging and help with plotting. 
