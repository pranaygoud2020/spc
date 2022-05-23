node('spc,123') {
	stage('scm') {
		git branch: 'main', url:'https://github.com/pranaygoud2020/spring-petclinic.git'
	}
	stage('build') {
		sh 'mvn package'
		}
}
