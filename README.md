**Documentation**

**Output:**

The website shows the calculation operation outputs in Json format.

After updation, Application is successfully updated for SIT737 Task 6C! by using url "http://localhost:3020/".

**Steps:**

Firstly, download Git from Git official website "https://git-scm.com/", and confirm the download by checking the version of Git.

Now pull the previous week's code from the  repostiory "https://github.com/vivekolladapu/sit737-2025-prac6p".

Now, the yaml files are already created.

The project structure should as mentioned below:

sit737-2025-prac6c |-- kubernetes-configs ||--(deployment.yaml) ||--(service.yaml) |--node_modules |--logs | |--(combined.log) | |--(error.log) |--server.js |-Dockerfile |--docker-compose.yml |--package.json |--package-lock.json |--README.md

Now build and push the image.

After pushing, check the current context by using "kubectl config current-context", and chnage it to "docker-desktop" by using "kubectl config use-context docker-desktop".

Now, create the deployment.yaml and service.yaml to deploy the application to kubernetes cluster by using "kubectl apply -f kubernetes-configs/".

Now, check the pods, services and svc.

After checking, forward the port traffic to access the application.

Now test the website and its operations.

Now, make changes to the server.js code. In this project, the get method is added at "/" endpoint, in whicb it prints "Application is successfully updated for SIT737 Task 6C!".

Now, build the new image by changing the version tag to v2 and push it.

Now, change the image version in the deployment.yaml file.

Now, delete the previously created depployments and services by using "kubectl delete -f kubernetes-configs/" and create it again.

Now, check the pods, service and svc.

Now, forward the port traffic to access the updated website.

Test the updated website and operations of it.





