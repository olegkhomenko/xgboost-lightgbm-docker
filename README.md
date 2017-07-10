# xgboost-lightgbm-docker
XGBoost and LightGBM inside Anaconda Docker container

Build and Start:
```
git clone https://github.com/olegkhomenko/xgboost-lightgbm-docker.git
cd xgboost-lightgbm-docker
docker build . -t xgboost-lightgbm-docker
docker run -i -t -p 8888:8888 xgboost-lightgbm-docker /bin/bash -c "/opt/conda/bin/jupyter notebook --ip='*' --port=8888 --no-browser"
```
