pipeline {
    agent {
        label "master"
    }
	stages {
        stage("clone code") {
            steps {
                script {
                    // Let's clone the source
                    git 'https://github.com/kiranpayyavuala/nexus-app.git';
                }
            }
        }
	}
	stage("mvn build") {
            steps {
                script {
                    sh "mvn clean install"
                }
            }
        }
}
