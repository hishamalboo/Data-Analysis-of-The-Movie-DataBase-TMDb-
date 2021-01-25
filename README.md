# Data-Analysis-of-The-Movie-DataBase-TMDb-



<a id='intro'></a>
<h1> Introduction</h1>

<p style="font-size:100%;color:#811F86"><strong>  Every year hundreds of movies get released but not all of them are successful. The aim of the project is to analyze the TMDB movie dataset which has details about the movies, their production cost and revenue generated along with rating inforamtion.I am going to gather and analyze data  <a href = "https://d17h27t6h515a5.cloudfront.net/topher/2017/October/59dd1c4c_tmdb-movies/tmdb-movies.csv">"TMDb movie"</a>. For that, data is gathered via manual download. After that I am going to wrangle , anlayze(exploratory and explantory),and make conclusion for this data.We are trying to analyze the dataset to find answers to the questions posed below.<br> We will start with a univariate analysis and then move ahead with a mutivariate analysis to understand the impact of certain factors in determining the success of the movie.</strong></p>
<p style="font-size:100%;color:#811F86"><b><u>The success of a movie could be measured in terms of the following metrics:</u></b></p>
   
<p style="font-size:100%;color:#3E8A10"><strong>a- Return on Investment: which will be a measure of the profit generated for movies.</strong></p>
<p style="font-size:100%;color:#3E8A10"><strong>b- Rating by Public: which will also take into account the number of votes posted for </strong></p>

<p style="font-size:100%;color:#330703"><strong> Based on successful metrics mention above ,we will  try to answer the following questions:</strong></p>

<ol style="font-size:100%;color:#207863"> <strong><li>Which three of genres of movies are the most  productive between 1960 and 2015?</li><li>Which three of genres of movies achieved the most total profit  between 1960-2015?</li><li>I3- Which three of genres of movies achieved the most total voting public between 1960-2015?</li><li>When did  the highest release of movies happen?</li><li>Is there a releationship between voting public and profit for genres of movies?</li><li>Which genres of movies achieved the most likely total profit in the  period which achieved the most total profit of all movies?</li><li>Which genre of movies achieved the most likely total voting count in the  period which achieved the most total voting count of all movies?</li></strong></ol>


<a id='sources'></a>
## Data Sources
>TMDb movie (tmdb-movies.csv)</li>
><ul>   
>    <li><b>Source:</b> <a href = "https://d17h27t6h515a5.cloudfront.net/topher/2017/October/59dd1c4c_tmdb-movies/tmdb-movies.csv">collected fromThe Movie Database (TMDb)</a></li>    
>    <li><b>Method of gathering:</b> Manual download</li>
></ul>

<h1 style="font-size:140%;color:#3A0101"> Define The Observations</h1>
<p style="font-size:120%;color:darkblue"><strong>The dataset has 10866  rows and 21 columns,it contains information about movies collected from The Movie Database (TMDb), including:</strong></p>

<ol style="font-size:100%;color:#0B5345"> <strong><li>id : index number in dataset</li><li>imdb_id: IMDb Site index</li><li>popularity: rating of a particular title on IMDb indicates</li>         
<li>budget : cost of movie (thousand million)</li>              
<li>revenue: revenue of movie (thousand million)</li>               
<li>original_title : the movie name</li>       
<li>cast: the group of actors who make up a movie</li>               
<li>homepage: website the movie</li>   
<li>director:  who controls the making of a film and supervises</li>              
<li>tagline: a short text which serves to clarify an idea for, or is designed with a form of, dramatic effect</li>             
<li>keywords: is a word (or group of connected words) attached to a title  describe any notable object, concept, style or action</li>            
<li>overview:  is a brief summary that gives audiences an idea of what a movie is about </li>           
<li>runtime: the amount of time that a movie lasts from beginning to end.</li>              
<li>genres: categories that define a movie based on its narrative elements, each genre is unique in the types of stories they tell</li>               
<li>production_companies: are a business that provide the physical basis for works in the fields of performing movies</li>  
<li>release_date: is when a completed movie is released for the public</li>          
<li>vote_count : rating by public </li>          
<li>vote_average: the average rating by public</li>          
<li>release_year: is when a completed movie is released for the public </li>          
<li>budget_adj: cost of movie (thousand million), associated movie in terms of 2010 dollars,accounting for inflation overtime.</li><li>revenue_adj :revenue of movie (thousand million) ,associated movie in terms of 2010 dollars,accounting for inflation overtime.</li></strong></ol>            



<a id='wrangling'></a>
## Data Wrangling


### `Cleaning steps:`

 <font size = 4 color='purple'>

1-Removing the duplicated rows.
        
2- Drop missing data.
        
3- Drop zero values.        
    
4- Create new column that contains the profit of movies.
  
5- Create new dataset that contains genre for each movie.    

    

<p style="font-size:120%;color:#B9770E"><strong>After removing missing values,zero values,duplicated values, and adding columns in dataset,the number of columns become <u>22</u> and the number of rows become <u>5165</u> </strong> </p>

<a id='conclusion'></a>
## Conclusion and Limitations

><font size=4 color ='black'><b><u> Conclusion:</b></u></font>
>    
<font size=3 color ='#36722C'><b>Based on successful metrics: return on investment and rating by public, by Exploring our dataset,we have tried to answer the following questions:</b></font>
>
>       
><font size=3 color ='#330D07'><b><i>1- Which three of genres of movies are the most  productive between 1960 and 2015?</b></i></font>
>
><font size=3 color ='blue'><b>From figure1, we can observe that the genre of movies"Drama " is the most productive between 1960 and 2015, second is "Comedy",third is "Thriller", that means the investment  between 1960-2015 focused in general on genres of movies  "Drama", "Comedy",and "Thriller".</b></font>
>    
><font size=3 color ='#330D07'><b><i>2- Which three of genres of movies achieved the most total profit  between 1960-2015?</b></i></font>
>    
><font size=3 color ='blue'><b>From figure2, we can observe that the genre of movies"Comedy" achieved the most total profit  between 1960 and 2015, second is "Action",third is "Adventure".</b></font>
>    
><font size=3 color ='#330D07'><b><i>3- Which three of genres of movies achieved the most total voting public between 1960-2015?</b></i></font>
>
><font size=3 color ='blue'><b>From figure3, we can observe that the genre of movies"Drama" achieved the most voting public  between 1960 and 2015, second is "Action",third is "Comedy".
>
><font size=3 color ='#330D07'><b><i>4- When did  the highest release of movies happen?</b></i></font>
>
><font size=3 color ='blue'><b>From figure4, we can observe that the trend of production of movies is increasing slightly between 1960 and 1993 and increasing sharply between 1993 and  2013 and decreasing sharply between 2013 and 2015, also we observe that the highest production of movies happend in 2011.
> 
><font size=3 color ='#330D07'><b><i>5-Is there a releationship between  voting public and profit for genres of movies?</b></i></font>
>
><font size=3 color ='blue'><b>from figure 5, we found the positive relationship between Vote Count and profit and its strength is strong , thats mean the voting public for each movie does impact strongly on profit for each movie.The correlation = 0.72.
>   
><font size=3 color ='#330D07'><b><i> 6-Which genres of movies achieved the most likely total profit in the  period which achieved the most total profit of all movies?</b></i></font>
>    
><font size=3 color ='blue'><b>From figure7, we can observe that the trend of total profit of movies is increasing slightly between 1960 and 2000 and increasing sharply between 2000 and  2015, and we can observe from figure 8 that the genres of movies achieved the most likely total profit between 2000 to 2015 are "Action" ,"Adventure","Comedy","Drama" ,"Family" ,,"Animimation","Science Fiction and "Thriller",while the genres of movies achieved the least likely total profit between 2000 to 2015 are "Crime","Foreign","Horror","Music", "Mystery","War","Western","Romance",Documentary","History" and "TV Movie".
</b></font>
 >
><font size=3 color ='#330D07'><b><i>7-Which genre of movies achieved the most likely total voting count in the  period which achieved the most total voting count of all movies?</b></i></font>
>    
><font size=3 color ='blue'><b>From figure 9, we can observe that the trend of total voting count of movies is increasing slightly between 1960 and 2007 and increasing sharply between 2007 and  2013 and dropping slightly, and we can observe from figure 10 that the genres of movies achieved the most likely total Voting Count  between 2007 to 2015 are "Action,"Adventure" ,"Comedy","Drama","Science Fiction"  and "Thriller",while the genres of movies achieved the least likely total Voting Count between 2007 to 2015 are "Family","Fantasy","Crime","Foreign","Horror","Music", "Mystery","War","Western","Animimation",Documentary","History" and "TV Movie".</b></font>
>
><font size=4 color ='black'><b><u>Limitations:</b></u></font>
>
><font size=3 color ='black'><b>The analyzes contained in this project are inaccurate and unreliable for several reasons:</b></font>
>
><font size=3 color='blue'><b><i>1-We lost about 50% of dataset because we dropped zero from  runtime and budget colunms,I think it is not plausible that runtime and budget  are equal zero.</b></i></font>
>
><font size=3 color='blue'><b><i>2-Many movies are a mix of different type of genres, we create new dataset that contains genre for each movie and distribute profit and vote_count(subject  our project)  equally for each genre,we assume the distribution is equal,accutally, we don't know the percentage of representation each genre for each movie .</b></i></font>
>
><font size=3 color='blue'><b><i>3-We haven't made the considerations about revenue and budget of movie associated in terms of 2010 dollars,accounting for inflation overtime.</b></i></font>
>   
><font size=4 color='#190216'><b><i>The analyzes contained in this project are useful only for educational purposes and not for purposes of presenting them for decision-making.</b></i></font>
