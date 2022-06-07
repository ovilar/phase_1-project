
## My Phase 1 Project for Flatiron School
Phase 1 Project for Flatiron School's Data Science Program

### OVERVIEW
In this project, I evaluate the performance of movies by their return on investment (locally, globally and in total)
compared to their production costs. I also analyze how a genre of a movie can be associated with its rate of return.
It is worth mentioning that the whole analysis uses statistical means. One could question that the use of the median would be better suited,
given the skewd nature of the series. I agree with that argument, even though the conclusions are robust to different specifications.

### BUSINESS UNDERSTANDING
Over the past years, there has been a trend of content development/streaming services investment by major companies, such as Apple, Amazon,
Netflix and others. We consider an hypothetical situation where Microsoft requested an analysis of the movie industry to evaluate whether
this would be a profitable strategy.

As briefly described in the Overview area, I provide analysis on which factors are key when assessing movies performance, their
characteristics and the main drivers of success. At the end of the analysis, I provide three strategies that Microsoft could pursue.

The results have a general implication to the investors decision-making process, but also can be extended to the industry as a whole, to
actors/directors/producers/staff in general and the general public.

### DATA AND ANALYSIS
The databases used are: IMDB, Rotten Tomatoes, Box Office Mojo, The Movie Database and The Numbers Movie Database.
The main variables used are: Title, Year, Genre, Production Cost, Domestic Gross and Worldwide Gross. I also create return metrics that
take into account how a movie fared domestically (domestic gross scaled by production costs - 1), in foreign markets (same metric, but
using worldwide gross as the numerator; and total return (the sum of both gross box offices, divided by production costs minus one).

It is worth mentioning that the use of return metrics provides a comparable index which circumvents potential inflation effects when 
comparing movies from different years. Even though straightforward, the limitation of the analysis is that we don't observe revenues from
different activities, such as licensing rights, spin-offs and other items. This is a suggestion of an analysis that can be extended using
other datasets.

The analysis considers a time-span from 1975 (the blockbuster-movie era) to 2018.

#### Production Costs, Domestic Gross, and Worlwide Gross
![Production Costs, Domestic Gross, and Worldwide Gross](https://github.com/ovilar/phase_1-project/blob/main/img/figure_00.png?raw=true)

#### The most profitable genres
Horror movies on average have a total return of 1,742%! They are followed by Thrillers and Mystery (711% and 625%, respectively).
![Most profitable genres: Horror, Thriller and Mystery](https://github.com/ovilar/phase_1-project/blob/main/img/figure_01.png?raw=true)

#### Other/Indie Studios
If we subsample our database using smaller studios, we find that Mystery, Drama and Thriller are the most profitable movies. On average,
these movies have production costs os $24 million and they fare $26 million and $62, domestically and worlwide - respectively.

![Other/Indie Studios](https://github.com/ovilar/phase_1-project/blob/main/img/figure_02.png?raw=true)

### CONCLUSION
I suggest three strategies: 
<ul>
<li>Going big: high production costs, aiming higher revenues and other sources of income, such as licensed products;</li>
<li>The safer route: developing content using niche movies such as Horror, Thriller and Mystery, since they have a higher
likelihood of performing better;</li>
<li>Start small: explore future synergies by starting small (indie movies), through a boutique approach.</li>
</ul>


#### Closing remarks
You will find at this repository: the jupyter notebook files, depicting all the processes run using Pandas;
this README.md file with general instructions. Unfortunately, given file size limitations the databases 
couldn't be uploaded to GitHub.

I hope you enjoy! Feel free to reach out with any suggestion and/or criticism.

#### LIMITATIONS
I do not analyze movies from the past and or the performance of series. Furthermore, one cool
analysis that might be interesting is merging this information with licensing products/rights datasets.
This would allow to check whether certain movies are able to grab a bigger piece of the revenue pie through
other activities.

Thank you!
