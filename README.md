# setup-clinic
Software installation and configuration for new Data Science Master's students 

## Secure Passwords

You'll need to create up to multiple new passwords today. In order to ensure security for yourself, Vanderbilt systems, and for data you will be entrusted with when you take on projects, you'll want to have strong, unique passwords for each system. I suggest you use a password service. See https://www.pcmag.com/picks/the-best-password-managers for an overview of options. 

## GitHub Signup

If you do not already have a GitHub account, please visit https://github.com/ and make one. See https://happygitwithr.com/github-acct.html for advice. 

Fill in the [DSI Master Student Account Information Form](https://forms.gle/5s6hjFNHCYP8rFtUA) and record your GitHub login. 

You'll be invited to both the Vanderbilt Data Science organization (https://github.com/vanderbilt-data-science) and the Vanderbilt Data Science Master's Program organization (https://github.com/vanderbilt-data-science-masters-program). 




## Anaconda

Visit [https://www.anaconda.com/distribution/](https://www.anaconda.com/download) and enter your email. Select your operating system from the icons on the bar on the top of the page (the default is MacOS). Select the 64 bit Graphical Installer. Execute the software once it is downloaded.  

##  Git Install

Visit https://git-scm.com/downloads and select the download for your operating system. Once the software has downloaded, execute it. 

See https://happygitwithr.com/install-git.html for step-by-step guidance. 

Set up your profile for your local git by following the directions at https://happygitwithr.com/hello-git.html. 

## Connecting to Git via SSH keys

Past methods used passwords to connect to github via the CLI. SSH keys provide a more secure connection to GitHub over unsecured networks. Please follow the instructions below to create an SSH key and add it to GitHub.  

1. Open a new terminal/bash shell
2. Type in the following command to create a new ssh key: ssh-keygen -t ed25519 -C "your_email@example.com"
   This creates a new SSH key, using the provided email as a label.
   When you're prompted to "Enter a file in which to save the key", you can press Enter to accept the default file location.  Please note that if you created SSH keys previously, ssh-keygen may ask you to rewrite another key, in which case we recommend creating a custom-named SSH key. To do so, type the default file location and replace id_ALGORITHM with your custom key name.
3. Navigate to where you just saved your new SSH key ``` cd ~/.ssh```
4. Open the ```id_ed25519.pub``` file (```cat id_ed25519.pub```). Copy the resulting output. It should look something like ```ssh-ed25519 AAHFBSJ287t....```
5. Navigate to GitHub settings > SSH and GPG Keys: https://github.com/settings/keys
6. Click "New SSH Key"
7. Give your key a useful title and paste in your SSH key .pub file contents.
8. Add your SSH key. You can now use GitHub using your machine from the command line. 

## OpenAI ChatPlus 

You will need a ChatPlus (paid) subscription to OpenAI. This will be the equivalent of a textbook for many or your courses. Go to the [OpenAI main page](https://openai.com/). 
- Select Sign Up in the upper right corner.
- Put in your Vanderbilt address, select continue.
- Choose a secure password.
- Enter in your payment information 

## Linux On Your Desktop (optional)

If you are running MacOS, you already have access to Linux on your machine. If you are running Windows, you can enable Windows Subsystem for Linux. Follow the instructions at https://docs.microsoft.com/en-us/windows/wsl/install-win10. To run PowerShell as administrator (the first step in the documentation), tap the Windows key, then type `powershell`. Select `Run as Administrator` to the right. Continue with the instructions.


## Printer Setup  **Skip for now**

The printer in the DSI common area  is available for your use. It is \\print.it.vanderbilt.edu\DSI_Engineering_300. 

To add the printer on a Mac, follow these  [directions](https://github.com/vanderbilt-data-science-masters-program/setup/blob/master/dsi_printer_setup_mac.md).

To add a printer on a Windows machine, follow these 
[directions]https://github.com/vanderbilt-data-science/setup/blob/master/dsi_printer_setup_windows.md).

## Building Tour

Take a walk and learn about the home of the Data Science Institute!  

## Slack

You should have received an invitation to join our Slack team, https://vandydatasciencems.slack.com. If you've note alread done so, downloading the Slack phone app lets you keep up-to-date: https://slack.com/downloads/ios or https://slack.com/downloads/android. You can set your notifications by mention, or by any activity in a particular channel. 

Be sure that you're also in the Data Science TIP Slack organization which is our main Slack org for data science work: https://datasciencetip.slack.com/ .

## Coffee Maker, Ice Maker, Filtered Water

As a DSI student, you have free access to the coffee machine in the common kitchen area. It is a Jura Impressa S9, and the operating manual is here https://us.jura.com/en/homeproducts/machines/IMPRESSA-S9-Classic-UL-13674/Manuals. 

The coffee maker can make extra hot water to make tea! The control is on the right-hand side--be sure to set it for exra-hot. 


## Install R

Download and install R from RStudio's CRAN mirror (https://cran.rstudio.com/). Follow the link for your operating system, and select the latest Base release, which will be 4.2.1 or greater. Once the file is downloaded, install the software.   

Also download and install Rtools if you are on Windows--you will find the link below Base on the list.

### Install RStudio

Download RStudio from the RStudio site (https://www.rstudio.com/products/rstudio/download/#download). Select your operating system, and install the software after download is complete. For Windows, select RStudio RStudio-2022.07.1-554.exe. For Mac, select RStudio-2022.07.1-554.dmg. 

### Install R Packages

If you are running Windows, install Rtools so that you can compile the necessary packages as needed. Go to https://cran.r-project.org/bin/windows/Rtools/ and download the 64 bit version. Click on the file after it downloads to install. When you are finished, copy the code below and paste it into the Console of RStudio. 

```r
install.packages("tidyverse")
install.packages("tidymodels")
install.packages("janitor")
install.packages("devtools")
install.packages("assertr")
install.packages("Hmisc")
```
### Connecting R to GitHub

New installations of git on MacOS and Windows SHOULD make use of built-in authentication so that you will not need to log into GitHub each time you perform an operation on a remote repo. It you find yourself having to sign in to GitHub when pushing or pulling, follow the guidelines at https://happygitwithr.com/connect-intro.html to set up caching or SSH keys. 

If you are on a Mac, and are not able to access git from RStudio, execute the following commands from with a terminal window:

xcode-select --install  

sudo xcode-select -switch /Library/Developer/CommandLineTools

### Testing Out Git/GitHub/RStudio

To test out whether RStudio is integrated with git on your computer, we will clone the repository locally to your computer. 

Click on the green "Code" button on this page, and copy the web URL listed there. Start up RStudio, click on 'File' on the menu, select 'New Project', the click on 'Version Control', 'Git', and paste the URL into the Repository URL field. If this repo is downloaded as an R project, your integration has worked. If not, e-mail us to let us know (go ahead and e-mail jesse.spencer-smith@vanderbilt.edu, and we'll get you sorted out). 

## VS Code Download
You'll be using VS Code for your first year programming course. You can [install VS Code](https://code.visualstudio.com/download) using the Download button for your system on this page.

## Huggingface Account
We'll be exploring the latest in AI architectures and approaches during the bootcamp. For this, you'll need a Huggingface account. The free account is sufficient. Sign up at [Huggingface.co](https://huggingface.co) using the Sign Up button at the top of the screen.
