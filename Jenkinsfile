pipeline {
    agent any
    parameters {
          
        string(
            defaultValue: '', 
            name: 'STRING-PARAMETER', 
            trim: true
        )        


    }

    stages {
        stage ('Speak') {
            when {
                
                expression { params.STRING-PARAMETER == 'Claukss' }
            }
            steps {
                echo "Hello, Claukss!"
            }
        }
    }
}