pipeline {
    agent any
stages 
[
 stages {
    stage('Checkout') {
        steps {
           echo 'Checking out code...'
         }
      }
      stage('Bulid') {
           steps


steps 
{
   echo 'Buliding and Validating Python application...'
   sh 'python3 -m py_complie app.py'
}
}
stages('Test') {
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
