elifePipeline {
    stage 'Checkout', {
        checkout scm
    }

    elifeMainlineOnly {
      stage 'Deploy to staging', {
          sh "helm upgrade --install basex-validator--staging ./helm/basex-validator --recreate-pods"
      }
    }
}