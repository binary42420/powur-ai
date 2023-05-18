## 
```bash
# Enable Document AI
gcloud services enable documentai.googleapis.com
```
### Environment variables
```bash
PROJECT_ID=$(gcloud config list --format "value(core.project)")

# Source on GitHub
GIT_USER="binary42420"
GIT_REPO="powur-ai"
GITHUB_SOURCE="https://github.com/$GIT_USER/$GIT_REPO.git"

# Local source
PROJECT_SOURCE=~/$GIT_REPO/powur-ai/src
```

### Source code

```bash
# Get the source code
cd ~
git clone $GITHUB_SOURCE

ls $PROJECT_SOURCE

```

## 🚀 Deploying to Cloud Run

```bash
gcloud services enable \
  artifactregistry.googleapis.com \
  cloudbuild.googleapis.com \
  run.googleapis.com
```
## deploy
```bash
SERVICE="powur-ai-demo"
CLOUD_RUN_REGION="europe-west6"
CLOUD_RUN_MEMORY="4Gi"

gcloud run deploy $SERVICE \
  --source $PROJECT_SOURCE \
  --region $CLOUD_RUN_REGION \
  --memory $CLOUD_RUN_MEMORY \
  --platform managed \
  --allow-unauthenticated \
  --quiet
```
## b

```bash
APP_URL=$( \
  gcloud run services describe $SERVICE \
    --region $CLOUD_RUN_REGION \
    --platform managed \
    --format "value(status.url)" \
)
```

##  endpoint:

```bash
curl $APP_URL/admin/processors/setup
```

## logs:

```bash
gcloud logging read \
  "resource.type=cloud_run_revision resource.labels.service_name=$SERVICE" \
  --project $PROJECT_ID \
  --format "value(textPayload)" \
  --freshness 5m
```
