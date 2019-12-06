<p style="margin-bottom: 10px !important; color: rgb(0, 0, 0); font-family: &quot;Times New Roman&quot;; font-size: medium; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; text-align: center;"><strong style="font-weight: 700;">Introduction</strong></p>
<p style="margin-bottom: 10px !important; color: rgb(0, 0, 0); font-family: &quot;Times New Roman&quot;; font-size: medium; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial;">
  <br>
</p>
<p style="margin-bottom: 10px !important; color: rgb(0, 0, 0); font-family: &quot;Times New Roman&quot;; font-size: medium; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial;">This project is a data mining analysis of the H1B visa applications that were submitted by employers located in the United States between 2011 and 2016. H1B visa is an employment-based, non-immigrant visa for temporary workers in the United States. For this visa, an employer must offer the applicant a job and apply for the H1B visa petiton with the US Immigration Department. Once the applicant has been sponsored by the company, the company needs to file the Labor Condition Application (LCA), which needs to be approved by United States Citizenship and Immigration Services (USCIS). If the USCIS approves it, the applicant needs to go through a lottery, and if he/she passes the lottery, the USCIS needs to review the application before approval. Once the USCIS approves the application, the applicant gets the visa.This dataset contains all the H1B Visa application submitted through the LCA to the USCIS between 2011 and 2016. If the case status says "Certified", it means that the applicant was approved to go through the lottery. However, this does not mean that the applicant eventually got the visa, and the dataset does not contain such information.</p>
<p>The dataset was retrieved from Kaggle in November 2019, and it was originally scraped from the webiste of the U.S. Office of Foreign Labor by a Kaggle user. The dataset contains over 3 million rows and 11 incolumns, which include the job title, the name of the company that sponsored the visa, and its geographic coordinates. The dataset is rather thorough and does not have many missing values. However, it would have been more interesting if it included the data from 2017 and 2018 as well, as it would have been interesting to asses the impact of the Trump administration on the visa application process</p>

<img width="577" alt="wordcloud" src="https://user-images.githubusercontent.com/54607208/70272123-ba27bb80-1775-11ea-9da7-6af997de3250.png">

<p style="color: rgb(0, 0, 0); font-family: &quot;Times New Roman&quot;; font-size: medium; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; text-align: left; margin-bottom: 10px !important;"><strong>Preliminary Analysis</strong></p>
<p>Firstly, we display some word clouds to show the most common words for the following columns: Job_Title, Worksite, State, and Employer_Name.&nbsp;</p>
<p>Then we will see how many applications got approved (certified), denied, or were withdrawn.&nbsp;</p>
<p><strong>Part 1: Most Sponsored Jobs</strong></p>
<p>This section will examine what were the most sponsored jobs between 2011 and 2016.&nbsp;</p>
<p><strong>Part 2: Salary Distribution</strong></p>
<p>This section examines the salary distribution of the jobs sponsored. The following graph is an histogram that displays the salary distribution of all the jobs sponsored between 2011 and 2016:</p>
<p>The next graph outlines the salary distribution of the jobs sponsored per year:&nbsp;</p>
<p><strong>Part 3: Companies that Sponsored the Largest Number of Visas</strong></p>
<p>The following are the top 20 companies that sponsored the largest number of visas over the time period analyzed:&nbsp;</p>
<p><strong>Part 4: Sponsored Visas by City and State</strong></p>This section examines what are the cities and the states where most visas get sponsored. Firstly, I was interested to see in what cities the companies that sponsored the most are located:&nbsp;
<p>Next, I plotted several maps of the U.S. to better understand where are the hubs where most of the visa gets sponsored:&nbsp;</p>
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
