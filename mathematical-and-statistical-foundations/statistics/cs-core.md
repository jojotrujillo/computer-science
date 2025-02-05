CS Core
================

<!-- "How foolish can you be? After starting your new lives in the Spirit, why are you now trying to become
perfect by your own human effort?" Galatians 3:3 (NLT) -->

### Statistics

#### Concepts

Many situations require information about a large group of elements
(individuals, companies, voters, households, products, customers, and so
on). But, because of time, cost, and other considerations, data can be
collected from only a small portion of the group. The larger group of
elements in a particular study is called the **population**, and the
smaller group is called the **sample**.

As an example of statistical inference, let us consider the study
conducted by Norris Electronics. Norris manufactures a high-intensity
lightbulb used in a variety of electrical products. In an attempt to
increase the useful life of the lightbulb, the product design group
developed a new lightbulb filament. In this case, the population is
defined as all lightbulbs that could be produced with the new filament.
To evaluate the advantages of the new filament, 200 bulbs with the new
filament were manufactured and tested. Data collected from this sample
showed the number of hours each lightbulb operated before filament
burnout.

#### Definitions

**Population**: the set of all elements of interest in a particular
study

**Sample**: a subset of the population

Create and interpret frequency tables…

``` r
library ('data.table')

data_table <- data.table(col1 = sample(6 : 9, 9,
    replace = TRUE),
    col2 = letters[1 : 3],
    col3 = c(1, 4, 1, 2, 2, 2, 1, 2, 2))

print ("Original DataFrame")
```

    ## [1] "Original DataFrame"

``` r
print (data_table)
```

    ##     col1   col2  col3
    ##    <int> <char> <num>
    ## 1:     6      a     1
    ## 2:     9      b     4
    ## 3:     8      c     1
    ## 4:     8      a     2
    ## 5:     7      b     2
    ## 6:     7      c     2
    ## 7:     8      a     1
    ## 8:     8      b     2
    ## 9:     9      c     2

``` r
freq <- table(data_table$col1)

print ("Modified Frequency Table")
```

    ## [1] "Modified Frequency Table"

``` r
print (freq)
```

    ## 
    ## 6 7 8 9 
    ## 1 2 4 2

``` r
print ("Cumulative Frequency Table")
```

    ## [1] "Cumulative Frequency Table"

``` r
cumsum <- cumsum(freq)
print (cumsum)
```

    ## 6 7 8 9 
    ## 1 3 7 9

``` r
print ("Relative Frequency Table")
```

    ## [1] "Relative Frequency Table"

``` r
prob <- prop.table(freq)
print (prob)
```

    ## 
    ##         6         7         8         9 
    ## 0.1111111 0.2222222 0.4444444 0.2222222

Measure of central tendency:

Variance:
