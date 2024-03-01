# Info 103 updated JupyterHub Docker container

This is a fork of the official UW JupyterHub Docker containers, but the [SciPy](./scipy/README.md) one is updated for Info 103 by adding install steps for various social media python apis (discord, praw, atproto, etc.).


## UW-IT JupyterHub for Teaching
Docker images for base JupyterLab environments used in [UW-IT JupyterHub for Teaching](https://itconnect.uw.edu/learn/tools/jupyterhub-for-teaching/) service. General information about working with base images is here: https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html

### Images:
* [Datascience](./datascience/README.md)
* [R](./r/README.md)
* [RStudio](./rstudio/README.md)
* [SciPy](./scipy/README.md)
* [Tensorflow](./tensorflow/README.md)

Running notebook locally
- `docker run -p 8888:8888 us-west1-docker.pkg.dev/uwit-mci-axdd/rttl-images/<image_name>:<image_tag>`
- Console output will include localhost url with access token. Add '/lab' to the end of the path portion for the JupyterLab interface, eg: `http://127.0.0.1:8888/lab`

Accessing server shell locally
- `docker run -it --entrypoint /bin/bash us-west1-docker.pkg.dev/uwit-mci-axdd/rttl-images/<image_name>:<image_tag>`