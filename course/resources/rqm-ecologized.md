# RQM, ecologized

* [On the necessary changes to the RQM syllabus](#general-comments-on-the-necessary-changes-to-the-rqm-syllabus)
* [Draft of proposed schedule](#draft-of-proposed-schedule)
    * [Week 1](#week-1)
    * [Week 2](#week-2)
    * [Week 3](#week-3)
    * [Week 4](#week-4)
    * [Week 5](#week-5)
    * [Week 6](#week-6)
    * [Week 7](#week-7)
    * [Week 8-12](#week-8-12)
* [Labs and lectures from Martin](#labs-and-lectures-from-martin)
    * [Structured population dynamics](#structured-population-dynamics)
    * [Predator prey population dynamics](#predator-prey-population-dynamics)
    * [Lectures](#lectures)
* [Topics in the original schedule](#topics-in-the-original-schedule)
    * [Discussions](#discussions)
    * [Exercises](#exercises)

## General comments on the necessary changes to the RQM syllabus
- To tailor the course for ecology students, we need to remove some of the existing material.
- Most of the topics in Christie's course involve both practical and theoretical aspects. For example, all of the R-coding would fall under reproducibility, but there are also discussions dedicated to reproducibility.
- I classified all the lectures and tutorials into the overarching themes of the RQM course, and quantified the number of classes dedicated to a theme in the original and proposed schedules (original -> proposed). This can serve as a rough overview for how the course direction is changing:
    - 13 -> 13 Reproducibility (includes all R classes)
    - 6 -> 1 Openness in data and science
    - 5 -> 1 Authorship and publishing
    - 5 -> 8 Project work
    - 0 -> 6 Ecology
- Note that there are 2 or 3 of these topics per week in the original RQM schedule. Timewise, this means that a topic approximately equals one class (lecture or tutorial). There are 29 topics here and will be 24 classes taught, so we will need to include 3/week in some cases or reduce this to from 29 to 24.

## Draft of proposed schedule
One conflict is to have the students get started with their project early, but also have the necessary knowledge about the ecology models that Martin want to incorporate. I still think that we should teach them ... Another point of consideration is whether we should teach all the R stuff with a common data set, so that we can streamline it for teaching the principles, and then hand out student data sets after a few weeks. I am leaning towards a common data for the first weeks, since this would make it faster and force students to go through these procedures at least twice, once with the common data set and once with their own, which is better for retention. I think classes can be quite choppy if everyone has their own data set specific problems come up, that's better dealt with in tutorials with the group specific TAs.

I originally split these into lecture and tutorial, but will just call it 1 and 2 now since both of them will hopefully be in a computer lab. The third item is for homework.

Do we want simple quizzes at the start of each lecture, for the first ~5 weeks? This could serve as an easy to grade item and make sure that the students put effort in at home. It will make it easier to say where students are at the drop date, and we can then reduce them as the course moves into the project based phase.

### Week 1
1. Introduction to the course, intro to the ecology part, motivation behind more reproducible workflows, talk briefly about spreadsheet and get straight into how to use R.
    - Since Martin mentioned we should expect no programming experience from these students, I want to introduce programming at the first lecture already, at least conceptually.
    - Probably based on a jupyter notebook I wrote previously with analogies between spreadsheet software and programming languages. It's in Python, but if you think this is a good idea, I will adopt it for R.
2. Basic R programming, vectors, data frames, loops, conditions, etc.
3. Before 2nd class: Everyone have R up and running. Maybe we can link them to some R intro course and ask them to complete 1 or 2 lectures there per week, which will also serve as the underlying material for the quiz? This one is good imo http://tryr.codeschool.com/. Watch Christie's talk https://www.youtube.com/watch?v=TthxI9mlvGE. 

### Week 2
1. Basic R-programming, repetition and continued, scripting.
2. dplyr intro, finalize R-prep by teaching outstanding items required to use R for the following ecology classes.
3. Again, link online lectures?

### Week 3
1. Ecology background knowledge for lab 1
2. Ecology lab 1 (or similar)
3. Lab report? Aka send in their code.

### Week 4
1. Ecology background knowledge for lab 2
2. Ecology lab 2 (or similar)
3. Lab report? Aka send in their code.

### Week 5
1. Present data sets, divide intro groups, think about interesting questions to ask, formulate hypothesis/plan of action.
2. Project work, getting started with their own data in R, tidy data principles, how to clean data, setting up a collaborative git environment with Rstudio (how much do we want to get into git?).
3. Reflections blog post of what they have learnt so far?

### Week 6
1. Data visualization in general and in R, ggplot, interactive (since plotly is just one additional line)?
2. Data visualization continued, project specific.
3. Online tutorial about plotting.

### Week 7
1. Stuff important for reproducible workflow, metadata, Rmarkdown, Roxygen?
2. Project work,
3. Write a data README?

### Week 8-12
I don't want to complete the entire course syllabus, since I expect there will be many things that will be reorganized anyways. Ideally one lecture per week from now on would be project work only. Potential ideas:
    - A couple of additional ecology lessons?
    - More info about working together on online collaborative platforms? Both for code and writing.
    - More about data openness?
    - Guest lectures?
    - Preparing a scientific item for academic publishing
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
I have put a checkmark on the lessons that seems relevant for the couple of labs that Martin forwarded. Note that this is based on "linguistic similarity" rather than me knowing exactly what topics are included in each lecture... I also don't know to what degree these topics are building on eachother, e.g. do student need to have taken all the previous topics to understand predator prey dynamics? It seems like this is _not_ the case, but maybe @mbonsma would know better?
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


## Topics in the original schedule
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
- The original RQM syllabus includes lectures, exercises and discussions. While the themes of the exercises largely map well to the lecture topics, the discussions are weighted more toward openness and publishing in general. Below is a list of discussion topics from the RQM course. We need to discuss how many of these we want to include, and if we think the time can be better spent on the lectures and tutorials (this will affect the grading also since some of the blog posts are to reflect on the discussion topics).
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
