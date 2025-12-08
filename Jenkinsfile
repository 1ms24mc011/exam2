pipeline {
  agent any
  triggers{
    POLLSCM: ("* * * * *")
  }

  stages {
    stage ("check python version") {
      steps {
        sh 'python3 --version'
      }
    }

    stage ("run the code") {
      steps {
        sh "python3 code.py"
      }
    }
    
  }
}
