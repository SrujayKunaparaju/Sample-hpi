pipeline {
  agent any

  stages{ // The content in this Jenkinsfile has the targeted keywords we will use in automation to track stages for dashboarding.
          // Please insure to at least leave these keywords inside the "stage" in your description of the activity to help keep clean
          // our automation processes
    stage('Lint') { 
      steps {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'eedd57d4-ab28-4a1d-8f67-eeca66f2c47e', url: 'https://github.dxc.com/NewOrleansDigitalTransformationCenter/hpi-em4s.git']]])
      }
    }
    
