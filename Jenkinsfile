node{
  stage('SCM Checkout'){
    git 'https://github.com/shankar-trainer/test1'
  }
  
  stage('Compile-Package'){
   tool name: 'maven', type: 'maven'
   sh 'mvn package'
  }
  
  stage('Test'){
   tool name: 'maven', type: 'maven'
   sh 'mvn test'
  }
}

