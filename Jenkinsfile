pipeline {
    agent { docker 'python:3.5.1' }
    stages {
        stage('deploy') {
            steps {
                retry(3){
                     sh 'echo "Hello World"'
                }
               timeout(time:3, unit: 'MINUTES'){
                    sh 'python --version'
               } 
               sh 'printenv'
            }
        }
    }
}
