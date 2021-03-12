node {
  stage('SCM checkout') {
    tool name: 'Default', type: 'git'
  }
  stage ('compile Package') {
    // get maven home
    def mvnhome = tool name: 'MAVEN-R', type: 'maven'
    sh "${mvnhome}/bin/mvn package"
  }
}
