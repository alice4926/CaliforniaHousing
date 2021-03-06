<h2><strong>Where Should You Invest In California Real Estate?</strong></h2>
<address>Team Members &nbsp;&nbsp;Xin Li, &nbsp;Chia-Hui Shen, &nbsp;Ying-Chen Chou,&nbsp;Danyang Chen </address>


<https://github.com/alice4926/CaliforniaHousing><br> 
<https://alice4926.github.io/CaliforniaHousing/>

<h3> Purpose </h3>

<p>According to statistics from U.S. Census Bureau in 2016, the median housing price in California is much higher than thoes 
    in U.S for over 50,000 dollars. The reasons are not only overwhelm demanding from residents or prospective residents but also the extraordinary price changes inside California. Although the median housing price is relatively high, we still can know more about regions where are worthwhile to invest and where should be avoided buying house with unreasonable price. 
    Therefore, in this project, we will use Zillow housing price data for each counties in California and some features to find the best combination of feature of house with housing price and let people know more about housing price in California.</p>

<div>
   <a href="https://plot.ly/~aenni0409/71/?share_key=aliiu2NR6RwVq2g9EcDqed" target="_blank" title="color-bar" style="display: block; text-align: center;"><img src="https://plot.ly/~aenni0409/71.png?share_key=aliiu2NR6RwVq2g9EcDqed" alt="color-bar" style="max-width: 40%;width: 500px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
   <script data-plotly="aenni0409:71" sharekey-plotly="aliiu2NR6RwVq2g9EcDqed" src="https://plot.ly/embed.js" async></script>
</div>


<h3> Data Sources </h3>

<a href="http://www.zillow.com/research/data/">Zillo</a> <br>
<a href="http://school-ratings.com/counties/Alameda.html?type=HS&rankFilter=10)">School Rating</a> <br>
<a href="https://www.census.gov/quickfacts/table/PST045216/06">U.S. Census Bureau</a> <br>
<a href="https://ucr.fbi.gov">Federal Bureau of Investigation</a> <br>
<a href="https://en.wikipedia.org/wiki/Southern_California#Counties">Wikipedia For Southern California</a> <br>

<h3> Data Description </h3>

<p>Fist, we discussed time-series housing data which comes from open data sourse Zillow. Part of dataframe are below</p>
<p><img src='./plot/Time_Series_Data.png' style="max-width: 100%;width: 800px;" width="600" ></p>
Because sold price has more complete data from 1996, we use sold price to discuss futher in Time-Series.

<p>Second, we discussed the rencent two year listing, sold price with features. Part of dataframe are below</p>
<p><img src='./plot/All_Data_Set.png' style="max-width: 100%;width: 800px;" width="600"></p>
Features : Unemployment rate, Income, Population, Criminal Rate, School Scores

Due to lots of missing value in our dataframe, especially two counties Sierra, Alpin which have much few population than others, we will omit thoes two counties in the following analysis.

<h3> Time-Series Data </h3>

<h4> <li> Mean and Median All-homes price in California from 1996 to 2016 </li></h4>
<p>According to the time-series line below, we can find that the housing price from 1996 to Jun 2007 was increased. However, after mid-year
    2007, the price started to decrease. One of the main reason is the subprime mortgage crisis has started and a collapse of housing bubble
    started from December 2007 to June 2009. Not until 2011, the housing price has started to increase. For the fill with gray is the error
    bar with one standard deviation. You can find that even in the California, in different counties still have significant difference in the
    median housing price. Therefore, we nee to discuss every county seperately later.
    </p>
   <div>
        <a href="https://plot.ly/~aenni0409/64/" target="_blank" title="plot from API (28)" style="display: block; text-align: center;"> <img src="https://plot.ly/~aenni0409/64.png" alt="plot from API (28)" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
     <script data-plotly="aenni0409:64" src="https://plot.ly/embed.js" async></script>
    </div> 


<h4> <li> Housing inventory from Jan 2010 to Jan 2017 </li></h4>
<div>
    <a href="https://plot.ly/~danielle91515/12/?share_key=AmJbymQR4ZcRftOERQli07" target="_blank" title="index-as-date" style="display: block; text-align: center;"><img src="https://plot.ly/~danielle91515/12.png?share_key=AmJbymQR4ZcRftOERQli07" alt="index-as-date" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="danielle91515:12" sharekey-plotly="AmJbymQR4ZcRftOERQli07" src="https://plot.ly/embed.js" async></script>
</div>

<p>
This is a time series plot to describe the number of houses available in all the counties of California from Jan 2010 to Jan 2017. We are interested to know that the influence of house supply on the median sold house price. If you look at Aug 2011, the house inventory in Los Angles is the highest, we have 32932 houses available in the market. The median house price at that time is roughly the lowest, which is 365.003k. Another good example will be in San Mateo, Marin and Santa Clara, the inventories of those two counties start to decrease since 2012. And the median sold house price start to increase since that time.</p>

<h4><li>Median All-home price and Unemployment Rate </li></h4>
<div>
    <a href="https://plot.ly/~alice4926/19/?share_key=NdSlTVEZPBPUSh9D4kKjLh" target="_blank" title="unemployment_vs_sold15_plot" style="display: block; text-align: center;"><img src="https://plot.ly/~alice4926/19.png?share_key=NdSlTVEZPBPUSh9D4kKjLh" alt="unemployment_vs_sold15_plot" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="alice4926:19" sharekey-plotly="NdSlTVEZPBPUSh9D4kKjLh" src="https://plot.ly/embed.js" async></script>
</div>

<p>To discuss if any relationship between housing price and unemployment rate, we plot the time series plot of each. From the plot, it’s clear that they might exist negative relationships. When the unemployment rate falls, the median housing price will increase. We inferred that this might because that the district might be in good economic times when the unemployment rate decrease. Therefore, people would be richer and tend to buy an estate.</p>


<h4><li> Median All-home price for each county </li></h4>
    
<p>For the county seperately, we can find that all of county has the same pattern as the overall median housing price in California above except
    San Francisco. Housing Price in San Francisco did not decline significantly during the subprime mortgage crisis. The top five most expensive 
    housing price counties in 2015 are San Francisco, San Mateo, Marin, Santa Clara, and Santa Cruz. Those five counties are all near Bay Area. For 2016, the top five most expensive housing price counties are San Francisco, San Mateo, Marin, Santa Clara, and Alameda. Similary, those two years are all near Bay Area.</p>
  
<div>
    <a href="https://plot.ly/~aenni0409/195/?share_key=XbZ0Mtq8KBB6ruwq1vWbAp" target="_blank" title="plot from API (17)" style="display: block; text-align: center;"><img src="https://plot.ly/~aenni0409/195.png?share_key=XbZ0Mtq8KBB6ruwq1vWbAp" alt="plot from API (17)" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="aenni0409:195" sharekey-plotly="XbZ0Mtq8KBB6ruwq1vWbAp" src="https://plot.ly/embed.js" async></script>
</div>

<h4> <li>Criminal Rate From 2005 to 2015</li> </h4>
<div>
    <a href="https://plot.ly/~63xinxin/32/?share_key=XP5ZFFRjLga6cYRETQNlWP" target="_blank" title="plot from API (12)" style="display: block; text-align: center;"><img src="https://plot.ly/~63xinxin/32.png?share_key=XP5ZFFRjLga6cYRETQNlWP" alt="plot from API (12)" style="max-width: 50%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="63xinxin:32" sharekey-plotly="XP5ZFFRjLga6cYRETQNlWP" src="https://plot.ly/embed.js" async></script>
</div>
<p> The size of the points depend on value of the housing price those years. In this plot we can see that in 2006, the criminal rate and housing price were very high. So the value in 2016 can be seen as outlier or unnormal case. For the points in other years we can find out a decrease trend of criminal rate through time. But there is a slightly increase for criminal rate in 2015. For housing price, there is also a decreasing trend from 2006 to 2012. And housing price starts to increase from 2013 to 2015. This plot implies that housing price has a increase trend in the future.</p>




<h3> Relation between Features and Housing Price</h3>

<h4> <li> Overall Housing Prices</li></h4>

<h5> 1. Scatterplot Matrix </h5>
<p>According to the scatter matrix, unemployment rate is decreaesed when sold price in 2015 increases and when school scores is increases. Because some variables, such as crime and population are lefe-skew, we take log tranformation to those two variables. Log population has negative relation with income per person. Log crime has negative relation with log population. We will discuss more about each feature seperately.</p>
<div>
   <a href="https://plot.ly/~aenni0409/77/?share_key=YUn5DjA89OUDq02T4mfSAn" target="_blank" title="Scatterplot Matrix" style="display: block; text-align: center;"><img src="https://plot.ly/~aenni0409/77.png?share_key=YUn5DjA89OUDq02T4mfSAn" alt="Scatterplot Matrix" style="max-width: 100%;width: 800px;"  width="800" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
   <script data-plotly="aenni0409:77" sharekey-plotly="YUn5DjA89OUDq02T4mfSAn" src="https://plot.ly/embed.js" async></script>
</div>


<h5> 2. Compound Annual Growth Rate(CAGR) for recent five year (2012-2016) </h5>

<p>To know which counties growth rate of housing price increase most, we used CAGR to as critian. The growth rate in Colusa, San Benito, Stanislaus, and Solano, and San Joaquin have highest positive growth rate. On the other hand, the  growth rate in Del Norte, which is the northest county in California, is the only one with negative growth rate.</p>

<div>
    <a href="https://plot.ly/~aenni0409/193/?share_key=7gNLmHmPwNZPMHQAuixSyr" target="_blank" title="CAGR" style="display: block; text-align: center;"><img src="https://plot.ly/~aenni0409/193.png?share_key=7gNLmHmPwNZPMHQAuixSyr" alt="CAGR" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="aenni0409:193" sharekey-plotly="7gNLmHmPwNZPMHQAuixSyr" src="https://plot.ly/embed.js" async></script>
</div>




<h4><li> Housing Price between Southern and Northen California </li></h4>
<div>
    <a href="https://plot.ly/~alice4926/25/?share_key=E57ttr0jCXyTAsgHdFBcNz" target="_blank" title="SvsN_sold15_plot" style="display: block; text-align: center;"><img src="https://plot.ly/~alice4926/25.png?share_key=E57ttr0jCXyTAsgHdFBcNz" alt="SvsN_sold15_plot" style="max-width: 100%;width: 985px;"  width="985" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="alice4926:25" sharekey-plotly="E57ttr0jCXyTAsgHdFBcNz" src="https://plot.ly/embed.js" async></script>
</div>

<p>The box plot showed the minimum, maximum, 25%, median, and 75% of the sold price in 2015 for Northern CA and Southern CA separately. The dash line represent the mean sold price. From the plot, price in Northern and Southern are distributed differently. However, their mean are close. To test if two price mean are the same, we do the two sample t test with the null hypothesis that the difference of two mean are zero. Base on the result of hypothesis, the p-value is large. We can conclude that two price mean are the same. </p>

<pre><code>## 
##  Welch Two Sample t-test
## 
## data:  CA_price15$sold_15 by CA_price15$district
## t = -1.0364, df = 19.248, p-value = 0.3128
## alternative hypothesis: true difference in means is not equal to 0
## 95 percent confidence interval:
##  -176277.24   59446.93
## sample estimates:
## mean in group north mean in group south 
##            339166.9            397582.1</code></pre>


<h4><li> Income vs Housing Price </li></h4>

<div>
    <a href="https://plot.ly/~alice4926/29/?share_key=PDMNGKhGsw1eYKZg1u0tUk" target="_blank" title="income_vs_sold15_plot" style="display: block; text-align: center;"><img src="https://plot.ly/~alice4926/29.png?share_key=PDMNGKhGsw1eYKZg1u0tUk" alt="income_vs_sold15_plot" style="max-width: 100%;width: 985px;"  width="985" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="alice4926:29" sharekey-plotly="PDMNGKhGsw1eYKZg1u0tUk" src="https://plot.ly/embed.js" async></script>
</div>
<p>For income, it seemed not to have significant effect on housing price. The housing price in counties with higher income per person  was similar to that in other counties. We can infer that income might not be an important factor to influencing the housing price. In this plot, there are some outlier points. Those are San Francisco, Marin. In this two counties, the income and housing price are both high. </p>

<h4><li> 4. Population vs Housing Price </li></h4>
<div>
    <a href="https://plot.ly/~alice4926/27/?share_key=8lmY90MD6kmniGWPS5rv1F" target="_blank" title="populaiton_vs_sold15_plot" style="display: block; text-align: center;"><img src="https://plot.ly/~alice4926/27.png?share_key=8lmY90MD6kmniGWPS5rv1F" alt="populaiton_vs_sold15_plot" style="max-width: 50%;width: 985px;"  width="985" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="alice4926:27" sharekey-plotly="8lmY90MD6kmniGWPS5rv1F" src="https://plot.ly/embed.js" async></script>
</div>
<p>Generally, the county where more people live will tend to have higher housing price. According to the plot, population might have some positive effect on the housing price. Especially for San Francisco, San Mateo, and Santa Clara, it was clear that there is higher population and also higher housing price. However, for Los Angeles, although the population is high but the housing price is not as high as expected.</p>

<h4> <li>Schools vs. Housing price </li></h4>
<h5> 1. Schools scores distribution </h5>
<div>
    <a href="https://plot.ly/~danielle91515/3/?share_key=JAKR1issa4h5YSqNcfuahN" target="_blank" title="county-level-choropleths-python" style="display: block; text-align: center;"><img src="https://plot.ly/~danielle91515/3.png?share_key=JAKR1issa4h5YSqNcfuahN" alt="county-level-choropleths-python" style="max-width: 50%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="danielle91515:3" sharekey-plotly="JAKR1issa4h5YSqNcfuahN" src="https://plot.ly/embed.js" async></script>
</div>
<p>
This is a county level choropleths map showing the trend of school scores 2016 obtained from <a href="https://www.schooldigger.com">Schooldigger</a>. For each county, I sum the elementary, middle and high school scores up and average them in each county. Then, since the averaged score is between 0 to 1, for making this map, I divide the score by 0.01 to change its scale to 0 to 100 and assign the color for each county based on the value. In the map above, the more red the region is, the higher school score the county has. For general trend, we can see that northern California is doing better than southern part of California. There are more red regions around San Francisco. The highest region is Marin (0.7644). The second runner up is San Jose (0.73). The third runner up is San Francisco (0.7242). They are all located at northern California. If we take a closer look at southern part of California, the highest score region is Irvien (0.6744). The second runner up is Santa Barbara (0.6471). Because Los Angeles has the most number of schools in California, the score range may be quite different. It does not the top rank county in southern part of California. The average score is 0.57.
</p>

<p><img src ="./plot/bar_error_school.png" style="max-width: 50%;width: 800px;"  width="300"></p>

<p>
This picture shows the variance of school scores in each county. It is interesting to see that the variance of los angeles is not huge. That means the reason Los Angeles is not the top rated county for school is that all the school scores in Los Angeles are not high. Trinity has the largest variance among all the counties. Its school scores range from 0.4 to 0.9. Marin, San Jose and San Francisco all have smaller variance. That means all the schools in those counties perform well.</p>

<h5> 2.Schools scores distribution Vs. Housing prices </h5>

<div>
    <a href="https://plot.ly/~danielle91515/9/?share_key=4DxT9ezsrhdrb8qrOigEb5" target="_blank" title="Average Sold Housing Price in 2015 v. School Scores in 2015" style="display: block; text-align: center;"><img src="https://plot.ly/~danielle91515/9.png?share_key=4DxT9ezsrhdrb8qrOigEb5" alt="Average Sold Housing Price in 2015 v. School Scores in 2015" style="max-width: 50%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="danielle91515:9" sharekey-plotly="4DxT9ezsrhdrb8qrOigEb5" src="https://plot.ly/embed.js" async></script>
</div>

<p>
This interactive plot shows the relationship between average median sold house price from zillow in each county and school scores in 2015. The size of the bubble depends on the number of schools in that county. The larger the bubble, the more school that county has. We can see that there is a positive correlation between these two variables. The higher the school score, the higher average sold house price. We can see that San Mateo and Marin have a good combination of the two.Tulane and Fresno have lowest school scores and average sold house price. </p>

<div>
    <a href="https://plot.ly/~danielle91515/7/?share_key=6PYY3NPYqP7nrOXrpGXBCg" target="_blank" title="Average Sold Housing Price in 2016 v. School Scores in 2016" style="display: block; text-align: center;"><img src="https://plot.ly/~danielle91515/7.png?share_key=6PYY3NPYqP7nrOXrpGXBCg" alt="Average Sold Housing Price in 2016 v. School Scores in 2016" style="max-width: 50%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="danielle91515:7" sharekey-plotly="6PYY3NPYqP7nrOXrpGXBCg" src="https://plot.ly/embed.js" async></script>
</div>


<p>
This interactive plot shows the relationship between average median sold house price from zillow in each county and school scores in 2016.The general trend is the same as the one in 2015. However, some counties has shifts in postion. For example, lake county has lower average school scores but higher average median sold house prices.
</p>


<h4><li> Criminal Rate vs Housing Price </li></h4>
<div>
    <a href="https://plot.ly/~63xinxin/4/?share_key=zcMf14QGDeRcg3rLVfj5TB" target="_blank" title="Housing-Price-vs-Criminal-Rate-in-2015" style="display: block; text-align: center;"><img src="https://plot.ly/~63xinxin/4.png?share_key=zcMf14QGDeRcg3rLVfj5TB" alt="Housing-Price-vs-Criminal-Rate-in-2015" style="max-width: 50%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="63xinxin:4" sharekey-plotly="zcMf14QGDeRcg3rLVfj5TB" src="https://plot.ly/embed.js" async></script>
</div>

<p> (a)The size of those points are population size. From this plot we can find out that there is negative relationship between housing price and criminal rate. The larger the price, the smaller the criminal rate.<br> 
    (b)Even though there is overlap between counties of high population and counties of low population, regions with small population tends to have higher criminal rate. This is a very interesting result. Because, most of the time we will think that if there are more people, there tends to be have larger criminal rate. <br> 
    (c) Counties with larger population tend to have higher housing price.<br> 
    Now, let's look at some unnormal counties. For example in San Francisco, it has the largest housing price and criminal rate. 
</p>




<h3> Conclusion</h3>
<p> According to time series analysis, each county in California has similar pattern with the overall sold price except San Francisco whose housing price did not decrease much even during the subprime mortgage crisis. Housing inventory dataset shows that house supply in California has negative relation with sold price. Both unemployment rate and criminal rate present negative relationship with housing price.<br> By analyzing different features that might relate to sold price in spacial aspect, we find out that almost all counties in California have positive growth rate of housing price from 2012 to 2016. Even though school scores in Northern California have higher value than those in Southern California, there is no difference of housing price between Southern and Northen California. What's more, income does not show significant relationship with housing price after exploring data in different counties. But there present positive relationship of sold price and school scores. Unemployment rate exhibit negative relationship with housing price. <br> In sum, after comparing all those results for each county, we think Orange county is the most appropriate county when choosing to buy a house in California. </p> 
