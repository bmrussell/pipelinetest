stage 'CI'
echo '==== STAGE: CI ===================================================='
node {
    try {
        echo 'Checking out...'
        scm checkout
        echo 'Checked out.'
        dir
        currentBuild.result = 'SUCCESS'
    } catch (Exception err) {
        currentBuild.result = 'FAILURE'
    }
    echo "RESULT: ${currentBuild.result}"
}