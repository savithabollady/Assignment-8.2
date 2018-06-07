library(RcmdrPlugin.IPSUR)
data(RcmdrTestDrive)
Perform the below operations:
1. Compute the measures of central tendency for salary and reduction which variable has highest center?

Answer:
boxplot(RcmdrTestDrive$salary, RcmdrTestDrive$reduction,
        names = c("salary","reduction"),
        main="Boxplots Comparing salary & reduction", 
        col='red')
Salary has highest center


2. Which measure of center is more appropriate for before and after?

boxplot(RcmdrTestDrive$before, RcmdrTestDrive$after,
        names = c("Before","After"),
        main="Boxplots Comparing Before & After", 
        col='green')
par(mfrow = c(1,2))
hist(RcmdrTestDrive$before,xlab = "before",
        main="Histogram Comparing Before ", 
        col='yellow')
hist(RcmdrTestDrive$after,xlab = "After",
     main="Histogram Comparing Before ", 
     col='blue')

