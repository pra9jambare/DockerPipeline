node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', '0b9cbed6-7bdd-4e39-b918-3fc6b11c8ac0') {

        def customImage = docker.build("pranavjambare/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}