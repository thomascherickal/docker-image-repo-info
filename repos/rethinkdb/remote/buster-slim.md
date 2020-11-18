## `rethinkdb:buster-slim`

```console
$ docker pull rethinkdb@sha256:17401c1edbafb8cc807fdc44016e556de7b686c35d86045fa1a4234b5857281d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a5b1c585ce5a5c45ae362bb92f1eea1a653f4326acfce1f76f26231a26722d25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51768068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5dd5b23cd2539cb34f37912ecc325d0cf53b2a905def5ac15dcb9a4ace4144f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:22:30 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:34 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 18 Nov 2020 12:22:34 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 18 Nov 2020 12:22:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:47 GMT
VOLUME [/data]
# Wed, 18 Nov 2020 12:22:47 GMT
WORKDIR /data
# Wed, 18 Nov 2020 12:22:47 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 18 Nov 2020 12:22:48 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447f5e1357f860f3451dcd3ab5cfe3c128cd2fece1ee9a36d64ad1609b4b5c3`  
		Last Modified: Wed, 18 Nov 2020 12:23:49 GMT  
		Size: 6.7 MB (6669182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e01b054557acaca0b77b081da248dd2c131f0976518577554f266a5cdf3cc3`  
		Last Modified: Wed, 18 Nov 2020 12:23:47 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e161d64e52b40a0973d2b765dd9d1fe8e69f825cccbc28eb1b76aed57c764d98`  
		Last Modified: Wed, 18 Nov 2020 12:23:51 GMT  
		Size: 18.0 MB (17990696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a53590d415b928b049c7903ed1b598541c171689418d6b6b775e94c49548d`  
		Last Modified: Wed, 18 Nov 2020 12:23:48 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
