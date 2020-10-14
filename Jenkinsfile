node('MAVEN') {

        stage ('SCM') {
		//git clone 
		git 'https://github.com/killerhack987/example-java.git'
	}
        stage('build the packages') {
			// mvn package
			sh 'mvn package'
	}
             
        stage ('archival and test results') {
			// archiveArtifacts artifacts: 'target/*jar'
				junit 'target / surefire-reports /*.xml'
	}
		stage ('mail the build status') {
			// mail bcc: '', body: '', cc: '', from: '', replyTo: '', subject: 'Build status', to: 'ravikishorefst@gmail.com'
			
		}
            
	}
	