pipeline {
  agent any
  stages {
    stage('Construyendo el sistema') {
      steps {
        echo 'Constuyendo el sistema'
      }
    }

    stage('Validacion') {
      steps {
        input '¿Apruebas el despliegue?'
      }
    }

    stage('Guardando Datos de despliegue') {
      steps {
        timestamps()
        echo 'Confirmacion Manual'
      }
    }

    stage('Desplegando') {
      steps {
        sh 'instanciaPresencial.sh'
      }
    }

  }
}