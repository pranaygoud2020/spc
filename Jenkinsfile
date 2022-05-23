pipeline {
	agent { label 'spc,123' }
	triggers {
		cron('* * * * *') 
	}
		stages {
		stage('scm') {
			steps {
				git branch: 'main', url: 'https://github.com/pranaygoud2020/spring-petclinic.git'
			}
		}
		stage('build'){
			steps {
				sh 'package'
		}
    	}
	}
}
