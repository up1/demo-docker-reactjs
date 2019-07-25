# Working with docker

### Step 1 :: Build docker image for React app with [multi-stage build](https://docs.docker.com/develop/develop-images/multistage-build/)
```
$docker image build -t react:1.0 -f Dockerfile .
$docker image ls
```
Try again !!! to see result ...

## Step 2 :: Improve Dockerfile
```
$docker image build -t react:1.0 -f Dockerfile-better .
$docker image ls
```
Try again !!! to see result ...

## Step 3 :: Run your container
```
$docker container run -d -p 8000:80 react:1.0
```
Open url=`http://localhost:8000/` in your browser

