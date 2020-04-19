#!goorvy

pipeline {
  agent any
  environment {
	  AWS_DEFAULT_REGION    = ""
  }
  stages {
    stage("preflight") {
      steps {
        echo "Preflight"
        sh "ls -al"
      }
    }
    stage("Build") {
      steps {
        echo "Build"
      }
    }
    stage("Unit Tests") {
      steps {
        echo "Unit Tests"
      }
    }
    stage("Static Analysis") {
      steps {
        parallel(
          SonarScan: {
            echo "Placeholder for Sonar Scan"
          },
          SecurityScan: {
            echo "Placeholder for Fortify Security Scan"
          }
        )
      }
    }
    stage("Dependancy Scan") {
      steps {
        echo "Depenancy Scan"
        echo "Placeholder for Dependency Scan"
      }
    }
    stage("Deploy Test") {
      steps {
        echo "Deploy Test"
        }
      }
    }
    stage("Functional Tests") {
      steps {
        echo "Functional Tests"
        echo "Placeholder for Functional Tests"
      }
    }
    stage("Packaging") {
      steps {
        echo "Packaging"
        }
      }
    }
    stage('Deploying') {
      steps {
	echo "Deploying"
      }
    }
    stage('Deploy Testing') {
      steps {
	echo "Deploy Testing"
      }
    }
    stage('Clean Up') {
      steps {
	echo "Clean up"
      }
    }
  }
}
