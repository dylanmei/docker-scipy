docker-scipy
------------

Docker image for doing data science with the [SciPy stack](https://en.wikipedia.org/wiki/SciPy).

# notebooks

Build a [Zeppelin](http://zeppelin.incubator.apache.org) notebook on top of `dylanmei/scipy`:

```
docker build -t zeppelin -f Dockerfile.zeppelin .
docker run --rm --name zeppelin -p 8080:8080 -v $(pwd)/notebook:/usr/zeppelin/notebook zeppelin
```
