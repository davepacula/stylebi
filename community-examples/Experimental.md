# Experimental Nightly Build

This file contains instructions on how to install the latest Experimental Nightly Build.

Save the [.env](.env) file to the Docker host machine by clicking on the link then click "Download raw file" button at upper right corner of the file editing area.

Place the .env file in the same directory as the docker-compose.yaml which was downloaded from the Quickstart guide. 

> **NOTE** The downloaded file may need to be renamed as ```.env```

Modify the downloaded .env file using a standard text editor to utilize the URL for the Experimental nightly build.

Continue following steps in the [Quickstart guide](https://github.com/inetsoft-technology/stylebi/edit/main/README.md#quickstart).

## Experimental best practices

When updating to an experimental nightly build, it is recommended to tag the image within your Docker environment or store a copy in your own repository. Because StyleBI nightly builds are not officially archived, maintaining your own tagged versions ensures that you can roll back to a previous build if necessary.

See the following docker documentation page for more information on [tagging](https://docs.docker.com/get-started/docker-concepts/building-images/build-tag-and-publish-an-image/#tagging-images).

To restore a tagged image, update the image field in your docker-compose.yaml file to reference the desired tag.
