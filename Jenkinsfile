pipeline {
    agent any
        stages {
            stage('First') {
                steps {
                    script {
                        env.EXECUTE="True"
                    }
                }
            }
 
 
            stage('Second') {
                when {
                    env1roment name: 'EXECUTE', value: "True"
                }
                steps { 
                    sh ' echo "updating Second Stage" '
              }
            }
 

            stage('Third') {
                when {
                    env1roment name: 'EXECUTE', value: "True"
                }
                steps { 
                    sh ' echo "updating Third Stage" '
              }
            }
        }
}
