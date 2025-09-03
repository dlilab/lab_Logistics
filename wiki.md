# Wiki

## Computational tools

This will change as machines get added to the lab. This doesn't include the workstations for students, which are three 12gb Dell Optiplex 5020. 

+ `server`: Dell server (PowerEdge T440, 128gb RAM, 32 Cores machine in LSB 125)

Below is a list of computational tools that I would like lab members to be cognizant of. 


+ `linux`: all lab computers will run the most current long term stable (LTS) release of Ubuntu. 
+ `git` and `Github`: version control is an important part of science. It allows real time progress updates, issue tracking, and version control. There are numerous guides to beginning to learn how to use git with Github [training](https://swcarpentry.github.io/git-novice-es/) and [further training](https://guides.github.com/activities/hello-world/). 
+ `R`: lab members are expected to be familiar with the R programming environment. This is not to say you can't program in other languages (e.g., Python or Julia are good alternatives), but the most overlap with other lab members will likely come through the use of R. I don't care if you want to use base or the fanciest new package to hit the tidyverse, but having a common computational language among lab members has clear benefits [training](http://swcarpentry.github.io/r-novice-inflammation/)
+ `(R) markdown`: markdown is a markup language used to create this file. R markdown allows embedding R code within markdown documents, creating a document that can be compiled to contain both explanatory text and the results of analyses. [markdown tutorial](https://www.markdowntutorial.com/), [R markdown tutorial](https://rmarkdown.rstudio.com/lesson-1.html)


## Lab server

To connect to the lab server, we need to be either on campus or use UA VPN to connect to UA intranet. The ip address is 128.104.98.132. To get access to it, we can use Terminal (`ssh user@128.104.98.132`) or go to your browser and enter http://128.104.98.132:8787/ or http://bot211.botany.wisc.edu:8787/ then login with your information.

We should save our projects in `/media/dli/Data`

### Set up new user

```bash
ssh root@server.ip.address
sudo adduser username
sudo usermod -aG sudo username
```

Then log in to set up RStudio server:

```bash
# specify where to install R packages
echo 'R_LIBS_USER="~/R"' > .Renviron
# to install binary packages
echo 'options(servr.daemon = TRUE, repos = c(rstudio_binary = "https://packagemanager.posit.co/all/__linux__/focal/latest"))' > .Rprofile
```

## Library resource

For some reason, I still cannot download articles directly from webpages even using the LSU VPN. Instead, I found that it is possible to replace the first part of the URL to get access to full text. Here is a list that I accumulated:

- List of databases from LSU library: https://login.ezproxy3.library.arizona.edu/menu
- Links with doi: https://doi-org.ezproxy3.library.arizona.edu/
- jstor links: https://www-jstor-org.ezproxy3.library.arizona.edu 
- Science: https://www-sciencemag-org.ezproxy3.library.arizona.edu or http://www.sciencemag.org.ezproxy3.library.arizona.edu 
- Nature: https://www-nature-com.ezproxy3.library.arizona.edu
- Royal Society Publishing: https://royalsocietypublishing-org.ezproxy3.library.arizona.edu/
- Wiley: https://onlinelibrary-wiley-com.ezproxy3.library.arizona.edu
- Science direct: https://www-sciencedirect-com.ezproxy3.library.arizona.edu
- U Chicago Press: https://www-journals-uchicago-edu.ezproxy3.library.arizona.edu/ 
- Springer: https://link-springer-com.ezproxy3.library.arizona.edu
- Cell press: https://www-cell-com.ezproxy3.library.arizona.edu
- PNAS: https://www-pnas-org.ezproxy3.library.arizona.edu
- Web of Science: https://apps-webofknowledge-com.ezproxy3.library.arizona.edu/WOS_GeneralSearch_input.do?product=WOS&search_mode=GeneralSearch&SID=8F8swBPcvR4AyxiPidm&preferencesSaved=
- Annual Reviews: https://www-annualreviews-org.ezproxy3.library.arizona.edu
- ProQuest dissertations: https://search-proquest-com.ezproxy3.library.arizona.edu


## Collaboration

I do not need to be coauthor on every manuscript coming out of the lab, and I encourage students to research and publish independently of me. That being said, research using lab resources may be more suitable for my coauthorship, and I am happy to actively contribute to the project, or to allow the student to work independently. I also encourage students to collaborate with other scientists within LSU and outside. However, new collaborations should be discussed with me before students initiate them (if possible). 


## University Authorization Process

If you need to get permission to drive a university vehicle, you need to [get authorization first](https://lsu.edu/riskmgt/vehicleuse/lsuam_vehicleuseprocedures.php).

## On board list

Here is a list for those who are just on board

- An official welcome (can be just an email)
- Tour of lab space
- Point to this Wiki
- [Request keys here](https://eeb.arizona.edu/about/department-resources/keys-keyless-access).
- Accessibility through email or office visits
- Talk about potential research projects
- Discuss the lab Github, protocols, and useful lab skill
- Weekly one-on-one meeting plus lab meeting
  - I expect everyone in the lab to create a weekly planning Google Doc and share it with me. Within this document, each of us should list what we have done this week and what we plan to do (_dodable actions_) next week. This file will also serve as an agenda for our one-to-one weekly meetings.
  

  
