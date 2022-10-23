## First Project, first blog post
Wrapping up phase 1 of my data science course, and finding Python to be a useful addition to my developer toolbox.

Jupyer notebooks are very powerful for prototyping, interactive coding, and sharing analysis.

### First Project
The [first project](https://github.com/learn-co-curriculum/dsc-phase-1-project-v2-4) for Data Science was an analysis on movie data for the purposes of advising a new studio on their launch.


### Data is messy
I found as I worked through the provided inputs that firstly, there is no useful identifier to map across datasets.  

This meant that when joining across vendor data sets I would have to fall back to release year & movie title.  
Strings like movie titles being messy means a lot of non-matches, so a lot of data had to be thrown away to proceed.

### A dollar isn't always a dollar
I realized pretty quickly that as this dataset went back decades, I had to account for inflation in some way.
Maybe if I had been doing this project in 2010-2019 I wouldn't have thought of this.  However after 2021-2022, the I word does seem to be on everyones mind.

Helpfully, I found the Minneapolis Fed had some very easy to use [CPI data](https://www.minneapolisfed.org/about-us/monetary-policy/inflation-calculator/consumer-price-index-1913-) so a few lines of code and I now had normalized to 2022 dollars.

### How do we define success
The objective of any business is to make money, even if movies are (supposed to be) an art.  So I did not use any of the provided moview review/rating data.  A studio does not control reviews & ratings, those are an outcome.  Whether a rating is good or bad matters only tangentially as an outcome.  So the measures I used were Profit & Return on Investment.

### What do studios control?
* Staffing
* Spending
* Genre
* Scheduling
* Runtime

### What I did
1. Genre - I measured the total net profit by Genre to see if there were any standout genres (there were)
2. Scheduling - I analyzed total box office sales by month & season to look at how strong seasonality was (strong)
3. Runtime - I looked at runtime and its relation to box office sales (minimal) 
4. Budget - Lastly I looked at how budget impacted profit and ROI (positively, until a point of diminishing returns)

### Visualizations 
### 1 Genre 
![genre](/images/post1_genres.png)
### 2 Scheduling
![schedule](/images/post1_season.png)
### Runtime
![runtime](/images/post1_runtime.png)
### Budget
![budget_roi](/images/post1_budget_roi.png)
![buget_profit](/images/post1_budget_profit.png)

### Thanks and so long folks
![byebye](https://media.giphy.com/media/bOwOAey4MDO3ivBkgK/giphy.gif?cid=ecf05e47ee85jfyqagqyk139l7l7vphstgw0mrc2ym3amhdz&rid=giphy.gif&ct=g)
