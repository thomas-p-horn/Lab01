Lab 00 - Hello IDS!
================
INSERT TEAM NAME HERE
2022-09-23

### Load packages and data

``` r
library(tidyverse) 
```

### Exercises 13–17

We set up the data frame.

``` r
usernames <- c("wilsonamy", "Thomas", "Logan", "chad", "trent") #Extend if necessary
nums <- c(18, 18, 1, 4, 7) #Extend if necessary
colours <- c("powderblue", "Green", "blue", "red", "black") #Extend if necessary
hobbies <- c("Hiking", "Tennis", "subway", "bouncing", "reading") #Extend if necessary

team_data <- tibble(username = usernames, die_roll = nums, colour = colours,
                    hobby = hobbies)
```

### Exercise 18

We now work on visualising our data.

``` r
# Uncomment the three lines below
 p1 <- ggplot(team_data, aes(x = username, y = die_roll)) +
   geom_col(fill = team_data$colour)
 p1
```

![](lab-00_files/figure-gfm/bar-plot-1.png)<!-- -->

### Exercise 19

*Remove this text (including the stars), and add your answer for
Exercise 19 here.* hello hello again \### Exercises 20–21

``` r
# Uncomment the three lines below
# p1 +
#   labs(x = "Insert text here", y = "Insert text here",
#        title = "Insert text here")
```

*Remove this text (including the stars), and add your answer for
Exercise 21 here.*

### Exercise 22

``` r
p2 <- ggplot(team_data, aes(x = hobby)) +
  geom_bar()
p2
```

![](lab-00_files/figure-gfm/new-bar-plot-1.png)<!-- -->

*Remove this text (including the stars) and add your answer for Exercise
22 here.*
