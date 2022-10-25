pipeline {
    agent any
    environment {
        PROJECT_ID = "****"
        CLUSTER_NAME = "****"
        LOCATION = "****"
        CREDENTIALS_ID = "****"
    }
    stages {
        stage("Deploy to GKE") {
            steps {
                echo "Deploying the application..."
                echo "Deploying deployment.yaml"
                step([$class: "KubernetesEngineBuilder",
                        projectId: env.PROJECT_ID,
                        clusterName: env.CLUSTER_NAME,
                        location: env.LOCATION,
                        manifestPattern: "deployment.yaml",
                        credentialsId: env.CREDENTIALS_ID,
                        verifyDeployments: true])
                echo "Deployment Finished"
            }
        }
    }
}
