# DevOps-Docker-practice
Homework for KPI DevOps subject by Yevhenii Borysenko

After creating an app we must build an image of it with

    docker -t evgeny2411/Devops-nodeapp .

It runs succsesfully and now we can push our image to docker hub

    docker push evgeny2411/devops-nodeapp

Now when image is on hub we can run it on machine with special restrict on CPU and memory using keys --memory and --cpus

    docker run -p 8080:8080 --cpus=".5" --memory="150m" evgeny2411/devops-nodeapp

That's all. We can see working HTML page.
