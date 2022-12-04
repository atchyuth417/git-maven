pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
		stage('Git') {
            steps {
                echo 'copying from scm'
				git branch: 'main', credentialsId: 'GitCredentials', url: 'https://github.com/atchyuth417/git-maven.git'
            }
        }
    }
}
