# Lab 1: Your first run. 

## Let's get started!

This guide will show you how to get started with Mayhem using Google Cloud
Shell.

**Time to complete**: About 10 minutes

Click the **Start** button to move to the next step.

## Create a Mayhem account

Create a new account by navigating to 
[training.forallsecure.com](https://training.forallsecure.com) and either choose:
   * Google account: Use your Google account on Mayhem
   * "Sign up": Create a local account on the Mayhem instance. 

![Mayhem Account Creation](https://raw.githubusercontent.com/dbrumley/fuzzing-cloudshell-tutorial/master/assets/images/account-creation.png)


## Log in the CLI

The `mayhem` CLI authenticates to the Mayhem server using an API token. The API
token  is available three places:

   * The [download screen](https://training.forallsecure.com/-/installation)
   * In your profile settings, located in the top-left under your username, then
     "Settings", then "API Tokens".
   * Under the "?" help window. 

Once you get your API token, log in the CLI:

```
mayhem login https://training.forallsecure.com/ <YOUR API KEY>
```

![API Token Locations](https://raw.githubusercontent.com/dbrumley/fuzzing-cloudshell-tutorial/master/assets/images/api-token-locations.png)


## Create a new Project

Let's reproduce an exploit for [lighttpd](https://www.lighttpd.net/)! (version
1.4.15, to be specific).

   * Create a new project by clicking the "plus" icon at the top of the screen.
![Create new project](https://raw.githubusercontent.com/dbrumley/fuzzing-cloudshell-tutorial/master/assets/images/create-new-project.png)
   * Select the Mayhem docker registry, and the play icon next to the
   `forallsecure/tutorial/lighttpd` version 1.14.15
   image. 
![Choose dockerhub
   image](https://raw.githubusercontent.com/dbrumley/fuzzing-cloudshell-tutorial/master/assets/images/project-from-registry.png)

## Configure Analysis

There are two tabs of analysis options: Basic and Advanced. We will be configuring three values:
   1. Under **Basic**, set the analysis to run 30 seconds. If omitted, analysis will run
      forever in continuous fuzz mode. 
   2. Under **Advanced**, enable the **Advanced Triage** option. This option performs additional
      in-depth analysis, and requires `libc6-dbg` installed.
   3. Under **Advanced**, click the **Tasks** button, and enable **Code
      Coverage**.

![Basic configuration](https://raw.githubusercontent.com/dbrumley/fuzzing-cloudshell-tutorial/master/assets/images/basic-configuration-options.png)

![Advanced configuration](https://raw.githubusercontent.com/dbrumley/fuzzing-cloudshell-tutorial/master/assets/images/advanced-configuration-options.png)

   
## Click start run!

Click the start run button at the bottom of your screen to begin analysis!

![Click start
run](https://raw.githubusercontent.com/dbrumley/fuzzing-cloudshell-tutorial/master/assets/images/start-run-button.png)

The run may take a few minutes to complete, as analysis and post-analysis
processing need to finish.

Congratulations!

You've just:
  * Learned how to log into the CLI.
  * Learned how to start a new Mayhem analysis job.
  * Found your first exploitable bug using Mayhem!
  


<walkthrough-conclusion-trophy></walkthrough-conclusion-trophy>
