Week 1 by AJ Jong
#R_week01
#get familiar with R and RStudio
#intalling a package
iris
plot(iris)
plot(iris$Sepal.Length, iris$Sepal.Width)
hist(iris$Sepal.Length)

#install.packages("ggplot2")
library(ggplot2)

# dataset:
data=data.frame(value=rnorm(100))
data=data.frame(value=iris$Sepal.Length)
# basic histogram
ggplot(data, aes(x=value)) + 
  geom_histogram()
