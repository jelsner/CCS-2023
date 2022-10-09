Climate Change: Day 12
=====================
date: October 2, 2014

Last time: Estimating the sensitivity of hurricane intensity to SST. Or, linking MPI theory with observations. 

![alt text](coldWake.jpg)

Today: The oceans are certainly heating up. So are we actually seeing stronger hurricanes?

======
![alt text](LIvsSST.png)

======
![alt text](Sensitivity.png)

Tracks as Grids
===============
![alt text](TracksAsGrids.png)


Term Project Datasets
=====================
Datasets for term project. I'll continue to post links. You choose one. The posted links are in your notes. Here are some additional ones related to today's topic:

[U.S. Hurricane Frequency](http://myweb.fsu.edu/jelsner/data/US.txt)

[Annual Atlantic Hurricane Intensity](http://myweb.fsu.edu/jelsner/Hint.txt)

[Annual Atlantic Hurricane Frequency](http://myweb.fsu.edu/jelsner/Hfrq.txt)

[Hourly Atlantic Tropical Storms](https://dl.dropboxusercontent.com/u/448842/NATracks.txt)
You can download the file. Then read it into R using read.table(). You can't read directly from the URL.

Increasing Intensity
====================

```r
L = "http://myweb.fsu.edu/jelsner/Hint.txt"
H = read.table(L, header = TRUE)
H[1:2, ]
```

```
  Year nTS AvgInt MaxInt
1 1851   6   59.8  101.1
2 1852   5   72.7  101.2
```

========

```r
library(ggplot2)
ggplot(H, aes(x = Year, y = MaxInt)) +
  geom_point() +
  geom_smooth(method = lm) +
  ylab("Maximum Hightest Intensity (m/s)") +
  theme_bw()
```

<img src="Day12-figure/unnamed-chunk-2.png" title="plot of chunk unnamed-chunk-2" alt="plot of chunk unnamed-chunk-2" width="700" height="500" style="display: block; margin: auto;" />

Lifetime Maximum Intensity
==========================
![alt text](LMI.png)

===========
![alt text](LMI2.png)

===========
![alt text](GlobalTCIntensityTrends.png)

Sensitivity
===========
![alt text](Sensitivity2.png)

[2008 Nature Paper](http://myweb.fsu.edu/jelsner/PDF/Research/ElsnerKossinJagger2008.pdf)

Get the Track Data
==================


```r
library(repmis)
All = source_DropboxData(file = "NATracks.txt", 
  key = "3q7v1kv2qxyrdtj", 
  sep = " ", 
  header = TRUE)
```

Compute LMI by Year and storm id
================================

```r
library(dplyr)
df = All %>%
  filter(WmaxS >= 34, SYear >= 1967) %>%
  group_by(SYear, Sid) %>%
  summarize(LMI = max(WmaxS) * .447)
```

Make the graph
==============

```r
ggplot(df, aes(x = factor(SYear), y = LMI)) +
  geom_boxplot() +
  theme_bw() +
  theme(axis.text.x = element_text(angle = 90, hjust = 1)) +
  xlab("") + ylab("Lifetime Maximum Intensity (m/s)")
```

<img src="Day12-figure/unnamed-chunk-5.png" title="plot of chunk unnamed-chunk-5" alt="plot of chunk unnamed-chunk-5" width="900" height="500" style="display: block; margin: auto;" />

Hurricane Climatology
=====================

![alt text](BookCover.png)

Nephila clavipes
================

![alt text](Nephila.jpg)
