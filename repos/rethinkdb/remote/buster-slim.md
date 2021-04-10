## `rethinkdb:buster-slim`

```console
$ docker pull rethinkdb@sha256:ef228aaa7f72799c143b5eecc5a0fa2bfabfdaea31ceefa5bb27b7da25645290
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:87b9e743d853c86cd2998223eb8badb5852a2de294d02f186d3f15b5314b71fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51824125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4250c5b26ae2ca851263ba2ebaa677466e42fed8cf45ebe581945d0bc3fc1f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:10:24 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:27 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 10 Apr 2021 17:10:28 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Sat, 10 Apr 2021 17:10:34 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:35 GMT
VOLUME [/data]
# Sat, 10 Apr 2021 17:10:35 GMT
WORKDIR /data
# Sat, 10 Apr 2021 17:10:35 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 10 Apr 2021 17:10:35 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e36f66c1815fb7b7ac84f2e19aaad0b7a00fdb61921150d29feab40023fde1c`  
		Last Modified: Sat, 10 Apr 2021 17:11:23 GMT  
		Size: 6.7 MB (6690291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b4f8dfad448c8753fff951042f3d7f0346ad2cd3a116cfbb39d3b0db993c`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fcc47b42337170ffdce3d5d3edc1913ae6d1f4d0960f973b0bcbc609f4f79`  
		Last Modified: Sat, 10 Apr 2021 17:11:19 GMT  
		Size: 18.0 MB (17991722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef48c89b3b8060a67e31c4182e08fba291533418ea7829341843ce728f24ab4`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
