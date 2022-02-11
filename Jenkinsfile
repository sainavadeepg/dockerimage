node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'Dockerhub') {

        def customImage = docker.build("sainavadeep/dockerapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
