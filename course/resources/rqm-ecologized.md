# RQM, ecologized

<!-- vim-markdown-toc GFM -->
* [On the necessary changes to the RQM syllabus](#on-the-necessary-changes-to-the-rqm-syllabus)
* [Draft of proposed schedule](#draft-of-proposed-schedule)
    * [Week 1](#week-1)
    * [Week 2](#week-2)
    * [Week 3](#week-3)
    * [Week 4](#week-4)
    * [Week 5](#week-5)
    * [Week 6](#week-6)
    * [Week 7](#week-7)
    * [Week 8](#week-8)
    * [Week 9](#week-9)
    * [Week 10](#week-10)
    * [Week 11](#week-11)
    * [Week 12](#week-12)
    * [Possible additional ideas](#possible-additional-ideas)
* [Labs and lectures from Martin](#labs-and-lectures-from-martin)
    * [Structured population dynamics](#structured-population-dynamics)
    * [Predator prey population dynamics](#predator-prey-population-dynamics)
    * [Lectures](#lectures)
* [The original RQM course](#the-original-rqm-course)
    * [Lecture topics](#lecture-topics)
    * [Discussions](#discussions)
    * [Exercises](#exercises)

<!-- vim-markdown-toc -->

## On the necessary changes to the RQM syllabus
- To tailor the course for ecology students, we need to remove some of the existing material.
- I have tried to summarize the differences between the original schedule and the schedule I propose further down. I did this by classifying all the lectures and tutorials into the overarching themes of the RQM course, and quantified the number of classes dedicated to a theme in the original and proposed schedules (original -> proposed). This can serve as a rough overview for how the course direction is changing:
    - 13 -> 8.5 Reproducibility (includes all R classes)
    - 5 -> 1.5 Authorship, collaboration and publishing
    - 6 -> 0 Openness in data and science
    - 5 -> 8 Project work
    - 0 -> 6 Theoretical ecology
- Most of the topics in Christie's course involve both practical and theoretical aspects. For example, all of the R-coding would fall under reproducibility, but there are also discussions dedicated to reproducibility.
- Note that there are 2 or 3 of these topics per week in the original RQM schedule. Time-wise, this means that a topic approximately equals one class (lecture or tutorial). There were 29 topics in the original RQM course, which we have reduced to 24 topics to fit our course. The total lecture time is still the same, just that each topic gets more attention.

## Draft of proposed schedule
- An immediate conflict to solve is how to ensure that the students get started with their project early, but also have the necessary knowledge about data analyses, R, and the ecology models that Martin wants to incorporate.
- As we are now incorporating some ecology classes into this schedule, I think it is important to make sure enough time is dedicated to teaching sound principles around the data analyse pipeline, as this is still the main focus of the course in my opinion.
- We will teach the introduction with a common data, since this will make it faster, clearer and force students to go through these procedures at least twice, once with the common data set and once with their own, which is advantageous or knowledge retention.
- I originally split these topics into lecture and tutorial, but I will just call it 1 and 2 instead, since both of them will hopefully be in a computer lab. The third item under each week is for suggested homework.
- Quizzes will be done using the automated blackboard setup to as large extent as possible. This will likely work very well for the initial programming multiple choice type exercises, together with some coding puzzles that would be manually graded.
    - This will give students a fair estimate on where they stand before the course drop rate.
- If possible we would like to record the classes, at least the slides and speaker voice through Google Hangouts as during our UofTCoders event.

### Week 1 (Joel)
1. Introduction to the course, intro to the ecology part, motivation behind more reproducible workflows, talk briefly about spreadsheet and get straight into how to use R.
    - Since Martin mentioned we should expect no programming experience from these students, I want to introduce programming at the first lecture already, at least conceptually.
    - We can do this borrowing concepts from a [jupyter notebook I wrote previously](https://github.com/joelostblom/resources/blob/master/from-spreadsheets-to-pandas/from-spreadsheets-to-pandas.ipynb) with analogies between spreadsheet software and programming languages. It's in Python, but if you think this is a good idea, we can adopt it for R. If not, we can do something else.
2. Basic R programming, vectors, data frames, loops, conditions, etc.
    - All coding will be taught in class, but we will provide references for those who want to practice for the quizzes on their own.
        - Interactive introductory exercises, [codeschool](http://tryr.codeschool.com/) and [swirl](http://swirlstats.com/).
        - Reference for data analyses in R, [R for data science](r4ds.had.co.nz).
3. Before 2nd class: Everyone should have Rstudio up and running, and have watched [Christie's talk](https://www.youtube.com/watch?v=TthxI9mlvGE?). Quizzes on portal to complete until next week.

### Week 2 (Joel)
1. Basic R-programming, repetition and continued, scripting.
2. dplyr intro, finalize R-prep by teaching outstanding items required to use R for the following ecology classes.
3. Quizzes on portal.

### Week 3 (Madeleine)
1. Qualitative review of population models
    - Main idea: - modeling a population with a differential equation - gaining insight about a system in several ways without necessarily solving the equation
    - Topics: - phase portraits in 1 dimension - careful, it's not technically a phase portrait if one of the axes isn't a variable - draw the actual 1D phase portrait as well - finding fixed points qualitatively - stability as the direction of a derivative - "stable", "unstable" - Examples: logistic equation and Allee effect
2. Qualitative population models in 2 dimensions
    - Main idea: - modeling interactions between multiple populations with a system of coupled differential equations
    - Topics: - introduce 2 dimensional phase portraits with both variables as axes - introduce null clines qualitatively - Examples: Lotka-Volterra predator-prey model and competition model
3. ???

### Week 4 (Madeleine)
1. Fixed points, null clines, and stability
    - Main idea: - can use math to find fixed points and null clines found by "luck" in previous lesson - can use math to find out if a fixed point is stable or unstable
    - Topics: - finding fixed points analytically - finding null clines analytically - stability analysis - this one is tricky and we might not get to it - probably better to do just graphically and computationally - Examples: spruce-bugworm model and different types of functional response
2. Modeling in R
    - Main idea: - using R to plot, analyze, and solve population models
    - Topics: - calculating trajectories using forward finite difference - plotting phase portraits in R - plotting null clines and fixed points - possibly solving in R as well? - Examples: use models previously analyzed on the board
3. ???

### Week 5 (Madeline & Luke)
1. Fitting models to data
2. Linear regression population dynamics models?
3. ???

### Week 6 (Luke)
1. Introduce data sets, divide intro groups, think about interesting questions to ask, formulate hypothesis/plan of action.
    - Potentially do this already the week before and have them take a survey with the data they want to work on and their background experience.
2. Project work, getting started with their own data in R, tidy data principles, how to clean data, setting up a collaborative git environment through Rprojects and [prodigenr](https://github.com/lwjohnst86/prodigenr) in Rstudio.
3. Quizzes on portal. Create a github account after the first class this week. Maybe write a data README?

### Week 7 (Lindsay)
1. Data visualization in general and in R, ggplot and interactive in plotly (one extra line of code).
2. Data visualization continued, project specific.
3. Quizzes on portal.

### Week 8 (Lina or Elliot)
1. Tools important for reproducible workflow, metadata and Rmarkdown.
2. Project work.
3. Quizzes on portal.

### Week 9 (Elliott)
1. Scientific collaboration. Dive deeper into Git and GitHub.
    - This will include a discussion item from the original RQM course, and serve as a checkup for how the collaboration in the project is going.
2. Project work.
3. Project progress report.

### Week 10 (Lina)
1. Preparing a scientific item for academic publishing.
2. Project work.
3. Project progress report.

### Week 11 (Everyone???)
1. Project work???
2. Project work.
3. Project progress report.

### Week 12 (Everyone)
1. All TAs available to help finishing project this week.
2. All TAs available to help finishing project this week.
3. Final scientific report.

### Possible additional ideas
- Guest lectures
- More about data openness
- Licensing and authorship

## Labs and lectures from Martin
These are the topics from what Martin sent us on Dropbox.

### Structured population dynamics
- Expressing population changes with matrix algebra
- Learning how to use R for matrix operations and basic plotting
- Eigenvalues
- Elasticity of growth rates
- Gaussian distribution fitting, mean, standard deviation, probability density function.

### Predator prey population dynamics
- First order, non-linear, differential equations.
- Stability analysis, non-trivial equilibrium.
- deSolve package in R.

### Lectures
I have put a checkmark on the lessons that seems relevant for the couple of labs that Martin forwarded. Note that this is based on "linguistic similarity" rather than me knowing exactly what topics are included in each lecture... I also don't know to what degree these topics are building on eachother, e.g. do students need to have taken all the previous topics to understand predator prey dynamics? At first glance, it seems like this is _not_ the case, but maybe @mbonsma would know better?
- [x] Abundance and distribution
- [x] Population growth
- [x] Limitation and regulation of populations
- [ ] Logistic growth
- [ ] Allee effects 
- [x] Alternate stable states
- [ ] Environmental stochasticity
- [ ] Demographic stochasticity
- [ ] Stage-structured populations
- [x] Sensitivity and elasticity
- [ ] Intro to chaotic population dynamics
- [ ] Chaos‐tribolium example, time series evidence
- [ ] Non‐stationarity and critical transitions
- [ ] Metapopulation dynamics
- [ ] Source sink dynamics, synchrony, portfolio effects
- [x] Dispersal, spatial spread, traveling waves
- [ ] Spread of infectious diseases
- [ ] Competition (phase portrait, case of coexistence)
- [ ] Competition (other scenarios)
- [x] Lotka‐voltera predator‐prey dynamics


## The original RQM course
I have written a short comment under each heading and then pasted from Christie's notes online to easier get an overview of what is included in the original course syllabus.

### Lecture topics
These are all the topics/bullet points from Christies course, in chronological order. I put a checkmark next to the topics I think are necessary to include, please feel free to add/remove checkmarks, just include comments with the rationale.

- [x] Course syllabus and expectations
- [x] Open science, open data, & reproducibility
- [ ] Rules and regulations from funders and institutions
- [ ] Overview of skills for collaborative science practice
- [x] Using other people’s data - intro to datasets
- [x] Spreadsheet best practices
- [x] Introduction to metadata
- [ ] Data creation and authorship
- [x] Introduction to data cleaning
- [ ] Grey data liberation
- [x] Introduction to Scripting
- [x] Data Cleaning in R
- [x] Version Control
- [x] R Review
- [x] The basics of programming in R
- [x] Even more with R (writing simple software)
- [ ] Getting a bit abstract, submit to conference
- [x] Further topics in R
- [x] Visual communication with data
- [ ] Ethics and risks in sharing data
- [x] Plotting in R
- [ ] Academic publishing, guest speaker
- [x] Project progress via github task list
- [x] Supported work period, Christie away
- [ ] More on Citizen science approaches, Christie away
- [ ] Special Guest: Auriel Fournier
- [x] Supported work period
- [ ] Open source beehives, Christie away
- [x] Supported work period
- [x] Supported work period
- [ ] Special guest mozilla open science
- [x] Preparing a paper for publication

### Discussions
The original RQM syllabus includes lectures, exercises and discussions. While the themes of the exercises largely map well to the lecture topics, the discussions are weighted more toward openness and publishing in general. Below is a list of discussion topics from the RQM course. We need to discuss how many of these we want to include, and if we think the time can be better spent on the lectures and tutorials (this will affect the grading also since some of the blog posts are to reflect on the discussion topics).
- Openness and reproducibility in research
    - So why bother with reproducibility? What's the big deal about openness? How do they fit together? in this, the first class discussion, let's think about your motivations for taking this class. We'll begin the discussion by watching the video together. 
- Authorship in science
- Grey data liberation
    - Refer back to Simon Leather’s post on unused data that needs love.
- Reproducibility and replication
    - What makes a scientific experiment repeatable? Repoducible? Replicable? Readings and video
- Licensing
    - For Tuesday: How do data and content licenses differ? What do you need to keep in mind when assigning a license more restrictive than CC-0 to your work? Talk about what happens if you are integrating multiple data sets and one data set is set as non-commercial while the other is only set as share-and-share alike. Think back to when we discussed MSU's IP policies and revisit what licenses you may or may not be allowed to apply to your work. 
- Authorship on data, authorship in collaboration
    - Now that you're a little deeper into the course, you're ready for a more in-depth discussion about scientific authorship. The readings here are meant to present some extreme views and really provoke discussion. Please read these readings prior to class on Thursday.
- Visualization for communication
    - For this discussion, there's a lot of material we could potentially look at, but the idea is to give you a taste of the things we need to consider when thinking about our visualizations. Conceptually, this is pretty open ended, but I want you to leave with an idea of why they should put a little bit more thought into graphing their data.
- Academic publishing
    - So, how do you decide where to publish? It’s easy to find resources about choosing a journal from a more conventional framework (TL:DR- most of them are some variation of “Choose the journal with the highest impact factor that also fits your work”)- but issues around open access muddies this old advice a bit. This is a really good opportunity to talk about issues with valuing science and scientists by impact factors of journals. We suggest reading High-impact open access journals and Eigenfactor Index of Open Access Fees to get you started. Open access seems simple on the surface, but we get into a very tangled web of corporate interests, biased metrics, and misinformation very quickly.
- Participatory models for bigger science
    - With increased connectivity, we have the opportunity to bring our work to audiences that have never been engaged in science before. This is a good opportunity for students to explore the differences in participatory models between fields, and discuss what engagement means in different fields. We provide a more extreme example, with participatory biomedical research- how do we engage people in our work when the direct ties to their well-being are more tenuous? Next week we'll look at participatory models in ecology.
- Check up on the collaborative process
    - An informal discussion that doubles as a chance to flesh out where the project is going. How is the collaborative process working? Do we need to make adjustments to get the project done? Use our answers to these questions to help populate/adjust the github issue list.
- Looking towards the future
    - Use this discussion as an opportunity to get feedback on the course, and to help guide students in embracing open science and reproducible research in their future endeavours. 


### Exercises
These are largely covered by the topics in the lectures, but if you see something that is not and that you think is important, comment on that line suggesting where to fit it in.

- Find university IP policy, and discuss
- Sign up for github
- Brainstorm questions for project data set
    - What you'd like to ask of your project data set? What questions can be answered with the data set directly? What questions can be answered with additional contextual data? Ask a variety of questions. Write down questions and hypotheses in your blog/etherpad so you have them on record.
- Selecting collaborative writing tools
    - Search the web with your group for collaborative writing tools and platforms. Some places to start: Overleaf, Authorea, Google Docs...even a Word file in a shared Dropbox… really, anything that would allow multiple people to have edit access to a document.
- DATA-README for the project
- Authorship exercise
    - It's always a good idea to set authorship expectations early in the game- it helps contributors understand their respective roles. Discuss with your group- who needs to be on the author list beyond the group members? If people outside the group are to be included, how will they know what their respective roles are? Author order can be determined at a later date, but begin thinking about this as well!
- Reading
    - To prep for next week’s activities, please skim through The Quartz guide to bad data.
- Personas
    - Do a “Persona” exercise designed to help understand goals and motivations of potential data donors. The persona is an imaginary data producer, and our goal is to get that person to share their data. Based on real-world observations and understandings of actual potential or current donors, sketch out this persona, and identify his or her motivations. The persona is used in business and software development to help designers understand and empathize with their users.
- Setup R-studio with Github
- Loops, Conditionals and functions
    - Brainstorm how your new knowledge will aide you in processing your data. 
    - Plot often, comments, R-help and error messages, autoformat?
- Loops, Conditionals and functions again
    - And student directed analyses! Look! See what you find! This is the fun part :)
- Project workshop time
    - Keep working on student-directed analyses.
- Making figures
    - Work through creating figures, based on your project data. Think about things like color palettes, and what that means for accessibility.
- Github issues
    - Use github issues to create a list of things to do for your paper, and assign tasks to group members. If you need a github referesher, this workshop can help guide you in setting up your whole project in github. Basically, what I want to see is a task list that can hold us all accountable to get our projects rounded out and ready to go!
- Revisit the list of github issues in project repo for tasks needing completion
    - Make this a comprehensive list- everything from writing the abstract to inserting the references. Assign specific collegues to tasks. Assess progress towards your goals.
- Work on project
- Preparing a manuscript for submission and review
    - Revisit github issue list to ensure all tasks that need completion prior to submission are represented. Use the ‘instructions for authors’ document provided by your journal of choice to help guide this. And if you're ready, submit the manuscript!
