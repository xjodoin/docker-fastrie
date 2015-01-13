docker-fastrie
==============

Automated Docker build of the fastrie repository. Mainly a proof of concept for now, but should work well based on
the build instructions at https://github.com/dave-andersen/fastrie.

Use the following command to start the container:

<pre>
docker run -d -name docker-fastrie arbedout/docker-fastrie /bin/bash 
-c "/usr/src/fastrie/xptMiner/xptminer -u username.riecoinworkername -p workerpassword"
</pre>

and file an issue if you have any difficulties. Note that we're using our own repository for the fastrie minor as we needed to modify the Makefile to avoid illegal instruction errors on compilation.
