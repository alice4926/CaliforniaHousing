<h2><strong>Where Should You Invest In California Real Estate?</strong></h2>
<address>Team Members &nbsp;&nbsp;Xin Li, &nbsp;Chia-Hui Shen, &nbsp;Ying-Chen Chou,&nbsp;Danyang Chen </address>


<https://github.com/alice4926/CaliforniaHousing><br> 
<https://alice4926.github.io/CaliforniaHousing/>

<h3> Purpose </h3>
    <p> According to statistics from U.S. Census Bureau in 2016, the median housing price in California is much higher than thoes 
    in U.S for over 50,000 dollars. The reasons are not only overwhelm demanding from residents or prospective residents but also the 
    extraordinary price changes inside California. Although the median housing price is relatively high, we still can know more about 
    regions where are worthwhile to invest and where should be avoided buying house with unreasonable price. 
    Therefore, in this project, we will use Zillow housing price data for each counties in California and some features to find the 
    best combination of feature of house with housing price and let people know more about housing price in California.
    </p>

<h3> Data Sources </h3>

### Datasets :
[Zillow](http://www.zillow.com/research/data/)<br>
[School Rating](http://school-ratings.com/counties/Alameda.html?type=HS&rankFilter=10)<br>
[U.S. Census Bureau](https://www.census.gov/quickfacts/table/PST045216/06)<br>
[Federal Bureau of Investigation](https://ucr.fbi.gov)

<h3> Data Description </h3>

<h3> Time-Series Data </h3>
<li> Mean and Median All-homes price in California from 1996 to 2016 </li>
<p>According to the time-series line below, we can find that the housing price from 1996 to Jun 2007 was increased. However, after mid-year
    2007, the price started to decrease. One of the main reason is the subprime mortgage crisis has started and a collapse of housing bubble
    started from December 2007 to June 2009. Not until 2011, the housing price has started to increase. For the fill with gray is the error
    bar with one standard deviation. You can find that even in the California, in different counties still have significant difference in the
    median housing price. Therefore, we nee to discuss every county seperately later.
   <div>
        <a href="https://plot.ly/~aenni0409/64/" target="_blank" title="plot from API (28)" style="display: block; text-align: center;"> <img src="https://plot.ly/~aenni0409/64.png" alt="plot from API (28)" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
     <script data-plotly="aenni0409:64" src="https://plot.ly/embed.js" async></script>
    </div> 
</p>

<li> Median All-home price for each county </li>
    
<p>For the county seperately, we can find that all of county has the same pattern as the overall median housing price in California above except
    San Francisco. 
    <div>
        <a href="https://plot.ly/~aenni0409/149/?share_key=LkvhYOxc9o2BO3dQkGGwtp" target="_blank" title="plot from API (1)" style="display: block; text-align: center;"><img src="https://plot.ly/~aenni0409/149.png?share_key=LkvhYOxc9o2BO3dQkGGwtp" alt="plot from API (1)" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
        <script data-plotly="aenni0409:149" sharekey-plotly="LkvhYOxc9o2BO3dQkGGwtp" src="https://plot.ly/embed.js" async></script>
    </div>
</p>

<h3> Relation between Features and Housing Price</h3>

<li> Overall </li>

<p>According to the scatter matrix, unemployment rate is decreaese when sold price in 2015 increases and when school scores is increases.
Moreover 
   <div>
       <a href="https://plot.ly/~aenni0409/77/?share_key=YUn5DjA89OUDq02T4mfSAn" target="_blank" title="Scatterplot Matrix" style="display: block; text-align: center;"><img src="https://plot.ly/~aenni0409/77.png?share_key=YUn5DjA89OUDq02T4mfSAn" alt="Scatterplot Matrix" style="max-width: 100%;width: 800px;"  width="800" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
       <script data-plotly="aenni0409:77" sharekey-plotly="YUn5DjA89OUDq02T4mfSAn" src="https://plot.ly/embed.js" async></script>
   </div>
</p>

<li> Income vs Housing Price </li>

<p>
   <div>
       <a href="https://plot.ly/~alice4926/9/?share_key=GCR8XsntiJ4JFp4qxYDvPR" target="_blank" title="Income vs Price" style="display: block; text-align: center;"><img src="https://plot.ly/~alice4926/9/?share_key=GCR8XsntiJ4JFp4qxYDvPR" alt="Income vs Pricex" style="max-width: 100%;width: 800px;"  width="800" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
   </div>
</p>


<h3> Conclusion</h3>
