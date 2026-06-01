pipeline {

    agent any
    tools {
        maven 'Maven'
        jdk 'JDK25'
    }
    stage('Check Java') {
        steps {
            sh 'java -version'
            sh 'echo $JAVA_HOME'
        }

        stages {
            stage('Build') {
                steps {
                    sh 'mvn -B -DskipTests clean install'
                }
            }
        }
    }
}