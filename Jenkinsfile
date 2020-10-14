node('MAVEN') {

        stage ('SCM') {
		//some block
		git 'https://github.com/killerhack987/example-java.git'
	}
        stage('build') {
			sh label: '',script: 'mvn package'
	}
             
        stage ('archival and test results') {
			// archive 'target/*jar'
				junit 'target / surefire-reports /*.xml'
		}
            
}
	