# GPT2-Web
A flask application that uses DialoGPT model.

## Try it!
Note: The model takes about 1 min to load. It will be improved.

https://flask-service-iolnexrvpa-ue.a.run.app

## Steps to Deploy:
1) Create docker image
``` command
   cd <project-directory>
   docker build -t <name> .
```
2) Test if it works by running
``` command
   docker run -p 8080:8080 <image-name>
```
3) Create a Google Cloud account, new project and install the CLI

4) Deploy it!
``` command
   cd <project-directory>
   gcloud builds submit --tag gcr.io/<project-name-ID>/<image>
   gcloud run deploy --image gcr.io/<project-name-ID>/<image> --cpu 2.0 --memory 8Gi
```

https://user-images.githubusercontent.com/111835151/226846308-524a2592-78e8-480f-bde5-f66bfcb3f6e3.mp4

