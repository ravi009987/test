
pipeline {
    agent any

    parameters {
        string(name: 'Pram', defaultValue: 'default_value', description: 'Parameter 1 description')
        booleanParam(name: 'PARAM2', defaultValue: true, description: 'Parameter 2 description')
        choice(name: 'PARAM3', choices: ['Option1', 'Option2', 'Option3'], description: 'Parameter 3 description')
    }

    stages {
        stage('Example Stage') {
            steps {
                echo "Parameter 1: ${params.PARAM1}"
                echo "Parameter 2: ${params.PARAM2}"
                echo "Parameter 3: ${params.PARAM3}"

                // You can use the parameter values in your steps
                // For example:
                // sh "echo ${params.PARAM1} > output.txt"
            }
        }
    }
}

