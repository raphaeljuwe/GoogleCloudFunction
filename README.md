# Google Cloud Functions Python Runtime Demo
This fucntion conncts  with Google cloud sql


## Deployment

```
$ gcloud components update
$ gcloud components install beta
$ gcloud beta functions deploy getUserDetails --runtime python37 --trigger-http --project <projectId>
```

Where `<projectId>` is your Google Cloud project ID.

## Testing

Point a browser at:

```
https://<region>-<projectId>.cloudfunctions.net/getUserDetails
```

Where:

* `<region>` is the Google Cloud region that you deployed to (e.g. `us-central1`)
* `<projectId>` is your Google Cloud project ID

(the full URL that you need will be displayed in the output of the `gcloud` command when deploying the function).
