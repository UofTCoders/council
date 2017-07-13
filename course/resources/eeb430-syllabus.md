# EEB430H1 Theoretical Ecology [24L, 12P]
This course focuses on theoretical ecology concepts and reproducible quantitative methods using R. Theoretical ecology uses models to explain biological phenomena such as the maintenance of biodiversity, population growth, competition, eco-evolutionary dynamics, epidemiology, spatial ecology, and species extinction. This course is designed to meet a growing demand for reproducible, openly accessible, analytically thorough, and well documented science. Students will learn to develop ecological population models, analyze data, and document their research using the R programming language. No prerequisite programming experience is required.

Prerequisites: MAT 136, BIO220H1, EEB225H1, and two of EEB319H1, EEB321H1,
EEB322H1, EEB323H1

# Time
Tue and Thu 2-4 pm.  

# Lecture halls
Tue, Ramsay Wright (RW 109).  
South west corner of Harbord and St George, 1st floor, enter from St George street.

Thu, Carr Hall (SMC 325).  
Corner of Queen's Park East and St. Joseph Street, 3rd floor, St. Michael's College.

Both lecture halls have access to individual computers for the students. To use the computer workstations, students can login with their UTORid and password. Installed programs and packages are wiped from the computers daily. Saved files will be accessible from any computer via the student's login. Students can use any of the lecture halls when there are no classes scheduled. See the [online schedules](http://lab.chass.utoronto.ca/carr.php) for available times.

# Contact info

## Teaching assistants
Joel Ostblom (course coordinator), joel.ostblom@mail.utoronto.ca  
Madeleine Bonsma, m.bonsma@mail.utoronto.ca  
Luke Johnston, luke.johnston@mail.utoronto.ca  
Lina Tran, lina.tran@mail.utoronto.ca  
Elliott Sales de Andrade, esalesde@physics.utoronto.ca  
Lindsay Coome, lindsay.coome@mail.utoronto.ca  

_Please address all general course-related email communication to joel.ostblom@mail.utoronto.ca, and project specific communication to the respective TA of your group. Prefix the subject matter with "EEB430". If you do not receive a reply within 48 hours (excluding week-ends), please send a reminder. Office hours: Contact us by e-mail to schedule a time._

## Supervising professor
Prof. Martin Krkosek, martin.krkosek@utoronto.ca, 416-978-3839, RW402

# Course Web page (on Blackboard)
All course information will be stored on Blackboard (http://portal.utoronto.ca/). You will have access to the Syllabus, Lecture Schedule & Recommended Readings for each lecture, Lab Schedule, Lab Instructions, Lecture slides (pdf files) and Lab Data sheets. If you have any problem accessing the material, let us know right away so we can fix the problem (e-mail is best).

# Recommended resources
- [R for Data science](http://r4ds.had.co.nz/), H Wickham, G Grolemund, 2017
    - Excellent open access resource for R.
- [Rstudio cheat sheets](https://www.rstudio.com/resources/cheatsheets/), Rstudio, 2017
    - As good as it sounds, great quick reference.
- [R for ecological data science](http://www.datacarpentry.org/R-ecology-lesson/index.html)
    - An inspiration for our lectures.

# Course learning outcomes
1. Integrate and apply concepts and theoretical models learnt in class.
2. Learn how to use basic statistics to analyze and interpret data.
3. Realize that data do not always fit theoretical models, but that it is important to interpret data with a larger theoretical framework in mind.
4. Learn how to work in group on a scientific product.
5. Learn what is required to generate a scientific item ready for publishing.

# Improving your writing skills
Effective communication is crucial in science. The University of Toronto provides services to help you improve your writing (see specific section on lab reports), from general advices on effective writing to writing centers and writing courses. See http://www.writing.utoronto.ca/. The Faculty of Arts & Science also offers an English Language Learning (ELL) program, which provides free individualized instruction in English skills. Take advantage of these!

# Academic integrity:
You should be aware of the University of Toronto Code of Behaviour on Academic Matters. Also see http://www.writing.utoronto.ca/advice/using-sources/how-not-to-plagiarize on How Not to Plagiarize. Note that it is NOT appropriate to use large sections from internet sources, and inserting a few words here and there does not make it an original piece of writing. Be careful in using internet sources – there is no review of most online material and there are MANY errors out there. Use only academic or government internet sources when absolutely necessary. Make sure you read material from many sources (published, peer-reviewed, trusted internet sources) and that you write an original text using this information. Always cite your sources. In case of doubt about plagiarism, talk to your instructor.

# Lecture schedule
| Week | Date   | Topic                                               | Instructor     |
|------|--------|-----------------------------------------------------|----------------|
| 1    | Sep 07 | Welcome to the course! Intro to programming         | Everyone       |
| 2    | Sep 12 | Basic R – Rstudio, Rmarkdown, assignment, vectors   | Joel           |
| 3    | Sep 14 | Basic R – functions, data frames, indexing          | Joel           |
| 4    | Sep 19 | Intro to dplyr data wrangling                       | Joel           |
| 5    | Sep 21 | More dplyr, ggplot intro                            | Joel           |
| 6    | Sep 26 | Qualitative review of population models             | Madeleine      |
| 7    | Sep 28 | Qualitative population models in 2 dimensions       | Madeleine      |
| 8    | Oct 03 | Fixed points, null clines, and stability            | Madeleine      |
| 9    | Oct 05 | Modeling in R                                       | Madeleine      |
| 10   | Oct 10 | Fitting models to data                              | Madeleine      |
| 11   | Oct 12 | Linear regression population dynamics models?       | Luke           |
| 12   | Oct 17 | Introduce data sets, hypotheses, start projects     | Luke           |
| 13   | Oct 19 | Project work, prodigenR, tidy data, git via rstudio | Luke           |
| 14   | Oct 24 | Data visualization in R                             | Lindsay        |
| 15   | Oct 26 | Project work, data visualizations                   | Lindsay        |
| 16   | Oct 31 | Reproducible workflow, metadata, Rmarkdown          | Lina           |
| 17   | Nov 02 | Project work, metadata                              | 1 TA/group     |
| -    | Nov 07 | Fall break                                          | -              |
| -    | Nov 09 | Fall break                                          | -              |
| 18   | Nov 14 | Scientific collaboration, Git and GitHub            | Elliot         |
| 19   | Nov 16 | Project work                                        | 1 TA/group     |
| 20   | Nov 21 | Preparing a scientific item for academic publishing | Lina           |
| 21   | Nov 23 | Project work                                        | 1 TA/group     |
| 22   | Nov 28 | Project work                                        | 1 TA/group     |
| 23   | Nov 30 | Project work                                        | Everyone       |
| 24   | Dec 05 | Project work                                        | Everyone       |

# Assessment schedule 
| Assesment             | Type                | Due date   | Marks |
|-----------------------|---------------------|------------|-------|
| Getting set up        | Individual          | Sep 11     | 4     |
| Basic R               | Individual          | Sep 18     | 8     |
| dplyr                 | Individual          | Sep 25     | 8     |
| Population models     | Individual          | Oct 02     | 8     |
| Modeling in R         | Individual          | Oct 09     | 8     |
| Linear regression?    | Individual          | Oct 16     | 8     |
| Setup github          | Project, Individual | Oct 23     | 8     |
| Data visualization    | Project, Individual | Oct 30     | 8     |
| Reproducible workflow | Project, Individual | Nov 06     | 8     |
| Final project work    | Project, Group      | Dec 9 – 20 | 32    |

_There will be a penalty of -5% per day (including week-ends) for late submissions._
