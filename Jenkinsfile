pipeline {
    agent any
    
    options {
        // Activer la notification par e-mail en cas de succès ou d'échec du pipeline
        success {
            emailext (
                to: 'mouhafall888@gmail.com',
                subject: "Succès du pipeline ${currentBuild.fullDisplayName}",
                body: "Le pipeline ${currentBuild.fullDisplayName} a été exécuté avec succès. Bon travail !"
            )
        }
        failure {
            emailext (
                to: 'mouhafall888@gmail.com',
                subject: "Échec du pipeline ${currentBuild.fullDisplayName}",
                body: "Le pipeline ${currentBuild.fullDisplayName} a échoué. Merci de vérifier et de corriger."
            )
        }
    }
    
}
