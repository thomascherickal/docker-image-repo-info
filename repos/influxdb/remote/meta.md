## `influxdb:meta`

```console
$ docker pull influxdb@sha256:201f64235273243359924d5f0b3ddac5160f554f7c501bb4e77a1043dec7f81d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:4863331c29f334af2347a7439230a5251da56d286b11e5fd62375a3446a9e01c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83448884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4d01e587d1e576a83d4d32427b9c089b4fd4f899f9e0ff470293298e5beeea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:22 GMT
ADD file:9f6f0c8b90de3204ad5db95d10d8aa76b42454def6ac811c888ad4e274292c9c in / 
# Thu, 16 Apr 2020 03:27:22 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:12:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:12:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 17 Apr 2020 07:07:19 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 17 Apr 2020 07:08:22 GMT
ENV INFLUXDB_VERSION=1.8.0-c1.8.0
# Fri, 17 Apr 2020 07:08:40 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 17 Apr 2020 07:08:40 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 17 Apr 2020 07:08:41 GMT
EXPOSE 8091
# Fri, 17 Apr 2020 07:08:41 GMT
VOLUME [/var/lib/influxdb]
# Fri, 17 Apr 2020 07:08:41 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 17 Apr 2020 07:08:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Apr 2020 07:08:41 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:7568c21980bd8003ca9d23a218302c6386aac91e069cc0c0be6bedf45476f056`  
		Last Modified: Thu, 16 Apr 2020 03:34:47 GMT  
		Size: 45.4 MB (45375910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9f2207c812b2530bc06352aa57cf50244726c52db6ff775ca9f9a76d6ea880`  
		Last Modified: Thu, 16 Apr 2020 04:20:21 GMT  
		Size: 10.8 MB (10797394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe350d2b14088b19ffff7a1c6683f0949fb0161e6ab87011a24e21e5d7fed4e`  
		Last Modified: Thu, 16 Apr 2020 04:20:19 GMT  
		Size: 4.3 MB (4340188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde77fc2d07196ffcbb2d5dcd967e70909969f23ca388558027fa4881c56566c`  
		Last Modified: Fri, 17 Apr 2020 07:08:59 GMT  
		Size: 2.8 KB (2771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61660e6612b29d8ccd3e59e108ecd8be4abe4464afa3851743be77399529cc7b`  
		Last Modified: Fri, 17 Apr 2020 07:10:21 GMT  
		Size: 22.9 MB (22932049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0235ad68ecddc19482232ee14b81a844a51db8e9e44d78e3d548cbe0dd4845`  
		Last Modified: Fri, 17 Apr 2020 07:10:17 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284b061eaef4973844861a9eb67e9eea042eac875ed9fea243101bf3cdb7aa20`  
		Last Modified: Fri, 17 Apr 2020 07:10:17 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
