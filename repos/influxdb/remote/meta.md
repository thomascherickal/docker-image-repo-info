## `influxdb:meta`

```console
$ docker pull influxdb@sha256:31500f40ed7a50fdb52e8a0990aea86bd8c0f50814d644754a9f57c35fca7ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:64534669863b8e1414ac4aa65a41d124604e61f8b9ce42b31e297cb2a8d15987
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84443975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6befdf4bac0b404e5ad4274eafa07f36729725f56bef2f3ae11f41259f0cc59d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:44:42 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 18 Nov 2021 09:45:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:45:05 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 18 Nov 2021 09:45:05 GMT
EXPOSE 8091
# Thu, 18 Nov 2021 09:45:05 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:45:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:45:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:45:06 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64521abd18cf018ab9316be9ab482c503cb3c6b8adeb380319d51c18556be12e`  
		Last Modified: Thu, 18 Nov 2021 09:49:24 GMT  
		Size: 23.4 MB (23416332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82be31c0c04837996a2f891230ea306a73ed63264076a52cff01efbae7234c49`  
		Last Modified: Thu, 18 Nov 2021 09:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6ebc4c9a6547fd06dd99b1c765524dfdd7a939834caad7a1fac1b01c95d3bd`  
		Last Modified: Thu, 18 Nov 2021 09:49:20 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
