Build: This phase of the pipeline pulls the environmint variables into the application and then installs node 14.0. The front end and back end dependencies are installed. The front end is linted. Finally, the front end and api are built through the build scripts in their respective package.json files.

Hold: I as the account manager have to approve the next phase of deployment.

Deploy: Similar to build, this phase first prepares the environment variables and installs node 14.0. Then the Elastic Beanstalk and AWS CLIs are installed and set up as they are used in later scripts. AWS does not work without an AWS Access Key ID, created through IAM and set through environment variables, so the next step is to configure this access key ID. Finally, the code on both frontend and backend is deployed!
