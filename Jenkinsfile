pipeline {

    agent any
    tools {
        maven 'Maven'
        jdk 'JDK25'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean install'
            }
        }
    }

}