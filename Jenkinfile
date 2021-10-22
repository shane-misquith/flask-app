node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub_id') {
        def customImage = docker.build("shanemisquith/jenkins-pipeline")
        customImage.push()
    }
}
