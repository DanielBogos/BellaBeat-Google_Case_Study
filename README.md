# BellaBeat-Google_Case_Study

### Project Overview
#### Description
Heeeeey again! Second project of mine so far...
This repository contains a comprehensive case study analyzing a wellness technology company specializing in women's health, covering its innovations, market positioning, challenges, and strategic opportunities for growth. 
#### Purpose
This repository is designed to serve as a resource and knowledge for junior researchers, students and data analysts who have interest in data, data science and business Intelligence.

Feel free to explore and contribute insights or discussions!
  
## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
4. [Key Findings](#key-findings)
5. [Files in This Repository](#files-in-this-repository)
6. [Technologies Used](#technologies-used)
7. [Conclusion](#conclusion)
   
## Dataset
- **Source**: The dataset was provided by a virtual technology wellnessc ompany and includes data collected by one of the Bellabeats products from 30+ volunteers. The data was collected during 60 days but in order for my analysis to be trustworthy and without any bias, I will focus only on 30 days (12th of April - 12th of May) since the data from this period of time does not have many missing values and is much more complete.
- **Key Fields**:
  - **Id**: Every participant has an unique id.
  - **Calories**: The amount of calories burned per day.
  - **Steps**: Indicates the number of steps per day.
  - **Fairly and intensive activity**: Indicates the time in minutes spent on these type of activities per day.
  - **Sedentary**: The amount of sedentary time per day including the sleep.
  - **Sleep**: Data about sleep(time in bed asleep and not asleep per day).
  - **Weight** Data about the weight of most of the participants.
 
## Methodology
1. **Data Cleaning**: Performed initial data cleaning to remove duplicates and correct inconsistencies such:
   - missing values,
   - removing the rows where the data is not reliable (ex: where the average sleep is less then 4 hours, where calories burnt throghout the day is close to zero, etc)
   - remove the unnecessary columns,
   - making sure the columns have the right type of values and fall in the validation range.
2. **Preparing data**:
   * I`ve checked if all columns have the right type of data and did converting when needed.
   * I created columns that will be useful for my analysis such: average_time_in_bed_awake, day_of_week, convert minutes in hours when needed, etc  
3. **Exploratory Data Analysis (EDA)**: Analyzed various metrics that focus on: participant, day of the month, day of the week, calories, steps sleep, etc
4. **Comparative Analysis**: Compared the values between different metrics and quantify the correlations:
   - sleep vs calories/ activity, steps,
   - calories vs activity, steps, running,
   - sedentary time vs steps, activity, etc
5. **Statistical Testing**: Applied statistical tests to identify significant differences between each participants and which activities are more common and more effective
   for burning calories.

## Key Findings
1. Participants demonstrate a greater interest in engaging in more physical activities (such as walking, running, and fitness) at the start of the week. However, from Wednesday onward, overall activity levels decrease, leading to a drop in calories burned, with the exception of Saturday, when there is a slight increase in activity;
2. Weekends are not active enough, despite having a time off from the job;
3. The sleep overall is neglected, with an average of only 7 hours;
4. The time spent in bed awake is about 40 minutes which can be reduced for longer and better quality sleep;
5. Longer intensive activities (gym and fitness), along with walking and running, clearly contribute to a more effective calorie burn.
6. Among all activities, the strongest correlation is observed between calories burned and intensive fitness activities.
7. Lastly, given the average sedentary time of 15 hours and adding the time spent at work, we can see that in general, the participants are not spending much time being active and that can be a cause of the relatively high BMI index (25.4).

## Files in This Repository
- `README.md`: This file, provides an overview of the project and the findings.
- `R_markdown_BellaBeat_Case_Study.Rmd`: R Markdown file with the full analysis code and findings.
- `snall_bike_df.csv`: Sample of the dataset used for analysis (due to the size limit, this is only a sample). Full dataset is coming soon.
- `R_markdown_BellaBeat_Case_Study.html` and `R_markdown_BellaBeat_Case_Study.pdf`: Rendered report of the R Markdown file for easier viewing of results and visualizations.


## Technologies Used
- **Excel**: Preliminary exploration, data inspection, data cleaning, creating new columns and data visualization.
- **R**: Used for merging all seasons into one big file, data converting, analysis, and visualization.
- **R Markdown**: Documented the analysis, the steps taken and rendered it into HTML and PDF for sharing.

## Conclusion
The analysis shows that Bellabeat has grown by effectively leveraging marketing strategies and online engagement. Its products help women track health aspects like stress, sleep, and menstrual cycles. However, while the website emphasizes women’s health, data shows many users lack active lifestyles. The products track metrics well but could do more to inspire healthier habits, aligning with the company’s mission. Here is what I believe the company can focus on.

Here are some ideas to help women stay motivated and more active, improving their sleep, activity levels, and calorie burn:
1. paid membership for personalized sleep support: Offering a membership that provides tailored advice on improving sleep quality. Challenges like limiting phone use before bed or achieving 7.5–8 hours of sleep could earn rewards (e.g., product discounts).
2. exclusive online content: Create a subscription-based platform (e.g., YouTube) featuring videos on women’s health, offering monthly memberships for access to valuable insights.
3. supportive products for active women: Develop products that encourage more intensive activities, like:
- fitness towels with motivational motto`s,
- smart water bottles that track hydration and connect to an app,
- comfortable wristwatches that track fitness, yoga, swimming, and gym workouts.
