pipeline {
     agent any
         stages {
             stage('One') {
                 steps {
                      script {
                          env.EXECUTE="True"
                      }
                 }
             }
               stage('Two') {
                   when {
                      environment name: 'EXECUTE', value: "True"
                    }
                 steps {
                     sh ' echo "Updating Second Stage" '
                 }
             }
              stage('Three') {
                   when {
                      environment name: 'EXECUTE', value: "True"
                   }
                 steps {
                     sh ' echo "Updating Third Stage" '
                 }
             }
         }
 }
