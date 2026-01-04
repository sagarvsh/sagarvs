#!/usr/bin/groovy
pipeline {
    agent any
    environment {
        LANG = "en_US.UTF-8"
    }
    stages {
        stage('Publish') {
            steps {
                sshagent(credentials: ['GitHub-SSH-Key']) {
                    sh '''#!/bin/sh
                        set -euo pipefail
                        python3 -m venv .venv
                        . .venv/bin/activate
                        pip install --upgrade pip
                        pip install --requirement=requirements.txt
                        mkdocs gh-deploy
                        '''
                }
            }
        }
    }
}