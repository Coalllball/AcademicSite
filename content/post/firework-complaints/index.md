---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Firework Complaints"
subtitle: ""
summary: ""
authors: []
tags: []
categories: []
date: 2022-12-12T22:47:31-05:00
lastmod: 2022-12-12T22:47:31-05:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---
Background
Every summer, New York City’s 311 platform receives a large number of complaints about illegal fireworks. For a metropolis like New York, the dangers of illegal fireworks are undoubtedly significant. Not only does the amount of noise disrupt the rest of the residents, but also the fire hazards threaten people’s lives and property safety. The situation is extremely complex to control, though, as it requires extensive police powers to deal with this relatively minor vandalous behavior. Additionally, New York City has a long tradition of large 4th of July fireworks celebrations, where complaints about illegal fireworks displays typically increase around the time of large fireworks shows. However, the long-standing problem was not considered severe compared to the situation in the summer of 2020. At that time, the COVID-19 pandemic caused a significant reduction in everyday NYC activities, yet compared to the calmness of the day, New York City was extraordinarily noisy at night. Complaints about illegal fireworks received by the 311 hotlines skyrocketed by 4,000 percent. This project will use GIS Analysis techniques to create a map and to review the uneven summer of 2020 visually.

Data Source
The dataset used in this project is extracted from Open NYC’s 311 Service Requests from 2010 to Present. The original dataset contains all 28.4 million complaint records received by the 311 hotlines over the past decade. Each record contains 41 factors, including the complaint type, complaint time, detailed street address, and coordinate information. This comprehensive dataset was very convenient for my work. Through a series of data cleaning process, the final selected dataset includes 48,327 illegal fireworks complaints received by 311 from May 1, 2020 to August 30, 2020.

Softwares
QGIS
In order to present the amount of illegal fireworks complaints in each region of New York City in a visual way, I chose to create a Choropleth map using QGIS, a free open source geographic information system analysis software. Its rich features and active community contributions make it very easy to use and popular. Users can use QGIS to perform GIS analysis and design attractive visualizations with a basic knowledge of geographic information file formats. In this project, I also used the New York City map and Community Districts map provided by Open NYC to support my analysis and design.

R Studio
R Studio is a free and open-source IDE for R. Users can use R Studio to manage data files and perform statistical analysis more efficiently. Its rich community contributions also make it easier to work with data analysis. This project utilizes R Studio for all data cleaning and performs data analysis on the illegal fireworks problem with graphs and charts to help the audience understand the results in more depth.

Inspiration
There have been many media stories about the flood of illegal fireworks in the summer of 2020. One of the articles from Gothamist.com interested me the most. This article included a dynamic map of fireworks complaints that visually illustrated the surge in the number of fireworks complaints in June 2020.