# xgboost-lightgbm-docker
XGBoost and LightGBM inside Anaconda Docker container

Build and Start:
```
git clone https://github.com/olegkhomenko/xgboost-lightgbm-docker.git
cd xgboost-lightgbm-docker
docker build -t xgboost-lightgbm-docker .
```
Then
If you use \*nix
```
docker run -i -t -p 8888:8888 -v /data/docker-volumes:/data/docker-volumes xgboost-lightgbm-docker /bin/bash -c "/opt/conda/bin/jupyter notebook --ip='*' --port=8888 --notebook-dir='/' --no-browser --allow-root"
```

If you use Windows 10
```
winpty docker run -i -t -p 8888:8888 -v /c/docker-volumes:/data/docker-volumes xgboost-lightgbm-docker //bin/bash -c "//opt/conda/bin/jupyter notebook --ip='*' --port=8888 --notebook-dir='/' --no-browser --allow-root"
```
