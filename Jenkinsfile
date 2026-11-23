pipeline {
    agent any

    tools {
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/chrifsmaya11/chrifsmaya.git'
            }
        }
        stage('Build Maven') {
            steps {
                sh 'mvn compile'
            }
        }
    }
}
