pipeline {
    agent {
        stage("maven-build") {
	sh '''
           mvn -Dmaven.test.failure.ignore clean package
        '''
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -Dmaven.test.failure.ignore clean package' 
            }
        }
    }
}
