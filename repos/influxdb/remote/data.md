## `influxdb:data`

```console
$ docker pull influxdb@sha256:a4d3c557c4391396d9eb233be35ec7c800a2c86b1a5fe34a54f95469aa49fd62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:0ecefccc269ab3f8982b45cf7c2ed7bf72ce2606f5c2f91b4e883324f369ac7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127524175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:782c8bead734acc5b192904fe9044b87fbef97e4d3b0d666f0616b6fe8b53b64`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 06:38:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 06:39:07 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Tue, 13 Jun 2023 06:39:18 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:39:18 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 13 Jun 2023 06:39:18 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 06:39:18 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:18 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:18 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 13 Jun 2023 06:39:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:18 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c9d07816682d141bc7609d0f37dc41c4a0ac99872a890541f9af74b09a55de`  
		Last Modified: Tue, 13 Jun 2023 06:40:50 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d592531342e8fbc257855e7dc977015fdc7d3cc4496f27a26e6682cd94bc5`  
		Last Modified: Tue, 13 Jun 2023 06:41:12 GMT  
		Size: 56.7 MB (56705099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3c1c1ee755486cae393e84464b6b00201f7bed92b87c1e8f4966b94af9a2e3`  
		Last Modified: Tue, 13 Jun 2023 06:41:05 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a60bca78e208c06956474dddb2d6beea9523af042f35381396d2cc5c784738`  
		Last Modified: Tue, 13 Jun 2023 06:41:05 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b347ac16f3ddb18e8a04ce0b844c67a326be1ea635a164c9fd15d11dac2b9edc`  
		Last Modified: Tue, 13 Jun 2023 06:41:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
