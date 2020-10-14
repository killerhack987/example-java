node('MAVEN') {

        stage ('SCM') {
		//git clone 
		git credentialsId: '5f358629-087a-4a67-be16-b47f66a1d5a7', url: 'https://github.com/killerhack987/example-java.git'
	}
        stage('build the packages') {
			// mvn package
			sh 'mvn package'
	}
             
        stage ('archival and test results') {
			// archiveArtifacts artifacts: 'target/*jar', followSymlinks: false
				junit 'target / surefire-reports /*.xml'
	}
		stage ('mail the build status') {
			// mail bcc: '', body: '', cc: '', from: '', replyTo: '', subject: 'Build status', to: 'ravikishorefst@gmail.com'
			
		}
            
	}
	