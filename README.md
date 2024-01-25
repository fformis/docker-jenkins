
# docker-jenkins

Imagem do Jenkins LTS com instalação do docker e do docker cli.




## Uso/Exemplos

```yaml
jenkins:
    image: fformis/docker-jenkins:lts
    restart: unless-stopped
    ports:
      - 50000:50000
    volumes:
      - ./jenkins/jenkins_home:/var/jenkins_home
      - /var/run/docker.sock:/var/run/docker.sock
      - /usr/bin/docker:/usr/bin/docker
```


## Licença

[MIT](https://choosealicense.com/licenses/mit/)

