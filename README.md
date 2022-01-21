# SettingUpGoogleCouldSDK
repo for instructions to set up google cloud sdk. Start upload &amp; download today with google cloud storage.

### Initialization

1. How to install google cloud sdk 
https://cloud.google.com/sdk/docs/quickstart
2. initiate:
``` gcloud init ```
3. It will ask to choose a cloud project. Choose mystical-accord-338912.
4. Log in with a different account afterwards:
``` gcloud auth login ```
5. Double-check with configuration:
``` gcloud config list```
6. Connect to the shared project, in case something goes wrong:
```gcloud config set project mystical-accord-338912```
7. Get a list of projects from google cloud:
``` gcloud projects list```
8. Make sure that you are in a right account:
```gcloud auth list```


### Commands
You have two choices for commands: ```gsutil``` and ```gcloud ```.
https://cloud.google.com/sdk/gcloud
gcloud gives much faster transfer speed. It is still in alpha stage, so use alpha.
list all buckets in the project:
```
gcloud alpha storage ls
```
When copying entrie directory to a bucket:
```
gcloud alpha storage cp -r LOCAL_DIRECTORY gs://hebarium2022-blurred/
```

