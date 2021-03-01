node {
  stage ('SCM checkout'){
    git 'https://github.com/rishireddyg/car-rentals.git'
    }
  stage ('mvn_build'){
  def mvnHome= tool name: 'maven3', type: 'maven'
  sh "${mvnHome}/bin/mvn test"
  }
}
  
  
