FROM amazonlinux

RUN yum install -y aws-cli tar gzip
RUN curl -O https://s3.us-west-2.amazonaws.com/amazon-eks/1.33.0/2025-05-01/bin/linux/amd64/kubectl && chmod +x ./kubectl && mkdir -p $HOME/bin && cp ./kubectl $HOME/bin/kubectl && export PATH=$HOME/bin:$PATHi
RUN curl -L https://get.helm.sh/helm-v3.18.2-linux-amd64.tar.gz -o helm.tar.gz && tar -zxvf helm.tar.gz && chmod +x linux-amd64/helm && mv linux-amd64/helm /usr/local/bin/helm
