#Cloud Foundry Hands-On Lab

##Prerequisites

Needless to say you'll need a laptop! Any OS is fine, but make sure to install the following prior to the session:

- [Git](http://git-scm.com/downloads) or "brew install git"

- The `cf` CLI from [https://github.com/cloudfoundry/cli#downloads] (https://github.com/cloudfoundry/cli#downloads) - download the latest version that is appropriate for your laptop and follow the instructions in README.txt. 
<p>
OR 
<p>
from [http://docs.cloudfoundry.org/devguide/installcf/install-go-cli.html](http://docs.cloudfoundry.org/devguide/installcf/install-go-cli.html).

- A Cloud Foundry instance, either [running on your laptop](https://github.com/cloudfoundry/bosh-lite) (16GB of laptop RAM recommended) or a hosted instance

- The labs from [https://github.com/ragsns/javaone-cloudfoundry-hol](https://github.com/ragsns/javaone-cloudfoundry-hol) installed **locally** either via a `git clone` command or by downloading a zip file from the remote repository.

During the live HOL we will help you with a sandbox environment (the details are below). If you are trying these exercises by yourself, we want to provide you choices for deployment. We've done limited testing of the exercises on multiple instances.


- [https://console.ng.bluemix.net/] (https://console.ng.bluemix.net/)
- [https://run.pivotal.io/](https://run.pivotal.io/)
- [http://www.anynines.com/] (http://www.anynines.com/)


##Samples and General Directions

Each directory is in a separate sub-directory. ***Ensure that you're in the sub-directory when you're working on a particular exercise and you're issuing the CLI commands from the subdirectory pertaining to the exercise.***

We've also provided a choice of samples. The **instructions will refer to the PCF-demo sample application** but they can be applied to the NodeJS app. or other Java apps as well.


##Recommended Exercises - User Related

It is recommended that you run through these exercises sequentially since they are progressive with some dependencies. Each exercise should take about 5-10 mins. to complete.

- Exercise 1: [Target the Cloud Foundry Instance](exercises/ex1)
- Exercise 2: [Push your application] (exercises/ex2)
- Exercise 3: [manifest.yml and more CLI commands] (exercises/ex3)
- Exercise 4: [Connect to a service] (exercises/ex4)
- Exercise 5: [Scale your application] (exercises/ex5)
- Exercise 6: [Health Monitoring] (exercises/ex6)
- Exercise 7: [Draining logs] (exercises/ex7) 
- Exercise 8: [Blue/Green Deploy] (exercises/ex8) [Advanced]
- Exercise 9: [Jenkins Integration](exercises/ex9) [Advanced]
- Exercise 10: [Using the Eclipse IDE Plugin](exercises/exa) [Advanced]
- Exercise 11: [Cloud Foundry Application Interoperability](exercises/exb) [Advanced]
- Exercise 12: [Rapid Deployment with JRebel] (exercises/exc) [Advanced]
- Exercise 13: [Monitoring with New Relic] (exercises/exd) [Advanced]
- Exercise 20: [Polyglot Adventures] (exercises/exl) [Advanced]
- Exercise 30: [Microservices Adventures] (exercises/exm) [Advanced]


##More Resources

Plenty of samples in multiple languages at [https://github.com/cloudfoundry-samples] (https://github.com/cloudfoundry-samples)

More samples at [https://github.com/Stackato-Apps] (https://github.com/Stackato-Apps)

##Contact

Please contact us on Twitter @ragss or @bcferrycoder.
