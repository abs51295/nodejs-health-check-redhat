@Library('github.com/yzainee/osio-pipeline@analytics-plugin')
node("launchpad-nodejs") {
  checkout scm
  stage("Build") {
    sh "npm install"
  }
  stage("Deploy") {
    sh "npm run openshift"
  }
}
