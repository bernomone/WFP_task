# WFP_task

World food program Data Science Assignemnt task. To make this repository work, be sure to have Docker installed. In the main folder run **docker build . --tag wfp:task** to build the image.
Then **docker run -p 8888:8888 --rm -v $(pwd):/app/ wfp:task** to run the container on port 8888 (please be sure this port available first). **localhost:8888** will show the notebooks for the analysis.