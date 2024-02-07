# docker-sonar-scanner-jdk14
This repo is for docker scanner with jdk14

# docker-sonar-scanner

Enables integration with SonarQube.

### Usage

Insert the snippet below after your build step in your .drone.yml, copy the sonar-project.properties to your project and fill out the missing bits.

```
  sonar-scanner:
    image: quay.io/ukhomeofficedigital/sonar-scanner:v4.8.1
    when:
      event:
        - push
        - pull_request
```

