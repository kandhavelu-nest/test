pipeline {
agent any
    stages {
        stage('git') {
                         steps {
        git url:'git@github.com:kandhavelu-nest/test.git', branch:"${BRANCH_NAME}", credentialsId: 'web-app-ssh-key'
      }
        }
        stage('Test') {
                         steps {
        sh """
        ls -la
		echo " dev request branch"
		sleep 100
        """
      }
        }
    }
}
