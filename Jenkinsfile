pipeline {
    agent any
    stages {
        
        stage('Jenkins Pipeline Hello World') {
            steps {
              sh 'echo '"Hello World"'
            }
        }
        
        stage('pull from GitHub') {
          steps {
            git 'https://github.com/AmareshACS/python-sample.git' 
            }
        }
        
        stage('Build with Maven') {
          steps {
            mvn compile test package
            }
        }
    }
}
