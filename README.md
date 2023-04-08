# How long do Leighton courthouse judges take to dispose of murder cases?
## by Joe Mahr/ Chicago Tribune

This analysis is one of several for a project the Chicago Tribune is doing on delays in the Cook County court system. It uses [R](https://www.r-project.org/) code, with source data from the Cook County State’s Attorney’s office which is updated several times a year. (Here’s a [nice primer](https://www.cookcountystatesattorney.org/about/open-data) on its data.) This analysis uses data published by that office on 1/23/2023. If you run this code with future files, you should expect different results.

I've included an R project file (Measuring_judges.Rproj) that walks you through the code. There's also rmd and html versions, if you prefer. It may simply be easier to download a zip file of this entire repository and work from your computer. (Side note: I'm a relative Github newbie, so I may be making rookie mistakes in how I upload these files. Apologies in advance.)

### **Getting the data**
This is all explained in the project, rmd and html files, but a quick recap.

The biggest thing is getting the raw data. Github doesn't allow hosting huge datasets -- and these are huge. I've stuggled finding ways to finagle them through Large File Storage. So you'll need to create a folder called raw_data in your working directory, and then put four files in there. You can get all four through [this Google Drive folder](https://drive.google.com/drive/folders/14ZmsHEKsgEgV64EnfvKtDNzAYwLxFeVq?usp=share_link).

### **Preparing/ crunching the data**

Again, there's more detail in the actual project, rmd and html files, but the gist is taking the states' attorney data, and measuring how long a case took, depending on which judge it was. We're taking the median of all those cases, from 2015 through 2022 (so there's a good chunk before the pandemic). In fairness to judges, we're measuring from a listed *arraignment* date, not an arrest date, because that's when the so-called "trial" judge first gets assigned the case. And because of limitations in the data, we limited this analysis to just veteran judges at the main courthouse. (More is explained in the project files.) There's also a Final_data folder with results, if you'd prefer just that. 

### **Questions/ comments?**

Contact Joe Mahr at jmahr@chicagotribune.com
