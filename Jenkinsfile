pipeline {
    agent {label 'ubuntu-slave'}

    stages {
        stage('git') {
            steps {
                git branch: 'main', url: 'https://github.com/dayanandgowda222/java.git'
            }
        }
        stage('java') {
            steps {
                sh '''javac demo.java
                      java demo'''
            }
        }
    }
}
