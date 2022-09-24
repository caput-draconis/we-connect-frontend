pipeline {
  agent any
  tools {
    nodejs "NodeJS"
  }
  stages {
stage('SonarQube Analysis') {
    def scannerHome = tool 'sonarqube';
    withSonarQubeEnv() {
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
  }
}
