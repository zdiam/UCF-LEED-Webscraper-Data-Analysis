# UCF-LEED-Webscraper-Data-Analysis


This project was a fun way to learn some basic webscraping and introduce myself to Power BI as a visualization software. UCF has chosen to require a LEED certification on all new building and major renovations since 2007 on its main campus in Orlando, FL. All the data was pulled from UCF's resources and three UCF web links were used for information:

1) https://oeis.ucf.edu/buildings 
2) https://oeis.ucf.edu/stats
3) https://energy.ucf.edu/high-performance-buildings/


## Analysis and Lessons Learned

The final analysis images produced in Power BI:

![](https://github.com/zdiam/UCF-LEED-Webscraper-Data-Analysis/blob/main/Reference%20Images/PowerBI%20Output.PNG)

Ultimately, the final output paints a picture that isn't exactly clear and possibly a little unreliable due to how the data was obtained.

#### Left Side 

From the Average EUI (Energy Use Intensity) panels , it can be assumed that LEED does produce more energy efficient buildings. But it appears that the LEED certified buildings are the least energy efficient on the campus and that doesn't mesh well with that narrative. A lot of the inconsistencies come from the amount of buildings (low samples), and some of hidden factors that go into a diverse campus. Classrooms, laborities, and student housing are all grouped together to a paint an overall picture, but that helps make the data muddier instead of clearer.

Also, the UCF website had some inconsistenies within itself. The #3 link (High Performance Buildings) above produced a list of with more LEED buildings (and updated statuses) than the #1 & #2 (Open Energy Information). It appeared as though two different parties were providing information, with each really providing part of the picture and not wholly communicating with the other. 

This makes sense for such a large campus with multiple departments interacting with the buildings, but it provided a messy picture when trying to pull a good analysis.

#### Right Side

The Green Power/Electricity information on the right side of the above image doesn't provide much in determing that LEED is drastically changing the campus in its energy efficiency goals. That being said, it is a more accurate source of data coming directly from one source (link #2).

The Green Power purchased histogram seems to wildly swing from a high end value to an actual value of 0, but the average seems to be realistically close to the other two data points. The other 3 histogram plots paint a painfully average change that implies that nothing is really happening more than some typical fluctuations. 

*On the other hand*, the percent change plot below the histograms paints a bit of a different picture. It looks like the campus is producing more electricty, while purchasing less green power and electricity overall. It is also producing a little less green energy. But what does that really mean?

UCF has its own power plant which is providing the campus with electricity, but is that really being more *energy efficient*, or are they being more cost efficient. The latter seems more likely, and really this data strays further away from the LEED energy efficiency talk. While UCF could justify the power plant on the campus will reduce greenhouse gas emissions, it doesn't make the campus more energy efficient just more environmentally conscious (which is still a great thing!).

### Final Thoughts

This was a great projection to introduce myself to webscraping with the Beautiful Soup Python library and get familiar with Power BI as a tool. Ultimately, it became pretty obvious that the data source was inconsistent and that the answer/message I wanted to deduce was not going to be all that clear. Intutively, producing LEED certified buildings would make a campus more energy efficient, but that wasn't reinforced too strongly with this analysis. I walked away from this project with a handful of new skills and techniques, but also a greater understanding of the importance of being able obtain a good source of data that is dependable and accurate.
