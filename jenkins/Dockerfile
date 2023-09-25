FROM jenkins/jenkins:latest
COPY config.yaml /var/jenkins_home/
ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false
ENV CASC_JENKINS_CONFIG /var/jenkins_home/config.yaml
COPY plugin_list.txt /usr/share/jenkins/ref/plugin_list.txt
RUN jenkins-plugin-cli -f /usr/share/jenkins/ref/plugin_list.txt
