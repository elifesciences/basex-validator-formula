elifePipeline {
    stage 'Checkout', {
        checkout scm
    }

    stage 'Deploy to staging', {
        sh "helm upgrade --install basex-validator--staging ./helm/basex-validator"
    }
}