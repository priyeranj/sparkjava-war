pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }
    stages {
        stage('git clone') {
            steps {
                git url: 'https://github.com/priyeranj/sparkjava-war.git', branch: 'main'
                    
            }
        }
        
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
