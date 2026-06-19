# udemy-courses-eda-project
# Udemy Courses - Exploratory Data Analysis (EDA)

This repository contains a structured Exploratory Data Analysis (EDA) project focused on a dataset of Udemy courses. Using Python's **Pandas**, **NumPy**, **Seaborn**, and **Matplotlib** ecosystems, this project explores course metrics, subscriber behavior, pricing dynamics, and specific technology trends (such as Python courses).

## 📌 Project Overview
The notebook demonstrates essential data-wrangling practices, including handling datetimes, isolating and dropping duplicate values, plotting categorical distributions, and evaluating correlations using scatter plots.

---

## 📊 Dataset Reference
The pipeline runs directly against the following source file:
* **Source Dataset File:** `5-udemy_courses.csv`

### Explored Features Include:
* **course_id:** Unique numeric identifier for each course[cite: 3].
* **course_title:** The visible title of the course[cite: 3].
* **url:** The direct platform web link[cite: 3].
* **is_paid:** Boolean flag indicating if the course is paid or free (`True`/`False`)[cite: 3].
* **price:** Cost of purchasing the course[cite: 3].
* **num_subscribers:** Total number of students enrolled[cite: 3].
* **num_reviews:** Total volume of feedback left by subscribers[cite: 3].
* **num_lectures:** Total count of individual instructional lessons[cite: 3].
* **level:** Target student expertise depth (e.g., *All Levels*, *Intermediate Level*)[cite: 3].
* **content_duration:** Total length of lecture content in hours[cite: 3].
* **published_timestamp:** Raw date-time string when the course went live[cite: 3].
* **subject:** Marketplace categorization field (e.g., *Business Finance*)[cite: 3].

---

## 🔍 Analytical Milestones
The codebase walks through 18 sequential steps, answering specific operational and business metrics:

1. **Initial Snapshots:** Displaying the top 10 rows[cite: 3] and bottom 5 rows[cite: 3] to check dataset structural integrity.
2. **Dimension Auditing:** Tracking matrix size bounds (total rows and columns)[cite: 3].
3. **Data Type Correction:** Spotting that `published_timestamp` is loaded as a generic string/object[cite: 3] and using `parse_dates` to cast it into a true datetime format[cite: 3].
4. **Data Cleansing:** Checking for structural missing/null entries across all features[cite: 3] and locating, reporting, and dropping duplicate observations[cite: 3].
5. **Subject Distribution:** Quantifying and visualizing total courses hosted across distinct subject matters using `sns.countplot`[cite: 3].
6. **Difficulty Level Tracking:** Slicing target offerings across core target experience levels[cite: 3].
7. **Monetization Breakdown:** Tallying total volume availability differences between Paid and Free formats[cite: 3].
8. **Lecture Densities:** Grouping data to find out whether Free or Paid structures average more instructional lectures[cite: 3].
9. **Subscriber Enrollment Drivers:** Evaluating whether Paid or Free structures draw a greater collective sum of student subscribers[cite: 3].
10. **Target Level Engagement:** Isolating which target experience level retains the largest aggregate subscriber base[cite: 3].
11. **Platform Popularity Peaks:** Pinpointing the single most-subscribed course title in the dataset[cite: 3] and expanding it to show the top 10 most popular courses overall[cite: 3].
12. **Feedback Volume:** Finding out which specific training courses managed to draw the highest volume of user reviews[cite: 3].
13. **Price vs. Engagement Correlation:** Evaluating if a higher course price directly impacts user review volumes using a scatter plot (`sns.scatterplot`)[cite: 3].
14. **Niche Keyword Filtering:** Locating all available courses focused specifically on **Python** using case-insensitive string filtering[cite: 3], counting them[cite: 3], and isolating the top 10 most popular Python classes[cite: 3].

---

## 🛠️ Tech Stack & Dependencies
To install the tracking libraries required for this workspace environment, run:
```bash
pip install pandas numpy seaborn matplotlib jupyter
