# Voyages Python Notebook

This project represents the first attempts, beginning in early 2022, to systematically use SlaveVoyages data as presented through a new REST API. I wrote the first quick pass at this, and Nishant Satpathy, in an internship with the CRC, built the examples out.

## Current state

In Decmeber 2023, I did a quick refactor of one of the notebooks in order to provide a working use-case for the api's dataframes endpoint, with an eye towards showing the UC side of the SV team:

1. How the dataframes endpoint works
1. What notebook coding looks like
1. How notebook coding can help with code documentation

This will hopefully help the team as they choose which technologies they want to use in their rebuild of the imputation and estimation algorithms.

### Dec. 2

I have refactored one notebook and published it out as a markdown and as an html file.

See [Bubble Map and Bar Graph HTML file](bubblemap)

The not-yet-refactored notebooks are in the appropriately-named subfolders.

## Steps to run notebook:

1. Install jupyter notebook on machine OR use VSCode for opening jupyter notebook. Run jupyter notebook using following command in the terminal: ```jupyter notebook```
1. Install necessary packages if missing such as ipywidgets, plotly, etc, using pip or whichever package manager is appropriate
1. Based on the ```app_secrets.py-example``` template file, create an ```app_secrets.py``` file to hold the token for the voyages-api server you're using
1. Check your base url
	1. If local (127...), run all required Docker containers
	1. If the cloud-hosted server, you should be good to go (if your token is valid)
1. Run 'Restart and Run all' under Kernel option