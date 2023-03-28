## modified
node {
    stage('Cont.Download') {
    https://github.com/venkat9822891/mynew-branch-scm.git
      }
	stage('Cont.Build') {
    sh 'mvn package'
      }
	stage('Cont.Deploy'){
        deploy adapters: [tomcat9(credentialsId: 'dded43c3-e568-4414-a254-d2060b25fbed', path: '', url: 'http://172.31.38.129:8080')], contextPath: '/my-test', war: '**/*.war'
      }
}
