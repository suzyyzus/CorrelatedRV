# Simulate Two Correlated Random Variables :people_holding_hands::people_holding_hands:

I have surveyed all of the 347 students in sta 302 class and collected 10 adults' forearm length and height. My response variable is forearm length and explanatory variable is height.


Highlight of my Code


```{r, echo = FALSE}
scat.plot <- ggplot(the_data, aes(x = height, y = forearm))+ geom_point()+
labs(x = "Height", y = "Forearm Length", title = "Scatter Plot of Height vs. 
     Forearm Length 7813") 
# scatter plot which can help us analyzing the relationship between these two variables 
scat.plot 
```
```{r, echo = FALSE}
my.data <- data.frame("values"=c(height, forearm), "variables"=c(rep('height', 10),
        rep('forearm', 10))) box.plot <- ggplot(data=my.data, aes(y=values, x=variables))+ geom_boxplot()+ labs(title = "Box Plot of Height vs. Forearm Length 7813")
#I draw a boxplot for my sample data to see the dispersion of the data. box.plot 
```

```{r, echo = FALSE}
hist.plot <- ggplot(the_data, aes(x = forearm, y = ..count..))+ 
  geom_histogram(binwidth = 1, color = "white")+ labs(x = "Forearm Length",
          y = "Frequncy", title = "Histogram of Forearm Length 7813") 
#Histogram help to see the distribution of random variable Forearm Length hist.plot 
```
