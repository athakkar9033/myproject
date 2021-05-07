pipeline {
    agent any

    stages {
        stage('Parameters'){
                steps {
                    script {
                    properties([
                            parameters([
                                [$class: 'ChoiceParameter', 
                                    choices: ['ONE', 'TWO'], 
                                    name: 'PARAMETER_01']])
                        ])
                    }
                }
            
        stage('prod') {
            steps {
                echo 'Building..'
            }
        }
        stage('UAT') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Dev') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
}
