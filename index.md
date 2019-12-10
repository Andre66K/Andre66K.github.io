<p><strong><span style="font-size: 24px;">A Data Mining Analysis of H1B Visas Applications (2011-2016)</span></strong></p>
<p><strong><span style="font-size: 18px;">Introduction</span></strong></p>
<p>
<p style="margin-bottom: 10px !important; color: rgb(0, 0, 0); font-family: &quot;Times New Roman&quot;; font-size: medium; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial;">This project is a data mining analysis of the H1B visa applications that were submitted by employers located in the United States between 2011 and 2016. H1B visa is an employment-based, non-immigrant visa for temporary workers in the United States. For this visa, an employer must offer the applicant a job and apply for the H1B visa petiton with the US Immigration Department. Once the applicant has been sponsored by the company, the company needs to file the Labor Condition Application (LCA), which needs to be approved by United States Citizenship and Immigration Services (USCIS). If the USCIS approves it, the applicant needs to go through a lottery, and if he/she passes the lottery, the USCIS needs to review the application before approval. Once the USCIS approves the application, the applicant gets the visa.This dataset contains all the H1B Visa application submitted through the LCA to the USCIS between 2011 and 2016. If the case status says "Certified", it means that the applicant was approved to go through the lottery. However, this does not mean that the applicant eventually got the visa, and the dataset does not contain such information.</p>
<p>The dataset was retrieved from Kaggle in November 2019, and it was originally scraped from the webiste of the U.S. Office of Foreign Labor by a Kaggle user. The dataset contains over 3 million rows and 11 incolumns, which include the job title, the name of the company that sponsored the visa, and its geographic coordinates. The dataset is rather thorough and does not have many missing values. However, it would have been more interesting if it included the data from 2017 and 2018 as well, as it would have been interesting to asses the impact of the Trump administration on the visa application process</p>

<p><strong><span style="font-size: 18px;">Preliminary Analysis</span></strong></p>

<p>Firstly, I will display some word clouds to show the most common words for the following columns: Job_Title, Worksite, State, and Employer_Name.&nbsp;</p>

<img width="400" alt="wordcloud1" src="https://user-images.githubusercontent.com/54607208/70571121-330a8700-1b6b-11ea-8cf4-e1b42e572afc.PNG"> <img width="400" alt="wordcloud2" src="https://user-images.githubusercontent.com/54607208/70570269-8f6ca700-1b69-11ea-9580-523593b2dba5.PNG">

<img width="400" alt="wordcloud3" src="https://user-images.githubusercontent.com/54607208/70570310-a1e6e080-1b69-11ea-9f78-c48650382bd5.PNG"> <img width="400" alt="wordcloud4" src="https://user-images.githubusercontent.com/54607208/70570328-af03cf80-1b69-11ea-8607-0ae9e3205e48.PNG">

<p>Then I will see how many applications got approved (certified), denied, or were withdrawn.&nbsp;</p>

<img width="500" alt="casestatus" src="https://user-images.githubusercontent.com/54607208/70570363-c04cdc00-1b69-11ea-9c30-d36606bc836e.PNG">
<p>
  <br>
</p>
<p><strong>Part 1: Most Sponsored Jobs</strong></p>
<p>This section will examine what were the most sponsored jobs between 2011 and 2016.&nbsp;</p>

<img width="600" alt="mostpopularjobs" src="https://user-images.githubusercontent.com/54607208/70570397-d0fd5200-1b69-11ea-93c1-ef082e371be8.PNG">


<p><strong>Part 2: Salary Distribution</strong></p>
<p>This section examines the salary distribution of the jobs sponsored. The following graph is an histogram that displays the salary distribution of all the jobs sponsored between 2011 and 2016:</p>

<img width="550" alt="histwagesgen" src="https://user-images.githubusercontent.com/54607208/70570515-0e61df80-1b6a-11ea-8022-491e3373d568.PNG">

<p>The next graph outlines the salary distribution of the jobs sponsored per year:&nbsp;</p>

<img width="550" alt="wagesoveryeargen" src="https://user-images.githubusercontent.com/54607208/70570548-1b7ece80-1b6a-11ea-8baf-3de8d2fcfd8b.PNG">


<p><strong>Part 3: Companies that Sponsored the Largest Number of Visas</strong></p>
<p>The following are the top 20 companies that sponsored the largest number of visas over the time period analyzed:&nbsp;</p>

<img width="600" alt="companies" src="https://user-images.githubusercontent.com/54607208/70570575-29345400-1b6a-11ea-9459-837138fa329c.PNG">


<p><strong>Part 4: Sponsored Visas by City and State</strong></p>This section examines what are the cities and the states where most visas get sponsored. Firstly, I was interested to see in what cities the companies that sponsored the most are located:&nbsp;

<img width="600" alt="cities" src="https://user-images.githubusercontent.com/54607208/70570608-3cdfba80-1b6a-11ea-9f75-a217ec375deb.PNG">

<p>Next, I plotted several maps of the U.S. to better understand where are the hubs where most of the visa gets sponsored:&nbsp;</p>

<img width="550" alt="map" src="https://user-images.githubusercontent.com/54607208/70570647-4c5f0380-1b6a-11ea-9c64-89c26e0f93d6.PNG">

<img width="550" alt="map1" src="https://user-images.githubusercontent.com/54607208/70570677-584ac580-1b6a-11ea-98e5-4caac7d895e8.PNG">

<p>Finally, I created a chloropleth map that displays the number of visas sponsored by state:&nbsp;</p>

<img width="600" alt="chlor1" src="https://user-images.githubusercontent.com/54607208/70570706-6567b480-1b6a-11ea-8fb9-b274df7e8570.PNG">


<p><strong>Part 5: Analysis of the Data Science Industry</strong></p>
<p>In this last section of the project, I will conduct a similar analysis to the one performed so far but I will focus on the data science inudstry only. As an foreigner who is getting is master in Data Science in the United States, and who is potentially interested in getting an H1B visa in the future, I am interested in finding out as much as I can about H1B visas applications in Data Science.</p>
<p>First of all, I take a look at how the number of Data Science applications changed over time:</p>

<img width="600" alt="numberDS" src="https://user-images.githubusercontent.com/54607208/70395387-1edc5380-19cc-11ea-9162-7133500ec210.PNG">

<p>Next, I will take a look at the wage distribution for the data science industry between 2011 and 2016:</p>

<img width="550" alt="wagesdsgen" src="https://user-images.githubusercontent.com/54607208/70395412-4af7d480-19cc-11ea-981a-6ec4c3eac255.PNG">

<p>And then for each year:&nbsp;</p>

<img width="550" alt="wagesyearDS" src="https://user-images.githubusercontent.com/54607208/70395416-61059500-19cc-11ea-8770-0039aab491b5.PNG">

<p>Moreover, it would be interesting to check what are the companies that sponsored the largest amount of visas in Data Science:</p>

<img width="600" alt="companiesDS" src="https://user-images.githubusercontent.com/54607208/70395422-7b3f7300-19cc-11ea-94e4-0cc46914c88f.PNG">

<p>And the cities that are considered the hotspots for Data Science:&nbsp;</p>

<img width="600" alt="citiesDS" src="https://user-images.githubusercontent.com/54607208/70395434-8eead980-19cc-11ea-829e-3b50be7cd07c.PNG">

<p>Finally, I will plot a couple of maps to display where ths hot spots for Data Science are:&nbsp;</p>

<img width="550" alt="mapdotsds" src="https://user-images.githubusercontent.com/54607208/70395457-d1acb180-19cc-11ea-9456-fefd5f173886.PNG">

<img width="550" alt="intensity2" src="https://user-images.githubusercontent.com/54607208/70395465-e2f5be00-19cc-11ea-84ba-a84b7e4afd66.PNG">

<p>And I also created a chloropleth to see what are the U.S. states that sponsored the largest amount of visas in Data Science between 2011 and 2016.&nbsp;</p>

<img width="600" alt="Chloropleth Data Science Visas" src="https://user-images.githubusercontent.com/54607208/70397776-1fccaf80-19e3-11ea-8b6c-5a7e64feb7d7.PNG">

<p><strong><span style="font-size: 18px;">Conclusions</span></strong></p>
<p><em>Complete Dataset</em></p>
<ul>
  <li>The vast majority of the H1B Visa application were approved. Only approximately 3% of the application was denied.&nbsp;</li>
  <li>The most sponsored jobs between 2011 and 2016 were jobs related to computers, software and technology in general. Finance-related jobs such as accountants and financial analysts were also in the top 20 most sponsored jobs.&nbsp;</li>
  <li>The wage distribution for all jobs between 2011 and 2016 is right skewed. When looking at the wage distribution for each year, we can see that they are right skewed as well and overall rather similar to each other, although there was a slow, yet steady increase of the first quartile, median, and third quartile for each year.&nbsp;</li>
  <li>The two companies that sponsored the largest number of visas are Infosys and Tata Consultancy Services, two Indian multinational consulting firms. Overall, consulting firms are the ones that sponsored the largest number of visas, followed by IT and tech giants such as Microsoft and Amazon.&nbsp;</li>
  <li>Eight cities among the top 20 cities that sponsored the largest number of visas are located in California. However, New York City is the city with the highest number of applications. Big tech and business hubs such as Seattle, Houston, and Atlanta are also among the top 20 cities.&nbsp;</li>
  <li>California, New York, and Texas are the states where the majority of the visas were sponsored. Additionally, a significant number of applications were filed in Illinois, New Jersey, and Washington state. </li>
</ul>
<p><em>Data Science</em></p>
<ul>
  <li>The applications to sponsor jobs in the data science field spiked between 2011 and 2016; however, data science jobs represented only 0.1 percent of the total jobs sponsored. This indicates that data science is becoming more popular and it is a booming field, but it is also a relatively new field and the number of data scientist is still relatively low. It would have been interesting to see if the trend was confirmed in 2017 and 2018. Most likely it was.&nbsp;</li>
  <li>The average salary of a data scientist is higher than the average salary of the total jobs sponsored.</li>
  <li>The companies that sponsored the largest number of data science jobs are well-known, tech giants such as Microsoft, Uber, and Facebook.&nbsp;</li>
  <li>Eleven cities out of the top 20 that sponsored the largest number of visas in data science are located in California. Unsurprisingly then, California is the state that sponsored most visas in the Data Science industry. Other states that sponsored quite a lot in the industry are New York, Washington, Illinois, and Texas. </li>
</ul>
<p><em>2017-2018 Trends</em></p>
<p>As stated before, one limitation of this dataset is that it does not contain the data for 2017 and 2018. However, I doubt that the major trends we saw in this analysis changed. The most sponsored jobs are most likely the ones related to software development, computers and consulting, and the companies that sponsor the majority of the visas are probably multinational companies operating in consulting, IT, and technology in general. Location-wise, the situation has probably not changed either. Cities like San Francisco, Seattle, and New York City are still major business and technology hubs where companies keep sponsoring a significant amount of visas every year. The trends in the Data Science industry most likely remained the same through 2017 and 2018. The only thing that might have changed significantly is the number of the application for Data Science, which I expect to have grown tremendously in the last two years.&nbsp;</p>
<p>Overall, the only major difference between the applications filed between 2011 and 2016 and the ones filed in 2017-2018 might be the denial rate. Indeed - according to several media outlets - the Trump Administration reportedly has been "aggressively" denying applications for H1B visas since Trump took office in January 2017.&nbsp;</p>
