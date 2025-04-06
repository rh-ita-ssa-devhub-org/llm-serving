# llm-serving
Firt of all you need to create the minio instance, in a namespace of your choice. 
You have to set up a password in the minio.yaml

The open-webui can be skipped

You have to import the serving-runtime.yaml within the custom runtimes section of RHOAI, ad use it when you want to deploy the model

The run the steps in the download-model-to-s3.iipynb you have to create a workbench add the following variables


HF_USERNAME your HF username
HF_TOKEN you HF token


# Model - Registy

if you want to write also something into the model registry, 
io have to apply the yamls in the model-registry folder

my-sql.yaml
model-registry.yaml

to use the python code, you have to grab the service url to get the right endpoint from service mesh
As it is not useful for serving the model you can just skip the model-registy part of this notebook
