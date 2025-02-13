pipeline {
    agent any

    tools { 
        jdk 'JAVA_HOME' 
        maven 'M2_HOME' 
    }

    stages {
        stage('GIT') {
            steps {
                git branch: 'main', url: 'https://github.com/MeryemBoukraa/DevOps.git'
            }
        }

        stage ('Compile Stage') {
            steps {
                sh 'mvn clean compile'
            }
        }
    }
}
