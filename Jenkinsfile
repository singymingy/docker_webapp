  
node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'access2dockerhub') {

        def customImage = docker.build("singymingy86/nginx_hello")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
