Exploring the Effectiveness of Proportional Graphs: A Comparative Analysis of Chart Types
===
### Team: 

**Pixel Master**: Gan-Erdene Benderiya, Jingni Cai, Ester Jere, Antonela Tamagnini


### Related links
Survey link: https://jcai0o0.github.io/revisit-project/

Survey repository: https://github.com/jcai0o0/revisit-project

Interview Questionnaire: [Post Survey Interview](https://github.com/jcai0o0/a3-Experiment/blob/main/post-survey-interview/post%20survey%20questionnaire.pdf)

____

### Introduction
Proportional graphs, also referred as "percentage" or "parts-of-a-whole" graphs, visually represent the parts of a whole entity and illustrate the proportion or percentage each part contributes to the total.

Understanding the effectiveness of different visualization techniques is pivotal for conveying complex data insights accurately and intuitively. In this study, we delve into the realm of parts-of-a-whole graphs, investigating the ease of comprehension and accuracy across four distinct chart types: treemap, pie chart, stacked bar chart, and donut chart.

Our study aims to conduct a survey-based investigation, where participants are presented with two dots marked in each visualization. Their task is to identify which proportion represents the smallest part in relation to the largest part, guided solely by the placement of these dots. By employing this novel approach, we can gauge the perceptual ease and accuracy associated with each chart type.

In our project, we conducted 60 individual surveys, and we measured accuracy in identifying relative proportions. This output allowed us to determine which chart types facilitate a more intuitive comprehension and precise interpretation. 

The findings of this research hold significant implications for data visualization practitioners. By unveiling the comparative effectiveness of parts-of-a-whole graphs, we can inform best practices in chart selection, ultimately enhancing the clarity and impact of data-driven communication strategies.


### Understanding Different Visualizations
- Pie Chart: Common for showing proportions within a whole, pie charts are intuitive for some comparisons but can be challenging for precise quantitative comparisons.
- Stacked Bar Chart: This visualization is effective for showing part-to-whole relationships and trends over time or across categories, potentially offering clearer quantitative assessment than pie charts.
- Treemap: Treemaps are useful for displaying hierarchical data and proportions within a whole, offering a different spatial representation than pie charts.
- Donut Chart: Similar to a pie chart, but with a blank center, a donut chart is used to display proportions or percentages of a whole.

---
### Hypotheses
- Users may find pie charts most intuitive for understanding general proportions but struggle with precise comparisons.
- Stacked bar charts may facilitate better quantitative analysis and comparison across categories than pie charts.
- Treemaps, while effective for displaying large datasets, may require more cognitive effort to interpret than pie or stacked bar charts.
- Donut charts with multiple concentric rings or hierarchical data may require more cognitive effort to interpret compared to simple pie charts or stacked bar charts.



### Revisit experiment screenshots
#### Landing page of the experiment
![](img/revisit-landing-page.png)

#### Visualization: Donut Chart
![](img/revisit-donutchart.png)

#### Visualization: Pie Chart
![](img/revisit-piechart.png)

#### Visualization: Stacked Bar Chart
![](img/revisit-stackedbarchart.png)

#### Visualization: Treemap
![](img/revisit-treemap.png)




## Results of the study
![](img/revisit-error-table.png)

The previous table displays the results of the Log2 Error results for each of the visualization types analyzed, the ranking of accuracy based on the error rate, with 1 being the most accurate, and the lower and upper confidence intervals.

![](img/revisit-boxplot.png)

The boxplot shows the log error value for the different graph types. The central point represents the median log error for each visualization type. The horizontal lines extending to the left and right from the median represent the confidence intervals, indicating the variability or spread of the log error in the data for that visualization type. The narrower the line, the less variability there is in the log error measurements for that type of visualization.

Considering the minimal variation in error rates among the four visualization types examined—treemap, donut chart, stacked bar chart, and pie chart—it can be inferred that while treemaps marginally outperform the others, the overall difference is not significative.
In conclusion, data visualization practitioners can confidently employ any of these formats knowing that they all similarly support accurate parts-of-a-whole interpretations.




### Design and Technical Achievements

#### Visualization Types Used (D3)

D3, a powerful tool to help in creating different types of visualizations like : -bar chart -donout chart -tree chart pie chart -It allows for the flexibility in terms of data visualization where they can be animated or not -The D3 has been used in esuring smooth transtions from one event to another

#### Program to Retrieve Data from Firebase Using Python

This was used because python easily establishes connection to firebase projection making it easy to retrieve data and incoporate it in a python application for manipulation -The use of python in firebase for data retreaval offers great scalability making it possible tomhandle large volumes of data with eaase -Python as a language offers a lot of flexibility in database manipulation as it can connect to any type of database like Object Orientented Relational Models or just SQL Queries it can handle it -although using python can be a good and efficient way to retrieve data, security is always a concern as Python does not offer much flexibility in protecting data from things like sql injections.

#### Console Logging and Debugging

This has helped the developers to quickly give feedback to the users as the errors were logged in real-time hence increases customer satisfaction. -This provided the ability to easily identify errors as they were being logged as this allows the developer to identify the types of errors to log hence making it to track any erros and quickly resolve it. -The system logged messages at important stages and this gave the developing team a chance to track data movement and trace where data is lost and where data was not converted as required. -console logging provides a security audit for the application as it logs userid and user operations it becomes easy to know user operations and trace what user did unneccessary transactions

#### Custom Styling and Layout

The simple and flexible layout of the experiment made it easy for users to quickly finish their surveys -The user interface had CSS applied to make the rendering apealing to the users -Although the design could display on both the mobile and computer devices, uses on mobile devices had some challenges compared to those who used laptops.

#### Dynamic Data Binding & Interaction Handling

This is powerful element ti include as it ensures that change in the data does not affect the object it is bound to hence making changes more flexible -The ability to respond to user events is well represented that no user clicks results in an undescriptive error -This allows for the implementation of random data manipulation as in the case hwere graphs and or questions are randomly generated -The ability to easily handle the errors like using try catch has been implemented well in the application

#### User Feedback

There were variations based on gender. Male particpants found the donut harder than the treemap while women found the treemap harder than the donot





For the scope of this project, assume the role of a scientist who runs experiments for a living.

For example: 

Q: How do we know that bar charts are "better" than pie charts?  
A: Controlled experiments!

In this assignment you'll implement a simple controlled experiment using some of the visualizations you’ve been building in this class. 
You'll need to develop support code for the experiment sequence, results file output, and other experiment components. 
(These are all simple with Javascript buttons and forms.)
The main goals for you are to a) test at least three competing visualizations or experiment conditions, b) implement data/stimuli generation and error calculation functions (if following the baseline, use Cleveland and McGill's 1984 paper and Heer and Bostock's 2010 replication), c) run the experiment with 10 participants (or equivalent number of trials), and d) do basic analysis and reporting of the results.

For this assignment you should aim to write everything from scratch. For experimentation it is often necessary to control all elements of the chart.
You should definitely *reference* demo programs from books or the web, and if you do please provide a References section with links at the end of your Readme.

Going Beyond Cleveland-McGill
---

Several have expressed interest in conducting surveys of various sorts. I encourage you go move beyond Cleveland and McGill if you can think of other interesting visualization experiment designs and corresponding analyses. 

You might study how people interpret COVID visualizations or design an experiment on shapes or color, for example.
If you decide to go in a custom route, do plan to sync with staff so we can help you set acceptable parameters that would be fair to folks following the original route.

(Basically, we still want you to do a multi-trial study with each participant, to raise the chance that you get solid results.)

How you measure "error" and similar facets also matter. But you can't go wrong with finding a good visualization study online to start from :)

Requirements
---

- Look it over Cleveland and McGill's original experiment (see the section below) and [watch this video](experiment-example.mp4) to get a sense of the experiment structure and where your visualizations will go.
- When viewing the example experiment video, note the following:
    - Trials are in random order.  
    - Each trial has a randomly generated set of 5-10 data points.  
    - Two of these data points are marked.  
    - (Note: the experiment UI and User Experience could be better. Plenty of design achievements here).
- Implement the data generation code **as described in the Cleveland & McGill and Heer & Bostock papers**. 
    - The goal is to generate a set of random datapoints (usually 5 or 10, with values be between 0 and 100) and to mark two of them for comparison in the trial. 
- Add 3 visualizations (i.e. conditions) to your experiment. When you are adding these visualizations, think about *why* these visualizations are interesting to test. In other words, keep in mind a *testable hypothesis* for each of the added visualization. Some good options include bar charts, pie charts, stacked-bar charts, and treemaps. You can also rotate your bar chart to be horizontal or upside-down as one of your conditions. You are encouraged to test unorthodox charts -- radar charts come to mind, but there are MANY possibilities here-- feel free to be creative!
    - Follow the style from Cleveland and McGill closely (e.g. no color, simple lines) unless you are specifically testing a hypothesis (e.g. color versus no color). Pay attention to spacing between elements like bars. Do not mark bars for comparison using color-- this makes the perceptual task too easy.
- After each trial, implement code that grades and stores participant’s responses.
- At the end of the experiment, to get the data, one easy option use Javascript to show the data from the current experiment\* (i.e. a comma separated list in a text box) and copy it into your master datafile. See the Background section below for an example of what this file should look like. (\*Alternately implement a server, if you're experienced with that sort of thing.)

** DATA SCIENTISTS! IT IS YOUR TIME TO SHINE **

- Figure out how to calculate "Error", the difference between the true percentage and the reported percentage.
- Scale this error using Cleveland and McGill’s log-base-2 error equation. For details, see the background section (there’s a figure with the equation). This becomes your “Error” column in the output. Make sure you use whole percentages (not decimal) in the log-base-2 equation. Make sure you handle the case of when a person gets the exact percentage correct (log-base-2 of 1/8 is -3, it is better to set this to 0). 
- Run your experiment with 10 or more participants, or-- make sure you get at least 200 trials **per visualization type** in total.  
    - Grab friends or people in the class.   
    - Run at least 20 trials per visualization type, per participant. This is to ensure that you cover the range of possible answers (e.g. 5%, 10%, ..., 95%)
- Make sure to save the resulting CSV after each participant. Compile the results into a master csv file (all participants, all trials).
- Produce a README with figures that shows the visualizations you tested and results, ordered by best performance to worst performance. Follow the modern Cleveland-McGill figure below -- though note that using names instead of icons is fine.
- To obtain the ranking, calculate and report the average log2Error for each visualization across all trials and participants. This should be straightforward to do in a spreadsheet.
- Use Bootstrapped 95\% confidence intervals for your error upper and lower bounds. Include these in your figures. Bootstrapped confidence intervals are easily implemented in R + ggplot2 using the `stat_summary` geom. You can also use Excel, Python, or many many other tools. Bootstrapped 95% CIs are **very** useful in modern experiment practice.
- Include example images of each visualization as they appeared in your experiment (i.e. if you used a pie chart show the actual pie chart you used in the experiment along with the markings, not an example from Google Images).

## General Requirements

0. Your code should be forked from the GitHub repo and linked using GitHub pages.
2. Your project should use d3 to build visualizations. 
3. Your writeup (readme.md in the repo) should contain the following:

- Working link to the experiment hosted on gh-pages or some other site.
- Concise description and screenshot of your experiment.
- Description of the technical achievements you attempted with this project.
- Description of the design achievements you attempted with this project.

Background
---

In 1984, William Cleveland and Robert McGill published the results of several controlled experiments that pitted bar charts against pies and stacked-bar variants. 
Their paper (http://www.cs.ubc.ca/~tmm/courses/cpsc533c-04-spr/readings/cleveland.pdf) (http://info.slis.indiana.edu/~katy/S637-S11/cleveland84.pdf) is considered a key paper in data visualization.
In particular, they ran a psychology-style experiment where users were shown a series of randomly-generated charts with two graphical elements marked like this:

![cleveland bar chart](img/cleveland-bar.png)

Participants were then asked, "What percentage is the smaller of the larger?". 
This was repeated hundreds of time with varying data and charts. 
By the end of the study, Cleveland and McGill had amassed a large dataset that looked like this:

![cleveland table](img/cleveland-table.png)

__Log-base-2 or "cm-error"__: The true percent is the actual percentage of the smaller to the larger, while the reported percent is what participants reported. 
Cleveland and McGill recognized that their analyses would be biased if they took `abs(ReportedPercent – TruePercent)` as their score for error. 
To compensate, they came up with a logarithmic scale for error with this equation:

![cleveland equation](img/cleveland-equation.png)

You’ll be implementing this error score as part of the lab. 
(Hint: it’s not a trick question, this is just to familiarize you with the experiment protocol). 
With this Cleveland-McGill error score you can better compare the performance of the charts you test to figure out which one performs the best.

As a baseline, compare your average Error scores to the following chart, which include both Cleveland and McGill’s results as well as more recent extensions of this experiment (lower error indicates better performance, and error bars are bootstrapped 95% confidence intervals (`http://en.wikipedia.org/wiki/Confidence_interval#Meaning_and_interpretation`)):

![cleveland results](img/cleveland-results.png)

GitHub Details
---

- Fork the GitHub Repository. You now have a copy associated with your username.
- Make changes to index.html to fulfill the project requirements. 
- Make sure your "master" branch matches your "gh-pages" branch. See the GitHub Guides referenced above if you need help.
- Edit this README.md with a link to your gh-pages site: e.g. http://YourUsernameGoesHere.github.io/Experiment/index.html
- Replace this file (README.md) with your writeup and Design/Technical achievements.
- To submit, make a [Pull Request](https://help.github.com/articles/using-pull-requests/) on the original repository.
- Name your submission using the following scheme: 
```
a3-FirstLastnameMember1-FirstLastnameMember2-FirstLastnameMember3-...
```
