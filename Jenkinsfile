node {
  stage ('SCM checkout'){
    git 'https://github.com/rishireddyg/car-rentals.git'
    }
  stage ('mvn_build'){
  def mvnHome= tool name: 'maven3', type: 'maven'
  sh "${mvnHome}/bin/make"
  }
   stage ('mvn_test'){
  def mvnHome= tool name: 'maven3', type: 'maven'
  sh "${mvnHome}/bin/make check"
  }
  stage ('mvn_compile'){
  def mvnHome= tool name: 'maven3', type: 'maven'
  sh "${mvnHome}/bin/compile"
  }
  stage ('mvn_deploy'){
  def mvnHome= tool name: 'maven3', type: 'maven'
  sh "${mvnHome}/bin/make publish"
  }
}
  
  
