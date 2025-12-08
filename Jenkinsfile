pipeline {
  agent any
  triggers {
    pollSCM("* * * * *")
  }

  stages {
    stage ("check python version") {
      steps {
        sh 'python3 --version'
      }
    }

    stage ("run the code") {
      steps {
        echo "Runnning..."
        sh "python3 code.py"
      }
    }
    
  }
}
