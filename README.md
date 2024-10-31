# cicd

docker build . -t ghcr.io/jookwankim/practice-devops/my-app:latest


docker buildx build . \
  --platform linux/amd64,linux/arm64 \
  --push \
  -t ghcr.io/jookwankim/${{ env.PACKAGE }}/${{ env.PROJECT_DIR }}:latest
  
  
  docker login ghcr.io \
	-u jookwankim \
	-p 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
   
   
docker push ghcr.io/jookwankim/practice-devops/my-app:latest
