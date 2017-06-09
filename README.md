## concourse-ci

Try Concourse CI with Vagrant

### Setup

` $ vagrant up`

` $ open http://192.168.100.4:8080`

### Authenticate on `local` target environment

`$ fly -t lite login -c http://192.168.100.4:8080`

### Create or update the `pipeline` on `local` target

`$ fly -t lite set-pipeline -p node-concourse-ci -c pipeline/pipeline.yml`

### Destroy the `pipeline` on `local` target

`$ fly -t lite destroy-pipeline --pipeline node-concourse-ci`
