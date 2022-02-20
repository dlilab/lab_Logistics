# Wiki

## Computational tools

This will change as machines get added to the lab. This doesn't include the workstations for students, which are three 12gb Dell Optiplex 5020. 

+ `2018 Macbook Pro`: lab laptop (16gb RAM laptop, currently lend to Flavia)
+ `server`: Dell server (PowerEdge T440, 128gb RAM, 32 Cores machine in LSB 125)

Below is a list of computational tools that I would like lab members to be cognizant of. 


+ `linux`: all lab computers will run the most current long term stable (LTS) release of Ubuntu. 
+ `git` and `Github`: version control is an important part of science. It allows real time progress updates, issue tracking, and version control. There are numerous guides to beginning to learn how to use git with Github [training](https://swcarpentry.github.io/git-novice-es/) and [further training](https://guides.github.com/activities/hello-world/). 
+ `R`: lab members are expected to be familiar with the R programming environment. This is not to say you can't program in other languages (e.g., Python or Julia are good alternatives), but the most overlap with other lab members will likely come through the use of R. I don't care if you want to use base or the fanciest new package to hit the tidyverse, but having a common computational language among lab members has clear benefits [training](http://swcarpentry.github.io/r-novice-inflammation/)
+ `(R) markdown`: markdown is a markup language used to create this file. R markdown allows embedding R code within markdown documents, creating a document that can be compiled to contain both explanatory text and the results of analyses. [markdown tutorial](https://www.markdowntutorial.com/), [R markdown tutorial](https://rmarkdown.rstudio.com/lesson-1.html)


## Lab server

To connect to the lab server, we need to be either on campus or use `GlobalProtect` VPN to connect to LSU intranet. The ip address is 130.39.115.238. To get access to it, we can use Terminal (`ssh user@130.39.115.238`) or go to your browser and enter http://130.39.115.238:8787/ (or http://lsb-125-srv.lsu.edu:8787/) then login with your information.

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
echo 'options(servr.daemon = TRUE, repos = c(rstudio_binary = "https://packagemanager.rstudio.com/all/__linux__/focal/latest"))' > .Rprofile
```



## Library resource

For some reason, I still cannot download articles directly from webpages even using the LSU VPN. Instead, I found that it is possible to replace the first part of the URL to get access to full text. Here is a list that I accumulated:

- List of databases from LSU library: https://login.libezp.lib.lsu.edu/menu
- Links with doi: https://doi-org.libezp.lib.lsu.edu/
- jstor links: https://www-jstor-org.libezp.lib.lsu.edu 
- Science: https://www-sciencemag-org.libezp.lib.lsu.edu or http://www.sciencemag.org.libezp.lib.lsu.edu 
- Nature: https://www-nature-com.libezp.lib.lsu.edu
- Royal Society Publishing: https://royalsocietypublishing-org.libezp.lib.lsu.edu/
- Wiley: https://onlinelibrary-wiley-com.libezp.lib.lsu.edu
- Science direct: https://www-sciencedirect-com.libezp.lib.lsu.edu
- U Chicago Press: https://www-journals-uchicago-edu.libezp.lib.lsu.edu/ 
- Springer: https://link-springer-com.libezp.lib.lsu.edu
- Cell press: https://www-cell-com.libezp.lib.lsu.edu
- PNAS: https://www-pnas-org.libezp.lib.lsu.edu
- Web of Science: https://apps-webofknowledge-com.libezp.lib.lsu.edu/WOS_GeneralSearch_input.do?product=WOS&search_mode=GeneralSearch&SID=8F8swBPcvR4AyxiPidm&preferencesSaved=
- Annual Reviews: https://www-annualreviews-org.libezp.lib.lsu.edu/action/showJournals
- ProQuest dissertations: https://search-proquest-com.libezp.lib.lsu.edu/?accountid=12154


## Collaboration

I do not need to be coauthor on every manuscript coming out of the lab, and I encourage students to research and publish independently of me. That being said, research using lab resources may be more suitable for my coauthorship, and I am happy to actively contribute to the project, or to allow the student to work independently. I also encourage students to collaborate with other scientists within LSU and outside. However, new collaborations should be discussed with me before students initiate them (if possible). 


## University Authorization Process

If you need to get permission to drive a university vehicle, you need to [get authorization first](https://lsu.edu/riskmgt/vehicleuse/lsuam_vehicleuseprocedures.php).

## Keys

[Request keys here](https://sites01.lsu.edu/faculty/biosci/work-request/). In the 'Purpose of Request' row, select 'Key Request'.