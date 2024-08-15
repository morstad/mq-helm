cd /Users/nancymheinz/git/morstad-external/mq-helm/charts
helm package ibm-mq                                                                     
mv ibm-mq-9.0.0.tgz ibm-mq
helm repo index ibm-mq --url https://raw.githubusercontent.com/morstad/mq-helm/main/repo
mv ibm-mq/index.yaml ../repo/index.yaml

