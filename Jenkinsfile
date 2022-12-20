pipeline {
    agent any
}
stage('Build') {
            steps {
               'https://github.com/violetadfs/proyectofinalvioleta.git'
            }
        }
 stage('SonarCloud Static Analysis') {
            steps {
                script {
                    withSonarQubeEnv ('SonarCloud') {
                        sonar-scanner.bat \
                            -D"sonar.organization=violetadfs" \
                            -D"sonar.projectKey=violetadfs_proyectofinalvioleta" \
                            -D"sonar.sources=proyectofinalvioleta/Jenkinsfile.\
                            -D"sonar.host.url=https://sonarcloud.io"
                      }
                    }
                }
     }
