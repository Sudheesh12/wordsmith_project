**Date :** 4-Jun-2025  Wednesday

**Last modified :** 4-Jun-2025  Wednesday 11:06 am

**Status:**   #Completed 

**Tags:**   [[Docker]] [[Container]] [[Project]] 

---
##  **Wordsmith_web_Dockerfile**


### **Initial testing** 



```
# ==== Using the image alpine 3.22 for smaller image size ====== #

FROM golang:alpine3.22

  

# setting the workdirectory as root

WORKDIR /app

  

# Copying the go code to the image #

COPY ./dispatcher.go /app/

  

RUN go build dispatcher.go

  

CMD ["./dispatcher"]

  

EXPOSE 80
```


Worked as expected, the output came as 
```
Listenting on port 80
```




## **References**
