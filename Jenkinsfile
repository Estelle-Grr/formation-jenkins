pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        sh 'date'
      }
    }

    stage('Stage 2') {
      steps {
        sh '''dpkg -l > /tmp/paquets
if test `grep -c user /etc/passwd` -ne 0
then
find / -user user > /tmp/user
f'''
      }
    }

    stage('Stage 3') {
      steps {
        sh '''if test `grep -c user /etc/passwd` -ne 0
then
find / -user user > /tmp/user
fi'''
      }
    }

  }
}