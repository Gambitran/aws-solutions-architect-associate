## EC2 User Data

* Bootstrap instance using user data script
* Bootstrapping means launching commands when a machine starts
* Script only <b>run once</b> at instance on <b>first start</b>
* Examples of automated boot tasks such as:
  * Installing updates
  * Installing software
  * Downloading common files from internet
  * Anything you can think of
* User data script runs with root user