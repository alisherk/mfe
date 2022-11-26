# Deployment notes 
- Location of child app remoteEntry.js must be known at build time 
- Many front-end deployment solutions assume you are deploying a single project
- need CI/CD pipeline of some sort 
- at present, the remoteEntry.js file is fixed. Need to think about caching issues

# Workflow
- whenever code is pushed to master and commit contains a change to the container 
- change into the container folder
- install deps 
- create prod build using webpack 
- upload the result to AWS S3