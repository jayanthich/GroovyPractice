pipeline {
    agent {
      node {
        label 'linux'
        def rootDir = pwd()
        def example = load "${rootDir}@script/DemoRun.Groovy "
      }

      stage('Node Details') {
          steps {
              println "${NODE_NAME}"
          }
      }

      stage("Release Inputs") {
          steps {
              DemoRun{
                Nothing=""
              }
          }
      }
    }
}
