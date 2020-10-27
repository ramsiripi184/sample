pipeline {
    agent any
    tools {
        maven 'maven'
        jdk 'java'
    }
    stages {
        stage('git clone') {
            steps {
                echo 'git cloning'
                git 'https://github.com/rangareddy7/test.git'
            }
        }
        
         stage('build') {
            steps {
                echo 'code building'
                bat 'mvn clean'
                bat 'mvn install'
            }
        }
    }
}
