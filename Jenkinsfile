node {
  stage 'checkout'
    git url: 'https://github.com/nbaars/spring-petclinic'

  stage 'build'
    def mvnHome = tool 'Maven'
    sh "${mvnHome}/bin/mvn -B clean install"
}
