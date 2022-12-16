pipeline {
    agent any
 
    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "M3"
    }
 
    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/violetadfs/proyectofinalvioleta.git
                 sh 'mvn -B -DskipTests clean package'
                // Run Maven on a Unix agent.
 
                // To run Maven on a Windows agent, use
                // bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }
        }
    }
}
