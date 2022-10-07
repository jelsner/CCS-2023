<style type="text/css">
.small-code pre code {
font-size: 1.3em;
}
</style>

Climate Change: Day 4
=====================
date: September 4, 2014

[Cumulus clouds in time lapse](http://www.shutterstock.com/video/clip-6568283-stock-footage-fast-motion-of-the-lumpy-puffy-sunny-clouds-on-deep-blue-sky-background-meditative-and-relaxing.html&download_comp=1)

<video width="320" height="240" controls>
  <source src="cumulusMotion.mp4" type="video/mp4">
</video>

+ Saturation and water vapor (not all heat warms)
+ Convection (the key to understanding future storms)
+ Is Florida getting hotter? (example term project)

Last Time
=========

+ Heat
+ Structure & Composition of the Atmosphere

[Poll Everywhere](http://www.polleverywhere.com/)

Water Vapor
===========
+ Water vapor & latent heat
+ Vapor pressure & saturation (dynamic equilibrium)
+ saturation vapor pressure vs temperature

Convection
==========
+ Radiation model (naked planet) / incompressible atmosphere
+ Dry vs moist convection
+ Environmental vs parcel lapse rates
+ Stability

Is Florida Getting Hotter?
==========================
class: small-code

```r
L = 'http://myweb.fsu.edu/jelsner/data/FLMonthlyT.txt'
df = read.table(L, header = TRUE)
library(ggplot2)
ggplot(df, aes(x = Year, y = Annual)) +
  geom_line() + ylab("Annual Temperature (F)")
```

<img src="Lecture4-figure/unnamed-chunk-1.png" title="plot of chunk unnamed-chunk-1" alt="plot of chunk unnamed-chunk-1" width="500" style="display: block; margin: auto;" />

Is Florida Getting Warmer?
==========================
class: small-code
<img src="Lecture4-figure/unnamed-chunk-2.png" title="plot of chunk unnamed-chunk-2" alt="plot of chunk unnamed-chunk-2" width="1000" style="display: block; margin: auto;" />

Old Weather Records
===================

[Old Weather Records](http://www.npr.org/player/v2/mediaPlayer.html?action=1&t=1&islist=false&id=341697516&m=345428587)
