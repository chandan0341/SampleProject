def workspace;
node{
    stage('Checkout')
    {
      checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '10a6b691-bc88-458f-bccf-35d903bd2ada', url: 'https://github.com/chandan0341/SampleProject.git']]])  
       workspace = pwd()
    }
    stage('Static code analysis')
    {
        echo "Static code analysis"
    }
    stage('Build'){
        echo "building the project"
    }
    stage('Unit testing'){
        echo "unit testing"
    }
    stage('Delivery'){
        echo "deliver the code"
        
    }
}
