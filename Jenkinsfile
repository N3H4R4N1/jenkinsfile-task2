@Library('SharedLib-Task-2') _

pipeline {
    agent any
    stages {
        stage('Run Maven Build via Shared Library') {
            steps {
                mavenBuildNotify(
                    repoUrl: 'https://github.com/opstree/spring3hibernate.git',
                    branch: 'main',
                    mavenCmd: 'clean package'
                )
            }
        }
    }
}
