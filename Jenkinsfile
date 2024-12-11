pipeline {
    agent {
        label "jenkins-agent"
    }
    tools {
        jdk 'Java17'
        maven "Maven3"
    }
    stages {
        stage("Clenup Workspace") {
            steps {
                cleanWs()
            }
        }
        stage("Checkout from SCM") {
            steps {
                git branch: 'main',  url: 'https://github.com/knovellcloud/complete-prodcution-e2e-pipeline'
            }
        }
    }
}