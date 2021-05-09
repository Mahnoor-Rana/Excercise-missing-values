# Excercise-missing-values
datasets::airquality
x<-airquality
x
is.na(x)
# missing value in dataset
sum(is.na(x))
# column wise
colSums(is.na(x))
#impute data of ozone
x$Ozone[is.na(x$Ozone)]<-mean(x$Ozone)
x$Ozone
na.omit(x)
