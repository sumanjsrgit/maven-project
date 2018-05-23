pipeline {
agent any
stages {
stage('BUILD'){
steps {
sh 'mvn clean package'
}
  post { success{
    echo "Now archieving "
    archiveartifacts artifacts: '**/target/*.war'
}
}
}
}
}
