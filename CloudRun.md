# Cloud Run

### Truy cap https://console.cloud.google.com/run
#

![alt text](./images/8.png "Title")

## Service settings
#
![alt text](./images/9.png "Title")
- Service name: Ten dich vu
- Region: chon khu vuc gan minh nhat (HongKong hoac Singapore)
- Next

## Configure the service's first revision
#
![alt text](./images/10.png "Title")
- Select container image URL: Chon container muon deploylen
- Next

## Configure how this service is triggered
#
![alt text](./images/11.png "Title")
- Chon Allow all traffic
- Authentication: Xac thuc
    + Allow unauthenticated invocation. Bo qua xac thuc.
    + Require authentication.(Can xac thuc)
- Create

## Sau khi tao xong
![alt text](./images/12.png "Title")

### Chon Edit & Deploy new revision
- 
Deploy
![alt text](./images/13.png "Title")

# CLI
Build
- gcloud builds submit --tag gcr.io/classfunc-com/tim-xe-api

Run
- gcloud run deploy --image gcr.io/classfunc-com/tim-xe-api --platform managed