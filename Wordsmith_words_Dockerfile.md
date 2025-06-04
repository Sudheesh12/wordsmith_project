**Date :** 4-Jun-2025  Wednesday

**Last modified :** 4-Jun-2025  Wednesday 11:06 am

**Status:**   

**Tags:**   

---
##  **Wordsmith_words_Dockerfile**

```
FROM ubuntu:latest

  

WORKDIR /app

  

RUN apt-get update && apt-get install -y maven

  

COPY . /app/

  

RUN mvn verify

  

CMD ["java", "-Xmx8m", "-Xms8m", "-jar", "target/words.jar" ]
```

OUTPUT
```
Server started

```
## **References**
