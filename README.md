# time_series_analysis
A series of notebooks to dive into time series analysis using popular public datasets


# How to run?
To run the whole environment with all the notebooks, install docker, go to the root directory of the project, then build the image with the following command (replace **<image-name>** with any name you want):

```
docker image build -t <image-name> .
```

Next, run the container. If you're on Windows, replace **(pwd)** with **{pwd}**

```
docker container run -p 8888:8888 -v $(pwd)/datasets/:/app/datasets/ -v $(pwd)/notebooks/:/app/notebooks/ <image-name>

