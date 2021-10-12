## `influxdb:data`

```console
$ docker pull influxdb@sha256:d04305dd8914c486e8ef3cbbcff811e54dc1738f4884be67bfcedcf4d15ae1f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:e7373d5b9b5c8427e7a920a37b66f0ab1576f3f9518ff1b837f60cc3027b79dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117733109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5698a773c4695af4f07c5c0048e86a2e902ec64cf473a5ccdec1af1a63d42b5b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 11 Oct 2021 23:20:26 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:20:32 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 11 Oct 2021 23:20:33 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:33 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:33 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:33 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:34 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe16c0b4bccccde6eb4a50c0557b13eaaba0dcc8c57e1214aa71f37724941f5`  
		Last Modified: Mon, 11 Oct 2021 23:23:02 GMT  
		Size: 56.7 MB (56708535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a832d21088fde43f8d6f8441268e6b19f9955d93fd2a4508973fe5cdd0a5558e`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793aaa7ad592f4bd291349c0afc6a3318bcd6f983d80f1909bbae21463cc3249`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6d48653c4e7352a26c96597a08281723742b610a46ec26a03b86beafe16e58`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
