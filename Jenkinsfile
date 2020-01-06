pipeline {
    agent {
        label "vm"
    }
    stages {
        stage("Invoking guix system docker-image") {
            steps {
                sh "guix system docker-image docker-image.tmpl"
            }
        }
    }
    post {
        always {
            sendNotifications currentBuild.result
        }
    }
}
