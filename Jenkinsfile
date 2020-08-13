  
node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', '04fa0f8f-1a8b-4fc9-a8b4-60badacb4202') {

        def customImage = docker.build("singymingy86/nginx_hello")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
