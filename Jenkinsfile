pipeline {
    agent { docker 'maven:3.3.3' }
    stages {
        stage('Build') {
            steps {
		sh 'mvn --version'
		sh 'docker -v'
                sh 'echo "Hello World"'
		sh '''
		    echo "Multiline shell steps works too"
		    ls -lah
		    pwd
		'''
		sh 'printenv'
            }
        }
    }
}
