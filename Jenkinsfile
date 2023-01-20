pipeline {
    agent any
    parameters {
        [        
        string(
            defaultValue: 'scriptcrunch', 
            name: 'STRING-PARAMETER', 
            trim: true
        )

        ]
        


    }

    stages {
        stage ('Speak') {
            when {
                // Only say hello if a "greeting" is requested
                expression { params.REQUESTED_ACTION == 'greeting' }
            }
            steps {
                echo "Hello, Claukss!"
            }
        }
    }
}