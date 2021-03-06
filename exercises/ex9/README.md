#Cloud Foundry Hands-On Labs

##Exercise 9: Jenkins Integration

a. Fork the repository [https://github.com/ragsns/PCF-demo] (https://github.com/ragsns/PCF-demo) on github.

b. Install Maven and Jenkins locally on you laptop. Once Jenkins is installed you can access the console at [http://localhost:8080] (http://localhost:8080) 

c. Install the Cloud Foundry plugin by clicking on `Manage Jenkins` in the console and by clicking on the appropriate tabs and searching for the plugin.

d. Create a new workspace called PCF-demo in Jenkins and Configure the project. Substitute the appropriate values for the GitHub URL below.

1. Pick `Git` for Source Code Management.
2. Provide the repository URL (in my case it is `https://github.com/ragsns/PCF-demo/`. Provide the URL of the forked repository)
3. Check off when a `Build when a change is pushed to GitHub`
4. Check off `Poll SCM` and provide the value `H/2 * * * *` in the `Schedule` which indicates poll the repository every 2 mins.
5. In `Build/Execute shell/Command` provide the command to build the project which is `mvn clean package`
6. In the `Post-build Actions/Push to Cloud Foundry` provide the credentials, organization and space and test it.
7. Check the `Reset app if already exists`.
8. Save the project

You can also create services if you want but we will skip that for now.

Change the manifest.yml (**make sure you substitute the UNIQUE below to something unique such as your name**) to

```
---
applications:
- name: pcfdemo
  memory: 300M 
  instances: 1
  host: pcfdemo-UNIQUE
  path: ./target/pcfdemo.war
  env:
   JAVA_OPTS: -Djava.security.egd=file:///dev/urandom
```
Stage this file and push it via the `git` command.

Pushing this will trigger a Jenkins build. If not do a `Build Now` manually in the Jenkins UI. If the build fails, rinse and repeat!

That's all there is to Jenkins integration!
