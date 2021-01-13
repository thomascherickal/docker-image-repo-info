## `influxdb:data`

```console
$ docker pull influxdb@sha256:4c1bd2ee5ba7f9e01cadefea4164dfa0bdbd3e82cd8291cd31df68d82337e49e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:6bc15e4a75c9684a6ef0139238a287208c53dfdc8c91830fa43b922cad6573db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126274764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be72aabcc2fd4ee36d13754f7937cc7942ece058b2c52bf959d45701435963f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

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
# Wed, 13 Jan 2021 00:04:22 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 13 Jan 2021 00:04:22 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 13 Jan 2021 00:04:22 GMT
EXPOSE 8086
# Wed, 13 Jan 2021 00:04:23 GMT
VOLUME [/var/lib/influxdb]
# Wed, 13 Jan 2021 00:04:23 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 13 Jan 2021 00:04:23 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 13 Jan 2021 00:04:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 00:04:23 GMT
CMD ["influxd"]
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
	-	`sha256:1f4f755c567c9075b10a4d2dad23b6259b9f74f950b30702870b7fd5f22f207d`  
		Last Modified: Wed, 13 Jan 2021 00:06:47 GMT  
		Size: 65.8 MB (65796040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af56dbdfb959bc175e19e02e385256411532c466cf823f9ae275a2aae132e803`  
		Last Modified: Wed, 13 Jan 2021 00:06:38 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66739de46fcc7a9558a23910ea67bf75e004dfaef28a86e0261d9e030fa4b957`  
		Last Modified: Wed, 13 Jan 2021 00:06:38 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de770c28159550010c7f8c678d078ee02d27909163c1233c60dab0d2046b1fb8`  
		Last Modified: Wed, 13 Jan 2021 00:06:40 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
