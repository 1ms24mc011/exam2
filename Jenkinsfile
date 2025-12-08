pipeline {
  agent any
  triggers {
    pollSCM("* * * * *")
  }

  stages {
    stage ("git-connect") {
      steps {
        git branch:'master', url:'https://github.com/1ms24mc011/exam2/'
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
