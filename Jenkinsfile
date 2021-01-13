pipeline {
    agent any
    tools {
    maven 'Mave-3.6.3'
    }
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
