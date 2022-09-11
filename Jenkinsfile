pipeline {
    agent {
        node {
            label 'built-in'
            customWorkspace '/data/project'
        }
    }

    stages {
        stage('clone') {
            steps {
				sh "rm -rf *"
                sh "git clone --single-branch --branch 22q1 https://github.com/vinay-aws/assignment.git q1"
				sh "git clone --single-branch --branch 22q2 https://github.com/vinay-aws/assignment.git q2"
				sh "git clone --single-branch --branch 22q3 https://github.com/vinay-aws/assignment.git q3"
            }
        }

    }
}



