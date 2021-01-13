pipeline {
    agent any
    stages {
        stage("SCM_checkout") {
            steps {
                git credentialsId: 'github_ID', url: 'https://github.com/Kubernetesjigalooru/spring-boot-mongo-docker.git'
            }
        }
	stage("Build_Artifact") {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
