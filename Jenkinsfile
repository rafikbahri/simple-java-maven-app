pipeline {
  agent any
  stages {
    stage('SHUTTLE-BUILD') {
      steps {
        echo 'SHUTTLE-BUILD'
      }
    }
    stage('SHUTTLE-DEP-REDHAT') {
      parallel {
        stage('SHUTTLE-DEP-REDHAT') {
          steps {
            echo 'SHUTTLE-DEP-REDHAT'
          }
        }
        stage('SHUTTLE-DEP-DEBIAN') {
          steps {
            echo 'DEP-REDHAT'
          }
        }
        stage('SHUTTLE-DEP-WINDOWS') {
          steps {
            sh '''echo "OK0";
echo "OK0";
echo "OK0";
echo "OK0";
echo "OK0";
echo "OK0";
echo "OK0";
echo "OK0";
echo "OK0";
echo "OK0";
echo "OK0";
'''
          }
        }
      }
    }
    stage('IT-TEST') {
      steps {
        echo 'END'
      }
    }
  }
}