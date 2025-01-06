# Baseball-Coding-Projects-R-and-Google-Colab
This project is a comprehensive analysis I conducted using my knowledge from my studies at the University of Michigan. In this project, I sought to bridge the gap between Nippon Professional Baseball (NPB) and Major League Baseball (MLB) by projecting the performance of NPB players in the MLB. The primary goal was to estimate how top NPB hitters would perform in the MLB environment, using various statistical projections and tools to better understand the potential contributions of these players. With the rise of international talent in MLB, including players like Shohei Ohtani, Ichiro Suzuki, and Yu Darvish, it’s crucial to have reliable methods for predicting how statistics from the NPB will translate to the MLB. This project was my first venture into using R for baseball analytics, and it was an exciting challenge, combining statistical analysis, data cleaning, and visualization to produce meaningful insights.

I began by gathering player performance data from various reliable sources, including Baseball Reference, MLB.com, and Baseballguru.com. I focused on top NPB hitters from the previous season, collecting key statistics such as batting average (BA), on-base percentage (OBP), slugging percentage (SLG), and other performance metrics. The real challenge lay in normalizing these statistics to account for differences between the two leagues. To make fair comparisons, I adjusted for league difficulty and park factors, using Jim Albright’s conversion methods, which have been popularized through his work on projecting players like Sadaharu Oh to the MLB. These methods provided the conversion factors for BA, OBP, and SLG, as well as specific multipliers for other statistics such as triples and home runs.

Once the data was collected and standardized, I calculated “Win Shares,” a stat that measures a player's overall value to their team, using a formula adapted for both NPB and MLB. This involved breaking down a player's hits into singles, doubles, triples, and home runs, and factoring in walks and outs. The calculation for Win Shares is based on a system that attempts to quantify a player's offensive contribution by weighing different types of hits, walks, and outs. I applied this formula first to the raw NPB data and then projected these statistics to the MLB using the conversion factors. For example, home runs are scaled down based on the historical differences between the two leagues, and triples are adjusted upwards due to the larger outfields in the MLB. Walks are also slightly increased in the MLB, given the league’s higher rates of walk generation.

Once I had projected the NPB statistics to MLB equivalents, I re-calculated the Win Shares for these players as if they were competing in the MLB. This allowed me to compare the performance of NPB hitters directly with MLB hitters. For comparison, I also pulled data for top MLB hitters and applied the same Win Shares formula to calculate their projected value over a 162-game season. This gave me a solid basis for evaluating how NPB players might perform in the MLB and which of them would be most valuable.

The insights from the projections were revealing. While some of the top NPB hitters—like Tyler Austin, Domingo Santana, and Hiroki Fukunaga—showed strong performances in their domestic league, their projected Win Shares in the MLB were generally more in line with the performance of players like Luis Arraez rather than the top-tier MLB stars such as Aaron Judge or Bobby Witt Jr. This indicates that, despite their dominance in the NPB, many of these players might face a significant adjustment when transitioning to the higher level of competition in the MLB. These projections provided a valuable tool for teams looking to evaluate the potential of Japanese players and assess their relative value before considering signing or trading for them.

This project also provided a solid foundation for my understanding of how statistical analysis and modeling can be applied to real-world sports scenarios. It helped me develop my skills in R, particularly with packages like tidyverse for data manipulation, and ggplot2 for visualization. I also became proficient in web scraping with rvest to collect data from websites, an essential skill for any data-driven analysis project. Using these tools, I built a structured workflow that allowed me to clean, process, and visualize the data to answer the project's key questions. By comparing Win Shares across leagues and incorporating historical projection methods, I was able to offer a compelling analysis of how NPB talent might perform in the MLB.

Looking back, I am proud of my work in this project, especially as it combined multiple aspects of data science, baseball analytics, and R programming. I could take concepts I learned at U of M, such as statistical modeling and data visualization, and apply them to a sports context, producing results that could be meaningful to baseball analysts, scouts, and operations teams. This project also ignited a deeper passion for baseball analytics, and I look forward to continuing my work in this field, combining my skills in data science with my love for the game of baseball. 
