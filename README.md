# Cloud Provider Scraper

The purpose of this repository is create a mechanism to get cloud docs, text, images, etc, from cloud providers. To do that, our approach was to use web crawlers to extract data from different data sources:

- [Azure](./azure)
- [Oracle](./oracle)

![img](./media/01-jupyter-lab-scraper-example.jpg)

## Docker

To run this scraper, you can use docker with follow command:

```PowerShell
# windows enviroment
docker run --rm -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes -v "C:\Users\user\your\folder\target":/home/jovyan/work pavelsjo/jupyter-scrapper

# linux environment
docker run --rm -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes -v your/folder/target:/home/jovyan/work pavelsjo/jupyter-scrapper
```

- **The `-v` command** enable a share folder between your local computer and docker image container. **Warning** please check this [recommendation-wsl](https://docs.docker.com/docker-for-windows/wsl/)

- This project is based on [Jupyter Docker Stacks](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html), and, fell free to use other [Image options](https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html). **Warning:** this approach will be required install aditional python libraries.


## Disclaimer

The views expressed on this repository are my own and do not reflect the views of the company(ies) I work (or have worked for) neither Oracle Corporation. The opinions expressed by visitors on this repository are theirs, not mine.

The information in this repository is written based on personal experiences. You are free to use the information on this repository but I am not responsible and will not compensate to you if you ever happen to suffer a loss/inconvenience/damage because of/while making use of this information.