for the Prisma Cloud NoteMaker simple demo
Steps to setup for demo:
1. add ./scripts to your PATH
2. fill in credentials and URL's into scripts/setup* scripts
3. source proper script   $ source setupEnvSaaS (or setupEnvSelfHosted) 
4. for CI/CD go to notemaker/build and run buildReleaseAll without options to see usage
5. for deployment go to notemaker/deploy and run any of the scripts in notemaker/deploy/scripts
   (run them from notemaker/deploy folder)
   first one would be 'initialDeploy'
   again, run script without any parameters to see usage
6. Container focused pen tests are in notemaker/pentest, check README.md file at that location 
 

 
