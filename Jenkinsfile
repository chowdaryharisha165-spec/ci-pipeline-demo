pipeline {
     agent any
  stages {
     stage('Checkout') {
          steps {
              echo 'Checking out repository code...'
              checkout scm
           }
        }
        stage('Bulid') {
             steps {
                 echo 'Validating application...'
                 sh 'python3 -m py_compile app.py'
              }
           }
           stage('Test') {
                steps {
                     echo 'Running Code Validation...'
                     sh 'python3 -c "import app; print(\'Validation Stage Completed Successfully!\')"
}
}
}
