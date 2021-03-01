node {
  stage ('SCM checkout'){
    git 'https://github.com/rishireddyg/car-rentals.git'
    }
 
  stage ('mvn_deploy'){
  def mvnHome= tool name: 'maven3', type: 'maven'
  sh "${mvnHome}/bin/mvn package"
  }
  stage ('clean after build'){
      cleanWs()
  }
  stage (' message'){
  echo 'your job is done| thanks for choosing jenkins'
  }
 
  stage ('error message'){

  }

}
  
  
