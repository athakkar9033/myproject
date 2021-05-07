pipeline {
    agent any

    stages {
        stage('Parameters'){
                steps {
                    script {
                    properties([
                            parameters([
                                [$class: 'ChoiceParameter', 
                                    choiceType: 'PT_SINGLE_SELECT', 
                                    description: 'Select the Environemnt from the Dropdown List']])
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
