# PRODIGY_DS_01
Task 1 Data Science Internship


library(readxl)

library(dplyr)

library(ggplot2)

dataset <- read_excel("C:/Users/GD DHANUSH/Downloads/Dataset.xlsx")

View(dataset)



# Create the bar chart
ggplot(dataset, aes(x = Gender)) +
  geom_bar(stat = "count") +  # count the number of employees in each gender category
  labs(title = "Distribution of Gender", x = "Gender", y = "Number of Employees")


![Screenshot 2024-05-30 175720](https://github.com/DhanushCU/PRODIGY_DS_01/assets/159162806/69b2d8ca-459a-4a6c-b114-cffbe03f6a63) 

# Create the histogram
ggplot(dataset, aes(x = Age)) +
  geom_histogram(bins = 10, color = "lightblue") +  # adjust the number of bins as needed
  labs(title = "Distribution of Age", x = "Age", y = "Number of Employees")

![Screenshot 2024-05-30 180624](https://github.com/DhanushCU/PRODIGY_DS_01/assets/159162806/7f4f47e3-16b9-4f06-8bf5-f55f73f054d2)
