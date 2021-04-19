
node {
    stage ("clone"){
        git "https://github.com/Snir-z89/git_python-exercise.git"
    }
    stage ("run script"){
        checkout([$class: 'GitSCM', branches: [[name: '**']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Snir-z89/git_python-exercise.git']]])
        bat "python myapp.py"
    }

}
