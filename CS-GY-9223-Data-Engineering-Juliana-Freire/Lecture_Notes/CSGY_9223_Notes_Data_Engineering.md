# CS-GY 9223: Data Engineering - [Hari Varsha V](mailto:hv2241@nyu.edu)
- Fall 2026

## Abstract
These are notes for NYU’s CS-GY 9223, a graduate class on Data Engineering, as taught by Juliana Freire in Fall 2026. Topics include . 

**Course description**: 

# September 5, 2026

## Introduction
1. Class starts off with a Guest Lecture by Parikshit Solunke on Foundations and Principles in Information Visualization.
2. Got introduced to this new tool called observable, looks really cool and is piquing my interest in high-performance ui engineering
3. Deep dive into visualization from a human perspective, and the principles behind good visualization.
4. Information Visualization = computer based, interactive, visual representation of abstract data to amplify cognition.
5. Why infoviz in a data engineering course? understanding data and building abstractions to understand data better.

## History
1. John Snow's Cholera Map. This was before germ theory was introduced, so this autistic guy basically mapped where people where dying and find a spatial pattern to see where people were dying the most.
2. Noticed there were too many deaths near a water pump. Once the pump was removed, magically the outbreak stopped. 
3. Map of Napoleon's march by Charles Minard. One of the best statistical graphics map. Showcases how russia's bait and switch tactic ruined Napolean's troops. The map beautifully visualizes all six variables (like army size and distance and time and temperature etc) simultaneously. Purely Hand-drawn btw.  
4. New York Time's piece on how different variations of y'all across the united states visualized beautifully. deffered to watch later.

## Deeper into the meaning of infoviz
1. Abstract Data - Data with no visual representation. Personal Time Logger.
2. Interactive - How data is visualized and how it is interacted with.
3. Cognitive Artifacts - Tools that help you think. It's easier to multiply numbers with a pen and paper rather than in your mind since we can store intermediary results in the paper than keeping the information in mind. Offload the work so you can understand data easier.

## Why use visualization
1. Explanatory
1.1. Show insight to others. Present findings, tell data stories, communicate clearly.
1.2. Find patterns yourself. Discover unknowns, generate hypotheses, understand data.
1.3. Validate Hypotheses. Test assumptions, verify patterns, and support decisions.
2. Pudding -  an excellent visualization website according to the lecturer.
3. How does one assess the quality of visualization? What makes one better than another? Subjectivity is only one part of the whole answer.

## Visual Perception.
1. Design principles were formalized in 1976. A chart should be effective(Use encodings that people decode better) and expressive (tell the truth and nothing but the truth).
2. Effective Measures - accuracy, discriminability, saliency, seprabality, and grouping
3. Large part of your brain is for visual sensitivity. You can build a data communication tool soley based on other senses but for deciphering data, visual is still king since your brain is hardwired for it (kinda makes sense when you think about finding danger)
4. Top-down (Eye Tracking) and Bottom-up processing(Visual Puzzles like the duck vs rabbit chart, the lamp vs two faces, same shape but looks different size)
5. Design visualization in such a way it exacts describes what it needs to say when one pays attention to it.
6. There's level to this neuroscience part of the info viz field. Multiple studies and experiments done to undertand how the brain understands data (aka i got distracted and took notes of the slides instead of the speaker).
7. Cleveland and McGill Result - We are worse at comparing angles than in comparing scores. That's why a bar chart is easier than a pie chart or the other way around. The encodings matter, that's the takeaway. 
8. Channel effective ranking - magnitude (ordered attributes like position on a common scale) and identity (categorial attributes) channels. 
9. 3D is better when you comparing volume. Avoid it for quantitative data.
10. Takeaway, use position for most important comparisons. Use color for categorical distinctions. 
11. Discriminability guidelines - do not overestimate the number of values a viewer can take in at a time. 
12. Pre-attentive processing - search time does not depend on number of distractors (take pop-out for example). Certain visual features are based on low level processing where we process parallel data and find out what stands out. 
13. Certain set of visual features we are tuned and others that aren't as effective
14. When certain needle shares the same features of others it gets hard. You need the needle to have genuine feature contrast (like bolding) for easier visualization.
15. Conjuction of two or more features and not pre-attentive and forces serial attentive search (go over stuff one by one)
16. Visual pop-out helps building better visualizations
17. Pre-attentive processing happens in 250ms thanks to massive parallelization
18. Gesalt: visualizations can be unintentionally miseleading, brains infer a trend where there is none.
19. Elements with same visual properties are grouped together. Spatial closeness alone is enough to differentiate elements (while elements are spatially close as perceived as grouped and our brains are forced to infer analogies from the data.)
20. Line drawn between 2 objects are more closely perceived to be grouped more than color itself.
21. Just Noticable Difference - amount of something must be changed to be noticeable at least 50% of the time. Like change in voltage or brightness.

## Data Types
1. Nominal data - categorial. No inherent meaning to a specific ranking or order. e.g: apple and orange don't really tell you much. 
2. Ordinal dats consists of values that have a specific ordering. Order matters here. e.g: change of brightness and contrast.
3. Time is a tricky one
4. Spatial - data can be shown in a map.
5. quantitative implies nominal which implies ordinal. 

## Notes 
1. Probably should start system level web development once I'm done with rust.
2. Go over beautiful Information visualization reddit channel.

# September 11, 2026

## Introduction 
1. Prof's background, research, and anecdotes on working in Bell Labs and other parts of life. 
2. HW - 35%, Final Project instead of exam - 40%, Labs + Quizzes - 20%, Class Participation - 5%.
3. Use NYU VPN to access papers from the NYU network.
4. Will be using JupyterHub and Dataproc.

## Data Engineering
1. DE - Practice of designing, building, and maintaining the systems that collect, store, and process raw data. 
2. Core Concepts, not written in stone, more like what the industry influenced: data ingestion, processing/transformation, storage, orchestration, monitoring + quality control 
3. Idealized Data Science: Dataset -> Train Model -> Predictions 
4. The above doesn't say the real story, read data is really messy and need to be worked on. Most of the time is gone for plumbing.

## Why Data Engineering
1. Helps you be a better data scientist. More open roles. Don't fall for hypes just yet.
2. You'll be learning modelling and quering data, the usual sql stuff. Especially, how to work with real world messy data for your real use-cases. 
3. Have pipelines to work with data like data warehouses and spark. Get an understanding of distributed computing.
4. Data Preparation: Techniques to gain insight from the data.
5. More specific topics and emerging trends relevant to data engineering.
6. Focus on the principles and algorithmic solutions for the problems. Think about efficient and performant every single time.
7. The goal is to learn the material.

## Data Driven Exploration 
1. Every domain has moved towards data driven exploration, this has become the 4th paradigm of science. 
2. Industry loves data so much it's like oil to them. Goverments use it to inform policies. All thanks to compute and storage being free and data is redundant.
3. Noble Prizes now given to computer scientists because of the insights they get from Big Data. Refer: OpenAI, Anthropic, and Deepmind scientific achievements.
4. Real example on how DE is used to make cities better - illegal conversions in nyc. 
5. Challenges: Data is too vast and require expertise in a wide range of topics to get the right insights. No one right path to do it.
6. Bottleneck is people !
7. Example on bad data visualization: McKinsey. Use proper colours.


## Notes
1. Content is experimental, get a crash course on DBs from UCB and CMU.

