pipeline {
    agent any
    parameters {
          
        string(
            defaultValue: 'scriptcrunch', 
            name: 'STRING-PARAMETER', 
            trim: true
        )

        
        


    }

    stages {
        stage ('Speak') {
            when {
                // Only say hello if a "greeting" is requested
                expression { params.STRING-PARAMETER == 'Claukss' }
            }
            steps {
                echo "Hello, Claukss!"
            }
        }
    }
}