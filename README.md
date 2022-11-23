# Visualization-in-R

## R studio commands
1. How to clear R studio console
`CNTRL + L`

2. installing ggplot libararies
```
install.packages('ggplot2', repos='http://cran.us.r-project.org')
```

3. import ggplot
``` 
library(ggplot2)
``` 

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




3.	To get data from head

<table>

<tr>
<td align="center"> To get <b>first 7</b> rows</td> 
<td align="center"> To get all rows <b>except last 7</b> </td>
</tr>

<tr>
<td> 

```R
head(cricket,7)
```
</td>
<td>

```R
head(cricket,-7)
```
</td>
</tr>
<tr>
<td align="center"> <p align="center"> <img src="https://user-images.githubusercontent.com/92450677/203500442-ec6ec5fb-813b-476c-8584-5a8a2f836b13.png"/> </td> 
<td align="center"> <img src="https://user-images.githubusercontent.com/92450677/203500385-04befdf5-2f80-4ba6-a5fd-c5d1a6a598e0.png"/> </td>
</tr>

</table>


4. To get data from tail

<table>

<tr>
<td align="center"> To get <b>last 7</b> rows</td> 
<td align="center"> To get all rows <b>except last 7</b> </td>
</tr>

<tr>
<td> 

```R
tail(cricket,7)
```
</td>
<td>

```R
tail(cricket,-7)
```
</td>
</tr>
<tr>
<td align="center"> <p align="center"> <img src="https://user-images.githubusercontent.com/92450677/203500313-ce9efab7-de25-4cf5-8413-2ff80cce75b0.png"/> </p></td> 
<td align="center"> <img src="https://user-images.githubusercontent.com/92450677/203500058-88281f9f-6972-4a91-967e-234255bc9c14.png"/> </td>
</tr>

</table>


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


9. Plotting Scatterplot
```
plot(cricket$Fifties~cricket$Hundreds,xlab="Hundreds" ,ylab="Fifties", main="Scatterplot for Hundreds vs Fifties", col=c("blue", "red"),pch=16)
```
![image](https://user-images.githubusercontent.com/66154908/203515709-66390640-37a3-4261-8212-71ae62533007.png)


10. Plotting Scatterplot with background theme and symbols
```
ggplot(data=cricket,aes(y=Fifties,x=Hundreds,col=Country))+geom_point()
```
![image](https://user-images.githubusercontent.com/92450677/203516332-ff05059f-5337-4153-8969-3c0b10c10074.png)

10. Plotting Barchart with background theme and symbols
```
ggplot(data=cricket,aes(x=Hundreds,fill=Country))+geom_histogram(bins=50)
```
![image](https://user-images.githubusercontent.com/92450677/203518005-c5a2ccac-0d81-4030-8f7a-eb867d134936.png)


