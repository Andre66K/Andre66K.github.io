<p style="margin-bottom: 10px !important; color: rgb(0, 0, 0); font-family: &quot;Times New Roman&quot;; font-size: medium; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; text-align: center;"><strong style="font-weight: 700;">Introduction</strong></p>
<p style="margin-bottom: 10px !important; color: rgb(0, 0, 0); font-family: &quot;Times New Roman&quot;; font-size: medium; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial;">
  <br>
</p>
<p style="margin-bottom: 10px !important; color: rgb(0, 0, 0); font-family: &quot;Times New Roman&quot;; font-size: medium; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial;">This project is a data mining analysis of the H1B visa applications that were submitted by employers located in the United States between 2011 and 2016. H1B visa is an employment-based, non-immigrant visa for temporary workers in the United States. For this visa, an employer must offer the applicant a job and apply for the H1B visa petiton with the US Immigration Department. Once the applicant has been sponsored by the company, the company needs to file the Labor Condition Application (LCA), which needs to be approved by United States Citizenship and Immigration Services (USCIS). If the USCIS approves it, the applicant needs to go through a lottery, and if he/she passes the lottery, the USCIS needs to review the application before approval. Once the USCIS approves the application, the applicant gets the visa.This dataset contains all the H1B Visa application submitted through the LCA to the USCIS between 2011 and 2016. If the case status says "Certified", it means that the applicant was approved to go through the lottery. However, this does not mean that the applicant eventually got the visa, and the dataset does not contain such information.</p>
<p>The dataset was retrieved from Kaggle in November 2019, and it was originally scraped from the webiste of the U.S. Office of Foreign Labor by a Kaggle user. The dataset contains over 3 million rows and 11 incolumns, which include the job title, the name of the company that sponsored the visa, and its geographic coordinates. The dataset is rather thorough and does not have many missing values. However, it would have been more interesting if it included the data from 2017 and 2018 as well, as it would have been interesting to asses the impact of the Trump administration on the visa application process</p>

<p style="color: rgb(0, 0, 0); font-family: &quot;Times New Roman&quot;; font-size: medium; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; text-align: left; margin-bottom: 10px !important;"><strong>Preliminary Analysis</strong></p>
<p>Firstly, we display some word clouds to show the most common words for the following columns: Job_Title, Worksite, State, and Employer_Name.&nbsp;</p>

<img width="500" alt="wordcloud1" src="https://user-images.githubusercontent.com/54607208/70393141-25ab9c00-19b5-11ea-93f0-e3bddf1fa8c1.PNG">

<img width="500" alt="wordcloud2" src="https://user-images.githubusercontent.com/54607208/70393165-5b508500-19b5-11ea-994d-1dd76b9b6a6c.PNG">

<img width="500" alt="wordcloud3" src="https://user-images.githubusercontent.com/54607208/70393181-95ba2200-19b5-11ea-97ca-555a9b469b0d.PNG">

<img width="500" alt="wordcloud4" src="https://user-images.githubusercontent.com/54607208/70393187-a4a0d480-19b5-11ea-8e6e-ba548aa4ad83.PNG">

<p>Then we will see how many applications got approved (certified), denied, or were withdrawn.&nbsp;</p>

<img width="293" alt="casestatus" src="https://user-images.githubusercontent.com/54607208/70393193-bbdfc200-19b5-11ea-9d2f-66f68b83d38e.PNG">

<p><strong>Part 1: Most Sponsored Jobs</strong></p>
<p>This section will examine what were the most sponsored jobs between 2011 and 2016.&nbsp;</p>

<img width="500" alt="mostpopularjobs" src="https://user-images.githubusercontent.com/54607208/70393227-ea5d9d00-19b5-11ea-9312-3701c99d12b1.PNG">

<p><strong>Part 2: Salary Distribution</strong></p>
<p>This section examines the salary distribution of the jobs sponsored. The following graph is an histogram that displays the salary distribution of all the jobs sponsored between 2011 and 2016:</p>

<img width="500" alt="histwagesgen" src="https://user-images.githubusercontent.com/54607208/70393235-fe090380-19b5-11ea-9ab0-2c1d06f038a2.PNG">

<p>The next graph outlines the salary distribution of the jobs sponsored per year:&nbsp;</p>

<img width="500" alt="wagesoveryeargen" src="https://user-images.githubusercontent.com/54607208/70393246-12e59700-19b6-11ea-8bb3-c0dd42a73a09.PNG">

<p><strong>Part 3: Companies that Sponsored the Largest Number of Visas</strong></p>
<p>The following are the top 20 companies that sponsored the largest number of visas over the time period analyzed:&nbsp;</p>

<img width="500" alt="companies" src="https://user-images.githubusercontent.com/54607208/70393264-2b55b180-19b6-11ea-83bb-6145d16446a9.PNG">

<p><strong>Part 4: Sponsored Visas by City and State</strong></p>This section examines what are the cities and the states where most visas get sponsored. Firstly, I was interested to see in what cities the companies that sponsored the most are located:&nbsp;

<img width="500" alt="cities" src="https://user-images.githubusercontent.com/54607208/70393284-4c1e0700-19b6-11ea-995e-623f4cb8854e.PNG">

<p>Next, I plotted several maps of the U.S. to better understand where are the hubs where most of the visa gets sponsored:&nbsp;</p>

<img width="500" alt="cities" src="https://user-images.githubusercontent.com/54607208/70393360-f564fd00-19b6-11ea-8b3e-7c7d47d71322.png">

<p>Finally, I created a chloropleth map that displays the number of visas sponsored by state:&nbsp;</p>
<p><strong>Part 5: Analysis of the Data Science Industry</strong></p>
<p>In this last section of the project, I will conduct a similar analysis to the one performed so far but I will focus on the data science inudstry only. As an foreigner who is getting is master in Data Science in the United States, and who is potentially interested in getting an H1B visa in the future, I am interesting in finding out as much as I can about H1B visas applications in Data Science.</p>
<p>First of all, I take a look at how the number of Data Science applications changed over time:</p>
<p>Next, I'll take a look at the wage distribution for the data science industry between 2011 and 2016:</p>
<p>And then for each year:&nbsp;</p>
<p>Moreover, it'd be interesting to check what are the companies that sponsored the largest amount of visas in Data Science:</p>
<p>And the cities that are considered the hotspots for Data Science:&nbsp;</p>
<p>Finally, I will plot a couple of maps to display where in the U.S. every single visa was sponsored:&nbsp;</p>
<p>And I also created a chloropleth to see what are the U.S. states that sponsored the largest amount of visas in Data Science between 2011 and 2016.&nbsp;</p>
<p><strong>Conclusion</strong></p>
<p>
  <br>
</p>

<p><em>Data Science</em></p>
<ul>
  <li>The applications to sponsor jobs in the data science field spiked between 2011 and 2016; however, data science jobs represented only 0.1 percent of the total jobs sponsored. This indicates that data science is becoming more popular and it is a booming field, but it is also a relatively new field and the number of data scientist is still relatively low. It would have been interesting to see if the trend was confirmed in 2017 and 2018. Most likely it was.&nbsp;</li>
  <li>The average salary of a data scientist is higher than the average salary of the total jobs sponsored.</li>
  <li>The companies that sponsored the largest number of data science jobs are well-known, tech giants such as Microsoft, Uber, and Facebook.&nbsp;</li>
  <li>Eleven cities out of the top 20 that sponsored the largest number of visas in data science are located in California. Unsurprisingly then, California is the state that sponsored most visas in the Data Science industry. Other states that sponsored quite a lot in the industry are New York, Washington, Illinois, and Texas.&nbsp;</li>
</ul>
<p>
  <br>
</p>
