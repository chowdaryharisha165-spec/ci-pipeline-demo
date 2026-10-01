pipeline {
     agent any

stages {
    stage('Checkout') {
            steps {
                echo 'Checking out code...'
           }
      }
      stage('Bulid') {
            steps {
                echo 'Buliding and Validating python applications...'
                sh 'python3 -m py_compile app.py'
            }
        }
        stage('Test') {
             steps {
                 echo 'Running tests...'
                 sh 'python3 -m unittest -v test_app.py'
             }
        }
        stage('Validation') {
              steps {
                 echo 'Validation stage completed successfully!'
            }
        }
    }
 }
