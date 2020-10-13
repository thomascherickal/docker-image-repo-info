## `rethinkdb:2-buster-slim`

```console
$ docker pull rethinkdb@sha256:7e85ad23b6382fbb83af993a65b37ef60a7e57a38195482ebd6c7e3634f74bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:82ab41f04983eb23c0cbccc2d5ecfb111c31b140b65d6fade4c2dfbd10b9d027
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51754789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc02d43272252404086d84ffbb128e9f8ebcbef2bb3b685a6f5f141a7e72c764`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:04:35 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Oct 2020 22:04:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 13 Oct 2020 22:04:45 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:46 GMT
VOLUME [/data]
# Tue, 13 Oct 2020 22:04:46 GMT
WORKDIR /data
# Tue, 13 Oct 2020 22:04:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Oct 2020 22:04:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ff2d863f5cb64cbf6e74cad8f981b6b9b5a3dfd323a549059ed3fe391221`  
		Last Modified: Tue, 13 Oct 2020 22:05:23 GMT  
		Size: 6.7 MB (6669162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e76d8854d8cc50116145a95caaaedc2d267de5c7680bd1ce2e695d5180de76`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84795ccb1d288c022adb90fd10839a7de78e636e0546c739e3dad1055cee0e4f`  
		Last Modified: Tue, 13 Oct 2020 22:05:27 GMT  
		Size: 18.0 MB (17990695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71976fa1d68a93d177f7529f95d65759cf1f0b6035e836d149fcda592c9b80b`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
