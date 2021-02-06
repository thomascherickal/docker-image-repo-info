## `influxdb:meta`

```console
$ docker pull influxdb@sha256:6857ed1b1ab8af5c645849ad8a6e8073a47e1fd98d7009620f4dcbdcb7852dac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:54976b70e19e5a1297aa3ad07007d043ff08019ec54f7a80cfb63eefea81272b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83859963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c224d5f496b04552b4b5da16bc49680e7cff5a9f97fc9eea2715b7beb821650`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Fri, 05 Feb 2021 22:20:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Feb 2021 22:20:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 06 Feb 2021 01:15:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 06 Feb 2021 01:16:40 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 06 Feb 2021 01:17:10 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 06 Feb 2021 01:17:10 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 06 Feb 2021 01:17:11 GMT
EXPOSE 8091
# Sat, 06 Feb 2021 01:17:11 GMT
VOLUME [/var/lib/influxdb]
# Sat, 06 Feb 2021 01:17:12 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 06 Feb 2021 01:17:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 06 Feb 2021 01:17:12 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ae0ade158685a8e718a6afd2289fa52e5c5a38342a07ad5e1b3b2fdd1c46bd`  
		Last Modified: Fri, 05 Feb 2021 22:27:08 GMT  
		Size: 11.3 MB (11268539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911674ee9a5463a175abbfc4306db7b2debd5f54db613c089a57891c574b105e`  
		Last Modified: Fri, 05 Feb 2021 22:27:07 GMT  
		Size: 4.3 MB (4341873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc1901fc424822bd4a3437531b99f24f26a03416663e188d00d59b48909241`  
		Last Modified: Sat, 06 Feb 2021 01:18:02 GMT  
		Size: 2.8 KB (2827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56e78934c5c6176b6fb9ff3ca579c9ab0d33579c4c51fbc0bef72204f10bc31`  
		Last Modified: Sat, 06 Feb 2021 01:19:58 GMT  
		Size: 22.9 MB (22866141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac35fcab466fb0c6b85aff9b153afce78b13c2c88e8378585cd7a4e12ae95970`  
		Last Modified: Sat, 06 Feb 2021 01:19:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ec37042a543b364b537d50c991df7378f3f05b2ed8d02c1baeffd7d7f0a64d`  
		Last Modified: Sat, 06 Feb 2021 01:19:53 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
