## `rethinkdb:latest`

```console
$ docker pull rethinkdb@sha256:3bddbf6732c70973145be6f9e5129398377ee6ce5461595caee491124a682ae2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:latest` - linux; amd64

```console
$ docker pull rethinkdb@sha256:805d290eddd0579b6db0ea8c87e03ef68ffb0cbef990a3e1278b64eae4c7520d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51838917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dba924599a6885e00488c7bd084e2ac902f9d995abbbff3a37df0d53adc3c9d5`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 06:07:11 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 06:07:46 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 02 Mar 2022 06:07:47 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 02 Mar 2022 06:07:54 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 06:07:54 GMT
VOLUME [/data]
# Wed, 02 Mar 2022 06:07:54 GMT
WORKDIR /data
# Wed, 02 Mar 2022 06:07:54 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 02 Mar 2022 06:07:54 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198fe77b0e22a0cb66b2ba2bdb069958bbc3dcc070be1c89f6a8beb8d40f0e25`  
		Last Modified: Wed, 02 Mar 2022 06:08:20 GMT  
		Size: 6.7 MB (6690995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e358a68c7b63335cba994b7388a6a013845c3142191307bfddf3be643df865a`  
		Last Modified: Wed, 02 Mar 2022 06:08:19 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be03d2533e80bd03b652680ef73021377c60951f4527adc8cb057dc0dee6d1c5`  
		Last Modified: Wed, 02 Mar 2022 06:08:22 GMT  
		Size: 18.0 MB (17991445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c22aa4a42b241daadb84b3edf4e646c71cb5b273671789b2c65ea716e459cb3`  
		Last Modified: Wed, 02 Mar 2022 06:08:19 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
