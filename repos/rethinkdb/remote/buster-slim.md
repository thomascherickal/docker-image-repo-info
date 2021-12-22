## `rethinkdb:buster-slim`

```console
$ docker pull rethinkdb@sha256:f7be561841c9d70935ee50ac160db4385d33510d3b6ec95e94a7f4d1ef313bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:569b037f4a268321ca526796ea7aeed4c7c08930506c79cb1ac1b66e789ba11e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51839003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e6c6ce395fee7a1c0ed6b4c68e561b3795ce941ad1c051f0c569599cb74230c`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:43:39 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:43:47 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 21 Dec 2021 23:43:47 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 21 Dec 2021 23:43:55 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:43:55 GMT
VOLUME [/data]
# Tue, 21 Dec 2021 23:43:55 GMT
WORKDIR /data
# Tue, 21 Dec 2021 23:43:55 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 21 Dec 2021 23:43:56 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d0d022cf11dc1fdbea4c8f72c0232730f74ff7dfcd147c2c9488cc7a65bd61`  
		Last Modified: Tue, 21 Dec 2021 23:44:17 GMT  
		Size: 6.7 MB (6691023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a36faa79d43961aeabc1583aac4011cff7ba5a107de34460818b238ad8e4dc3`  
		Last Modified: Tue, 21 Dec 2021 23:44:16 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95281dc1ae7e6e3fcef2e3bf1c7f41dd133030fbb91c1796a7a1f3d571cd98df`  
		Last Modified: Tue, 21 Dec 2021 23:44:19 GMT  
		Size: 18.0 MB (17991518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf90828cab3a406b776760a5321026e3f6a3093fb9f9c0f75263a8d8c9ecd0ce`  
		Last Modified: Tue, 21 Dec 2021 23:44:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
