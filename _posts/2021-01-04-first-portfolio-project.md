---
layout: post
title: First Portfolio Project
subtitle: Data Wrangling with Water Chemistry

tags: [python,data wrangling,data visualization]
---
For this unit's portfolio project I looked for something to combine my existing strength in the geosciences as well as maybe find something that had some personal relevance. That search ended up landing on a topic that was actually quite close to home for me, literally.

My hometown of Norfolk, Virginia is known for many things. Some people think of sprawling dockyards churning out ships. Some think of waiting in traffic to get through one of our beautiful bridge-tunnels. Still others would probably mention our naval station, the largest in the world. For anyone who has ever lived here though, what's most likely the defining quality of our city is the water.

In Norfolk the water is everywhere, it surrounds us on every side and even if you try to get away from it, it'll come find you when it floods next week. We have a certain special relationship with it. Loving it as the undoubtable lifeblood of every industry the city has ever had, and hating it for the innumerable inconveniences it poses. It is important to us.

I am proud to say that this unique relationship with our ocean, three rivers, half dozen bays, scores of lakes, and countless creeks has made our city and our neighbors more than usually interested in the health of our waterways. Over the past two decades millions of data points have been collected to monitor water quality and guide the preservation and rejuvenation of these water systems. Luckily the results produced by this enduring and concerted effort has yielded definite signs of improvement, however conducting this continuous monitoring is costly and time consuming, relying in many cases on the availability of dedicated volunteers to travel out, often to remote parts of the Hampton Roads area, and collect water samples. 

Considering the fact that this monitoring would be required for the forseeable future I decided it would be a worthwhile endeavor to invesitigate potential relationships between water quality in these larger water system and one other thing that we have in abundance here in Norfolk: Rain.

Rain is of course a sensible choice for investigation because all of the water that ends up in lakes, rivers, ponds, creeks, and bays was at one point rain. Beyond that however it's significant because rainfall data is easy to collect. It's a passive collection method requiring very little time, and it can even be automated. Furthermore its data that's already being collected and for which there exists and extensive backlog of data which I could use for my investigation.

For my project I would focus exclusively on one body of water, Back Bay in Virginia Beach as it represents a large but contained body of water with a somewhat developed drainage area and a robust amount of data. The water quality parameters I chose to study were temperature, salinity, pH, dissolved oxygen content, Secchi depth, and water depth. These were chosen by the US Fish and Wildlife Service as most significant to overall health of inland/coastal water systems. Finally, considering the brevity of the assignment and the early stage of my personal research into the subject I decided to keep the experiment simple trying to find if there is or is not a statistically significant relationship between precipitation events (defined here as half an inch or more) and each one of these water parameters.

Null Hypotheses: There is no significant difference in mean (water quality parameter) levels between days with rain and days without rain.
Hypotheses: There is a significant difference in mean (water quality parameter) levels between days with rain and days without rain.

The actual data processing and investigation was simple. Water quality data came from the US Fish and Wildlife Service and historical rain data was collected from the NOAA records. The study period was from 2007 to 2017. Once collected and merged with precipitation data, water quality data were then sorted based on whether they were collected on days with precipitaion events or days without precipitation. Once thus separated it was easy to run two sample T-tests were conducted to compare days with rain to days without rain for each parameter of water quality.

The results were less dramatic than had been hoped but not without value. For five of the six water quality parameters calculations yielded p-values above the 0.05 threshold. Thus my experiment failed to disprove the null hypothesis in the case of water temperature, depth, salinity, dissolved oxygen content, and Secchi depth. However in the case of pH the two sample T-test yielded a p-value of 0.041. In this case I was able to confidently reject the null hypothesis and state that there is a statistically significant difference in water pH between rainy and non-rainy days.

In all honesty these were not the results I was hoping for. I wanted to find dramatic fluctuations in water quality related to rainfall. I wanted this experiment to have never occurred to anyone before and to amaze the scientific world. Acclaim and accolades and a Nobel all would have been accepted reluctantly but with grace. In reality though these results are still important. They show us that (at least in systems like Back Bay) our waterways are more resistant to precipitation based change than was initially expected. Additionally, they provide us with avenues of further research, either in confirming these results or taking the investigation of the relationship between precipitation and pH change farther. With enough study it is even conceivable that a model could be developed to predict what kind of acidification will result from rainstorms before they happen.

For now though I suppose we'll just have to content ourselves with knowing that, should we ever take a water sample on one of Norfolks many rainy days, we can safely expect it to be a little more acidic than usual.


