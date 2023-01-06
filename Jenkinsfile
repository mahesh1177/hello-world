pipeline {
    agent any
    environment {
        PATH="/opt/apache-maven-3.8.7/bin:$PATH"
    }

    stages {
        stage('SCM') {
            steps {
                git 'https://github.com/mahesh1177/hello-world.git'
            }
        }
        stage('BUILD') {
            steps {
                sh "mvn package"
            }
        }
    }
}
