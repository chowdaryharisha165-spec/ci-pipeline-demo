pipeline {

  ageent any
 stages {
     stage('Checkout') {
         steps {
            checkout scms
          }
       }
       stage('Bulid') {
           steps {
              echo 'Validating code compilation...'
              sh 'python3 -m py_complie app.py'
            }
          }
          stage('Test') {
               steps {
                   echo 'Running Unit Tests...'
                   sh 'pytest test_app.py'
                }
              }
              stage('Validation') {
                    steps {
                        echo 'Running code Validation...'
                        sh 'python3 -c "import app; print(\'Validation Stage Completed Successfully
                     }
                 }
             }
