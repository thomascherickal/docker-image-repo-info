## `influxdb:data`

```console
$ docker pull influxdb@sha256:981102d27aad76c76b325c8f861ecac6db0aca6749fac3f402a35703b8ea644e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:a3d956523801f10660895a4085efba4745af3de84aa21e4b3c5463d3cedff712
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127804235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19b7965fdf4b5c6003b4fd2aa8d5bc50e628cb61e446f1c6171eb1aa2346bf64`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 24 Jun 2021 01:32:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 24 Jun 2021 01:33:47 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Thu, 24 Jun 2021 01:33:54 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 24 Jun 2021 01:33:54 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 24 Jun 2021 01:33:55 GMT
EXPOSE 8086
# Thu, 24 Jun 2021 01:33:55 GMT
VOLUME [/var/lib/influxdb]
# Thu, 24 Jun 2021 01:33:55 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 24 Jun 2021 01:33:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 24 Jun 2021 01:33:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 24 Jun 2021 01:33:56 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817e62a1a541a16e30de932a8d4c9a537b6aac51f5aa2ae2a6a4ac1fe20a5b53`  
		Last Modified: Thu, 24 Jun 2021 01:35:08 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36963b11b4b3308ec531fa72638249443c08ff61aeb5fa0994fc8525eeea07ac`  
		Last Modified: Thu, 24 Jun 2021 01:36:41 GMT  
		Size: 66.8 MB (66782661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1b51137d5e983d9b537482b7d629f6c58c496667c60db7b650799caf4ac3d4`  
		Last Modified: Thu, 24 Jun 2021 01:36:32 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3bb89c6c2062f5225f802e01c306dcfabc37971b3af8ee87671945aa421394`  
		Last Modified: Thu, 24 Jun 2021 01:36:32 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c041e8cb994983dc6daa9b810a296032e3043f9fb643fd18d51102c4e149d36`  
		Last Modified: Thu, 24 Jun 2021 01:36:32 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
