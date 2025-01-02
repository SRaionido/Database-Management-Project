# Database-Management-Project
This is a project from the UCR class CS236, Database Management Systems. The goal is to implement Hilbert R-Trees on social media data. This project was to be done individually.

## API and Software Used
- API: Apache Sedona, Numpy, Json, Pandas, Geopandas, Time
- Software: Google Colab

## Description
This project is meant to get familiar with the Apache Sedona API and implement topics from research papers read within class. The main ideas to implement being R-Trees, Hilbert Curves, and Hilbert R-Trees.

This project starts by downloading necessary drivers and obtaining the Twitter data to be manipulating. The main information we plan to use in the data is the longitutde, latitude, and time of each twitter post. The first part of the code implements Apache Sedona to read the data file and create a Resilient Distributed Dataset (RDD) and create a R-Tree index with that. From there the code then tests the time it takes for various queries to be completed.

The second part of the code under "Project Milestone 2 Section" implements a form of hilbert curves by interleaving the bits of the coordinate data.

The last part of the project then converts the coordinate data into hilbert curve data and creates an R-Tree on the hilbert curve and time coordinate pair. The time in this case is converted to Unix time. Lastly, this part then records the time to complete various size queries with the new Hilbert R-Tree index.
