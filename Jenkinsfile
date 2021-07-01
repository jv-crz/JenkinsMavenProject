pipeline {
	agent any
	stages {
		stage("Parallel Execution") {
			steps {
				parallel(
				      a: {
					bat "mvn clean"
				      },
				      b: {
					bat "mvn test"
				      },
				      c: {
					bat "mvn package"
				      }
				)
			}
		}
	}
}
