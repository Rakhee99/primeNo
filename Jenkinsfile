node {
  stage('SCM checkout') {
    git credentialsId: 'f461d2a6-f07b-491b-a9d7-b361cf79644d', url: 'https://github.com/Rakhee99/primeNo.git'
  }
  stage ('compile Package') {
    // get maven home
    def mvnhome = tool name: 'MAVEN-R', type: 'maven'
    sh "${mvnhome}/bin/mvn package"
  }
}
