# Subscripts-and-Indices-of-Dataframes
### SUBSCRIPTS AN INDICES ###

worms<-read.table("worms.txt", header = TRUE)
View(worms)
attach(worms)

names(worms)

worms[4,5] #To extract the value of the 4th row in the 5th column (Soil.pH)

worms[15:18,6] #To extract the value of the 15th to 18th rows of the 6th column (Damp)

worms[1:6, 1:4] #To extract the 1st to 6th rows of the 1st to 4th columns (Field names to Vegetation)

worms[4, ] #To extract all the columns of the 4th row

worms[ ,4] #To extract all the rows of the 4th column (Vegetation)

class(worms[4,])  # the will show a data.frame

class(worms[ , 4]) #what the class of the 4th column (Vegetation)

worms[ , c(1,7)] #To extract the 1st and 7th column (Field.name and worm density) using concatenate func

worms[c(1,7), ]  #To extract the 1st and 7th row using concatenate func


worms[c(1,7), c(1,5)] #To extract the the 1st and 7th row of the 1st and 5th columns  ()

worms[c(1:7), ]  # Extract the 1st 7 rows 






