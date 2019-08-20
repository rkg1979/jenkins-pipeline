import hudson.model.*
import hudson.EnvVars
import java.net.URL

node{
    stage('git checkout'){
        git('https://github.com/rkg1979/DevOpsClassCodes.git')
    }
    stage('maven compile'){
        withMaven(maven:'MyMaven'){
            sh 'mvn compile'
        }
    }
    stage('maven package'){
        withMaven(maven:'MyMaven'){
            sh 'mvn package'
        }
    }
}
