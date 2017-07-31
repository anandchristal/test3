node {
  version = "1.0" + env.BUILD_NUMBER
  currentBuild.displayName = env.JOB_BASE_NAME + '-'+ version

  stage 'CheckOut'
  git "https://github.com/anandchristal/test3.git"


  stage 'Build'
  def mvnHome = tool 'M3'
 //  sh "${mvnHome}/bin/mvn -B verify"
  sh "npm run build"

 }
