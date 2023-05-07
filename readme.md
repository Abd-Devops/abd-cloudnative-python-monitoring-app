Name : Deploy Cloud Native Monitoring Application on Kubernetes




AWS Commands
----------------
1. aws configure                   //to authenticate the cli by providing key and secret
2. aws iam list-users              // to list the users

794977028651.dkr.ecr.us-west-2.amazonaws.com/my_monitoring_app_image2

Python Commands
---------------
1. pip3 install -r requirement.txt OR Pip install <module name>            //if any moduel is missing run this command to get the dependecies 
2. python --version                                                        // To check the python versoin
3. python ecr.py                                                           // To run python files 



Docker
--------------
1. docker build -t my-flask-app-2 .         //to build an image out of docker file (. docker file is in a current directory)
2. docker images                            //Shows available images
3. docker run -p 50000:50000 <imagename>    // to run the container out of docker image 
4. docker container ls                      //lists the running container
5. docker rm -f <container Id>              //To remove/kill any container using container id
6. docker rmi <imagename:taganame>          //To remove image from repo. tag name is optional
7. docker tag my-flask-app 794977028651.dkr.ecr.us-west-2.amazonaws.com/my_monitoring_app_image:latest


Boto4
-----------------
1. aws ecr get-login-password --region us-west-2 | docker login --username AWS --password-stdin 794977028651.dkr.ecr.us-west-2.amazonaws.com/my_monitoring_app_image

