<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `influxdb`

-	[`influxdb:1.10-data`](#influxdb110-data)
-	[`influxdb:1.10-data-alpine`](#influxdb110-data-alpine)
-	[`influxdb:1.10-meta`](#influxdb110-meta)
-	[`influxdb:1.10-meta-alpine`](#influxdb110-meta-alpine)
-	[`influxdb:1.10.3-data`](#influxdb1103-data)
-	[`influxdb:1.10.3-data-alpine`](#influxdb1103-data-alpine)
-	[`influxdb:1.10.3-meta`](#influxdb1103-meta)
-	[`influxdb:1.10.3-meta-alpine`](#influxdb1103-meta-alpine)
-	[`influxdb:1.8`](#influxdb18)
-	[`influxdb:1.8-alpine`](#influxdb18-alpine)
-	[`influxdb:1.8-data`](#influxdb18-data)
-	[`influxdb:1.8-data-alpine`](#influxdb18-data-alpine)
-	[`influxdb:1.8-meta`](#influxdb18-meta)
-	[`influxdb:1.8-meta-alpine`](#influxdb18-meta-alpine)
-	[`influxdb:1.8.10`](#influxdb1810)
-	[`influxdb:1.8.10-alpine`](#influxdb1810-alpine)
-	[`influxdb:1.8.10-data`](#influxdb1810-data)
-	[`influxdb:1.8.10-data-alpine`](#influxdb1810-data-alpine)
-	[`influxdb:1.8.10-meta`](#influxdb1810-meta)
-	[`influxdb:1.8.10-meta-alpine`](#influxdb1810-meta-alpine)
-	[`influxdb:1.9-data`](#influxdb19-data)
-	[`influxdb:1.9-data-alpine`](#influxdb19-data-alpine)
-	[`influxdb:1.9-meta`](#influxdb19-meta)
-	[`influxdb:1.9-meta-alpine`](#influxdb19-meta-alpine)
-	[`influxdb:1.9.11-data`](#influxdb1911-data)
-	[`influxdb:1.9.11-data-alpine`](#influxdb1911-data-alpine)
-	[`influxdb:1.9.11-meta`](#influxdb1911-meta)
-	[`influxdb:1.9.11-meta-alpine`](#influxdb1911-meta-alpine)
-	[`influxdb:2.7`](#influxdb27)
-	[`influxdb:2.7-alpine`](#influxdb27-alpine)
-	[`influxdb:2.7.1`](#influxdb271)
-	[`influxdb:2.7.1-alpine`](#influxdb271-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.10-data`

```console
$ docker pull influxdb@sha256:16f8b28bc4fe11a9b425118d0b7512207e63f5b28df3bd06e04a4d656ea0e670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:d437bef4e11ddb812b22aa440cda87c5df6bff75d43212743de540a824fa2f32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110885629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b3301227100c06c8a2a11c783e468300d99373fcdae972ac5a842e3443af166`
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
# Tue, 13 Jun 2023 06:39:49 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Tue, 13 Jun 2023 06:39:54 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:39:54 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 13 Jun 2023 06:39:54 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 06:39:54 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 13 Jun 2023 06:39:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:55 GMT
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
	-	`sha256:b06b2af7278cc24339b9c112d4bc1c630c365c412f5387e5fd8e27fdc7d0e0d1`  
		Last Modified: Tue, 13 Jun 2023 06:42:04 GMT  
		Size: 40.1 MB (40066550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2623f3783dd24d1bf884c15076dfd1f5060c523c3f7c122c2b1e75c6d628c5`  
		Last Modified: Tue, 13 Jun 2023 06:41:58 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5378ab5bfc706810fc27a919b43ff42aedadc2580d3dfb06a6f4e8c9ebcc420c`  
		Last Modified: Tue, 13 Jun 2023 06:41:58 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91c5c0b77c2ee31603071911e68153e43be67961fb4c8d5c28abe8d3ea3cbd6`  
		Last Modified: Tue, 13 Jun 2023 06:41:58 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-data-alpine`

```console
$ docker pull influxdb@sha256:4256026ced6a674c11e9cbb5916f85dfb73632f2b833fe428d21dfe117e4c8e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:36001c5575829c1123c780bb4648039e4d7b2e862f43bc5b832f6a1bece91f11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44875176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:519e3fd8737778dee854382543f970556cbd1cf3be477f435752f7db74742066`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 17 Apr 2023 22:40:32 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Mon, 17 Apr 2023 22:40:38 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 17 Apr 2023 22:40:38 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 17 Apr 2023 22:40:39 GMT
EXPOSE 8086
# Mon, 17 Apr 2023 22:40:39 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:39 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 17 Apr 2023 22:40:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:39 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51913dd07d90ac6d253a453fc1b3620587fdd325300225b5af43cbddf520f18`  
		Last Modified: Mon, 17 Apr 2023 22:42:40 GMT  
		Size: 40.0 MB (40026472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fdda652573b5764017cdccbbf0ac08937ce1ef39ce25cc481a3b779a4e80a3`  
		Last Modified: Mon, 17 Apr 2023 22:42:34 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d2e3246ce58b81d42293a4610c3b572b694dde5db71b80ef0fd08dceeb509e`  
		Last Modified: Mon, 17 Apr 2023 22:42:34 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977542182f1e2457f40c37f57d386920c1614e860dbb901f480e7f16560c55a6`  
		Last Modified: Mon, 17 Apr 2023 22:42:34 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta`

```console
$ docker pull influxdb@sha256:f983efd0b04acd40f7dc162cb09adb815a1631a7348e73103e83efb9d80f2635
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:781906c97faef32538ee48a71e628de7c3b2d1fb6fa2aba7d1fb53a6b9eefd3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91051928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfc96138ae952179c5bd48ffc8a85edfd025df31bbe8a33184a2c07cb0f44e5a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 06:38:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 06:39:49 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Tue, 13 Jun 2023 06:40:03 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:40:03 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 13 Jun 2023 06:40:03 GMT
EXPOSE 8091
# Tue, 13 Jun 2023 06:40:04 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:40:04 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:40:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:40:04 GMT
CMD ["influxd-meta"]
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
	-	`sha256:397747ccded9c734da6ca692374a4144d3f734314bd55b7a78596e9510c92223`  
		Last Modified: Tue, 13 Jun 2023 06:42:15 GMT  
		Size: 20.2 MB (20234058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ade76d30436b374a5a7367b21d783ac2e47ff2e789bd80c5c1b8a1feb1a188c`  
		Last Modified: Tue, 13 Jun 2023 06:42:12 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9618c51bd8ae3e346b366fb345d316d08f2e5d5178a853dc0cb81c6b55b88fc`  
		Last Modified: Tue, 13 Jun 2023 06:42:12 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta-alpine`

```console
$ docker pull influxdb@sha256:01cef2781f742081583267d4aa4c37a6eeb492d772dccc5cc55eb4c5d9efbf61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9b456945f66833e2a533c8a33e1c38a44452d4d8138eadc280a3515244943f3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (25048154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592bced53f727226779f8723f98470008b04e543a196ca24bfa9e12f002693ac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 17 Apr 2023 22:40:32 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Mon, 17 Apr 2023 22:40:52 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 17 Apr 2023 22:40:52 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 17 Apr 2023 22:40:52 GMT
EXPOSE 8091
# Mon, 17 Apr 2023 22:40:52 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:53 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:53 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bee8161c601cd13ee9ba6482350fdbafe7284b7047998cb99f633301e56e4e`  
		Last Modified: Mon, 17 Apr 2023 22:43:04 GMT  
		Size: 20.2 MB (20200650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89224e710552d9d222bad854acde3d61ab225b5fe0257324075791f7f86e92e9`  
		Last Modified: Mon, 17 Apr 2023 22:43:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514771564dbcb811991a03ce5486d563216e01a84ff76d5432e7ae2800d22eb`  
		Last Modified: Mon, 17 Apr 2023 22:43:01 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.3-data`

```console
$ docker pull influxdb@sha256:16f8b28bc4fe11a9b425118d0b7512207e63f5b28df3bd06e04a4d656ea0e670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.3-data` - linux; amd64

```console
$ docker pull influxdb@sha256:d437bef4e11ddb812b22aa440cda87c5df6bff75d43212743de540a824fa2f32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110885629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b3301227100c06c8a2a11c783e468300d99373fcdae972ac5a842e3443af166`
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
# Tue, 13 Jun 2023 06:39:49 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Tue, 13 Jun 2023 06:39:54 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:39:54 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 13 Jun 2023 06:39:54 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 06:39:54 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 13 Jun 2023 06:39:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:55 GMT
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
	-	`sha256:b06b2af7278cc24339b9c112d4bc1c630c365c412f5387e5fd8e27fdc7d0e0d1`  
		Last Modified: Tue, 13 Jun 2023 06:42:04 GMT  
		Size: 40.1 MB (40066550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2623f3783dd24d1bf884c15076dfd1f5060c523c3f7c122c2b1e75c6d628c5`  
		Last Modified: Tue, 13 Jun 2023 06:41:58 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5378ab5bfc706810fc27a919b43ff42aedadc2580d3dfb06a6f4e8c9ebcc420c`  
		Last Modified: Tue, 13 Jun 2023 06:41:58 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91c5c0b77c2ee31603071911e68153e43be67961fb4c8d5c28abe8d3ea3cbd6`  
		Last Modified: Tue, 13 Jun 2023 06:41:58 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.3-data-alpine`

```console
$ docker pull influxdb@sha256:4256026ced6a674c11e9cbb5916f85dfb73632f2b833fe428d21dfe117e4c8e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.3-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:36001c5575829c1123c780bb4648039e4d7b2e862f43bc5b832f6a1bece91f11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44875176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:519e3fd8737778dee854382543f970556cbd1cf3be477f435752f7db74742066`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 17 Apr 2023 22:40:32 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Mon, 17 Apr 2023 22:40:38 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 17 Apr 2023 22:40:38 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 17 Apr 2023 22:40:39 GMT
EXPOSE 8086
# Mon, 17 Apr 2023 22:40:39 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:39 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 17 Apr 2023 22:40:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:39 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51913dd07d90ac6d253a453fc1b3620587fdd325300225b5af43cbddf520f18`  
		Last Modified: Mon, 17 Apr 2023 22:42:40 GMT  
		Size: 40.0 MB (40026472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fdda652573b5764017cdccbbf0ac08937ce1ef39ce25cc481a3b779a4e80a3`  
		Last Modified: Mon, 17 Apr 2023 22:42:34 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d2e3246ce58b81d42293a4610c3b572b694dde5db71b80ef0fd08dceeb509e`  
		Last Modified: Mon, 17 Apr 2023 22:42:34 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977542182f1e2457f40c37f57d386920c1614e860dbb901f480e7f16560c55a6`  
		Last Modified: Mon, 17 Apr 2023 22:42:34 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.3-meta`

```console
$ docker pull influxdb@sha256:f983efd0b04acd40f7dc162cb09adb815a1631a7348e73103e83efb9d80f2635
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.3-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:781906c97faef32538ee48a71e628de7c3b2d1fb6fa2aba7d1fb53a6b9eefd3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91051928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfc96138ae952179c5bd48ffc8a85edfd025df31bbe8a33184a2c07cb0f44e5a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 06:38:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 06:39:49 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Tue, 13 Jun 2023 06:40:03 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:40:03 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 13 Jun 2023 06:40:03 GMT
EXPOSE 8091
# Tue, 13 Jun 2023 06:40:04 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:40:04 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:40:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:40:04 GMT
CMD ["influxd-meta"]
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
	-	`sha256:397747ccded9c734da6ca692374a4144d3f734314bd55b7a78596e9510c92223`  
		Last Modified: Tue, 13 Jun 2023 06:42:15 GMT  
		Size: 20.2 MB (20234058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ade76d30436b374a5a7367b21d783ac2e47ff2e789bd80c5c1b8a1feb1a188c`  
		Last Modified: Tue, 13 Jun 2023 06:42:12 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9618c51bd8ae3e346b366fb345d316d08f2e5d5178a853dc0cb81c6b55b88fc`  
		Last Modified: Tue, 13 Jun 2023 06:42:12 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.3-meta-alpine`

```console
$ docker pull influxdb@sha256:01cef2781f742081583267d4aa4c37a6eeb492d772dccc5cc55eb4c5d9efbf61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.3-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9b456945f66833e2a533c8a33e1c38a44452d4d8138eadc280a3515244943f3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (25048154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592bced53f727226779f8723f98470008b04e543a196ca24bfa9e12f002693ac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 17 Apr 2023 22:40:32 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Mon, 17 Apr 2023 22:40:52 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 17 Apr 2023 22:40:52 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 17 Apr 2023 22:40:52 GMT
EXPOSE 8091
# Mon, 17 Apr 2023 22:40:52 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:53 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:53 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bee8161c601cd13ee9ba6482350fdbafe7284b7047998cb99f633301e56e4e`  
		Last Modified: Mon, 17 Apr 2023 22:43:04 GMT  
		Size: 20.2 MB (20200650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89224e710552d9d222bad854acde3d61ab225b5fe0257324075791f7f86e92e9`  
		Last Modified: Mon, 17 Apr 2023 22:43:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514771564dbcb811991a03ce5486d563216e01a84ff76d5432e7ae2800d22eb`  
		Last Modified: Mon, 17 Apr 2023 22:43:01 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:f6d4d2839c4b97fcbe3593a90d88e66703ff4ea2d40447be2617a0b4116493e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:9786c3b6c668d090c7063f60d89edb2c033976587ae3f7b23e9bce49b39f556a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125704752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45d257d75944e2a03433be269858a3ab969c78ddc802d71d4b81e1ebe316426a`
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
# Tue, 13 Jun 2023 06:38:58 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 13 Jun 2023 06:39:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 13 Jun 2023 06:39:03 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 13 Jun 2023 06:39:03 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 06:39:03 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:03 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:03 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 13 Jun 2023 06:39:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:03 GMT
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
	-	`sha256:73627d928d0bcb9962d8e678ee68fea1a269f74088acbd3c87b34862516cc39a`  
		Last Modified: Tue, 13 Jun 2023 06:40:57 GMT  
		Size: 54.9 MB (54885738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a97895a22daffc6abc6801b9f1cea3f9cbacc6c3d73e44cfc8b472e8673fb4`  
		Last Modified: Tue, 13 Jun 2023 06:40:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6691a9ab9d07cbc7fe621f36fcc7f1d60a01649da47cb798736ff9d4d32db36b`  
		Last Modified: Tue, 13 Jun 2023 06:40:50 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d25ad13ac5d14ff98f4150de091f7ba553423c97f98ead61c2517490f921751`  
		Last Modified: Tue, 13 Jun 2023 06:40:50 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:186689d7c4049260d9fccb9b08edd4b5f55fa3790a9b54939bd041464f2d7a88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116695238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ccccb09106e705087001c52b4ea509809ab73f41c36e87bdd12618d0f7cf55a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 23 May 2023 00:57:45 GMT
ADD file:d8748d34e524d93a6df76d2a8ea8ca32ca04897521719f9f1f2a88ec692dd69e in / 
# Tue, 23 May 2023 00:57:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 13:58:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 May 2023 13:58:29 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 23 May 2023 13:58:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 23 May 2023 13:58:34 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 23 May 2023 13:58:34 GMT
EXPOSE 8086
# Tue, 23 May 2023 13:58:35 GMT
VOLUME [/var/lib/influxdb]
# Tue, 23 May 2023 13:58:35 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 23 May 2023 13:58:35 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 23 May 2023 13:58:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 13:58:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:29949e2d07dd1e283862cb4c3d4ec3043f1d54a1ac59f7b7a998ed9038a0243c`  
		Last Modified: Tue, 23 May 2023 01:01:23 GMT  
		Size: 50.2 MB (50210000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf40f65a7bdc041e615a5825b6ae62227f6a7ceec53af9e210fb62293e0bd2`  
		Last Modified: Tue, 23 May 2023 10:04:45 GMT  
		Size: 14.9 MB (14868582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486549426e25d5b97a0fa2a63fcad2fe13e259007bb850898620070285428f6c`  
		Last Modified: Tue, 23 May 2023 13:58:42 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc12a93a223f546972e9f38632cf744468b71bb60c0b8258c62a6757704ce2c`  
		Last Modified: Tue, 23 May 2023 13:58:49 GMT  
		Size: 51.6 MB (51613143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d040126afec4093890fa87cba2a8c5adc8cedd22602a23f87ef12330da7caed4`  
		Last Modified: Tue, 23 May 2023 13:58:42 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2af18d07617ae9285e0190173d0575582616bf155c7c5f4dcef565022a0ab89`  
		Last Modified: Tue, 23 May 2023 13:58:42 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9355659a32224b2c2aba3c1153c7aea1fe5b7c8c1548b569096439cfed259358`  
		Last Modified: Tue, 23 May 2023 13:58:42 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:18f5a0116c226c5eab9ef38c0f7a6441a78d4d2b5578df6d608516c5660dbdda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120684264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e97439b4f9685f7188e8d17fbc6d3e7fb0da7336bc673a8e588dc0f4a59f0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:28:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 05:28:29 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 13 Jun 2023 05:28:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 13 Jun 2023 05:28:33 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 13 Jun 2023 05:28:33 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 05:28:33 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 05:28:34 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 13 Jun 2023 05:28:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 13 Jun 2023 05:28:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 05:28:34 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be6cbbcd08580c2a7d75d5dab3cf13339b9aa76188ed8e8c43a4bf320452e9b`  
		Last Modified: Tue, 13 Jun 2023 05:29:11 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fdc7ffdba83945c331ae30140bf42739cd8132530bb96d51a02fc7f0879343`  
		Last Modified: Tue, 13 Jun 2023 05:29:16 GMT  
		Size: 51.2 MB (51230050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd1ca690aac5ecd46663499a8c5d36737f2ea8aadf4e3e50d2fdc06bccf62cd`  
		Last Modified: Tue, 13 Jun 2023 05:29:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cecafe9addc5e4b8fbbb37d8701521536def5440574c01ad699ca755b684d6c`  
		Last Modified: Tue, 13 Jun 2023 05:29:11 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ef26059edd4fdd2cdc54b106347608c63f3a930553f82bc405134308ebb64f`  
		Last Modified: Tue, 13 Jun 2023 05:29:11 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:90b697d4b32da71fe361c126a10b750de906682555ba79818c7e0b218063d4c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d47f18f760acc211135a360e94268942bfbc8f3ed8f8c8667712767f311cefad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59495244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d918bc1feeef58203db58b5c00f0729fece29cbbb82b0381c1e8253c702c6737`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 21:58:39 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 29 Mar 2023 21:58:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 21:58:47 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 29 Mar 2023 21:58:47 GMT
EXPOSE 8086
# Wed, 29 Mar 2023 21:58:47 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Mar 2023 21:58:47 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 29 Mar 2023 21:58:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 29 Mar 2023 21:58:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 21:58:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda9e84a688a6ab52c0b7ded3beaa72ee135b535f1cfd57d2612300c053f9bb1`  
		Last Modified: Wed, 29 Mar 2023 22:01:04 GMT  
		Size: 54.6 MB (54646594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef72d41d728fe85f7eb05a25e3fae9f35dcf5827ac8ce524f8fe3c0228253959`  
		Last Modified: Wed, 29 Mar 2023 22:00:56 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83adaa25b3977861b23887b15fef66da416f82452418ef8105b4991c14e61303`  
		Last Modified: Wed, 29 Mar 2023 22:00:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ef0bbe69f83f8b5c0b8b1b564afd893482ebc34ce7f4e25189621713a5a3b1`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:a4d3c557c4391396d9eb233be35ec7c800a2c86b1a5fe34a54f95469aa49fd62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

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

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:f4bd05a5999e70974eb7cbbdd5906442e00931d94b37b0c75921832c8ef821c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:62264fc25317633f3eeedbccf78f6ed24719552a6ba3c1a24873335ac7452d20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61352415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c899524c343137f88073bb6cf5fb3fec60a14b665168584e5358b35a3732774f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 21:58:51 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 29 Mar 2023 21:58:59 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 21:58:59 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 29 Mar 2023 21:58:59 GMT
EXPOSE 8086
# Wed, 29 Mar 2023 21:58:59 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Mar 2023 21:58:59 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 29 Mar 2023 21:59:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 29 Mar 2023 21:59:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 21:59:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02516d8c55b0db59be8396fd753bf49b2941067b34ddb8fa0e3c0f6fb3b2b67a`  
		Last Modified: Wed, 29 Mar 2023 22:01:20 GMT  
		Size: 56.5 MB (56503710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffee1bc09b30b9683a0acf9fab57079713eb0fdc7a98fd65d2c634e30022f090`  
		Last Modified: Wed, 29 Mar 2023 22:01:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a563df1bf32f0c1127cc5f3bdd71d477e1cd9dbe08888e5b95ce6a825d0b7a2f`  
		Last Modified: Wed, 29 Mar 2023 22:01:13 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e7e9e92a23ad02049e7817d3fb044533ed427734531e4e797530630ef4335a`  
		Last Modified: Wed, 29 Mar 2023 22:01:13 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:2c8c7614714d9a06d763edfea8fa1aab6f8122e4f7de15205e1e44307174c459
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:bf1e545a6de716ea69c1030bb6c60f23821cac25eafaa61926f802ed9d033c9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94230635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2ec25a6c572ea425630cafa756a87ba035e880e6a05002d2f6d79231cb10eea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

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
# Tue, 13 Jun 2023 06:39:27 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:39:27 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 13 Jun 2023 06:39:27 GMT
EXPOSE 8091
# Tue, 13 Jun 2023 06:39:27 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:27 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:28 GMT
CMD ["influxd-meta"]
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
	-	`sha256:2273cff380bceea2d73c2f39770beb52c84a0e16f780ea173c3450f6a6c8500b`  
		Last Modified: Tue, 13 Jun 2023 06:41:25 GMT  
		Size: 23.4 MB (23412766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827cbbf29aa75e7b8b6a9e76ef25a0a84d38fe7b14fe681bde2074cd8d13d924`  
		Last Modified: Tue, 13 Jun 2023 06:41:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cfbbba820bd8a221143222ccd73e6bf3c73ad2b6a66847d466b1e00d007643`  
		Last Modified: Tue, 13 Jun 2023 06:41:23 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:194a713fa6ba49261a2f26a716ecd00d003f40816590b46e951cff0a327770e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:314ca1c6300ee8c6bb1b4d43d5aef05916ee674008b2f6ff955e70c5b45e8bcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28140962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c74605fdbfde7d4168bb2a2c833947d1c6ce587d48f9c9440d1d82c5a7e0b4b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 21:58:51 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 29 Mar 2023 21:59:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 21:59:10 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 29 Mar 2023 21:59:10 GMT
EXPOSE 8091
# Wed, 29 Mar 2023 21:59:10 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Mar 2023 21:59:10 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 29 Mar 2023 21:59:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 21:59:11 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd5a97558827d022b888dd08ed218825a01293d976efdf8c79fd06b4ad855f5`  
		Last Modified: Wed, 29 Mar 2023 22:01:35 GMT  
		Size: 23.3 MB (23293462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bec4b2874a0829997c1b4c248d9d5ccfdb01fc8363fcc347c936df50e3859c`  
		Last Modified: Wed, 29 Mar 2023 22:01:32 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e542b866df0708d65bbb8968c7c641e8c19eac04855e4c4c6b53bc30dc397ff`  
		Last Modified: Wed, 29 Mar 2023 22:01:32 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10`

```console
$ docker pull influxdb@sha256:f6d4d2839c4b97fcbe3593a90d88e66703ff4ea2d40447be2617a0b4116493e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:9786c3b6c668d090c7063f60d89edb2c033976587ae3f7b23e9bce49b39f556a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125704752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45d257d75944e2a03433be269858a3ab969c78ddc802d71d4b81e1ebe316426a`
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
# Tue, 13 Jun 2023 06:38:58 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 13 Jun 2023 06:39:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 13 Jun 2023 06:39:03 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 13 Jun 2023 06:39:03 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 06:39:03 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:03 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:03 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 13 Jun 2023 06:39:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:03 GMT
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
	-	`sha256:73627d928d0bcb9962d8e678ee68fea1a269f74088acbd3c87b34862516cc39a`  
		Last Modified: Tue, 13 Jun 2023 06:40:57 GMT  
		Size: 54.9 MB (54885738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a97895a22daffc6abc6801b9f1cea3f9cbacc6c3d73e44cfc8b472e8673fb4`  
		Last Modified: Tue, 13 Jun 2023 06:40:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6691a9ab9d07cbc7fe621f36fcc7f1d60a01649da47cb798736ff9d4d32db36b`  
		Last Modified: Tue, 13 Jun 2023 06:40:50 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d25ad13ac5d14ff98f4150de091f7ba553423c97f98ead61c2517490f921751`  
		Last Modified: Tue, 13 Jun 2023 06:40:50 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:186689d7c4049260d9fccb9b08edd4b5f55fa3790a9b54939bd041464f2d7a88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116695238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ccccb09106e705087001c52b4ea509809ab73f41c36e87bdd12618d0f7cf55a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 23 May 2023 00:57:45 GMT
ADD file:d8748d34e524d93a6df76d2a8ea8ca32ca04897521719f9f1f2a88ec692dd69e in / 
# Tue, 23 May 2023 00:57:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 13:58:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 May 2023 13:58:29 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 23 May 2023 13:58:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 23 May 2023 13:58:34 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 23 May 2023 13:58:34 GMT
EXPOSE 8086
# Tue, 23 May 2023 13:58:35 GMT
VOLUME [/var/lib/influxdb]
# Tue, 23 May 2023 13:58:35 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 23 May 2023 13:58:35 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 23 May 2023 13:58:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 13:58:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:29949e2d07dd1e283862cb4c3d4ec3043f1d54a1ac59f7b7a998ed9038a0243c`  
		Last Modified: Tue, 23 May 2023 01:01:23 GMT  
		Size: 50.2 MB (50210000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf40f65a7bdc041e615a5825b6ae62227f6a7ceec53af9e210fb62293e0bd2`  
		Last Modified: Tue, 23 May 2023 10:04:45 GMT  
		Size: 14.9 MB (14868582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486549426e25d5b97a0fa2a63fcad2fe13e259007bb850898620070285428f6c`  
		Last Modified: Tue, 23 May 2023 13:58:42 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc12a93a223f546972e9f38632cf744468b71bb60c0b8258c62a6757704ce2c`  
		Last Modified: Tue, 23 May 2023 13:58:49 GMT  
		Size: 51.6 MB (51613143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d040126afec4093890fa87cba2a8c5adc8cedd22602a23f87ef12330da7caed4`  
		Last Modified: Tue, 23 May 2023 13:58:42 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2af18d07617ae9285e0190173d0575582616bf155c7c5f4dcef565022a0ab89`  
		Last Modified: Tue, 23 May 2023 13:58:42 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9355659a32224b2c2aba3c1153c7aea1fe5b7c8c1548b569096439cfed259358`  
		Last Modified: Tue, 23 May 2023 13:58:42 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:18f5a0116c226c5eab9ef38c0f7a6441a78d4d2b5578df6d608516c5660dbdda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120684264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e97439b4f9685f7188e8d17fbc6d3e7fb0da7336bc673a8e588dc0f4a59f0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:28:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 05:28:29 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 13 Jun 2023 05:28:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 13 Jun 2023 05:28:33 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 13 Jun 2023 05:28:33 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 05:28:33 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 05:28:34 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 13 Jun 2023 05:28:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 13 Jun 2023 05:28:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 05:28:34 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be6cbbcd08580c2a7d75d5dab3cf13339b9aa76188ed8e8c43a4bf320452e9b`  
		Last Modified: Tue, 13 Jun 2023 05:29:11 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fdc7ffdba83945c331ae30140bf42739cd8132530bb96d51a02fc7f0879343`  
		Last Modified: Tue, 13 Jun 2023 05:29:16 GMT  
		Size: 51.2 MB (51230050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd1ca690aac5ecd46663499a8c5d36737f2ea8aadf4e3e50d2fdc06bccf62cd`  
		Last Modified: Tue, 13 Jun 2023 05:29:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cecafe9addc5e4b8fbbb37d8701521536def5440574c01ad699ca755b684d6c`  
		Last Modified: Tue, 13 Jun 2023 05:29:11 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ef26059edd4fdd2cdc54b106347608c63f3a930553f82bc405134308ebb64f`  
		Last Modified: Tue, 13 Jun 2023 05:29:11 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-alpine`

```console
$ docker pull influxdb@sha256:90b697d4b32da71fe361c126a10b750de906682555ba79818c7e0b218063d4c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d47f18f760acc211135a360e94268942bfbc8f3ed8f8c8667712767f311cefad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59495244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d918bc1feeef58203db58b5c00f0729fece29cbbb82b0381c1e8253c702c6737`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 21:58:39 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 29 Mar 2023 21:58:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 21:58:47 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 29 Mar 2023 21:58:47 GMT
EXPOSE 8086
# Wed, 29 Mar 2023 21:58:47 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Mar 2023 21:58:47 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 29 Mar 2023 21:58:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 29 Mar 2023 21:58:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 21:58:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda9e84a688a6ab52c0b7ded3beaa72ee135b535f1cfd57d2612300c053f9bb1`  
		Last Modified: Wed, 29 Mar 2023 22:01:04 GMT  
		Size: 54.6 MB (54646594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef72d41d728fe85f7eb05a25e3fae9f35dcf5827ac8ce524f8fe3c0228253959`  
		Last Modified: Wed, 29 Mar 2023 22:00:56 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83adaa25b3977861b23887b15fef66da416f82452418ef8105b4991c14e61303`  
		Last Modified: Wed, 29 Mar 2023 22:00:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ef0bbe69f83f8b5c0b8b1b564afd893482ebc34ce7f4e25189621713a5a3b1`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data`

```console
$ docker pull influxdb@sha256:a4d3c557c4391396d9eb233be35ec7c800a2c86b1a5fe34a54f95469aa49fd62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

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

## `influxdb:1.8.10-data-alpine`

```console
$ docker pull influxdb@sha256:f4bd05a5999e70974eb7cbbdd5906442e00931d94b37b0c75921832c8ef821c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:62264fc25317633f3eeedbccf78f6ed24719552a6ba3c1a24873335ac7452d20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61352415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c899524c343137f88073bb6cf5fb3fec60a14b665168584e5358b35a3732774f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 21:58:51 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 29 Mar 2023 21:58:59 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 21:58:59 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 29 Mar 2023 21:58:59 GMT
EXPOSE 8086
# Wed, 29 Mar 2023 21:58:59 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Mar 2023 21:58:59 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 29 Mar 2023 21:59:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 29 Mar 2023 21:59:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 21:59:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02516d8c55b0db59be8396fd753bf49b2941067b34ddb8fa0e3c0f6fb3b2b67a`  
		Last Modified: Wed, 29 Mar 2023 22:01:20 GMT  
		Size: 56.5 MB (56503710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffee1bc09b30b9683a0acf9fab57079713eb0fdc7a98fd65d2c634e30022f090`  
		Last Modified: Wed, 29 Mar 2023 22:01:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a563df1bf32f0c1127cc5f3bdd71d477e1cd9dbe08888e5b95ce6a825d0b7a2f`  
		Last Modified: Wed, 29 Mar 2023 22:01:13 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e7e9e92a23ad02049e7817d3fb044533ed427734531e4e797530630ef4335a`  
		Last Modified: Wed, 29 Mar 2023 22:01:13 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta`

```console
$ docker pull influxdb@sha256:2c8c7614714d9a06d763edfea8fa1aab6f8122e4f7de15205e1e44307174c459
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:bf1e545a6de716ea69c1030bb6c60f23821cac25eafaa61926f802ed9d033c9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94230635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2ec25a6c572ea425630cafa756a87ba035e880e6a05002d2f6d79231cb10eea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

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
# Tue, 13 Jun 2023 06:39:27 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:39:27 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 13 Jun 2023 06:39:27 GMT
EXPOSE 8091
# Tue, 13 Jun 2023 06:39:27 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:27 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:28 GMT
CMD ["influxd-meta"]
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
	-	`sha256:2273cff380bceea2d73c2f39770beb52c84a0e16f780ea173c3450f6a6c8500b`  
		Last Modified: Tue, 13 Jun 2023 06:41:25 GMT  
		Size: 23.4 MB (23412766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827cbbf29aa75e7b8b6a9e76ef25a0a84d38fe7b14fe681bde2074cd8d13d924`  
		Last Modified: Tue, 13 Jun 2023 06:41:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cfbbba820bd8a221143222ccd73e6bf3c73ad2b6a66847d466b1e00d007643`  
		Last Modified: Tue, 13 Jun 2023 06:41:23 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta-alpine`

```console
$ docker pull influxdb@sha256:194a713fa6ba49261a2f26a716ecd00d003f40816590b46e951cff0a327770e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:314ca1c6300ee8c6bb1b4d43d5aef05916ee674008b2f6ff955e70c5b45e8bcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28140962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c74605fdbfde7d4168bb2a2c833947d1c6ce587d48f9c9440d1d82c5a7e0b4b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 21:58:51 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 29 Mar 2023 21:59:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 21:59:10 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 29 Mar 2023 21:59:10 GMT
EXPOSE 8091
# Wed, 29 Mar 2023 21:59:10 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Mar 2023 21:59:10 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 29 Mar 2023 21:59:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 21:59:11 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd5a97558827d022b888dd08ed218825a01293d976efdf8c79fd06b4ad855f5`  
		Last Modified: Wed, 29 Mar 2023 22:01:35 GMT  
		Size: 23.3 MB (23293462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bec4b2874a0829997c1b4c248d9d5ccfdb01fc8363fcc347c936df50e3859c`  
		Last Modified: Wed, 29 Mar 2023 22:01:32 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e542b866df0708d65bbb8968c7c641e8c19eac04855e4c4c6b53bc30dc397ff`  
		Last Modified: Wed, 29 Mar 2023 22:01:32 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data`

```console
$ docker pull influxdb@sha256:5f810b818669a7f5b2af67ae5d7d6d9561d28b4cef453513c6c1a7f4d9bb87d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:a6a9dc01ec18b36e1effed80b223967cde9906d615ead04275dbda47754788e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.0 MB (103986739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57b99b643c3b08f9ad95cfc16a94ebcbc2064883b5ff64860e1984a8c2f2722c`
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
# Tue, 13 Jun 2023 06:39:32 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Tue, 13 Jun 2023 06:39:36 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:39:36 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 13 Jun 2023 06:39:37 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 06:39:37 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:37 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:37 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 13 Jun 2023 06:39:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:37 GMT
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
	-	`sha256:220f40436bb3901f7bbb559b867cff58907700b9d13ef81b1cc0c1d630d652f0`  
		Last Modified: Tue, 13 Jun 2023 06:41:40 GMT  
		Size: 33.2 MB (33167666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac62f1fc8a2864e151cd05e8941fe6721b671970af7c730ce0345cd6af6d78a`  
		Last Modified: Tue, 13 Jun 2023 06:41:35 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c6c452d4082dc9bc5575dca2c64a6b2170ee2d8dfeecee06fa203f8409573d`  
		Last Modified: Tue, 13 Jun 2023 06:41:35 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0403552c437819ffa7aa5c90b262ceba0912f51e7df126f3c3d489c7a6d616da`  
		Last Modified: Tue, 13 Jun 2023 06:41:35 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:18b21dbcc2ff1030193c9b6297b8dae1fa9bc444636bc16f197f5a52886a6c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:2a9f0116ae9d755fa3c4dbd9f61e16729cc28bbd92650319077b8d503a7facad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37975736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae5711a11ac73002a72f21b4a931164b3c24c18087c7eb2aaf63db1b7585513`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 17 Apr 2023 22:40:02 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Mon, 17 Apr 2023 22:40:08 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 17 Apr 2023 22:40:09 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 17 Apr 2023 22:40:09 GMT
EXPOSE 8086
# Mon, 17 Apr 2023 22:40:09 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:09 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 17 Apr 2023 22:40:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640bb67089a54be4a5b2a43a995078478336493a707df939ad60679afc0ddf97`  
		Last Modified: Mon, 17 Apr 2023 22:41:52 GMT  
		Size: 33.1 MB (33127031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c3fc1142e6cb99eaa21e0a65a6bf31d9432900d335030adae70526e751a1d9`  
		Last Modified: Mon, 17 Apr 2023 22:41:47 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef31b2105f2c7e8028789e64900508378068aa2218d85039b14454f5743384a`  
		Last Modified: Mon, 17 Apr 2023 22:41:46 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f531b229fbd8d09a34b041054c9b30cf11f21864793d9dea45c34249d8e7ca4`  
		Last Modified: Mon, 17 Apr 2023 22:41:46 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:d952a36eb41ed1810c2d55e7ede6ad70dadbba510f87bf14d1803f78db4b60ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:974946cb96f5e29e09c327da79e20675c540f710ff1931b4d8b67f1a362ba711
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83432406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8915df4c51eb04f8ebc6f500def936548d71e0ac9c77c80da4dcec6aa13d2f9e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 06:38:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 06:39:32 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Tue, 13 Jun 2023 06:39:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:39:44 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 13 Jun 2023 06:39:44 GMT
EXPOSE 8091
# Tue, 13 Jun 2023 06:39:45 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:45 GMT
CMD ["influxd-meta"]
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
	-	`sha256:f88d72f1f039c3e64efe139d9e2842445cdb8b867aea81f4a0402ffbbd516453`  
		Last Modified: Tue, 13 Jun 2023 06:41:51 GMT  
		Size: 12.6 MB (12614533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e680b7d052f52e8ed39385f993b97408b6c4e5a591335549e10fd135cd07b4`  
		Last Modified: Tue, 13 Jun 2023 06:41:49 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9875a7b90225ae82dc7a7b133a29a140900b300048a4a07f8beac9885e90f8e`  
		Last Modified: Tue, 13 Jun 2023 06:41:49 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:8d0c6e149229548e76d45716ed3ab2be44dc8764e7261f5b36d8a462f26ac84f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9f9af2d33c551b48b56f9d68f6901c35cd27af5cf8ee518f1a9f39c5ac05a805
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17427251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d89117685b426ad9c96c62ab1feb9e726b7a9dc6c9fc7ffc5487f0dca7f943`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 17 Apr 2023 22:40:02 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Mon, 17 Apr 2023 22:40:22 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 17 Apr 2023 22:40:22 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 17 Apr 2023 22:40:22 GMT
EXPOSE 8091
# Mon, 17 Apr 2023 22:40:22 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:22 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:23 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025511ae5ae5cc2a2bc89f82c52edffa117531029438e7529108727070d042f4`  
		Last Modified: Mon, 17 Apr 2023 22:42:12 GMT  
		Size: 12.6 MB (12579747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ddd8f1fedbb4b8872e6059cad7033104e3f43e47a467f241d03cf0c274195a`  
		Last Modified: Mon, 17 Apr 2023 22:42:10 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275047e5e18b5c345eacec52caea1aa59a45763e94e2826a4018a3bc34d2b295`  
		Last Modified: Mon, 17 Apr 2023 22:42:10 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.11-data`

```console
$ docker pull influxdb@sha256:5f810b818669a7f5b2af67ae5d7d6d9561d28b4cef453513c6c1a7f4d9bb87d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:a6a9dc01ec18b36e1effed80b223967cde9906d615ead04275dbda47754788e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.0 MB (103986739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57b99b643c3b08f9ad95cfc16a94ebcbc2064883b5ff64860e1984a8c2f2722c`
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
# Tue, 13 Jun 2023 06:39:32 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Tue, 13 Jun 2023 06:39:36 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:39:36 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 13 Jun 2023 06:39:37 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 06:39:37 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:37 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:37 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 13 Jun 2023 06:39:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:37 GMT
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
	-	`sha256:220f40436bb3901f7bbb559b867cff58907700b9d13ef81b1cc0c1d630d652f0`  
		Last Modified: Tue, 13 Jun 2023 06:41:40 GMT  
		Size: 33.2 MB (33167666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac62f1fc8a2864e151cd05e8941fe6721b671970af7c730ce0345cd6af6d78a`  
		Last Modified: Tue, 13 Jun 2023 06:41:35 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c6c452d4082dc9bc5575dca2c64a6b2170ee2d8dfeecee06fa203f8409573d`  
		Last Modified: Tue, 13 Jun 2023 06:41:35 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0403552c437819ffa7aa5c90b262ceba0912f51e7df126f3c3d489c7a6d616da`  
		Last Modified: Tue, 13 Jun 2023 06:41:35 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.11-data-alpine`

```console
$ docker pull influxdb@sha256:18b21dbcc2ff1030193c9b6297b8dae1fa9bc444636bc16f197f5a52886a6c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.11-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:2a9f0116ae9d755fa3c4dbd9f61e16729cc28bbd92650319077b8d503a7facad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37975736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae5711a11ac73002a72f21b4a931164b3c24c18087c7eb2aaf63db1b7585513`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 17 Apr 2023 22:40:02 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Mon, 17 Apr 2023 22:40:08 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 17 Apr 2023 22:40:09 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 17 Apr 2023 22:40:09 GMT
EXPOSE 8086
# Mon, 17 Apr 2023 22:40:09 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:09 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 17 Apr 2023 22:40:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640bb67089a54be4a5b2a43a995078478336493a707df939ad60679afc0ddf97`  
		Last Modified: Mon, 17 Apr 2023 22:41:52 GMT  
		Size: 33.1 MB (33127031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c3fc1142e6cb99eaa21e0a65a6bf31d9432900d335030adae70526e751a1d9`  
		Last Modified: Mon, 17 Apr 2023 22:41:47 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef31b2105f2c7e8028789e64900508378068aa2218d85039b14454f5743384a`  
		Last Modified: Mon, 17 Apr 2023 22:41:46 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f531b229fbd8d09a34b041054c9b30cf11f21864793d9dea45c34249d8e7ca4`  
		Last Modified: Mon, 17 Apr 2023 22:41:46 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.11-meta`

```console
$ docker pull influxdb@sha256:d952a36eb41ed1810c2d55e7ede6ad70dadbba510f87bf14d1803f78db4b60ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:974946cb96f5e29e09c327da79e20675c540f710ff1931b4d8b67f1a362ba711
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83432406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8915df4c51eb04f8ebc6f500def936548d71e0ac9c77c80da4dcec6aa13d2f9e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 06:38:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 06:39:32 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Tue, 13 Jun 2023 06:39:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:39:44 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 13 Jun 2023 06:39:44 GMT
EXPOSE 8091
# Tue, 13 Jun 2023 06:39:45 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:45 GMT
CMD ["influxd-meta"]
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
	-	`sha256:f88d72f1f039c3e64efe139d9e2842445cdb8b867aea81f4a0402ffbbd516453`  
		Last Modified: Tue, 13 Jun 2023 06:41:51 GMT  
		Size: 12.6 MB (12614533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e680b7d052f52e8ed39385f993b97408b6c4e5a591335549e10fd135cd07b4`  
		Last Modified: Tue, 13 Jun 2023 06:41:49 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9875a7b90225ae82dc7a7b133a29a140900b300048a4a07f8beac9885e90f8e`  
		Last Modified: Tue, 13 Jun 2023 06:41:49 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.11-meta-alpine`

```console
$ docker pull influxdb@sha256:8d0c6e149229548e76d45716ed3ab2be44dc8764e7261f5b36d8a462f26ac84f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.11-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9f9af2d33c551b48b56f9d68f6901c35cd27af5cf8ee518f1a9f39c5ac05a805
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17427251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d89117685b426ad9c96c62ab1feb9e726b7a9dc6c9fc7ffc5487f0dca7f943`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 17 Apr 2023 22:40:02 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Mon, 17 Apr 2023 22:40:22 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 17 Apr 2023 22:40:22 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 17 Apr 2023 22:40:22 GMT
EXPOSE 8091
# Mon, 17 Apr 2023 22:40:22 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:22 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:23 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025511ae5ae5cc2a2bc89f82c52edffa117531029438e7529108727070d042f4`  
		Last Modified: Mon, 17 Apr 2023 22:42:12 GMT  
		Size: 12.6 MB (12579747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ddd8f1fedbb4b8872e6059cad7033104e3f43e47a467f241d03cf0c274195a`  
		Last Modified: Mon, 17 Apr 2023 22:42:10 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275047e5e18b5c345eacec52caea1aa59a45763e94e2826a4018a3bc34d2b295`  
		Last Modified: Mon, 17 Apr 2023 22:42:10 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7`

```console
$ docker pull influxdb@sha256:ee57776e5866f10db31242d2a27d02d6bf4c04430cda46b5746a5db78862ad7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7` - linux; amd64

```console
$ docker pull influxdb@sha256:11c5ec3b6f57701fb9ba1822a6ba58cf39e2deab5aa8d37b52de06fc6ec76723
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114635264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f18cacff1c509a29f5fdfe486023182743bda556c5810b07bb7fbb170d7aa71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 06:40:16 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 06:40:17 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 13 Jun 2023 06:40:18 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 13 Jun 2023 06:40:18 GMT
ENV GOSU_VER=1.12
# Tue, 13 Jun 2023 06:40:20 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 13 Jun 2023 06:40:20 GMT
ENV INFLUXDB_VERSION=2.7.1
# Tue, 13 Jun 2023 06:40:25 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 13 Jun 2023 06:40:25 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 13 Jun 2023 06:40:28 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 13 Jun 2023 06:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 13 Jun 2023 06:40:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 13 Jun 2023 06:40:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 13 Jun 2023 06:40:29 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:40:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:40:29 GMT
CMD ["influxd"]
# Tue, 13 Jun 2023 06:40:29 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 06:40:29 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 13 Jun 2023 06:40:29 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 13 Jun 2023 06:40:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 13 Jun 2023 06:40:29 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360595884e7af284fd67763cd8008ab20365866c6e004a4840dfff2d0297964a`  
		Last Modified: Tue, 13 Jun 2023 06:42:28 GMT  
		Size: 6.3 MB (6327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bb27e4cd4a636b5351088458a96365c81ba86126d3f48871da65502c803b6c`  
		Last Modified: Tue, 13 Jun 2023 06:42:26 GMT  
		Size: 6.4 MB (6434099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39336e30949fd04db4d2f217b51fea774c8514025e44f1e57f74b162c842f962`  
		Last Modified: Tue, 13 Jun 2023 06:42:25 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60da549ac656b4c38223710ca916e2fc6ed64920b45105e8ec642e15c1c78515`  
		Last Modified: Tue, 13 Jun 2023 06:42:25 GMT  
		Size: 982.0 KB (982043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90e4fdc689d5da1feaba1f3d2f1d81f5967def0a679214f53691b7a8ad7c36b`  
		Last Modified: Tue, 13 Jun 2023 06:42:28 GMT  
		Size: 46.3 MB (46334326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f08c78ee51bc014ef50f6e78df6f42ee7de2565017f2f57fcbb62aa69625d5`  
		Last Modified: Tue, 13 Jun 2023 06:42:26 GMT  
		Size: 23.1 MB (23128348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160fded0d1c89cc7f828db027c84ea71571a9ce8205112dde4b9aa473462f88`  
		Last Modified: Tue, 13 Jun 2023 06:42:23 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00ead136998e14cf8ddceae2a65ac44d1386fbf059880de31b940eb809ed9c1`  
		Last Modified: Tue, 13 Jun 2023 06:42:23 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94f4e3a2ac1b0aef3670a8defed127927796275c464d9cbb05c07d0e99aa9a7`  
		Last Modified: Tue, 13 Jun 2023 06:42:24 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4b607dc86adf22a4777bcbc4ff46a606910494838a3c250a0562436722518895
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.4 MB (109351907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7201c66f900deb14957c145cb93f0a4e39c973f7d058fd9269142bae87655b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:28:44 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:28:46 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 13 Jun 2023 05:28:46 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 13 Jun 2023 05:28:46 GMT
ENV GOSU_VER=1.12
# Tue, 13 Jun 2023 05:28:48 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 13 Jun 2023 05:28:48 GMT
ENV INFLUXDB_VERSION=2.7.1
# Tue, 13 Jun 2023 05:28:54 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 13 Jun 2023 05:28:54 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 13 Jun 2023 05:28:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 13 Jun 2023 05:28:57 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 13 Jun 2023 05:28:57 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 13 Jun 2023 05:28:57 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 13 Jun 2023 05:28:57 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Tue, 13 Jun 2023 05:28:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 05:28:57 GMT
CMD ["influxd"]
# Tue, 13 Jun 2023 05:28:57 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 05:28:57 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 13 Jun 2023 05:28:58 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 13 Jun 2023 05:28:58 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 13 Jun 2023 05:28:58 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726ef1d252dce95117393ad2b879e59dec13e0f440d29cee7cdfbfa612cd8a3`  
		Last Modified: Tue, 13 Jun 2023 05:29:33 GMT  
		Size: 6.3 MB (6308748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb125b95d5432d1d940feb01b804f404bd4d72593e86fb1efcfb1078735230`  
		Last Modified: Tue, 13 Jun 2023 05:29:32 GMT  
		Size: 6.0 MB (5953752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df67cf330f0c96a2bb2fbff3f6b17fa0d480df56b162e0c9efdfbd5e5cc118`  
		Last Modified: Tue, 13 Jun 2023 05:29:31 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8158844395a059507fafefa0920d381c119e3101ada8f58e340dc3a1bd5f73b`  
		Last Modified: Tue, 13 Jun 2023 05:29:31 GMT  
		Size: 916.9 KB (916927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069c31f471edbf227cc2a4ff94dfd615b181a0221eca11963dd9cd232e1add8f`  
		Last Modified: Tue, 13 Jun 2023 05:29:32 GMT  
		Size: 44.4 MB (44435827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b777598b9c676819e1a937f78601156ba563beeef17bc3da39781fff8abe4b3`  
		Last Modified: Tue, 13 Jun 2023 05:29:31 GMT  
		Size: 21.7 MB (21662568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863d108fd0fc4070d5a0e946b40c9a9b42f069c786b74aa85fb87e15578e264a`  
		Last Modified: Tue, 13 Jun 2023 05:29:29 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4af016f70a576e2a92e2e3f4adc808b69162423c9150c646c0448163e66ec85`  
		Last Modified: Tue, 13 Jun 2023 05:29:29 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:addf27ab731b987ee5136422c445886a2ba6c4bc5e26232e51430de7b5bf4e21`  
		Last Modified: Tue, 13 Jun 2023 05:29:29 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7-alpine`

```console
$ docker pull influxdb@sha256:b5af62ae7701a6e32bccfb27f3bdb8a7863bfc0242bc8f55e3cbeaf560080272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:11c6b4d43ea0937dc066f66507a3ccc46abc6ff3570cd4f73ae8a5214eb3bb0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87856767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db7e93350a803792acdc854e88e8d32904b7c888ae022daaaf03de056bf0f48`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Apr 2023 21:20:35 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Fri, 28 Apr 2023 21:20:36 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Apr 2023 21:20:36 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 28 Apr 2023 21:20:36 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Apr 2023 21:20:40 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Apr 2023 21:20:40 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Apr 2023 21:20:42 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Apr 2023 21:20:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Apr 2023 21:20:43 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Apr 2023 21:20:43 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Apr 2023 21:20:43 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Fri, 28 Apr 2023 21:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 21:20:43 GMT
CMD ["influxd"]
# Fri, 28 Apr 2023 21:20:43 GMT
EXPOSE 8086
# Fri, 28 Apr 2023 21:20:43 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Apr 2023 21:20:44 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Apr 2023 21:20:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Apr 2023 21:20:44 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d7dc0a4b41042d396238efdac4efe4682b1f5cc690c335c53d4a8646c93e5`  
		Last Modified: Fri, 28 Apr 2023 21:21:36 GMT  
		Size: 8.6 MB (8576775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b482c5db797c1c984a5e3f6f31b353ddddcf288557b87203c04f3c921ab403c7`  
		Last Modified: Fri, 28 Apr 2023 21:21:35 GMT  
		Size: 6.4 MB (6434109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d27004b6acf7e99f42533ea66fbad5f12a0a1abdd8368a171a47efc17e8910`  
		Last Modified: Fri, 28 Apr 2023 21:21:34 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af04990a72e4c745563a3c0b97609e4f173e2ae2ffcf980bfc9b8534f05001d3`  
		Last Modified: Fri, 28 Apr 2023 21:21:38 GMT  
		Size: 46.3 MB (46334277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcc0561bea1e0cbecd82599132a0c4517d35409c8b8b47074332861595835a0`  
		Last Modified: Fri, 28 Apr 2023 21:21:35 GMT  
		Size: 23.1 MB (23128348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7301a56a7c58467ed1cff18150eb126b4603999a1ad5a4456fa4c7397c4bae61`  
		Last Modified: Fri, 28 Apr 2023 21:21:32 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb8fd6a87fffeb5b236a00db39629118ec354162fbc3bb35627bad0e9592597`  
		Last Modified: Fri, 28 Apr 2023 21:21:32 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b810f70b9c54097b183f25446685bb2f288141e19d31e3b75ec620896aaec6d0`  
		Last Modified: Fri, 28 Apr 2023 21:21:33 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:005dabe011e81f67f3153b16be5f48419884d440fcf241109bcd63bc01958822
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83817951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59bf9c20f2022ebb0219b3dbc152d14a5b9c2a6ea2737c399bbb7762429989cb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Apr 2023 21:39:58 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Fri, 28 Apr 2023 21:39:59 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Apr 2023 21:39:59 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 28 Apr 2023 21:39:59 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Apr 2023 21:40:03 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Apr 2023 21:40:03 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Apr 2023 21:40:05 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Apr 2023 21:40:06 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Apr 2023 21:40:06 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Apr 2023 21:40:06 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Apr 2023 21:40:06 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Fri, 28 Apr 2023 21:40:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 21:40:06 GMT
CMD ["influxd"]
# Fri, 28 Apr 2023 21:40:06 GMT
EXPOSE 8086
# Fri, 28 Apr 2023 21:40:06 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Apr 2023 21:40:06 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Apr 2023 21:40:06 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Apr 2023 21:40:07 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed363db396bd455184362560a01cd691a111fe2dea827312e4f70ec9d621fee`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28ff246cd804fbc3d235f50fe1078f62888f7e42ad7bfd8bca560649dcd9073`  
		Last Modified: Fri, 28 Apr 2023 21:40:34 GMT  
		Size: 8.5 MB (8495245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b31ae73aa9925c66ea75c05dc5dd7206a62b0153e602996f7625da9fcc6c6`  
		Last Modified: Fri, 28 Apr 2023 21:40:34 GMT  
		Size: 6.0 MB (5953750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d03a48c74d23252fcc605ac1bd41a25da07c2f6b2a9a566c104018bbfaddaa`  
		Last Modified: Fri, 28 Apr 2023 21:40:33 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d18aa8094a07588057db15152ac5bb9250a7f9420aa0e735f8171f486a4c7b`  
		Last Modified: Fri, 28 Apr 2023 21:40:35 GMT  
		Size: 44.4 MB (44435822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098051d87eda37f2cb28958545ded9313db46d2a5524d04f07e43cabca414648`  
		Last Modified: Fri, 28 Apr 2023 21:40:33 GMT  
		Size: 21.7 MB (21662589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72466e38d886fd781cb8da4b311ec32fe30b284a47d3bbbdeb26d89accf349c`  
		Last Modified: Fri, 28 Apr 2023 21:40:31 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31617e798529b16f57014416aa924a482c1d2da1658b09ebc99a3379abdc7fa0`  
		Last Modified: Fri, 28 Apr 2023 21:40:31 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882ab3721c4c6b3ab1a0aeac2c5afcb6b75e0a02c3fcf0e8630ea07782137023`  
		Last Modified: Fri, 28 Apr 2023 21:40:31 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.1`

```console
$ docker pull influxdb@sha256:ee57776e5866f10db31242d2a27d02d6bf4c04430cda46b5746a5db78862ad7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.1` - linux; amd64

```console
$ docker pull influxdb@sha256:11c5ec3b6f57701fb9ba1822a6ba58cf39e2deab5aa8d37b52de06fc6ec76723
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114635264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f18cacff1c509a29f5fdfe486023182743bda556c5810b07bb7fbb170d7aa71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 06:40:16 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 06:40:17 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 13 Jun 2023 06:40:18 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 13 Jun 2023 06:40:18 GMT
ENV GOSU_VER=1.12
# Tue, 13 Jun 2023 06:40:20 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 13 Jun 2023 06:40:20 GMT
ENV INFLUXDB_VERSION=2.7.1
# Tue, 13 Jun 2023 06:40:25 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 13 Jun 2023 06:40:25 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 13 Jun 2023 06:40:28 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 13 Jun 2023 06:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 13 Jun 2023 06:40:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 13 Jun 2023 06:40:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 13 Jun 2023 06:40:29 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:40:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:40:29 GMT
CMD ["influxd"]
# Tue, 13 Jun 2023 06:40:29 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 06:40:29 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 13 Jun 2023 06:40:29 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 13 Jun 2023 06:40:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 13 Jun 2023 06:40:29 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360595884e7af284fd67763cd8008ab20365866c6e004a4840dfff2d0297964a`  
		Last Modified: Tue, 13 Jun 2023 06:42:28 GMT  
		Size: 6.3 MB (6327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bb27e4cd4a636b5351088458a96365c81ba86126d3f48871da65502c803b6c`  
		Last Modified: Tue, 13 Jun 2023 06:42:26 GMT  
		Size: 6.4 MB (6434099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39336e30949fd04db4d2f217b51fea774c8514025e44f1e57f74b162c842f962`  
		Last Modified: Tue, 13 Jun 2023 06:42:25 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60da549ac656b4c38223710ca916e2fc6ed64920b45105e8ec642e15c1c78515`  
		Last Modified: Tue, 13 Jun 2023 06:42:25 GMT  
		Size: 982.0 KB (982043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90e4fdc689d5da1feaba1f3d2f1d81f5967def0a679214f53691b7a8ad7c36b`  
		Last Modified: Tue, 13 Jun 2023 06:42:28 GMT  
		Size: 46.3 MB (46334326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f08c78ee51bc014ef50f6e78df6f42ee7de2565017f2f57fcbb62aa69625d5`  
		Last Modified: Tue, 13 Jun 2023 06:42:26 GMT  
		Size: 23.1 MB (23128348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160fded0d1c89cc7f828db027c84ea71571a9ce8205112dde4b9aa473462f88`  
		Last Modified: Tue, 13 Jun 2023 06:42:23 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00ead136998e14cf8ddceae2a65ac44d1386fbf059880de31b940eb809ed9c1`  
		Last Modified: Tue, 13 Jun 2023 06:42:23 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94f4e3a2ac1b0aef3670a8defed127927796275c464d9cbb05c07d0e99aa9a7`  
		Last Modified: Tue, 13 Jun 2023 06:42:24 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4b607dc86adf22a4777bcbc4ff46a606910494838a3c250a0562436722518895
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.4 MB (109351907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7201c66f900deb14957c145cb93f0a4e39c973f7d058fd9269142bae87655b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:28:44 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:28:46 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 13 Jun 2023 05:28:46 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 13 Jun 2023 05:28:46 GMT
ENV GOSU_VER=1.12
# Tue, 13 Jun 2023 05:28:48 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 13 Jun 2023 05:28:48 GMT
ENV INFLUXDB_VERSION=2.7.1
# Tue, 13 Jun 2023 05:28:54 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 13 Jun 2023 05:28:54 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 13 Jun 2023 05:28:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 13 Jun 2023 05:28:57 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 13 Jun 2023 05:28:57 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 13 Jun 2023 05:28:57 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 13 Jun 2023 05:28:57 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Tue, 13 Jun 2023 05:28:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 05:28:57 GMT
CMD ["influxd"]
# Tue, 13 Jun 2023 05:28:57 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 05:28:57 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 13 Jun 2023 05:28:58 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 13 Jun 2023 05:28:58 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 13 Jun 2023 05:28:58 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726ef1d252dce95117393ad2b879e59dec13e0f440d29cee7cdfbfa612cd8a3`  
		Last Modified: Tue, 13 Jun 2023 05:29:33 GMT  
		Size: 6.3 MB (6308748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb125b95d5432d1d940feb01b804f404bd4d72593e86fb1efcfb1078735230`  
		Last Modified: Tue, 13 Jun 2023 05:29:32 GMT  
		Size: 6.0 MB (5953752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df67cf330f0c96a2bb2fbff3f6b17fa0d480df56b162e0c9efdfbd5e5cc118`  
		Last Modified: Tue, 13 Jun 2023 05:29:31 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8158844395a059507fafefa0920d381c119e3101ada8f58e340dc3a1bd5f73b`  
		Last Modified: Tue, 13 Jun 2023 05:29:31 GMT  
		Size: 916.9 KB (916927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069c31f471edbf227cc2a4ff94dfd615b181a0221eca11963dd9cd232e1add8f`  
		Last Modified: Tue, 13 Jun 2023 05:29:32 GMT  
		Size: 44.4 MB (44435827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b777598b9c676819e1a937f78601156ba563beeef17bc3da39781fff8abe4b3`  
		Last Modified: Tue, 13 Jun 2023 05:29:31 GMT  
		Size: 21.7 MB (21662568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863d108fd0fc4070d5a0e946b40c9a9b42f069c786b74aa85fb87e15578e264a`  
		Last Modified: Tue, 13 Jun 2023 05:29:29 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4af016f70a576e2a92e2e3f4adc808b69162423c9150c646c0448163e66ec85`  
		Last Modified: Tue, 13 Jun 2023 05:29:29 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:addf27ab731b987ee5136422c445886a2ba6c4bc5e26232e51430de7b5bf4e21`  
		Last Modified: Tue, 13 Jun 2023 05:29:29 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.1-alpine`

```console
$ docker pull influxdb@sha256:b5af62ae7701a6e32bccfb27f3bdb8a7863bfc0242bc8f55e3cbeaf560080272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:11c6b4d43ea0937dc066f66507a3ccc46abc6ff3570cd4f73ae8a5214eb3bb0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87856767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db7e93350a803792acdc854e88e8d32904b7c888ae022daaaf03de056bf0f48`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Apr 2023 21:20:35 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Fri, 28 Apr 2023 21:20:36 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Apr 2023 21:20:36 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 28 Apr 2023 21:20:36 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Apr 2023 21:20:40 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Apr 2023 21:20:40 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Apr 2023 21:20:42 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Apr 2023 21:20:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Apr 2023 21:20:43 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Apr 2023 21:20:43 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Apr 2023 21:20:43 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Fri, 28 Apr 2023 21:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 21:20:43 GMT
CMD ["influxd"]
# Fri, 28 Apr 2023 21:20:43 GMT
EXPOSE 8086
# Fri, 28 Apr 2023 21:20:43 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Apr 2023 21:20:44 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Apr 2023 21:20:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Apr 2023 21:20:44 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d7dc0a4b41042d396238efdac4efe4682b1f5cc690c335c53d4a8646c93e5`  
		Last Modified: Fri, 28 Apr 2023 21:21:36 GMT  
		Size: 8.6 MB (8576775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b482c5db797c1c984a5e3f6f31b353ddddcf288557b87203c04f3c921ab403c7`  
		Last Modified: Fri, 28 Apr 2023 21:21:35 GMT  
		Size: 6.4 MB (6434109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d27004b6acf7e99f42533ea66fbad5f12a0a1abdd8368a171a47efc17e8910`  
		Last Modified: Fri, 28 Apr 2023 21:21:34 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af04990a72e4c745563a3c0b97609e4f173e2ae2ffcf980bfc9b8534f05001d3`  
		Last Modified: Fri, 28 Apr 2023 21:21:38 GMT  
		Size: 46.3 MB (46334277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcc0561bea1e0cbecd82599132a0c4517d35409c8b8b47074332861595835a0`  
		Last Modified: Fri, 28 Apr 2023 21:21:35 GMT  
		Size: 23.1 MB (23128348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7301a56a7c58467ed1cff18150eb126b4603999a1ad5a4456fa4c7397c4bae61`  
		Last Modified: Fri, 28 Apr 2023 21:21:32 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb8fd6a87fffeb5b236a00db39629118ec354162fbc3bb35627bad0e9592597`  
		Last Modified: Fri, 28 Apr 2023 21:21:32 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b810f70b9c54097b183f25446685bb2f288141e19d31e3b75ec620896aaec6d0`  
		Last Modified: Fri, 28 Apr 2023 21:21:33 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:005dabe011e81f67f3153b16be5f48419884d440fcf241109bcd63bc01958822
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83817951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59bf9c20f2022ebb0219b3dbc152d14a5b9c2a6ea2737c399bbb7762429989cb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Apr 2023 21:39:58 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Fri, 28 Apr 2023 21:39:59 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Apr 2023 21:39:59 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 28 Apr 2023 21:39:59 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Apr 2023 21:40:03 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Apr 2023 21:40:03 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Apr 2023 21:40:05 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Apr 2023 21:40:06 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Apr 2023 21:40:06 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Apr 2023 21:40:06 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Apr 2023 21:40:06 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Fri, 28 Apr 2023 21:40:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 21:40:06 GMT
CMD ["influxd"]
# Fri, 28 Apr 2023 21:40:06 GMT
EXPOSE 8086
# Fri, 28 Apr 2023 21:40:06 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Apr 2023 21:40:06 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Apr 2023 21:40:06 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Apr 2023 21:40:07 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed363db396bd455184362560a01cd691a111fe2dea827312e4f70ec9d621fee`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28ff246cd804fbc3d235f50fe1078f62888f7e42ad7bfd8bca560649dcd9073`  
		Last Modified: Fri, 28 Apr 2023 21:40:34 GMT  
		Size: 8.5 MB (8495245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b31ae73aa9925c66ea75c05dc5dd7206a62b0153e602996f7625da9fcc6c6`  
		Last Modified: Fri, 28 Apr 2023 21:40:34 GMT  
		Size: 6.0 MB (5953750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d03a48c74d23252fcc605ac1bd41a25da07c2f6b2a9a566c104018bbfaddaa`  
		Last Modified: Fri, 28 Apr 2023 21:40:33 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d18aa8094a07588057db15152ac5bb9250a7f9420aa0e735f8171f486a4c7b`  
		Last Modified: Fri, 28 Apr 2023 21:40:35 GMT  
		Size: 44.4 MB (44435822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098051d87eda37f2cb28958545ded9313db46d2a5524d04f07e43cabca414648`  
		Last Modified: Fri, 28 Apr 2023 21:40:33 GMT  
		Size: 21.7 MB (21662589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72466e38d886fd781cb8da4b311ec32fe30b284a47d3bbbdeb26d89accf349c`  
		Last Modified: Fri, 28 Apr 2023 21:40:31 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31617e798529b16f57014416aa924a482c1d2da1658b09ebc99a3379abdc7fa0`  
		Last Modified: Fri, 28 Apr 2023 21:40:31 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882ab3721c4c6b3ab1a0aeac2c5afcb6b75e0a02c3fcf0e8630ea07782137023`  
		Last Modified: Fri, 28 Apr 2023 21:40:31 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:b5af62ae7701a6e32bccfb27f3bdb8a7863bfc0242bc8f55e3cbeaf560080272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:11c6b4d43ea0937dc066f66507a3ccc46abc6ff3570cd4f73ae8a5214eb3bb0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87856767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db7e93350a803792acdc854e88e8d32904b7c888ae022daaaf03de056bf0f48`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Apr 2023 21:20:35 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Fri, 28 Apr 2023 21:20:36 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Apr 2023 21:20:36 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 28 Apr 2023 21:20:36 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Apr 2023 21:20:40 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Apr 2023 21:20:40 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Apr 2023 21:20:42 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Apr 2023 21:20:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Apr 2023 21:20:43 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Apr 2023 21:20:43 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Apr 2023 21:20:43 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Fri, 28 Apr 2023 21:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 21:20:43 GMT
CMD ["influxd"]
# Fri, 28 Apr 2023 21:20:43 GMT
EXPOSE 8086
# Fri, 28 Apr 2023 21:20:43 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Apr 2023 21:20:44 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Apr 2023 21:20:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Apr 2023 21:20:44 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d7dc0a4b41042d396238efdac4efe4682b1f5cc690c335c53d4a8646c93e5`  
		Last Modified: Fri, 28 Apr 2023 21:21:36 GMT  
		Size: 8.6 MB (8576775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b482c5db797c1c984a5e3f6f31b353ddddcf288557b87203c04f3c921ab403c7`  
		Last Modified: Fri, 28 Apr 2023 21:21:35 GMT  
		Size: 6.4 MB (6434109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d27004b6acf7e99f42533ea66fbad5f12a0a1abdd8368a171a47efc17e8910`  
		Last Modified: Fri, 28 Apr 2023 21:21:34 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af04990a72e4c745563a3c0b97609e4f173e2ae2ffcf980bfc9b8534f05001d3`  
		Last Modified: Fri, 28 Apr 2023 21:21:38 GMT  
		Size: 46.3 MB (46334277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcc0561bea1e0cbecd82599132a0c4517d35409c8b8b47074332861595835a0`  
		Last Modified: Fri, 28 Apr 2023 21:21:35 GMT  
		Size: 23.1 MB (23128348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7301a56a7c58467ed1cff18150eb126b4603999a1ad5a4456fa4c7397c4bae61`  
		Last Modified: Fri, 28 Apr 2023 21:21:32 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb8fd6a87fffeb5b236a00db39629118ec354162fbc3bb35627bad0e9592597`  
		Last Modified: Fri, 28 Apr 2023 21:21:32 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b810f70b9c54097b183f25446685bb2f288141e19d31e3b75ec620896aaec6d0`  
		Last Modified: Fri, 28 Apr 2023 21:21:33 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:005dabe011e81f67f3153b16be5f48419884d440fcf241109bcd63bc01958822
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83817951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59bf9c20f2022ebb0219b3dbc152d14a5b9c2a6ea2737c399bbb7762429989cb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Apr 2023 21:39:58 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Fri, 28 Apr 2023 21:39:59 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Apr 2023 21:39:59 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 28 Apr 2023 21:39:59 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Apr 2023 21:40:03 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Apr 2023 21:40:03 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Apr 2023 21:40:05 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Apr 2023 21:40:06 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Apr 2023 21:40:06 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Apr 2023 21:40:06 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Apr 2023 21:40:06 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Fri, 28 Apr 2023 21:40:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 21:40:06 GMT
CMD ["influxd"]
# Fri, 28 Apr 2023 21:40:06 GMT
EXPOSE 8086
# Fri, 28 Apr 2023 21:40:06 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Apr 2023 21:40:06 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Apr 2023 21:40:06 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Apr 2023 21:40:07 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed363db396bd455184362560a01cd691a111fe2dea827312e4f70ec9d621fee`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28ff246cd804fbc3d235f50fe1078f62888f7e42ad7bfd8bca560649dcd9073`  
		Last Modified: Fri, 28 Apr 2023 21:40:34 GMT  
		Size: 8.5 MB (8495245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b31ae73aa9925c66ea75c05dc5dd7206a62b0153e602996f7625da9fcc6c6`  
		Last Modified: Fri, 28 Apr 2023 21:40:34 GMT  
		Size: 6.0 MB (5953750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d03a48c74d23252fcc605ac1bd41a25da07c2f6b2a9a566c104018bbfaddaa`  
		Last Modified: Fri, 28 Apr 2023 21:40:33 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d18aa8094a07588057db15152ac5bb9250a7f9420aa0e735f8171f486a4c7b`  
		Last Modified: Fri, 28 Apr 2023 21:40:35 GMT  
		Size: 44.4 MB (44435822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098051d87eda37f2cb28958545ded9313db46d2a5524d04f07e43cabca414648`  
		Last Modified: Fri, 28 Apr 2023 21:40:33 GMT  
		Size: 21.7 MB (21662589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72466e38d886fd781cb8da4b311ec32fe30b284a47d3bbbdeb26d89accf349c`  
		Last Modified: Fri, 28 Apr 2023 21:40:31 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31617e798529b16f57014416aa924a482c1d2da1658b09ebc99a3379abdc7fa0`  
		Last Modified: Fri, 28 Apr 2023 21:40:31 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882ab3721c4c6b3ab1a0aeac2c5afcb6b75e0a02c3fcf0e8630ea07782137023`  
		Last Modified: Fri, 28 Apr 2023 21:40:31 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:f4bd05a5999e70974eb7cbbdd5906442e00931d94b37b0c75921832c8ef821c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:62264fc25317633f3eeedbccf78f6ed24719552a6ba3c1a24873335ac7452d20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61352415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c899524c343137f88073bb6cf5fb3fec60a14b665168584e5358b35a3732774f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 21:58:51 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 29 Mar 2023 21:58:59 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 21:58:59 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 29 Mar 2023 21:58:59 GMT
EXPOSE 8086
# Wed, 29 Mar 2023 21:58:59 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Mar 2023 21:58:59 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 29 Mar 2023 21:59:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 29 Mar 2023 21:59:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 21:59:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02516d8c55b0db59be8396fd753bf49b2941067b34ddb8fa0e3c0f6fb3b2b67a`  
		Last Modified: Wed, 29 Mar 2023 22:01:20 GMT  
		Size: 56.5 MB (56503710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffee1bc09b30b9683a0acf9fab57079713eb0fdc7a98fd65d2c634e30022f090`  
		Last Modified: Wed, 29 Mar 2023 22:01:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a563df1bf32f0c1127cc5f3bdd71d477e1cd9dbe08888e5b95ce6a825d0b7a2f`  
		Last Modified: Wed, 29 Mar 2023 22:01:13 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e7e9e92a23ad02049e7817d3fb044533ed427734531e4e797530630ef4335a`  
		Last Modified: Wed, 29 Mar 2023 22:01:13 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:ee57776e5866f10db31242d2a27d02d6bf4c04430cda46b5746a5db78862ad7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:11c5ec3b6f57701fb9ba1822a6ba58cf39e2deab5aa8d37b52de06fc6ec76723
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114635264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f18cacff1c509a29f5fdfe486023182743bda556c5810b07bb7fbb170d7aa71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 06:40:16 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 06:40:17 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 13 Jun 2023 06:40:18 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 13 Jun 2023 06:40:18 GMT
ENV GOSU_VER=1.12
# Tue, 13 Jun 2023 06:40:20 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 13 Jun 2023 06:40:20 GMT
ENV INFLUXDB_VERSION=2.7.1
# Tue, 13 Jun 2023 06:40:25 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 13 Jun 2023 06:40:25 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 13 Jun 2023 06:40:28 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 13 Jun 2023 06:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 13 Jun 2023 06:40:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 13 Jun 2023 06:40:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 13 Jun 2023 06:40:29 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:40:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:40:29 GMT
CMD ["influxd"]
# Tue, 13 Jun 2023 06:40:29 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 06:40:29 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 13 Jun 2023 06:40:29 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 13 Jun 2023 06:40:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 13 Jun 2023 06:40:29 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360595884e7af284fd67763cd8008ab20365866c6e004a4840dfff2d0297964a`  
		Last Modified: Tue, 13 Jun 2023 06:42:28 GMT  
		Size: 6.3 MB (6327784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bb27e4cd4a636b5351088458a96365c81ba86126d3f48871da65502c803b6c`  
		Last Modified: Tue, 13 Jun 2023 06:42:26 GMT  
		Size: 6.4 MB (6434099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39336e30949fd04db4d2f217b51fea774c8514025e44f1e57f74b162c842f962`  
		Last Modified: Tue, 13 Jun 2023 06:42:25 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60da549ac656b4c38223710ca916e2fc6ed64920b45105e8ec642e15c1c78515`  
		Last Modified: Tue, 13 Jun 2023 06:42:25 GMT  
		Size: 982.0 KB (982043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90e4fdc689d5da1feaba1f3d2f1d81f5967def0a679214f53691b7a8ad7c36b`  
		Last Modified: Tue, 13 Jun 2023 06:42:28 GMT  
		Size: 46.3 MB (46334326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f08c78ee51bc014ef50f6e78df6f42ee7de2565017f2f57fcbb62aa69625d5`  
		Last Modified: Tue, 13 Jun 2023 06:42:26 GMT  
		Size: 23.1 MB (23128348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160fded0d1c89cc7f828db027c84ea71571a9ce8205112dde4b9aa473462f88`  
		Last Modified: Tue, 13 Jun 2023 06:42:23 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00ead136998e14cf8ddceae2a65ac44d1386fbf059880de31b940eb809ed9c1`  
		Last Modified: Tue, 13 Jun 2023 06:42:23 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94f4e3a2ac1b0aef3670a8defed127927796275c464d9cbb05c07d0e99aa9a7`  
		Last Modified: Tue, 13 Jun 2023 06:42:24 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4b607dc86adf22a4777bcbc4ff46a606910494838a3c250a0562436722518895
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.4 MB (109351907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7201c66f900deb14957c145cb93f0a4e39c973f7d058fd9269142bae87655b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:28:44 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:28:46 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 13 Jun 2023 05:28:46 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 13 Jun 2023 05:28:46 GMT
ENV GOSU_VER=1.12
# Tue, 13 Jun 2023 05:28:48 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 13 Jun 2023 05:28:48 GMT
ENV INFLUXDB_VERSION=2.7.1
# Tue, 13 Jun 2023 05:28:54 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 13 Jun 2023 05:28:54 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 13 Jun 2023 05:28:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 13 Jun 2023 05:28:57 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 13 Jun 2023 05:28:57 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 13 Jun 2023 05:28:57 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 13 Jun 2023 05:28:57 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Tue, 13 Jun 2023 05:28:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 05:28:57 GMT
CMD ["influxd"]
# Tue, 13 Jun 2023 05:28:57 GMT
EXPOSE 8086
# Tue, 13 Jun 2023 05:28:57 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 13 Jun 2023 05:28:58 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 13 Jun 2023 05:28:58 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 13 Jun 2023 05:28:58 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726ef1d252dce95117393ad2b879e59dec13e0f440d29cee7cdfbfa612cd8a3`  
		Last Modified: Tue, 13 Jun 2023 05:29:33 GMT  
		Size: 6.3 MB (6308748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb125b95d5432d1d940feb01b804f404bd4d72593e86fb1efcfb1078735230`  
		Last Modified: Tue, 13 Jun 2023 05:29:32 GMT  
		Size: 6.0 MB (5953752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df67cf330f0c96a2bb2fbff3f6b17fa0d480df56b162e0c9efdfbd5e5cc118`  
		Last Modified: Tue, 13 Jun 2023 05:29:31 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8158844395a059507fafefa0920d381c119e3101ada8f58e340dc3a1bd5f73b`  
		Last Modified: Tue, 13 Jun 2023 05:29:31 GMT  
		Size: 916.9 KB (916927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069c31f471edbf227cc2a4ff94dfd615b181a0221eca11963dd9cd232e1add8f`  
		Last Modified: Tue, 13 Jun 2023 05:29:32 GMT  
		Size: 44.4 MB (44435827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b777598b9c676819e1a937f78601156ba563beeef17bc3da39781fff8abe4b3`  
		Last Modified: Tue, 13 Jun 2023 05:29:31 GMT  
		Size: 21.7 MB (21662568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863d108fd0fc4070d5a0e946b40c9a9b42f069c786b74aa85fb87e15578e264a`  
		Last Modified: Tue, 13 Jun 2023 05:29:29 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4af016f70a576e2a92e2e3f4adc808b69162423c9150c646c0448163e66ec85`  
		Last Modified: Tue, 13 Jun 2023 05:29:29 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:addf27ab731b987ee5136422c445886a2ba6c4bc5e26232e51430de7b5bf4e21`  
		Last Modified: Tue, 13 Jun 2023 05:29:29 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:2c8c7614714d9a06d763edfea8fa1aab6f8122e4f7de15205e1e44307174c459
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:bf1e545a6de716ea69c1030bb6c60f23821cac25eafaa61926f802ed9d033c9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94230635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2ec25a6c572ea425630cafa756a87ba035e880e6a05002d2f6d79231cb10eea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

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
# Tue, 13 Jun 2023 06:39:27 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 13 Jun 2023 06:39:27 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 13 Jun 2023 06:39:27 GMT
EXPOSE 8091
# Tue, 13 Jun 2023 06:39:27 GMT
VOLUME [/var/lib/influxdb]
# Tue, 13 Jun 2023 06:39:27 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 13 Jun 2023 06:39:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 06:39:28 GMT
CMD ["influxd-meta"]
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
	-	`sha256:2273cff380bceea2d73c2f39770beb52c84a0e16f780ea173c3450f6a6c8500b`  
		Last Modified: Tue, 13 Jun 2023 06:41:25 GMT  
		Size: 23.4 MB (23412766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827cbbf29aa75e7b8b6a9e76ef25a0a84d38fe7b14fe681bde2074cd8d13d924`  
		Last Modified: Tue, 13 Jun 2023 06:41:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cfbbba820bd8a221143222ccd73e6bf3c73ad2b6a66847d466b1e00d007643`  
		Last Modified: Tue, 13 Jun 2023 06:41:23 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:194a713fa6ba49261a2f26a716ecd00d003f40816590b46e951cff0a327770e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:314ca1c6300ee8c6bb1b4d43d5aef05916ee674008b2f6ff955e70c5b45e8bcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28140962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c74605fdbfde7d4168bb2a2c833947d1c6ce587d48f9c9440d1d82c5a7e0b4b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:58:39 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 21:58:51 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 29 Mar 2023 21:59:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 29 Mar 2023 21:59:10 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 29 Mar 2023 21:59:10 GMT
EXPOSE 8091
# Wed, 29 Mar 2023 21:59:10 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Mar 2023 21:59:10 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 29 Mar 2023 21:59:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 21:59:11 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055916911d66d2f812f4a74308557a513233bd1430df8cf1430ba2d06b19b1c3`  
		Last Modified: Wed, 29 Mar 2023 22:00:57 GMT  
		Size: 1.5 MB (1472067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd5a97558827d022b888dd08ed218825a01293d976efdf8c79fd06b4ad855f5`  
		Last Modified: Wed, 29 Mar 2023 22:01:35 GMT  
		Size: 23.3 MB (23293462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bec4b2874a0829997c1b4c248d9d5ccfdb01fc8363fcc347c936df50e3859c`  
		Last Modified: Wed, 29 Mar 2023 22:01:32 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e542b866df0708d65bbb8968c7c641e8c19eac04855e4c4c6b53bc30dc397ff`  
		Last Modified: Wed, 29 Mar 2023 22:01:32 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
