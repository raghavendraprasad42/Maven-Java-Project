pipeline {
    agent { label 'buildserver'}

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "maven3.6"
    }

    stages {
        stage('Prepare-Workspace') {
            steps {
                // Get some code from a GitHub repository
                git credentialsId: 'github-server-credentials', url: 'https://github.com/raghavendraprasad42/Maven-Java-Project.git'    
	    }
	}
    }
}
