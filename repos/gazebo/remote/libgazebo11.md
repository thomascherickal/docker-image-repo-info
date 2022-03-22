## `gazebo:libgazebo11`

```console
$ docker pull gazebo@sha256:fafb858af1a6bc481a0238badf4d4499579803d1cd76c4262014ea7cec5aeace
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo11` - linux; amd64

```console
$ docker pull gazebo@sha256:bd6817ba66e24e11055f36a0406b9b493655c2c51cfeb40c8a4a85f7812bf540
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.1 MB (610089549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8065fe17f60faa5f0d819b18328c5b56fa12d55d2689b31666529af5ef3fa99`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 21 Mar 2022 21:32:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Mon, 21 Mar 2022 21:32:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Mon, 21 Mar 2022 21:32:14 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Mon, 21 Mar 2022 21:35:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 21 Mar 2022 21:35:16 GMT
EXPOSE 11345
# Mon, 21 Mar 2022 21:35:17 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Mon, 21 Mar 2022 21:35:17 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Mon, 21 Mar 2022 21:35:17 GMT
CMD ["gzserver"]
# Mon, 21 Mar 2022 21:39:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.10.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035b6689c6ca0e98debb81a680ccfb6d099d5a0d25325e1c0a590d787f8174b`  
		Last Modified: Mon, 21 Mar 2022 21:41:33 GMT  
		Size: 16.2 MB (16170793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8e38426b469013d78c97d0a9e8df53401d6f7fc27ccf5bd199135f371de09`  
		Last Modified: Mon, 21 Mar 2022 21:41:30 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e36cc5650761261ef8d96767e16f421b018afe8f984c68ea2d537f92a329408`  
		Last Modified: Mon, 21 Mar 2022 21:41:30 GMT  
		Size: 5.5 KB (5501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6d35042788c1ca0a638153ec14b3d88e1cc4ec53d02fc42b82fcff663bde12`  
		Last Modified: Mon, 21 Mar 2022 21:42:03 GMT  
		Size: 275.9 MB (275856642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cb954b0062e844e9a2a30e8e2da6567d85ff01b69ffdfda06d45aa1b30605c`  
		Last Modified: Mon, 21 Mar 2022 21:41:30 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cb368f574453687f3be5947ed0be869a0791d952270f236f5e40d952a906bc`  
		Last Modified: Mon, 21 Mar 2022 21:43:00 GMT  
		Size: 288.3 MB (288306746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
