---
layout: page
title: Professional Portfolio
permalink: /professional-portfolio/
---   
	
Here are some of the projects / analyses / processes I have helped enable over the years.  Please note that I have had to leave certain details out and blur screenshots to respect employer privacy.  

### Travel & Entertainment Expense Fraud Review Process

**Problem:** Travel & entertainment (T&E) expenses were growing and particularly risky for multinational pharma companies.  We wanted to monitor, however knew that sampling would be too limited and time-consuming.  Further, I believed that the suggested approach of analyzing the population (e.g., top-10 spenders, largest cash expenses, etc.) would not be effective.  

**Solution:** I developed an end-to-end program to consume, transform, score & rank, and visualize the T&E data.  My approach employed 19 different analytical tests that were methodically scored and analyzed collectively from an individual employee perspective.  

**Impact:** T&E expenses are now audited on a quarterly basis with very limited effort.  Previoulsy, this was a high-effort, low-yield audit process.  While I cannot provide details, the value produced has been significant, including the benefits of audit efficiency, significantly improved violation detection, and of course violation deterrance due to the automated process.     
 
**Tools:** ACL, ACL Server, Python, R, Tableau  

![TE Audit Program](/psuanm5030.github.io/img/TE Audit Program.png){:height="80%" width="80%" style="
    display: block;
    margin: 0 auto;
"}

### Portfolio Opportunity Analysis

**Problem:** My company was faced with certain headwinds that made it imperative they reviewed the market to ensure they weren't missing any opportunities.  Leadership wanted an analytical approach, as they didnt trust the current state of analysis and suspected it was inaccurate / outdated due to the manual process currently employed.  The market data was mostly un-interrogated due to its size. 

**Solution:** I was engaged to analyze the data to uncover trends and gaps, as well as, make this visually consumable by a wide variety of audiences, including analysts and leaders.  

**Impact:** Shared with the top-50 operational leaders via live, in-person demo (as well as through 55" touch screen).  Later demoed in-person to the CEO, then presented to the board of directors interactively by the company president.  Originally intended to be an ad-hoc review has been sponsored and is being "operationalized" by a team of two individuals.  
 
**Tools:** Tableau, Alteryx  

![Portfolio Opportunity Analysis](/psuanm5030.github.io/img/Portfolio Opportunity Analysis.png){:height="80%" width="80%" style="
    display: block;
    margin: 0 auto;
"}

### Pharmaceutical Market Exploration

**Problem:** We purchase expensive pharmaceutical market data from IMS, a well known health data aggregator, however we have struggled mightily to extract value from it.  Most often, the data was serving the needs of very few (typically one-off queries), despite the generous license we had and the opportunities we all knew the data held.  Further, the pipeline the data (up to 50M rows) travelled was extremely inefficient.

**Solution:** We tackled the pipeline first, upskilling the IMS team with the ETL workflow tool, Alteryx.  Second, we built a number of dashboards that made insight generation easier for the user.  Finally, we shared the wealth, training scores of people across the enterprise to use the dashboards. 

**Impact:**    
* Data pipeline that takes under 4 hours to complete quarterly, which features various improvements to the underlying data (e.g., additional / more efficient features, validation, centralization and redundancy).  This saved them nearly 160+ hours per quarter.  
* Nearly 20+ dashboards deployed to 200 users worldwide, from many different functions - most with unique reasons for consuming the data.  
* Enabled company to look at data against custom dimensions, never before analyzed.

**Tools:** Tableau, Alteryx  

![Pharma Market Dashboards](/psuanm5030.github.io/img/Pharma Market Dashboards.png){:height="80%" width="80%" style="
    display: block;
    margin: 0 auto;
"}

### Customer Call Analysis

**Problem:** The need to understand sentiment from our customers and predict future issues was of high priority.  Calls from customers were being logged but several attempts to extract insights from this data were unsuccessful, mostly due to the low volume of calls.  Current intelligence consisted of a weekly email to leaders showing calls per call type and product.   There wasn't anything that actually communicated a trend or alerted stakeholders when a product or area was out of bounds.  Further, this dashboard needed to be consumed by an audience of both analysts and executives.  

**Solution:** As the data was limited in detail and low volume, we determined that a focused dashboard, comparing the near-term to long-term averages, was ideal.  This not only surfaced the needed insights (while avoiding the low volume issue) but was also valuable to the various audiences (from customer support rep to executive).  Additionally we built a pipeline that automated the extraction, transformation and storage of the data, such that the data could be viewed hourly (as opposed to the weekly standard).

**Impact:** This dashboard was praised for the simplicity and insights generation - for multiple stakeholders.  It was also determined that this new process saved over 12 hours per month and exposed the data for further usages.
 
**Tools:** Tableau, Alteryx  

![Customer Call Analysis](/psuanm5030.github.io/img/Customer Calls.png){:height="80%" width="80%" style="
    display: block;
    margin: 0 auto;
"}  

### Audit Analytics Program  

**Problem:** Our company and audit department were both growing significantly, however our audit process was still very "old school" in a number of ways.  One key area of limitation was our lack of integrated audit analytics, which were being outsourced in a limited fashion.  The outsourced analytics were expensive, low quality and only applied where absolutely required.  

**Solution:**  With the support of audit leadership, I was able to insource our analytical efforts and develop our audit analtyics methodology.  We documented our processes and made key technology decisions to effectively and efficiently support our methodology and the audit process.  We also placed heavy emphasis on educating our audit professionals on the value of analytics in their audit process.   

**Impact:**  Nearly all audits experienced valuable gains in efficiency and effectivness, while the traditional audit process was transformed to emphasize the analytics component.  Some of my analytic deliverables were shared with the highest levels of company leadership, including the CFO, CEO and board of directors.  Within 2 years, two positions were created to support anlytics exclusively in Internal Audit.  
   
**Tools:**  ACL, ACL Server, Python, R  

![Audit Manual](/psuanm5030.github.io/img/Internal Audit Manual - Contents.png){:height="50%" width="50%" style="
    display: block;
    margin: 0 auto;
"}  

### Legal Contracts Management

**Problem:** Legal was struggling to understand why the business was complaining about the speed at which contracts get approved.  They knew one thing - they were not issue - however had trouble proving this and locating the root-cause, primarily because their data wasn't robust enough to help them understand the timeline of legal actions on a contract.  

**Solution:** While we were not experts in the legal domain, we knew that the data needed some love.  We built a dataset that combined several different tables and required complex sorting prior to feature creation (primarily timing notation) at the right level of detail, such that tools like Tableau could consume.  While the primary ask was to help them find the root-cause of the bottleneck, we were also able to build some intuitive operational and expoloratory dashboards that enabled better understanding of the state of contracts - for lawyers and leaders across the world.  
 
**Impact:** Initial hypothesis validation turned into an analytical toolset used by more than 35 people in over 12 countries.    

**Tools:** Alteryx (automated pipeline), Tableau (analyses and dashboards)  

### Operational Scorecard

**Problem:** There were 12 functions reporting to operational leadership on a monthly and quarterly basis.  Each group had their own slide deck, ranging from 1 slide to 35 slides, with endless styles of charts / tables / metrics / timing.  The manual nature and disorganized result was finally too much to take.  

**Solution:** The 12 groups were vastly different functions, however they were all reporting on metrics on the same time frames (mostly monthly, some quarterly).  Therefore we organized the various Key Performance Indicators (KPI), along with their metadata, into a KPI database that set the foundation for stable, consistent reporting.  

**Impact:** Time spent compiling the monthly reporting was reduced significantly due to the consolidation and singular methodology.  Besides the time saved, satisfaction is substantially improved with the metric consumers.  

**Tools:** Sharepoint, Alteryx, Tableau  

![Operational Scorecards](/psuanm5030.github.io/img/Operational Scorecard.png){:height="80%" width="80%" style="
    display: block;
    margin: 0 auto;
"}   