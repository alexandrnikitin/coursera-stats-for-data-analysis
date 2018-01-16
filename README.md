# coursera-stats-for-data-analysis

### HOWTO: run jupyter in docker container

```bash
docker run -d -p 8888:8888 --user root \
    -v /home/nikitin/notebooks:/home/jovyan/work \
    -e NB_UID=1000 -e NB_GID=1000 -e GRANT_SUDO=yes \
    jupyter/datascience-notebook start-notebook.sh --NotebookApp.token=''
```
