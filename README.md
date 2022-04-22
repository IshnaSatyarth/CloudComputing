The objective of this assignment is for you to demonstrate the ability to go all the way from source code to a/an application deployed in the cloud via CI/CD processes. Additionally we have some requisite lab assignments.
 
Everything you need for Items 1 through 5, we have done collectively together in class and made the code available in our repository (including notes and commands).
 
(1) Create a public repository in Github with your application code. [5 points]
Deliverables: A link to the repository that can be accessed publicly without authentication. The repo must contain the code for some application - it could be anything that you have written, or it could even be our simple webserver code - all I ask if you use the simple webserver code is that you modify it in some way (maybe the basic page includes your name or something).


 
(2) Include a Dockerfile to package your application up to run as a container [5 points]
Deliverables: The Dockerfile must be part of your repository such that I can just clone the repository and run docker build to build the image successfully.
 
(3) Setup a workflow to build your application via Cloudbuild upon checkins [20 points]
Deliverables: Your workflow is part of your repository so I should be able to see it. And clicking on the 'Actions' tab, I should be able to see history of you making checkins (they can be trivial checkins) to kick off the workflow and successfully use Cloudbuild to build the app (this would automatically include submitting the build logs and your image the container registry in your GCP project. Hint: You will need to set up your GCP info correctly (preferably as secrets but I am ok with hardcoding for this assignment). Either way I do not need to see your credentials or GCP info, but I should be able to look at the workflow history (in Actions) and see it running successfully.  
 
(4) Update your workflow to deploy your application to CloudRun as the next step [20 points]
Deliverables: As before, since your workflow is part of the repository, I should be able to see the updated code and I should be able to see the history of you executing this step successfully (in the Actions tab).
 
(5) Have your CloudRun application/service run under a dedicated service account [5 points]
Deliverables: I should be able to see the command in your workflow updated correctly.
 
![image](https://user-images.githubusercontent.com/65250405/164832063-3c1c9080-b9c2-4021-a039-05a602982671.png)
