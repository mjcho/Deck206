---
title       : An Analysis of the Bachelor Data
subtitle    : 
author      : 
job         : COMM 206 In-class Activity
logo        : bachelor.jpeg
framework   : io2012               # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js         # {highlight.js, prettify, highlight}
hitheme     : tomorrow             # 
widgets     : [mathjax, bootstrap, quiz] # {mathjax, quiz, bootstrap}
mode        : selfcontained        # {standalone, draft}
knit        : slidify::knit2slides
--- #DA

<style>
body {
  background-color: #000;
}
.quiz-option label{
  display: inline;
  font-size: 1em;
}
ul.nav li::before { content: ""; }  
ul.nav li{ font-size: 18px; line-height: 24px;}
</style>





## Descriptive Analysis
### Collected Variables

```
##  [1] "Season"            "Showtype"          "Date"             
##  [4] "Star"              "Star.Age"          "Star.Hair.Color"  
##  [7] "Star.Occupation"   "Winner"            "Winner.Hair.Color"
## [10] "Proposal"          "Outcome"
```
### Used Variables

```
##  [1] "Season"            "Showtype"          "year"             
##  [4] "Star.Age"          "Star.Hair.Color"   "Winner.Hair.Color"
##  [7] "Proposal"          "Outcome"           "duration"         
## [10] "color.agree"
```

--- #DA2
## Descriptive Analysis
### Proposal by Showtype

```
## Source: local data frame [3 x 3]
## Groups: Showtype
## 
##       Showtype Proposal  n
## 1     Bachelor       No  8
## 2     Bachelor      Yes 10
## 3 Bachelorette      Yes 10
```

--- #DA3
## Descriptive Analysis
### Average Show Duration and Age of the Bachelor

```
## Source: local data frame [5 x 6]
## Groups: Showtype, Proposal
## 
##       Showtype Proposal Outcome n avg.duration  avg.age
## 1     Bachelor       No   Apart 8     51.62500 31.12500
## 2     Bachelor      Yes   Apart 9     60.44444 31.88889
## 3     Bachelor      Yes Married 1     64.00000 30.00000
## 4 Bachelorette      Yes   Apart 7     63.42857 28.00000
## 5 Bachelorette      Yes Married 3     60.66667 28.00000
```

--- #DA4
## Correlations: Age and Show duration with Outcome

```
##   Star.Age   duration 
## -0.2121486  0.1039581
```

--- #DA5
## Correlations: Age and Show duration with Proposal

```
##   Star.Age   duration 
## -0.1746002  0.4326910
```



