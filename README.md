<p align="center">
  <a href="https://github.com/XpressAI/xircuits/tree/master/xai_components#xircuits-component-library-list">Component Libraries</a> •
  <a href="https://github.com/XpressAI/xircuits/tree/master/project-templates#xircuits-project-templates-list">Project Templates</a>
  <br>
  <a href="https://xircuits.io/">Docs</a> •
  <a href="https://xircuits.io/docs/Installation">Install</a> •
  <a href="https://xircuits.io/docs/category/tutorials">Tutorials</a> •
  <a href="https://xircuits.io/docs/category/developer-guide">Developer Guides</a> •
  <a href="https://github.com/XpressAI/xircuits/blob/master/CONTRIBUTING.md">Contribute</a> •
  <a href="https://www.xpress.ai/blog/">Blog</a> •
  <a href="https://discord.com/invite/vgEg2ZtxCw">Discord</a>
</p>





<p align="center"><i>Xircuits Component Library for Apache Spark! Process and analyze big data with powerful, scalable components.</i></p>

---
## Xircuits Component Library for Spark

The Spark component library makes it easy to use Apache Spark within Xircuits workflows. You can process, analyze, and visualize large datasets efficiently.

## Table of Contents

- [Preview](#preview)
- [Prerequisites](#prerequisites)
- [Main Xircuits Components](#main-xircuits-components)
- [Try the Examples](#try-the-examples)
- [Installation](#installation)

## Preview

### SparkLinePlot Example

<img src="https://github.com/user-attachments/assets/098c9ce7-e7c4-44d1-9b38-5640c31920da" alt="SparkLinePlot_example"/>

### SparkLinePlot Result

<img src="https://github.com/user-attachments/assets/1294489b-db91-4371-9d18-f0ce8778bb20" alt="SparkLinePlot"/>

### SparkLogisticRegressionSample Example

<img src="https://github.com/user-attachments/assets/a8325851-69a9-4d2b-ba14-b54ce09252c8" alt="SparkLogisticRegressionSample_example"/>

### SparkLogisticRegressionSample Result

<img src="https://github.com/user-attachments/assets/9bba50c3-bbf4-492a-b07f-67ea3075b0f3" alt="SparkLogisticRegressionSample_result"/>

### SparkSQLPlotBar Example 

<img src="https://github.com/user-attachments/assets/104ad16f-9ff5-4103-a028-a74722c74d6c" alt="SparkSQLPlotBar_example"/>

### SparkSQLPlotBar Result

<img src="https://github.com/user-attachments/assets/7bbc5723-d982-4f2e-928f-34b37030763c" alt="SparkSQLPlotBar_result"/>

## Main Xircuits Components

### xSparkSession
Initializes a Spark session to enable distributed data processing.

<img src="https://github.com/user-attachments/assets/04fa8a54-5972-44c3-a0ed-61bbf2779bae" alt="xSparkSession" width="200" height="100" />

### SparkReadFile Component:
Reads data from files in formats like csv, json, parquet, or orc into a Spark DataFrame.

<img src="https://github.com/user-attachments/assets/4adea79f-026f-42d6-868f-c2f8ec6a0743" alt="SparkReadFile" width="200" height="85" />

### SparkWriteFile Component:
Saves Spark DataFrames to files in formats such as csv, parquet, or orc.

<img src="https://github.com/user-attachments/assets/4db5149f-cec1-4248-9f94-8b42ba587780" alt="SparkWriteFile" width="200" height="100" />

### SparkReadCSV Component:
Reads CSV files into a Spark DataFrame with options for custom delimiters and headers.

<img src="https://github.com/user-attachments/assets/8d9dc79f-47f2-4526-9971-a20f11f95faf" alt="SparkReadCSV" width="200" height="125" />

### SparkSQL Component:
Executes SQL queries on a Spark DataFrame, returning query results as a new DataFrame.

<img src="https://github.com/user-attachments/assets/ee007db0-f147-496e-9b83-7d37de6dc8ff" alt="SparkSQL" width="200" height="125" />

### SparkVisualize Component:
Creates bar, scatter, or line plots from Spark DataFrames and saves them as images.

<img src="https://github.com/user-attachments/assets/ae89d1d0-01a2-4b71-a56e-f151bbf6449c" alt="SparkVisualize" width="200" height="150" />

### SparkSplitDataFrame Component:
Splits a Spark DataFrame into training and testing sets based on a specified ratio.

<img src="https://github.com/user-attachments/assets/8c813df1-3919-4467-8d0c-c4ec4009001d" alt="SparkSplitDataFrame" width="200" height="100" />


### SparkLogisticRegression Component:
Trains a logistic regression model using a Spark DataFrame.

<img src="https://github.com/user-attachments/assets/85e4840d-12f4-472b-8ed6-08a9ff00677e" alt="SparkLogisticRegression" width="200" height="100" />

### SparkPredict Component:
Uses a trained Spark model to make predictions on a test DataFrame.

<img src="https://github.com/user-attachments/assets/093cf834-f576-4da8-b0ba-809bf05745a7" alt="SparkPredict" width="200" height="85" />

## Try the Examples

We have provided an example workflow to help you get started with the Spark component library. Give it a try and see how you can create custom Spark components for your applications.

### SparkLinePlot 

This example demonstrates creating a line plot from a CSV file using Spark. It reads the dataset, processes it into a Spark DataFrame, and visualizes the relationship between the Year and Wind columns as a line plot saved as Lineplot.png.

### SparkLogisticRegressionSample 

This example uses the SparkLoadLIBSVM component to load data, splits it for training and testing with SparkSplitDataFrame, and trains a multinomial logistic regression model to make predictions.

### SparkSQLPlotBar

This example loads penguin data from a CSV file, queries species information using Spark SQL, and generates a bar plot visualizing species distribution, saving it as 'pinguin_distribution.png'.

## Installation
To use this component library, ensure that you have an existing [Xircuits setup](https://xircuits.io/docs/main/Installation). You can then install the Spark library using the [component library interface](https://xircuits.io/docs/component-library/installation#installation-using-the-xircuits-library-interface), or through the CLI using:

```
xircuits install spark
```
You can also do it manually by cloning and installing it:
```
# base Xircuits directory  
git clone https://github.com/XpressAI/xai-spark xai_components/xai_spark  
pip install -r xai_components/xai_spark/requirements.txt  
```