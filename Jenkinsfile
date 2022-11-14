pipeline
{
 agent any
 stages {

 /*stage('build'){
 steps{
 script{
sh " ansible-playbook  /var/lib/jenkins/workspace/livraison/Ansible/build.yml -i Ansible/inventory/host.yml"
 }
 }
 
 }*/
 /*stage('docker')
 {
 steps{
 script{
 sh " ansible-playbook  /var/lib/jenkins/workspace/livraison/Ansible/docker.yml -i Ansible/host.yml "
 }
 }
 }*/
   stage('Docker login') {

                                         steps {
                                          sh 'echo "login Docker ...."'
                   	sh "docker login -u farahbenmahmoud -p Farahdocker"
                               }  }
 stage('docker registry')
 {
 steps{
 script{
 sh " ansible-playbook /var/lib/jenkins/workspace/livraison/Ansible/docker-registry.yml -i Ansible/host.yml "
 }
 }
 }
 }
 }
