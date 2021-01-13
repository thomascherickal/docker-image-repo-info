## `influxdb:meta`

```console
$ docker pull influxdb@sha256:9e9b31d8677be4038d762b0e43d48a0e27c2a4686106b953998652b4e1a05e0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:22696dca2b75eec6349db3306e3bffb1a0af61f153615cd0cff50c5da88198c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83342810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34664e75a6f5189c4944b76eed173f9f01af274fdbb263cc2444bc9d78dced2f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 04:00:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 04:00:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jan 2021 00:03:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 Jan 2021 00:04:14 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Wed, 13 Jan 2021 00:04:35 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 13 Jan 2021 00:04:35 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 13 Jan 2021 00:04:35 GMT
EXPOSE 8091
# Wed, 13 Jan 2021 00:04:36 GMT
VOLUME [/var/lib/influxdb]
# Wed, 13 Jan 2021 00:04:36 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 13 Jan 2021 00:04:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 00:04:36 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953fe5c215cb5f929e0e42e5a1011f33edce9278a650faf10655e855a670f79f`  
		Last Modified: Tue, 12 Jan 2021 04:08:01 GMT  
		Size: 10.8 MB (10753468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3f270c7deffd353181076af3b5746c8dbeac5abf454169a75e7822587bdab`  
		Last Modified: Tue, 12 Jan 2021 04:07:59 GMT  
		Size: 4.3 MB (4340646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81696497404d5b0c28802af968f980fe26d1a5ad4f1336891f53d07cea78c20`  
		Last Modified: Wed, 13 Jan 2021 00:05:21 GMT  
		Size: 2.8 KB (2824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007ad2855e3b28cd6d6ce1d5c82c3626a02a6a4c7000b28150e9a981bad90fa4`  
		Last Modified: Wed, 13 Jan 2021 00:07:05 GMT  
		Size: 22.9 MB (22865288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db497bd2e183f923eb15bc9a2f89d4f4be4d9c6c1de0a1264ca0f8f8ecf6d4`  
		Last Modified: Wed, 13 Jan 2021 00:06:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b46eb21a0f86104e62322809b7c1262ed8aa0ca497027196225bc234df470`  
		Last Modified: Wed, 13 Jan 2021 00:06:59 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
