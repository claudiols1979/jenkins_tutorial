pipeline {
    agent any
    parameters {
        choice(
            choices: ['greeting' , 'silence'],
            description: '',
            name: 'REQUESTED_ACTION')

        text(
            defaultValue: '''
            this is a multi-line 
            string parameter example
                           ''', 
            name: 'MULTI-LINE-STRING'
        )
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
                expression { params.REQUESTED_ACTION == 'greeting' }
            }
            steps {
                echo "Hello, Claukss!"
            }
        }
    }
}