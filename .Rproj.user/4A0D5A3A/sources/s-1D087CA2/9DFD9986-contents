# Author: Obunge
# Topic: Univariate Analysis
# Strategy: EDA
# Dataset: bike_buyers- dataset with various vaiables of prospect buyers of the bike
# 
# Objectives of EDA strategy
#  1. Understand the variables.
#  2. Understand the pattern formed by the variable.
#  3. Help informing modeling approach to undertake.


#get and set the working directory
getwd()
setwd("C:/Users/dobunge/Desktop/Workfolder/Projects/R/UnivariateAnalysis")

# load the dataset
bikebuyers_data <- read.csv("bike_buyers.csv")


# look at the overview of the dataset
View(head(bikebuyers_data))
View(bikebuyers_data)

# check on the structure of the datasets
str(bikebuyers_data)

# convert columns to from int to factors: @NumOfChildrens n @NumCars
bikebuyers_data$Children <-as.factor(bikebuyers_data$Children)
bikebuyers_data$Cars<-as.factor(bikebuyers_data$Cars)
#' 
#' @verify the conversion using str
str(bikebuyers_data)

# #data wrangling using dplyr and tidyverse 
# load the dplyr package

library(dplyr)
head(bikebuyers_data)
# convert data frame to tbl class for easy of view on the 
dplyr::tbl_df(bikebuyers_data)

# get dense information summary about the data
dplyr::glimpse(bikebuyers_data)
# remove ID column
bikebuyers_data<-bikebuyers_data %>% select(-ï..ID)
dplyr::tbl_df(head(bikebuyers_data))

# visualize variables one by one_of()
library(ggplot2)
income_plot<-ggplot(bikebuyers_data,aes(Income))+geom_histogram()
income_plot

income_boxplot<-ggplot(bikebuyers_data, aes(Income))+geom_boxplot()
income_boxplot
summary(bikebuyers_data)
