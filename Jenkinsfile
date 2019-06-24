#!/usr/bin/env groovy

pipeline {
  agent any

  parameters {
    choice(
      name: 'targetEnv',
      choices:"int\nfto\nprod",
      description: "Which (UCP-) environment do you want to deploy to?")
    string(
      gitParameter  name: 'TAG'
                    type: 'PT_TAG'
                    defaultValue: 'master'
  }

  stages {

    stage("Git checkout tag") {
      steps {
        script {
          echo "Git checkout of tag..."
        }
      }
    }

    stage("Init") {
      steps {
        script {
          echo "Initializing"
        }
      }
    }

    stage("Deploy") {
      steps {
        script {
          echo"Deploying"
        }
      }
    }
  }
}
