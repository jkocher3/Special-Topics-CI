
node {
  stage('checkout sources') {
        // You should change this to be the appropriate thing
        git url: 'https://github.com/jkocher3/Special-Topics-CI'
  }

  stage('Build') {
    // you should build this repo with a maven build step here
    withMaven (maven: 'maven3'){
        sh "mvn package"
    }
  }

    // you should add a test report here


        junit 'target/surefire-reports/*.xml'
}
