# Project Covid 19 Cases

**Project Covid 19 Cases** is a Comprehensive data analysis tool designed to streamline data exploration, analysis, and visualisation. The tool supports multiple data formats and provides an intuitive interface for both novice and expert data scientists.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)


## Dataset Content
* Data Set is with 50000 rows and 10 columns so reduced it to 10000 rows and after manipulation added 6 other columns



## Business Requirements
* Want to see how many confirmed cases and number of deaths occuring per region and country and what was the moving avrage of 4 days. Number of cases monthwise per region.


## Hypothesis and how to validate?
* Did USA have most cases over time. True the data shows USA had the most cases, validated through plots.
Was it thursday most cases emerging. True on thursday most cases emerged than rest of the days validated through Box plot.

## Project Plan
* Explored the whole dataset for missing values and data types  of
columns. Looked for columns if they have are necessary to stay within the dataset.
* Downloaded the dataset on computer from Kaggle as csv file in a seperate folder as Raw dataset and loaded in VS code for processing. Once the data was processed, cleaned data was loaded back in seperate folder as clean processed data and transformed data after Feature Engnineering.
* Why did you choose the research methodologies you used?

## The rationale to map the business requirements to the Data Visualisations
* To see relationsips among number of cases, active and number of deaths per region over time through different plotting methods

## Analysis techniques used
* Pandas, Numpy, Seaborn, Matplotlib, Plotly, Feature Engine Encoders and Imputers used. 
Could not use histograms very much as plotting in Vs code was taking enormous time and histograms were not appearing properly.
* There were not many categorical columns so from Date column created a new column Day. Fill values of one Categorical column Province/state where many values were NaN so filled them with Unknown. Calculated Moving averages, used groupby and other functions. Used Feature Engineering.
* The columns in dataset had extreme uneven values not allowing to plot Histograms and Kde plots. The histograms were taking long time to appear. After filtering some columns the heatmap was also no appearing correctly.
* Used Feature Engineering tools, Ordinal Encoder for categoriacal variables, Winsorizer for outliers numerical for continuous variables. 

## Ethical considerationshttps:
* So far not many data privacy issues as it was issued by WHO and put on Kaggle.
* so far no legal issues.

## Unfixed Bugs
* There are 2 columns in dataset Deaths and Recovered could not be shown in Sunburst plot when hovered over the data despite using several techniques and considerable amount of time.


## Development Roadmap
* Main challenges were in plotting different plots, used help with Chatgpt.
* Need to learn logscaling and when animating in plotly, how to control speed of animation.

## Main Data Analysis Libraries
* Pandas, Numpy, Seaborn, Matplotlib, Plotly, Feature Engine pipeline, Encoders and Imputers used.
example is:
import seaborn as sns
sns.kdeplot(data=df, x='Active',hue='WHO Region',ax=axes[0],fill=True,  palette='Set1')
plt.show()

## Credits 

* Used Code Institute Lms and Chatgpt help for syntactical errors. 


## Acknowledgements (optional)
* Special thanks to John and Vasi in Code Institute who provided support and help through this project.