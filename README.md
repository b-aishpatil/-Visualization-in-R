# Visualization-in-R

## R studio commands
1. How to clear R studio console
`CNTRL + L`

## Visualization Commands

1. How to load dataset
```
cricket <- read.csv("C:/Users/User/Downloads/cs.csv")
```

2. How to view data 
```
View(cricket)
```
![image](https://user-images.githubusercontent.com/92450677/203500520-e40743c1-10a1-45aa-a400-4104644648fa.png)


3.	To get first 7 rows
```
head(cricket,7)
```
![image](https://user-images.githubusercontent.com/92450677/203500442-ec6ec5fb-813b-476c-8584-5a8a2f836b13.png)


4. To remove last 7 rows and print remaining data 
```
head(cricket,-7)
```
![image](https://user-images.githubusercontent.com/92450677/203500385-04befdf5-2f80-4ba6-a5fd-c5d1a6a598e0.png)


5. To get last 7 rows
```
tail(cricket,7)
```
![image](https://user-images.githubusercontent.com/92450677/203500313-ce9efab7-de25-4cf5-8413-2ff80cce75b0.png)


6. To remove first 7 rows and print remaining data 
```
tail(cricket,-7)
```
![image](https://user-images.githubusercontent.com/92450677/203500058-88281f9f-6972-4a91-967e-234255bc9c14.png)

7. To summaries dataset 
```
summary(cricket)
```
![image](https://user-images.githubusercontent.com/92450677/203502539-15dc4e2f-8165-4912-90f3-6ee7e2d478bc.png)

8. Creating pie-chart
```
pie(table(cricket$Country), main = "Pie Chart of the cricket data set of contries", col = c("orange","pink","red","blue","yellow","green","violet"), radius = 1)
```
![image](https://user-images.githubusercontent.com/92450677/203504766-10d56da1-2310-4a12-8d5c-2ae7c0eedb3f.png)

9. Plotting Histogram
```
hist(cricket$Sixes, col=c("green", "red", "blue"), xlab="Number of Sixes", ylab= "Frequncy of Sixes", main="Histogram of Sixes")
```
![image](https://user-images.githubusercontent.com/92450677/203508360-b1e81092-8567-4deb-b0ac-a3cc35a9f1df.png)






