node{
  stage('SCM Checkout'){
    git 'https://github.com/shankar-trainer/test1'
  }
  
  stage('Compile-Package'){
    def mvnHome=tool name: 'maven', type: 'maven'
    sh '${mvnHome}/bin/mvn package'
  }
  
  stage('Test'){
   tool name: 'maven', type: 'maven'
   sh '${mvnHome}/bin/mvn test'
  }
}

