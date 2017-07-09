node {
  stage('Clean workspace') {
    deleteDir()
    sh 'ls -lah'
  }

  stage 'checkout'
    git url: 'https://github.com/nbaars/spring-petclinic'

  stage 'build'
    def mvnHome = tool 'maven'
    sh "${mvnHome}/bin/mvn -B clean install"
}
