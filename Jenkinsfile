#!groovy

node {
    git url: 'git@github.com:jyasveer/python-manifest-repo.git'
    
    def response = bayesianAnalysis url: 'https://recommender.api.openshift.io'
    if (response.success) {
        echo "Results here: ${response.getAnalysisUrl()}"
    }
    echo "${response.content}"
}
