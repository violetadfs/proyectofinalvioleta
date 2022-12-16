pipeline {
    agent any

 

   tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "M3"
    }

 

   stages {
        stage('Build') {
            
            steps {
                dir(path:'cidr_convert_api/java/cidr-api/'){
                // Get some code from a GitHub repository
                sh 'echo "this is my building stege"'
                 sh 'mvn -B -DskipTests clean package'
                    }
            }
        }
    }
}
