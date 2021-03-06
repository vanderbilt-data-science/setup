# setup-clinic
Software installation and configuration for new Data Science Master's students 

## Secure Passwords

You'll need to create up to three new passwords today. In order to ensure security for yourself, Vanderbilt systems, and for data you will be entrusted with when you take on projects, you'll want to have strong, unique passwords for each system. I suggest you use a password service. See https://www.cnet.com/news/the-best-password-managers-of-2019/ for an overview of options. 

## GitHub Signup

If you do not already have a GitHub account, please visit https://github.com/ and make one. See https://happygitwithr.com/github-acct.html for advice. 

Visit https://forms.gle/5s6hjFNHCYP8rFtUA and record your GitHub login. You'll be invited to both the Vanderbilt Data Science organization (https://github.com/vanderbilt-data-science) and the Vanderbilt Data Science Master's Program organization (https://github.com/vanderbilt-data-science-masters-program). 

## Computing Cluster Signup

Visit the ACCRE Getting Started page (https://www.vanderbilt.edu/accre/getting-started/) to register for an account. 

Request an account by visiting the ACCRE New Account page (https://www.accre.vanderbilt.edu/?page_id=3563). For Department, select `Data Science Institute`. For School or Affiliation, choose `Trans-Institutional Programs (e.g. Data Science Institute)`. For Group, select `Data Science Institute (p_dsi)`. For primary application, choose `Existing application`. For application, select `Jupyter`. Enter that you anticipate running one job at a time. Indicate your level of Linux experience (if you're not already, you'll be Intermediate by the end of the semester, and Expert by the end of the Master's program!). You can enter `R, Python` for languages, and can leave the rest of the responses unfilled. Answer the Captcha question at the end, and send. 

We'll authorize your access as soon as possible. 

Visit the ACCRE page (https://www.vanderbilt.edu//accre/) for more information about the cluster. We'll be arranging trainings for the class on using the cluster. 

## Linux On Your Desktop (optional)

If you are running MacOS, you already have access to Linux on your machine. If you are running Windows, you can enable Windows Subsystem for Linux. Follow the instructions at https://docs.microsoft.com/en-us/windows/wsl/install-win10. To run PowerShell as administrator (the first step in the documentation), tap the Windows key, then type `powershell`. Select `Run as Administrator` to the right. Continue with the instructions.


## Install R

Download and install R from RStudio's CRAN mirror (https://cran.rstudio.com/). Follow the link for your operating system, and select the latest Base release, which will be 3.6.1 or greater. Once the file is downloaded, install the software.   

Also download and install Rtools if you are on Windows--you will find the link below Base on the list.

## Install RStudio

Download RStudio from the RStudio site (https://www.rstudio.com/products/rstudio/download/#download). Select your operating system, and install the software after download is complete. For Windows, select RStudio 1.2.1335 - Windows 7+ (64-bit). For Mac, select RStudio 1.2.1335 - macOS 10.12+ (64-bit). 

## Install R Packages

Once R and RStudio are download, load RStudio, and copy-paste the following code in the console:

```r
install.packages("tidyverse")
install.packages("janitor")
install.packages("devtools")
install.packages("assertr")
install.packages("Hmisc")
```
## Anaconda

Visit https://www.anaconda.com/distribution/ and click on `Download`. Select your operating system from the icons on the bar on the top of the page (the default is MacOS). Select the 64 bit Graphical Installer. Execute the software once it is downloaded.  

##  Git Install

Visit https://git-scm.com/downloads and select the download for your operating system. Once the software has downloaded, execute it. 

See https://happygitwithr.com/install-git.html for step-by-step guidance. 

Set up your profile for your local git by following the directions at https://happygitwithr.com/hello-git.html. 

## Connecting to GitHub

New installations of git on MacOS and Windows SHOULD make use of built-in authentication so that you will not need to log into GitHub each time you perform an operation on a remote repo. It you find yourself having to sign in to GitHub when pushing or pulling, follow the guidelines at https://happygitwithr.com/connect-intro.html to set up caching or SSH keys. 

If you are on a Mac, and are not able to access git from RStudio, execute the following commands from with a terminal window:

xcode-select --install  
sudo xcode-select -switch /Library/Developer/CommandLineTools

## Testing Out Git/GitHub/RStudio

To test out whether RStudio is integrated with git on your computer, we will clone the repository locally to your computer. 

Click on the green "Code" button on this page, and copy the web URL listed there. Start up RStudio, click on 'File' on the menu, select 'New Project', the click on 'Version Control', 'Git', and paste the URL into the Repository URL field. If this repo is downloaded as an R project, your integration has worked. If not, e-mail us to let us know (go ahead and e-mail jesse.spencer-smith@vanderbilt.edu, and we'll get you sorted out). 

## TopHat Setup

Vanderbilt University has a site license for TopHat (https://www.vanderbilt.edu/tophat/). Take a few minutes and set up a student account. 

## Printer Setup

The printer in the DSI common is available for your use. It is \\print.it.vanderbilt.edu\DSI_Engineering_300. 

To add the printer on a Mac, follow these  [directions](https://github.com/vanderbilt-data-science-masters-program/setup/blob/master/dsi_printer_setup_mac.md).

To add a printer on a Windows machine, follow these 
[directions](https://github.com/vanderbilt-data-science-masters-program/setup/blob/master/dsi_printer_setup_windows.md).

## Building Tour

Take a walk and learn about the home of the Data Science Institute! Information on our LEED Gold-certified home is at https://www.vanderbilt.edu/esb/. 

## Slack

You should have received an invitation to join our Slack team, https://vandydatasciencems.slack.com. If you've note alread done so, downloading the Slack phone app lets you keep up-to-date: https://slack.com/downloads/ios or https://slack.com/downloads/android. You can set your notifications by mention, or by any activity in a particular channel. 

## Coffee Maker, Ice Maker, Filtered Water

As a DSI student, you have free access to the coffee machine in the common kitchen area. It is a Jura Impressa S9, and the operating manual is here https://us.jura.com/en/homeproducts/machines/IMPRESSA-S9-Classic-UL-13674/Manuals. 

The coffee maker can make extra hot water to make tea! The control is on the right-hand side--be sure to set it for exra-hot. 

The ice maker is available for your use. The water reservoir can be refilled using the cold water from the tap. The cold water line is filtered. 


