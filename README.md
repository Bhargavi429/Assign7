# Assign7


data("airquality") 

list(airquality) 

head(airquality)

summary(airquality)

mys3class <- list(Ozone = "41", Month = "5",Day = "1")

class(mys3class) <- "airquality"

mode(mys3class)

class(mys3class)

attributes(mys3class)

setClass("airquality",representation(Ozone = "numeric",Month = "numeric",Day = "numeric"))

mys3class <- new("airquality", Ozone = 41, Month = 5, Day = 1)

mode(mys3class)

isS4(mys3class)

#Example of S3 using Function UseMethod()

student <-list(name = "Leo", Experience = 3 , major = "Bioinformatics") 

class(student) <-"student" 

get_info <-function(x) 

get_info.student <-function(x) 

my_student <-student

get_info(my_student)

setClass("Person", slots = c(name = "character", experience = "numeric", major = "character"))

setGeneric("summary")

person1 <- new("Person", name = "Leo", experience = 3, major = "Bioinformatics")

summary(person1)
