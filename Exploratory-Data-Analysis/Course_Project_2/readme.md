## Peer-graded Assignment: Course Project 2
## Introduction
Fine particulate matter (PM2.5) is an ambient air pollutant for which there is strong evidence 
that it is harmful to human health. In the United States, the Environmental Protection Agency (EPA)
is tasked with setting national ambient air quality standards for fine PM and for tracking the emissions 
of this pollutant into the atmosphere. Approximatly every 3 years, the EPA releases its database on emissions
of PM2.5. This database is known as the National Emissions Inventory (NEI). You can read more information about
the NEI at the [EPA National Emissions Inventory web site](http://www.epa.gov/ttn/chief/eiinformation.html).

## Data
PM2.5 Emissions Data (_summarySCC_PM25.rds_): 
This file contains a data frame with all of the PM2.5 emissions data for 1999, 2002, 2005, and 2008.
For each year, the table contains number of tons of PM2.5 emitted from a specific type of source for 
the entire year. Here are the variables.
* __fips__: A five-digit number (represented as a string) indicating the U.S. county
* __SCC__: The name of the source as indicated by a digit string (see source code classification table)
* __Pollutant__: A string indicating the pollutant
* __Emissions__: Amount of PM2.5 emitted, in tons
* __type__: The type of source (point, non-point, on-road, or non-road)
* __year__: The year of emissions recorded

Source Classification Code Table (_Source_Classification_Code.rds_): This table provides a mapping from the 
SCC digit strings in the Emissions table to the actual name of the PM2.5 source. The sources are categorized 
in a few different ways from more general to more specific and you may choose to explore whatever categories 
you think are most useful. For example, source “10100101” is known as “Ext Comb /Electric Gen /Anthracite Coal /Pulverized Coal”.

## Assignment
### Questions
1. Have total emissions from PM2.5 decreased in the United States from 1999 to 2008? Using the base plotting system, 
make a plot showing the total PM2.5 emission from all sources for each of the years 1999, 2002, 2005, and 2008.

<p align="center" width="100%">
  <img src="https://github.com/rcflorestal/Data-Science-Specialization/blob/main/Exploratory-Data-Analysis/Course_Project_2/plot1.png">
</p>
 
2. Have total emissions from PM2.5 decreased in the Baltimore City, Maryland (fips == "24510") from 1999 to 2008?
Use the base plotting system to make a plot answering this question.

<p align="center" width="100%">
  <img src="https://github.com/rcflorestal/Data-Science-Specialization/blob/main/Exploratory-Data-Analysis/Course_Project_2/plot2.png">
  </p>
  
3. Of the four types of sources indicated by the type (point, nonpoint, onroad, nonroad)
variable, which of these four sources have seen decreases in emissions from 1999–2008 for Baltimore City?
Which have seen increases in emissions from 1999–2008? Use the ggplot2 plotting system to make a plot answer this question.

<p align="center" width="100%">
  <img src="https://github.com/rcflorestal/Data-Science-Specialization/blob/main/Exploratory-Data-Analysis/Course_Project_2/plot3.png">
  </p>
  
4. Across the United States, how have emissions from coal combustion-related sources changed from 1999–2008?

<p align="center" width="100%">
  <img src="https://github.com/rcflorestal/Data-Science-Specialization/blob/main/Exploratory-Data-Analysis/Course_Project_2/plot4.png">
  </p>

5. How have emissions from motor vehicle sources changed from 1999–2008 in Baltimore City?

<p align="center" width="100%">
  <img src="https://github.com/rcflorestal/Data-Science-Specialization/blob/main/Exploratory-Data-Analysis/Course_Project_2/plot5.png">
  </p>
  
 6. Compare emissions from motor vehicle sources in Baltimore City with emissions from motor vehicle sources in Los Angeles County, California (fips == "06037"). Which city has seen greater changes over time in motor vehicle emissions?
 
 <p align="center" width="100%">
  <img src="https://github.com/rcflorestal/Data-Science-Specialization/blob/main/Exploratory-Data-Analysis/Course_Project_2/plot6.png">
  </p>
  
