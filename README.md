# Private-registry
### Description:
- Build your private registry for saving containers images safely using ssl and a user password for authentification in your personal server.

### Getting started
``` bash
git clone git@github.com:ozennou/Your-Private-Registry.git
docker compose up -d
```
- For pulling and pushing the container images you should authenticate:
``` bash
docker login https://registry.domain_example/v2
```
- After login successfully you can simply push any container image, but you should specify the right tag:
``` bash
docker image tag IMAGE[:TAG] [REGISTRYHOST/][USERNAME/]NAME[:TAG]
```