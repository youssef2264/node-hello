pipeline {
    agent any
    tools { 
        nodejs 'nodejs' 
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }
	    
	  stage ('Build') {
            steps {
                sh 'npm clean package'
            }
        }
    }
}
