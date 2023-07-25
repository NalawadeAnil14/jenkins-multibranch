pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo "Hello"
      }
    }

    stage('fix1') {
      when {
        branch 'fix'
      }

      steps {
        echo "Only for fix branch"
      }
    }

    stage('PR') {
      when {
        branch '"PR-*"'
      }

      steps {
        echo "When PR is created"
      }
    }
  }
}
