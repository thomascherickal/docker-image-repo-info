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
-	[`influxdb:2.5`](#influxdb25)
-	[`influxdb:2.5-alpine`](#influxdb25-alpine)
-	[`influxdb:2.5.1`](#influxdb251)
-	[`influxdb:2.5.1-alpine`](#influxdb251-alpine)
-	[`influxdb:2.6`](#influxdb26)
-	[`influxdb:2.6-alpine`](#influxdb26-alpine)
-	[`influxdb:2.6.1`](#influxdb261)
-	[`influxdb:2.6.1-alpine`](#influxdb261-alpine)
-	[`influxdb:2.7`](#influxdb27)
-	[`influxdb:2.7-alpine`](#influxdb27-alpine)
-	[`influxdb:2.7.0`](#influxdb270)
-	[`influxdb:2.7.0-alpine`](#influxdb270-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.10-data`

```console
$ docker pull influxdb@sha256:15e6e87ff6573116fa9fece23dc0fcbc6b87fbcd7dfed19cb7f082cea7786652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:86e8569b72ad3e8af4532392bfd867b805f065fbf9791976fb1d002cd7550d62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111166287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af723a9cfc5b4c2385f92084129f5c175db3cff9d9fc75ce55e496dcebdb5f51`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 17 Apr 2023 22:40:25 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Mon, 17 Apr 2023 22:40:29 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 17 Apr 2023 22:40:30 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 17 Apr 2023 22:40:30 GMT
EXPOSE 8086
# Mon, 17 Apr 2023 22:40:30 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 17 Apr 2023 22:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd5f3c2c8bf784f4ebb64613f7e25fbabd809342fb066a57cfa92430583b2be`  
		Last Modified: Mon, 17 Apr 2023 22:42:25 GMT  
		Size: 40.1 MB (40066532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fadc2b58021cc57554fcf85cc2167cc07464493953c7f07ff6d860783693682`  
		Last Modified: Mon, 17 Apr 2023 22:42:19 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c294b82147d68680334e2f10b56f9007a2503d283a0d3a63d7e02d5a5bb2334`  
		Last Modified: Mon, 17 Apr 2023 22:42:19 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfd5f79f5bee7cf05212d29cb047a055cbcba46ee487c6035ae266598ed3eef`  
		Last Modified: Mon, 17 Apr 2023 22:42:20 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:9aa23d27bc28e83a35cc45b9780306f0d6cef0a887c6e67ee727c68c05f60084
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:a18012971eb9375b6d90d7de82da85e4bbaa138f4f056c0e5d4bff0a7e4103b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.3 MB (91332601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f35a121a1f8cfdc56bcf1d1295079a8ca30500c5962248619c64d5be8519b108`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 17 Apr 2023 22:40:25 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Mon, 17 Apr 2023 22:40:45 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 17 Apr 2023 22:40:45 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 17 Apr 2023 22:40:45 GMT
EXPOSE 8091
# Mon, 17 Apr 2023 22:40:45 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:45 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6391ccb380588e88242343b07bb9d4a514f18a36df2c405df66edd023ddb2a22`  
		Last Modified: Mon, 17 Apr 2023 22:42:52 GMT  
		Size: 20.2 MB (20234049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a268b344bf24dea4a957c998eaf1d7f24318d07bc9b84815721b558ac02388`  
		Last Modified: Mon, 17 Apr 2023 22:42:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda9bff955632ecd7bea2a7d2bb36d77bcf6ee658e5eb5f8262693d82fb37cc1`  
		Last Modified: Mon, 17 Apr 2023 22:42:49 GMT  
		Size: 375.0 B  
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
$ docker pull influxdb@sha256:15e6e87ff6573116fa9fece23dc0fcbc6b87fbcd7dfed19cb7f082cea7786652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.3-data` - linux; amd64

```console
$ docker pull influxdb@sha256:86e8569b72ad3e8af4532392bfd867b805f065fbf9791976fb1d002cd7550d62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111166287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af723a9cfc5b4c2385f92084129f5c175db3cff9d9fc75ce55e496dcebdb5f51`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 17 Apr 2023 22:40:25 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Mon, 17 Apr 2023 22:40:29 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 17 Apr 2023 22:40:30 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 17 Apr 2023 22:40:30 GMT
EXPOSE 8086
# Mon, 17 Apr 2023 22:40:30 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 17 Apr 2023 22:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd5f3c2c8bf784f4ebb64613f7e25fbabd809342fb066a57cfa92430583b2be`  
		Last Modified: Mon, 17 Apr 2023 22:42:25 GMT  
		Size: 40.1 MB (40066532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fadc2b58021cc57554fcf85cc2167cc07464493953c7f07ff6d860783693682`  
		Last Modified: Mon, 17 Apr 2023 22:42:19 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c294b82147d68680334e2f10b56f9007a2503d283a0d3a63d7e02d5a5bb2334`  
		Last Modified: Mon, 17 Apr 2023 22:42:19 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfd5f79f5bee7cf05212d29cb047a055cbcba46ee487c6035ae266598ed3eef`  
		Last Modified: Mon, 17 Apr 2023 22:42:20 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:9aa23d27bc28e83a35cc45b9780306f0d6cef0a887c6e67ee727c68c05f60084
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.3-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:a18012971eb9375b6d90d7de82da85e4bbaa138f4f056c0e5d4bff0a7e4103b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.3 MB (91332601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f35a121a1f8cfdc56bcf1d1295079a8ca30500c5962248619c64d5be8519b108`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 17 Apr 2023 22:40:25 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Mon, 17 Apr 2023 22:40:45 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 17 Apr 2023 22:40:45 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 17 Apr 2023 22:40:45 GMT
EXPOSE 8091
# Mon, 17 Apr 2023 22:40:45 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:45 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6391ccb380588e88242343b07bb9d4a514f18a36df2c405df66edd023ddb2a22`  
		Last Modified: Mon, 17 Apr 2023 22:42:52 GMT  
		Size: 20.2 MB (20234049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a268b344bf24dea4a957c998eaf1d7f24318d07bc9b84815721b558ac02388`  
		Last Modified: Mon, 17 Apr 2023 22:42:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda9bff955632ecd7bea2a7d2bb36d77bcf6ee658e5eb5f8262693d82fb37cc1`  
		Last Modified: Mon, 17 Apr 2023 22:42:49 GMT  
		Size: 375.0 B  
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
$ docker pull influxdb@sha256:5b72c48cf1af164440ad3ee1700c4d108da7e13235670b8e526a29bc336f0839
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:6075c5259c7e68e0ea5c6c5a904ece5b344cbf7f0fe57162d230f05c44204a77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125985473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b222f64dfd2bdf5722315f46c34ae5798e98d363693552a93dec6231f71c273`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 14:03:50 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 12 Apr 2023 14:03:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 12 Apr 2023 14:03:54 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 12 Apr 2023 14:03:54 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 14:03:54 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 14:03:54 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 12 Apr 2023 14:03:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 Apr 2023 14:03:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 14:03:54 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773d866633eeeaf0252c8acfee1415bed1888dbc1dfd397552a40ca6dfc7a9fc`  
		Last Modified: Wed, 12 Apr 2023 14:05:43 GMT  
		Size: 54.9 MB (54885777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223bf54a2f64350ccf38beff038e7ae2668b2dbd166920a5dd522a616475b13c`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bd74071a75dfdd6ffa9545d67e61e979904ce85b8cd9fc94fd84b3f372acea`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573c8d4c16921caf260708f11f5552304ae08c15169f87fa9092eb19a82a48c7`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:1f50793808721879a7d1e7dc57c6b2f59d5c51b3bb6ea7fba4517b2a62d44884
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (116985975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5161dd91ce3bd6d80a017de34c0303dd280bca77d64b8cea7c953f187f2c83d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:35 GMT
ADD file:75c57df33c95251a80549b7949853df282a42bc4e5f19176764907a54b74caa9 in / 
# Tue, 11 Apr 2023 23:59:36 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:35:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:35:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 21:19:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 21:19:16 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 12 Apr 2023 21:19:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 12 Apr 2023 21:19:21 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 12 Apr 2023 21:19:21 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 21:19:21 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 21:19:21 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 12 Apr 2023 21:19:21 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 Apr 2023 21:19:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 21:19:21 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4feff9b88735325634445419eaaec2ed47500b63027cfd2de34b8bc6d55ee85c`  
		Last Modified: Wed, 12 Apr 2023 00:02:57 GMT  
		Size: 50.2 MB (50216882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5f77534be142d18fb6441aad5ebb0a6b1fbd1128fee964f14c772d3f48978f`  
		Last Modified: Wed, 12 Apr 2023 09:45:07 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0797973d3ff4c7bfddd6439ceacd815ea867f868a8c75686d5b80ee1a3eca322`  
		Last Modified: Wed, 12 Apr 2023 09:45:08 GMT  
		Size: 10.2 MB (10217876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ce36643d1855bf3e0e882b4da972cec8ca6f91360c6c2830f042af2a393ff8`  
		Last Modified: Wed, 12 Apr 2023 21:19:28 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a5141d3095fb8ad8a3b76ff34a4aca88c6ada9b9120de2c79c16580c151bee`  
		Last Modified: Wed, 12 Apr 2023 21:19:35 GMT  
		Size: 51.6 MB (51613126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00dedc995080c8eb04620bb927be8d0d28ac0c93ac1aeb3e4f284874b9ebc188`  
		Last Modified: Wed, 12 Apr 2023 21:19:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23b33f718ba9d62ed87483188577ca3a3d7144ad007dbace2d10e3038d5bc`  
		Last Modified: Wed, 12 Apr 2023 21:19:28 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf676218d5417bf09d5a6e0c866dfc9a530ee7ad4da9faac7468a50b3844fe6`  
		Last Modified: Wed, 12 Apr 2023 21:19:28 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:1c64e6158697eb79b7b920e08e0dfa2e89a34ff08f1598eb68e77ffb283edd6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (120965553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e423ee859533e7e8ca001faf0ee6499fdd7deff4d8ba3d048f70bb3d791edeb2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 03:33:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 03:33:56 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 12 Apr 2023 03:33:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 12 Apr 2023 03:34:00 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 12 Apr 2023 03:34:00 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 03:34:00 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 03:34:00 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 12 Apr 2023 03:34:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 Apr 2023 03:34:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 03:34:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d04ea5239158b09c9d446ca05fddb7c77a30967337df3ba40a9bfc70a89c8e4`  
		Last Modified: Wed, 12 Apr 2023 03:34:57 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80cc7f8c49497a4f9f3555504b458e76e788740b29493c20fb99518db617652`  
		Last Modified: Wed, 12 Apr 2023 03:35:03 GMT  
		Size: 51.2 MB (51230104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870efcd9046fed61962366eade17475df7afb013c2f65ff40711b1f0efe0222e`  
		Last Modified: Wed, 12 Apr 2023 03:34:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc52b3ceea36bb638fe6627a69214b2f40b62539baf479456bb21b92acbdaa9b`  
		Last Modified: Wed, 12 Apr 2023 03:34:58 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a1cd3dbfb71b9126894ec2f36b9ddc43a9ff7ba2e6fc21aadc879fa1a6cf4e`  
		Last Modified: Wed, 12 Apr 2023 03:34:57 GMT  
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
$ docker pull influxdb@sha256:651fb015520279fc2eb70429e5e39a0cb27a00e373270af4abce43e1324d8bf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:d8c700b1e793262594120826f9773525711d5da51c8a507f903a8e52e5eccd57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127804861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:991f6378bce35ee5f4e6068f9d196d026a42957cba592edbe3d8faf0aa0406bc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 14:03:59 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 12 Apr 2023 14:04:05 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 Apr 2023 14:04:05 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 12 Apr 2023 14:04:05 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 14:04:05 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 14:04:06 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 12 Apr 2023 14:04:06 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 Apr 2023 14:04:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 14:04:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cf5d0ed10ace6baeea02705ffa1ffda74ce779efe566c6fe809b8394cc35e2`  
		Last Modified: Wed, 12 Apr 2023 14:05:59 GMT  
		Size: 56.7 MB (56705107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d3b9ddf0193b06f898d957b9b6e124283fcf97ba7145e80b4600cfd6d665bd`  
		Last Modified: Wed, 12 Apr 2023 14:05:52 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437cc0e198df5b2772d7092253d0eef4b36ee456285c417834d11e3c0c1c6582`  
		Last Modified: Wed, 12 Apr 2023 14:05:52 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be58dc3ea55fc0f5be05a6b9f6db5b99ced026fe55b99e291afe6bdefd620e29`  
		Last Modified: Wed, 12 Apr 2023 14:05:52 GMT  
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
$ docker pull influxdb@sha256:8b8e0f30019a3e43168ef1093f15f04f7ea044d1e9d23b27dac170621034abf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:e5abdeaae36b91e4896be90948f0223c58652a82ab9e2c5572ecd148533d9346
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94511353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b5008aee83e3a9cee431e796df5e69d029b9f99106a3ff40fb9fb7bc0faf52`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 14:03:59 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 12 Apr 2023 14:04:16 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 Apr 2023 14:04:16 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 12 Apr 2023 14:04:17 GMT
EXPOSE 8091
# Wed, 12 Apr 2023 14:04:17 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 14:04:17 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 12 Apr 2023 14:04:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 14:04:17 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0bb276fc62e020dd98ab120e4174c470a49b8ca3038ec79dea13dce5cb180`  
		Last Modified: Wed, 12 Apr 2023 14:06:13 GMT  
		Size: 23.4 MB (23412806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7ea4ee8b2b00dfcf27aa5da85c49615b0abffe26b0c2aadf01092cccf622c3`  
		Last Modified: Wed, 12 Apr 2023 14:06:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21df78c7760fcc2ae463fe4b3480b417d6c074c71aa2738671e877df5b07964`  
		Last Modified: Wed, 12 Apr 2023 14:06:10 GMT  
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
$ docker pull influxdb@sha256:5b72c48cf1af164440ad3ee1700c4d108da7e13235670b8e526a29bc336f0839
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:6075c5259c7e68e0ea5c6c5a904ece5b344cbf7f0fe57162d230f05c44204a77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125985473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b222f64dfd2bdf5722315f46c34ae5798e98d363693552a93dec6231f71c273`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 14:03:50 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 12 Apr 2023 14:03:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 12 Apr 2023 14:03:54 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 12 Apr 2023 14:03:54 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 14:03:54 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 14:03:54 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 12 Apr 2023 14:03:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 Apr 2023 14:03:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 14:03:54 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773d866633eeeaf0252c8acfee1415bed1888dbc1dfd397552a40ca6dfc7a9fc`  
		Last Modified: Wed, 12 Apr 2023 14:05:43 GMT  
		Size: 54.9 MB (54885777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223bf54a2f64350ccf38beff038e7ae2668b2dbd166920a5dd522a616475b13c`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bd74071a75dfdd6ffa9545d67e61e979904ce85b8cd9fc94fd84b3f372acea`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573c8d4c16921caf260708f11f5552304ae08c15169f87fa9092eb19a82a48c7`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:1f50793808721879a7d1e7dc57c6b2f59d5c51b3bb6ea7fba4517b2a62d44884
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (116985975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5161dd91ce3bd6d80a017de34c0303dd280bca77d64b8cea7c953f187f2c83d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:35 GMT
ADD file:75c57df33c95251a80549b7949853df282a42bc4e5f19176764907a54b74caa9 in / 
# Tue, 11 Apr 2023 23:59:36 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:35:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:35:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 21:19:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 21:19:16 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 12 Apr 2023 21:19:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 12 Apr 2023 21:19:21 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 12 Apr 2023 21:19:21 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 21:19:21 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 21:19:21 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 12 Apr 2023 21:19:21 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 Apr 2023 21:19:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 21:19:21 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4feff9b88735325634445419eaaec2ed47500b63027cfd2de34b8bc6d55ee85c`  
		Last Modified: Wed, 12 Apr 2023 00:02:57 GMT  
		Size: 50.2 MB (50216882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5f77534be142d18fb6441aad5ebb0a6b1fbd1128fee964f14c772d3f48978f`  
		Last Modified: Wed, 12 Apr 2023 09:45:07 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0797973d3ff4c7bfddd6439ceacd815ea867f868a8c75686d5b80ee1a3eca322`  
		Last Modified: Wed, 12 Apr 2023 09:45:08 GMT  
		Size: 10.2 MB (10217876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ce36643d1855bf3e0e882b4da972cec8ca6f91360c6c2830f042af2a393ff8`  
		Last Modified: Wed, 12 Apr 2023 21:19:28 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a5141d3095fb8ad8a3b76ff34a4aca88c6ada9b9120de2c79c16580c151bee`  
		Last Modified: Wed, 12 Apr 2023 21:19:35 GMT  
		Size: 51.6 MB (51613126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00dedc995080c8eb04620bb927be8d0d28ac0c93ac1aeb3e4f284874b9ebc188`  
		Last Modified: Wed, 12 Apr 2023 21:19:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23b33f718ba9d62ed87483188577ca3a3d7144ad007dbace2d10e3038d5bc`  
		Last Modified: Wed, 12 Apr 2023 21:19:28 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf676218d5417bf09d5a6e0c866dfc9a530ee7ad4da9faac7468a50b3844fe6`  
		Last Modified: Wed, 12 Apr 2023 21:19:28 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:1c64e6158697eb79b7b920e08e0dfa2e89a34ff08f1598eb68e77ffb283edd6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (120965553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e423ee859533e7e8ca001faf0ee6499fdd7deff4d8ba3d048f70bb3d791edeb2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 03:33:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 03:33:56 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 12 Apr 2023 03:33:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 12 Apr 2023 03:34:00 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 12 Apr 2023 03:34:00 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 03:34:00 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 03:34:00 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 12 Apr 2023 03:34:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 Apr 2023 03:34:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 03:34:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d04ea5239158b09c9d446ca05fddb7c77a30967337df3ba40a9bfc70a89c8e4`  
		Last Modified: Wed, 12 Apr 2023 03:34:57 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80cc7f8c49497a4f9f3555504b458e76e788740b29493c20fb99518db617652`  
		Last Modified: Wed, 12 Apr 2023 03:35:03 GMT  
		Size: 51.2 MB (51230104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870efcd9046fed61962366eade17475df7afb013c2f65ff40711b1f0efe0222e`  
		Last Modified: Wed, 12 Apr 2023 03:34:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc52b3ceea36bb638fe6627a69214b2f40b62539baf479456bb21b92acbdaa9b`  
		Last Modified: Wed, 12 Apr 2023 03:34:58 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a1cd3dbfb71b9126894ec2f36b9ddc43a9ff7ba2e6fc21aadc879fa1a6cf4e`  
		Last Modified: Wed, 12 Apr 2023 03:34:57 GMT  
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
$ docker pull influxdb@sha256:651fb015520279fc2eb70429e5e39a0cb27a00e373270af4abce43e1324d8bf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:d8c700b1e793262594120826f9773525711d5da51c8a507f903a8e52e5eccd57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127804861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:991f6378bce35ee5f4e6068f9d196d026a42957cba592edbe3d8faf0aa0406bc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 14:03:59 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 12 Apr 2023 14:04:05 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 Apr 2023 14:04:05 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 12 Apr 2023 14:04:05 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 14:04:05 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 14:04:06 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 12 Apr 2023 14:04:06 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 Apr 2023 14:04:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 14:04:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cf5d0ed10ace6baeea02705ffa1ffda74ce779efe566c6fe809b8394cc35e2`  
		Last Modified: Wed, 12 Apr 2023 14:05:59 GMT  
		Size: 56.7 MB (56705107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d3b9ddf0193b06f898d957b9b6e124283fcf97ba7145e80b4600cfd6d665bd`  
		Last Modified: Wed, 12 Apr 2023 14:05:52 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437cc0e198df5b2772d7092253d0eef4b36ee456285c417834d11e3c0c1c6582`  
		Last Modified: Wed, 12 Apr 2023 14:05:52 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be58dc3ea55fc0f5be05a6b9f6db5b99ced026fe55b99e291afe6bdefd620e29`  
		Last Modified: Wed, 12 Apr 2023 14:05:52 GMT  
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
$ docker pull influxdb@sha256:8b8e0f30019a3e43168ef1093f15f04f7ea044d1e9d23b27dac170621034abf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:e5abdeaae36b91e4896be90948f0223c58652a82ab9e2c5572ecd148533d9346
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94511353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b5008aee83e3a9cee431e796df5e69d029b9f99106a3ff40fb9fb7bc0faf52`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 14:03:59 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 12 Apr 2023 14:04:16 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 Apr 2023 14:04:16 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 12 Apr 2023 14:04:17 GMT
EXPOSE 8091
# Wed, 12 Apr 2023 14:04:17 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 14:04:17 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 12 Apr 2023 14:04:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 14:04:17 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0bb276fc62e020dd98ab120e4174c470a49b8ca3038ec79dea13dce5cb180`  
		Last Modified: Wed, 12 Apr 2023 14:06:13 GMT  
		Size: 23.4 MB (23412806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7ea4ee8b2b00dfcf27aa5da85c49615b0abffe26b0c2aadf01092cccf622c3`  
		Last Modified: Wed, 12 Apr 2023 14:06:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21df78c7760fcc2ae463fe4b3480b417d6c074c71aa2738671e877df5b07964`  
		Last Modified: Wed, 12 Apr 2023 14:06:10 GMT  
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
$ docker pull influxdb@sha256:194255854e060ff86b2bdb77a5e41f6faf23d462a386adfdf59dee8754f4f988
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:8de389e880d24b94d0ab869e5c022350f3f4bb21d5c14c03668b6dd107dcfff9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104267435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f34f7c5a8b9c03de1b98ebe60ce184d49de748c925075fe1725d428bc4c60500`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 17 Apr 2023 22:39:56 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Mon, 17 Apr 2023 22:40:00 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 17 Apr 2023 22:40:00 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 17 Apr 2023 22:40:00 GMT
EXPOSE 8086
# Mon, 17 Apr 2023 22:40:00 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:00 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 17 Apr 2023 22:40:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f0351f2d46bf09a9978bda6def1fede4738d3dbb8152828774eaeaa561e118`  
		Last Modified: Mon, 17 Apr 2023 22:41:38 GMT  
		Size: 33.2 MB (33167682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77adb75570486e8025a271a62e001f9c28db954b95ca188a5917e60d01e10df1`  
		Last Modified: Mon, 17 Apr 2023 22:41:33 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9937617ca8bc1191eaecf76549e86a6350cb2afb4122fcd9fe2035b09adde7`  
		Last Modified: Mon, 17 Apr 2023 22:41:33 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e14ef454c7166d811031e6335d0b07ba0e6d3fb86b669f1c076ec66b6e9d41e`  
		Last Modified: Mon, 17 Apr 2023 22:41:33 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:7f4d2afae0bafa0c842918806b89e2ee801a2aff9aba4446d06800a627744c3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ef726c1459394c01a1603c6af5f11767b2e1017299573fe992c39e4055549e27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.7 MB (83713096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ad82414b32eed0908b1605ec838a64bbdf23043007821ea2a1f3fbc37ef096a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 17 Apr 2023 22:39:56 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Mon, 17 Apr 2023 22:40:15 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 17 Apr 2023 22:40:15 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 17 Apr 2023 22:40:15 GMT
EXPOSE 8091
# Mon, 17 Apr 2023 22:40:15 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:15 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:16 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfe9e8a6165a09e238b565febd5cc5926311173b90b025fe136efd5f3d00b8c`  
		Last Modified: Mon, 17 Apr 2023 22:42:02 GMT  
		Size: 12.6 MB (12614548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e06b49bafbf331fd2f6ef2d065390647033c8127804ba1aa9e51e1fbd86a7c`  
		Last Modified: Mon, 17 Apr 2023 22:42:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8fe027a707e03da6cc723050ec2019f55c27f6e045595cd7599145f47ecdeb`  
		Last Modified: Mon, 17 Apr 2023 22:42:00 GMT  
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
$ docker pull influxdb@sha256:194255854e060ff86b2bdb77a5e41f6faf23d462a386adfdf59dee8754f4f988
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:8de389e880d24b94d0ab869e5c022350f3f4bb21d5c14c03668b6dd107dcfff9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104267435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f34f7c5a8b9c03de1b98ebe60ce184d49de748c925075fe1725d428bc4c60500`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 17 Apr 2023 22:39:56 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Mon, 17 Apr 2023 22:40:00 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 17 Apr 2023 22:40:00 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 17 Apr 2023 22:40:00 GMT
EXPOSE 8086
# Mon, 17 Apr 2023 22:40:00 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:00 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 17 Apr 2023 22:40:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f0351f2d46bf09a9978bda6def1fede4738d3dbb8152828774eaeaa561e118`  
		Last Modified: Mon, 17 Apr 2023 22:41:38 GMT  
		Size: 33.2 MB (33167682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77adb75570486e8025a271a62e001f9c28db954b95ca188a5917e60d01e10df1`  
		Last Modified: Mon, 17 Apr 2023 22:41:33 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9937617ca8bc1191eaecf76549e86a6350cb2afb4122fcd9fe2035b09adde7`  
		Last Modified: Mon, 17 Apr 2023 22:41:33 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e14ef454c7166d811031e6335d0b07ba0e6d3fb86b669f1c076ec66b6e9d41e`  
		Last Modified: Mon, 17 Apr 2023 22:41:33 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:7f4d2afae0bafa0c842918806b89e2ee801a2aff9aba4446d06800a627744c3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ef726c1459394c01a1603c6af5f11767b2e1017299573fe992c39e4055549e27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.7 MB (83713096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ad82414b32eed0908b1605ec838a64bbdf23043007821ea2a1f3fbc37ef096a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 17 Apr 2023 22:39:56 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Mon, 17 Apr 2023 22:40:15 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 17 Apr 2023 22:40:15 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 17 Apr 2023 22:40:15 GMT
EXPOSE 8091
# Mon, 17 Apr 2023 22:40:15 GMT
VOLUME [/var/lib/influxdb]
# Mon, 17 Apr 2023 22:40:15 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 17 Apr 2023 22:40:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Apr 2023 22:40:16 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfe9e8a6165a09e238b565febd5cc5926311173b90b025fe136efd5f3d00b8c`  
		Last Modified: Mon, 17 Apr 2023 22:42:02 GMT  
		Size: 12.6 MB (12614548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e06b49bafbf331fd2f6ef2d065390647033c8127804ba1aa9e51e1fbd86a7c`  
		Last Modified: Mon, 17 Apr 2023 22:42:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8fe027a707e03da6cc723050ec2019f55c27f6e045595cd7599145f47ecdeb`  
		Last Modified: Mon, 17 Apr 2023 22:42:00 GMT  
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

## `influxdb:2.5`

```console
$ docker pull influxdb@sha256:cf3f55ef67ab686029e8cffc2a5da36f8ebe98f07f7c10bba66c9165e2713a3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5` - linux; amd64

```console
$ docker pull influxdb@sha256:dd29c78848bd355b9fcf5b15702998e109dcffff3566172961ce7dac97eb9e4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99114328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84273b1428d4dad889f08df8d40578bdbfbfb7ae3fb1411bfd781cb2967be91d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:48:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:48:52 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 01:48:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 01:48:53 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 01:48:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 01:48:56 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 12 Apr 2023 01:49:00 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 01:49:00 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 12 Apr 2023 01:49:02 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 01:49:03 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 01:49:03 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 01:49:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 01:49:03 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 01:49:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:49:03 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 01:49:03 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 01:49:04 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 01:49:04 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 01:49:04 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 01:49:04 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631d89e80e4efea8f2c84cb5859b809336e7f53594b8db437806fb3129cf21d`  
		Last Modified: Wed, 12 Apr 2023 01:50:14 GMT  
		Size: 6.3 MB (6327895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60742865a130d899cb9320c3a041fe9b11b34ade8ac793a1bc1c83f6501a4f65`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 7.0 MB (7049185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f3017aa8d7ad8894b072504c2c5cb8b438869314a672ebbaf85313121a3da6`  
		Last Modified: Wed, 12 Apr 2023 01:50:11 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f60e0bc8b1363351a48dc6cffc215f18c8f46611920aca91d34d7fa97b71d`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 982.0 KB (982037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83446baa1b081c1cf6fe8579219d7d1cecb125421fcc58a5f71b4823f7b96fbb`  
		Last Modified: Wed, 12 Apr 2023 01:50:15 GMT  
		Size: 47.2 MB (47217003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f339a6071c401dea61a49627d9069de80d03e675459a6820648e96088a2fb4c7`  
		Last Modified: Wed, 12 Apr 2023 01:50:11 GMT  
		Size: 6.1 MB (6108866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57592f94c83b448408fbb1b1c4abdfda801ae878499c81613f55cb155c0701cf`  
		Last Modified: Wed, 12 Apr 2023 01:50:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6614e416a547f0e63121567579c2052029f7e8ba464264cea954762a126bcd0`  
		Last Modified: Wed, 12 Apr 2023 01:50:09 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80279af81be5e64a56da52f86df7381e855f34da240bce31cfcc756059fb53f6`  
		Last Modified: Wed, 12 Apr 2023 01:50:10 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:bade164cfc81931144f904ca6b6d73767be5d698fd456f1058d8caf7a8af3894
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 MB (95108670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9873c3eb1ea56b1883def8389d0242427761d1da9f602eca211c26587a05497`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:34:08 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:34:09 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 03:34:10 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 03:34:10 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 03:34:12 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 03:34:12 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 12 Apr 2023 03:34:16 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 03:34:17 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 12 Apr 2023 03:34:19 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 03:34:20 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 03:34:20 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 03:34:20 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 03:34:20 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 03:34:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 03:34:20 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 03:34:20 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 03:34:20 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 03:34:20 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 03:34:20 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 03:34:20 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b243f57d3a1ebfedb4718e25ead24072a440224c350ebe24f3822295c87282`  
		Last Modified: Wed, 12 Apr 2023 03:35:14 GMT  
		Size: 6.3 MB (6308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9df8ad4ddd6a2b1c0cae9d3204053c8346ee8a6aa7a5d37d8d54273daa21c7`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 6.6 MB (6643035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27a311d7f96094d6c9e8d0f73ebf4f9d1710ef98e86d7fe08576a30d1df33bb`  
		Last Modified: Wed, 12 Apr 2023 03:35:12 GMT  
		Size: 4.1 KB (4120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3784a77e687bbe1d8bef04cb5527d2cc3a956ee846a51a299f412b13ef9e1ee`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 916.9 KB (916933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc8ce6cbaad413122d483e329e090e4991c557503c7460477907087c05f5958`  
		Last Modified: Wed, 12 Apr 2023 03:35:15 GMT  
		Size: 45.5 MB (45530976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868b8659e4e3348c61880c18207af16863152d7cce8756cb09f1f9f622f14e3a`  
		Last Modified: Wed, 12 Apr 2023 03:35:12 GMT  
		Size: 5.6 MB (5634078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7692517b0a7bf56944a1c1589a537234c4aaefb56648daa7543b6021a17a247a`  
		Last Modified: Wed, 12 Apr 2023 03:35:11 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939e72172450ceff54e7316e90768d9ef2ae76ded26c2b6c1f23fac1ffe41dea`  
		Last Modified: Wed, 12 Apr 2023 03:35:11 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acfe876097d96c0015500149f8bd86dff7f3c5fef7d78b35870a0fea8232b90`  
		Last Modified: Wed, 12 Apr 2023 03:35:11 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.5-alpine`

```console
$ docker pull influxdb@sha256:aebbb6723d25c4ae25edd7943f5f0e5c8a3054682909e77589c5612bb0facedd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d794495e3ba2f3c03f42deb9a27b94e6cc6fcfaf5d10124e45d8c60359ac7757
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69083680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b425b14f094637bb2926d16eeae6e11b18fec4e46db6b7e9b40e4cab359169`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:59:54 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 29 Mar 2023 21:59:54 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 29 Mar 2023 22:00:10 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 29 Mar 2023 22:00:15 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 29 Mar 2023 22:00:15 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 29 Mar 2023 22:00:18 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 29 Mar 2023 22:00:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 29 Mar 2023 22:00:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 29 Mar 2023 22:00:18 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 29 Mar 2023 22:00:18 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 29 Mar 2023 22:00:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:00:18 GMT
CMD ["influxd"]
# Wed, 29 Mar 2023 22:00:19 GMT
EXPOSE 8086
# Wed, 29 Mar 2023 22:00:19 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 29 Mar 2023 22:00:19 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 29 Mar 2023 22:00:19 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 29 Mar 2023 22:00:19 GMT
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
	-	`sha256:c1afb36336fe98dd703c1041000d89b9bae5d279480c46f77620057018d3e2b2`  
		Last Modified: Wed, 29 Mar 2023 22:02:42 GMT  
		Size: 12.4 MB (12374741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b2ee057b405e8d7b36616d40cb252eca7fb22085cad6642982f54ab0ca2baa`  
		Last Modified: Wed, 29 Mar 2023 22:02:40 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119fbd4b43c866a865d6998cd4ffb17916807b3032ded33da2c902eaf27f5b02`  
		Last Modified: Wed, 29 Mar 2023 22:03:01 GMT  
		Size: 47.2 MB (47217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea7d2556fbfff20d803b8f49da9c265150b6d327a15d78d4d3578b2e987d50e`  
		Last Modified: Wed, 29 Mar 2023 22:02:56 GMT  
		Size: 6.1 MB (6108852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70cadf8cf66c0315902a33974f34c11527f51f3b6dd98cb4bfe67ad68d88041f`  
		Last Modified: Wed, 29 Mar 2023 22:02:55 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab0fd66e7260feb706847680a068d395650b1461aab2391c65b8dfc58b4a707`  
		Last Modified: Wed, 29 Mar 2023 22:02:55 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7be7ac61a283aa230677c4d78c17886dd92852b59d3147f31f1a6dff2fde8b`  
		Last Modified: Wed, 29 Mar 2023 22:02:55 GMT  
		Size: 6.4 KB (6440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:5c8d331461f6f4e1a7dfdd827072275e66ce63b353ccb40903938be63755587f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66463339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:948da4c28b1a62ed078837a9a237fd2e90a998c3da8c5ccb9d36d6b7c18aa43e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 04:17:15 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 30 Mar 2023 04:17:16 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 30 Mar 2023 04:17:30 GMT
ENV INFLUXDB_VERSION=2.5.1
# Thu, 30 Mar 2023 04:17:35 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 30 Mar 2023 04:17:35 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Thu, 30 Mar 2023 04:17:38 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 30 Mar 2023 04:17:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 30 Mar 2023 04:17:38 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 30 Mar 2023 04:17:38 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 30 Mar 2023 04:17:38 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 30 Mar 2023 04:17:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 04:17:39 GMT
CMD ["influxd"]
# Thu, 30 Mar 2023 04:17:39 GMT
EXPOSE 8086
# Thu, 30 Mar 2023 04:17:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 30 Mar 2023 04:17:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 30 Mar 2023 04:17:39 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 30 Mar 2023 04:17:39 GMT
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
	-	`sha256:73b6f835aacf2662a2b94c43a8ea49fa6bb22e7462d8ac83f92e9fcb65b3adf4`  
		Last Modified: Thu, 30 Mar 2023 04:18:06 GMT  
		Size: 12.0 MB (12027921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16b3409528a44a440ba66163e99ee9e4c43bc43aa2a65788460f2007c77cc47`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61534712ca931db10a517c943e592c8b8a812af1843fdc6d882fbf2fa749ec4`  
		Last Modified: Thu, 30 Mar 2023 04:18:20 GMT  
		Size: 45.5 MB (45530966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b246ac58f3c6df3391e615b24b11aaa6221d759d5a0101b595e95a626c01604`  
		Last Modified: Thu, 30 Mar 2023 04:18:18 GMT  
		Size: 5.6 MB (5634075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de09135493c9df313a0aad7f05ddfd89ff4dbd6a589d22eb8e349f4efc0ece5`  
		Last Modified: Thu, 30 Mar 2023 04:18:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86d3a792a2fdc0f60e8a91a6dcaa947029dfba4b60c76ed09b4df17f9f7f2cf`  
		Last Modified: Thu, 30 Mar 2023 04:18:17 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0900bef299516d8c14de5fac14c25d901bb29b20b074fc0ad84d1b1a95e9ab`  
		Last Modified: Thu, 30 Mar 2023 04:18:17 GMT  
		Size: 6.4 KB (6440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.5.1`

```console
$ docker pull influxdb@sha256:cf3f55ef67ab686029e8cffc2a5da36f8ebe98f07f7c10bba66c9165e2713a3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5.1` - linux; amd64

```console
$ docker pull influxdb@sha256:dd29c78848bd355b9fcf5b15702998e109dcffff3566172961ce7dac97eb9e4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99114328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84273b1428d4dad889f08df8d40578bdbfbfb7ae3fb1411bfd781cb2967be91d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:48:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:48:52 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 01:48:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 01:48:53 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 01:48:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 01:48:56 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 12 Apr 2023 01:49:00 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 01:49:00 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 12 Apr 2023 01:49:02 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 01:49:03 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 01:49:03 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 01:49:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 01:49:03 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 01:49:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:49:03 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 01:49:03 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 01:49:04 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 01:49:04 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 01:49:04 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 01:49:04 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631d89e80e4efea8f2c84cb5859b809336e7f53594b8db437806fb3129cf21d`  
		Last Modified: Wed, 12 Apr 2023 01:50:14 GMT  
		Size: 6.3 MB (6327895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60742865a130d899cb9320c3a041fe9b11b34ade8ac793a1bc1c83f6501a4f65`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 7.0 MB (7049185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f3017aa8d7ad8894b072504c2c5cb8b438869314a672ebbaf85313121a3da6`  
		Last Modified: Wed, 12 Apr 2023 01:50:11 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f60e0bc8b1363351a48dc6cffc215f18c8f46611920aca91d34d7fa97b71d`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 982.0 KB (982037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83446baa1b081c1cf6fe8579219d7d1cecb125421fcc58a5f71b4823f7b96fbb`  
		Last Modified: Wed, 12 Apr 2023 01:50:15 GMT  
		Size: 47.2 MB (47217003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f339a6071c401dea61a49627d9069de80d03e675459a6820648e96088a2fb4c7`  
		Last Modified: Wed, 12 Apr 2023 01:50:11 GMT  
		Size: 6.1 MB (6108866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57592f94c83b448408fbb1b1c4abdfda801ae878499c81613f55cb155c0701cf`  
		Last Modified: Wed, 12 Apr 2023 01:50:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6614e416a547f0e63121567579c2052029f7e8ba464264cea954762a126bcd0`  
		Last Modified: Wed, 12 Apr 2023 01:50:09 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80279af81be5e64a56da52f86df7381e855f34da240bce31cfcc756059fb53f6`  
		Last Modified: Wed, 12 Apr 2023 01:50:10 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:bade164cfc81931144f904ca6b6d73767be5d698fd456f1058d8caf7a8af3894
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 MB (95108670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9873c3eb1ea56b1883def8389d0242427761d1da9f602eca211c26587a05497`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:34:08 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:34:09 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 03:34:10 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 03:34:10 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 03:34:12 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 03:34:12 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 12 Apr 2023 03:34:16 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 03:34:17 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 12 Apr 2023 03:34:19 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 03:34:20 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 03:34:20 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 03:34:20 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 03:34:20 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 03:34:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 03:34:20 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 03:34:20 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 03:34:20 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 03:34:20 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 03:34:20 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 03:34:20 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b243f57d3a1ebfedb4718e25ead24072a440224c350ebe24f3822295c87282`  
		Last Modified: Wed, 12 Apr 2023 03:35:14 GMT  
		Size: 6.3 MB (6308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9df8ad4ddd6a2b1c0cae9d3204053c8346ee8a6aa7a5d37d8d54273daa21c7`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 6.6 MB (6643035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27a311d7f96094d6c9e8d0f73ebf4f9d1710ef98e86d7fe08576a30d1df33bb`  
		Last Modified: Wed, 12 Apr 2023 03:35:12 GMT  
		Size: 4.1 KB (4120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3784a77e687bbe1d8bef04cb5527d2cc3a956ee846a51a299f412b13ef9e1ee`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 916.9 KB (916933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc8ce6cbaad413122d483e329e090e4991c557503c7460477907087c05f5958`  
		Last Modified: Wed, 12 Apr 2023 03:35:15 GMT  
		Size: 45.5 MB (45530976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868b8659e4e3348c61880c18207af16863152d7cce8756cb09f1f9f622f14e3a`  
		Last Modified: Wed, 12 Apr 2023 03:35:12 GMT  
		Size: 5.6 MB (5634078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7692517b0a7bf56944a1c1589a537234c4aaefb56648daa7543b6021a17a247a`  
		Last Modified: Wed, 12 Apr 2023 03:35:11 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939e72172450ceff54e7316e90768d9ef2ae76ded26c2b6c1f23fac1ffe41dea`  
		Last Modified: Wed, 12 Apr 2023 03:35:11 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acfe876097d96c0015500149f8bd86dff7f3c5fef7d78b35870a0fea8232b90`  
		Last Modified: Wed, 12 Apr 2023 03:35:11 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.5.1-alpine`

```console
$ docker pull influxdb@sha256:aebbb6723d25c4ae25edd7943f5f0e5c8a3054682909e77589c5612bb0facedd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:d794495e3ba2f3c03f42deb9a27b94e6cc6fcfaf5d10124e45d8c60359ac7757
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69083680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b425b14f094637bb2926d16eeae6e11b18fec4e46db6b7e9b40e4cab359169`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:59:54 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 29 Mar 2023 21:59:54 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 29 Mar 2023 22:00:10 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 29 Mar 2023 22:00:15 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 29 Mar 2023 22:00:15 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 29 Mar 2023 22:00:18 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 29 Mar 2023 22:00:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 29 Mar 2023 22:00:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 29 Mar 2023 22:00:18 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 29 Mar 2023 22:00:18 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 29 Mar 2023 22:00:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:00:18 GMT
CMD ["influxd"]
# Wed, 29 Mar 2023 22:00:19 GMT
EXPOSE 8086
# Wed, 29 Mar 2023 22:00:19 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 29 Mar 2023 22:00:19 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 29 Mar 2023 22:00:19 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 29 Mar 2023 22:00:19 GMT
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
	-	`sha256:c1afb36336fe98dd703c1041000d89b9bae5d279480c46f77620057018d3e2b2`  
		Last Modified: Wed, 29 Mar 2023 22:02:42 GMT  
		Size: 12.4 MB (12374741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b2ee057b405e8d7b36616d40cb252eca7fb22085cad6642982f54ab0ca2baa`  
		Last Modified: Wed, 29 Mar 2023 22:02:40 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119fbd4b43c866a865d6998cd4ffb17916807b3032ded33da2c902eaf27f5b02`  
		Last Modified: Wed, 29 Mar 2023 22:03:01 GMT  
		Size: 47.2 MB (47217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea7d2556fbfff20d803b8f49da9c265150b6d327a15d78d4d3578b2e987d50e`  
		Last Modified: Wed, 29 Mar 2023 22:02:56 GMT  
		Size: 6.1 MB (6108852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70cadf8cf66c0315902a33974f34c11527f51f3b6dd98cb4bfe67ad68d88041f`  
		Last Modified: Wed, 29 Mar 2023 22:02:55 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab0fd66e7260feb706847680a068d395650b1461aab2391c65b8dfc58b4a707`  
		Last Modified: Wed, 29 Mar 2023 22:02:55 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7be7ac61a283aa230677c4d78c17886dd92852b59d3147f31f1a6dff2fde8b`  
		Last Modified: Wed, 29 Mar 2023 22:02:55 GMT  
		Size: 6.4 KB (6440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:5c8d331461f6f4e1a7dfdd827072275e66ce63b353ccb40903938be63755587f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66463339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:948da4c28b1a62ed078837a9a237fd2e90a998c3da8c5ccb9d36d6b7c18aa43e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 04:17:15 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 30 Mar 2023 04:17:16 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 30 Mar 2023 04:17:30 GMT
ENV INFLUXDB_VERSION=2.5.1
# Thu, 30 Mar 2023 04:17:35 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 30 Mar 2023 04:17:35 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Thu, 30 Mar 2023 04:17:38 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 30 Mar 2023 04:17:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 30 Mar 2023 04:17:38 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 30 Mar 2023 04:17:38 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 30 Mar 2023 04:17:38 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 30 Mar 2023 04:17:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 04:17:39 GMT
CMD ["influxd"]
# Thu, 30 Mar 2023 04:17:39 GMT
EXPOSE 8086
# Thu, 30 Mar 2023 04:17:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 30 Mar 2023 04:17:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 30 Mar 2023 04:17:39 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 30 Mar 2023 04:17:39 GMT
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
	-	`sha256:73b6f835aacf2662a2b94c43a8ea49fa6bb22e7462d8ac83f92e9fcb65b3adf4`  
		Last Modified: Thu, 30 Mar 2023 04:18:06 GMT  
		Size: 12.0 MB (12027921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16b3409528a44a440ba66163e99ee9e4c43bc43aa2a65788460f2007c77cc47`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61534712ca931db10a517c943e592c8b8a812af1843fdc6d882fbf2fa749ec4`  
		Last Modified: Thu, 30 Mar 2023 04:18:20 GMT  
		Size: 45.5 MB (45530966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b246ac58f3c6df3391e615b24b11aaa6221d759d5a0101b595e95a626c01604`  
		Last Modified: Thu, 30 Mar 2023 04:18:18 GMT  
		Size: 5.6 MB (5634075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de09135493c9df313a0aad7f05ddfd89ff4dbd6a589d22eb8e349f4efc0ece5`  
		Last Modified: Thu, 30 Mar 2023 04:18:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86d3a792a2fdc0f60e8a91a6dcaa947029dfba4b60c76ed09b4df17f9f7f2cf`  
		Last Modified: Thu, 30 Mar 2023 04:18:17 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0900bef299516d8c14de5fac14c25d901bb29b20b074fc0ad84d1b1a95e9ab`  
		Last Modified: Thu, 30 Mar 2023 04:18:17 GMT  
		Size: 6.4 KB (6440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6`

```console
$ docker pull influxdb@sha256:c3431c48e0ddf212ef899ac39034e7b3bacb90a6f4d87b698162ca985041caa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6` - linux; amd64

```console
$ docker pull influxdb@sha256:62bb8be55010a76e14e3b11079cd4003e428ae90ec60497782e586dd9dbda94d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.8 MB (98844194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d51928ea51ac6919522f26ae831e0a2afb7cd661fd7ab16fc847b1ddf0cad62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:48:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:48:52 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 01:48:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 01:48:53 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 01:48:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 01:49:09 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 12 Apr 2023 01:49:14 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 01:49:15 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 12 Apr 2023 01:49:17 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 01:49:17 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 01:49:17 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 01:49:17 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 01:49:17 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 01:49:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:49:18 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 01:49:18 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 01:49:18 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 01:49:18 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 01:49:18 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 01:49:18 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631d89e80e4efea8f2c84cb5859b809336e7f53594b8db437806fb3129cf21d`  
		Last Modified: Wed, 12 Apr 2023 01:50:14 GMT  
		Size: 6.3 MB (6327895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60742865a130d899cb9320c3a041fe9b11b34ade8ac793a1bc1c83f6501a4f65`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 7.0 MB (7049185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f3017aa8d7ad8894b072504c2c5cb8b438869314a672ebbaf85313121a3da6`  
		Last Modified: Wed, 12 Apr 2023 01:50:11 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f60e0bc8b1363351a48dc6cffc215f18c8f46611920aca91d34d7fa97b71d`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 982.0 KB (982037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1b9bc550809addbcb98ad55da16980ad44d965c58669536593eca8ae569aba`  
		Last Modified: Wed, 12 Apr 2023 01:50:29 GMT  
		Size: 46.8 MB (46844107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fe08a3a2859345f346424985678900248af89fa4d792ca18f23bc71913262e`  
		Last Modified: Wed, 12 Apr 2023 01:50:25 GMT  
		Size: 6.2 MB (6211630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e0c85494b984c55e971aa73c1ec6d46d1f762751c469744a2ed5fdbe1eb312`  
		Last Modified: Wed, 12 Apr 2023 01:50:24 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1cbb330ff7c2610b90b69365ed987f63cfb38f9b2a9e46c400a99729b3f870`  
		Last Modified: Wed, 12 Apr 2023 01:50:24 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afeff2769623c61bc9ca643ffae4cf045c82dc9109ef96d16f99c000b8b17a`  
		Last Modified: Wed, 12 Apr 2023 01:50:24 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c445197c39fd9bb3bad57d899e672bbdde186379963d678a939561bac3528466
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94795444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e2fd68c2504e5334898c52d6c813c3efea70ab46849841f8bc658fc91544b44`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:34:08 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:34:09 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 03:34:10 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 03:34:10 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 03:34:12 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 03:34:26 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 12 Apr 2023 03:34:30 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 03:34:31 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 12 Apr 2023 03:34:34 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 03:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 03:34:34 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 03:34:34 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 03:34:34 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 03:34:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 03:34:35 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 03:34:35 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 03:34:35 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 03:34:35 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 03:34:35 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 03:34:35 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b243f57d3a1ebfedb4718e25ead24072a440224c350ebe24f3822295c87282`  
		Last Modified: Wed, 12 Apr 2023 03:35:14 GMT  
		Size: 6.3 MB (6308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9df8ad4ddd6a2b1c0cae9d3204053c8346ee8a6aa7a5d37d8d54273daa21c7`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 6.6 MB (6643035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27a311d7f96094d6c9e8d0f73ebf4f9d1710ef98e86d7fe08576a30d1df33bb`  
		Last Modified: Wed, 12 Apr 2023 03:35:12 GMT  
		Size: 4.1 KB (4120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3784a77e687bbe1d8bef04cb5527d2cc3a956ee846a51a299f412b13ef9e1ee`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 916.9 KB (916933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc4a594750ed3298b8c82984d8146fe252a4118bcd01d88d3a47ac02d55179b`  
		Last Modified: Wed, 12 Apr 2023 03:35:27 GMT  
		Size: 45.1 MB (45145830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482849bdfb23fbd4ef3c8e23dfb775437bfb12d85234b72feee1dcb33a445467`  
		Last Modified: Wed, 12 Apr 2023 03:35:24 GMT  
		Size: 5.7 MB (5705995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe9d0e60fe6e48c74b22456817ca0906c61a5b1231e6c7311658b35c42a0e34`  
		Last Modified: Wed, 12 Apr 2023 03:35:23 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b13c4887b6da1387d739ad24613502771b2b05f734b3f6b6dff8060232288c`  
		Last Modified: Wed, 12 Apr 2023 03:35:23 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b09b4c5bb5580c61b23d4751e3159540abced859dd5a6f6b8dbe535a89ad632`  
		Last Modified: Wed, 12 Apr 2023 03:35:23 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6-alpine`

```console
$ docker pull influxdb@sha256:44a366dd7724453547c612a9fef7a00f9dcfbfafa30e6a1fe164f640d492051c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:87b888ae6fd20ba37c52e820792d062565455fd22f1e06c92db70799f0f8f6b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68813553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f293d68a70a77a309865be452fc9105c40052a028062346b3c73286a5e49e25c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:59:54 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 29 Mar 2023 21:59:54 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 29 Mar 2023 22:00:23 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 29 Mar 2023 22:00:27 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 29 Mar 2023 22:00:27 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 29 Mar 2023 22:00:29 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 29 Mar 2023 22:00:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 29 Mar 2023 22:00:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 29 Mar 2023 22:00:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 29 Mar 2023 22:00:29 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 29 Mar 2023 22:00:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:00:29 GMT
CMD ["influxd"]
# Wed, 29 Mar 2023 22:00:30 GMT
EXPOSE 8086
# Wed, 29 Mar 2023 22:00:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 29 Mar 2023 22:00:30 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 29 Mar 2023 22:00:30 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 29 Mar 2023 22:00:30 GMT
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
	-	`sha256:c1afb36336fe98dd703c1041000d89b9bae5d279480c46f77620057018d3e2b2`  
		Last Modified: Wed, 29 Mar 2023 22:02:42 GMT  
		Size: 12.4 MB (12374741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b2ee057b405e8d7b36616d40cb252eca7fb22085cad6642982f54ab0ca2baa`  
		Last Modified: Wed, 29 Mar 2023 22:02:40 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4e244e44c220124d50f4b21f2c127272a1eb13cb3dd1490e1f3e62e888ac51`  
		Last Modified: Wed, 29 Mar 2023 22:03:15 GMT  
		Size: 46.8 MB (46844109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b977b87996ce033faf2c8183c2a398750b2b340a4ca825945b9f618f5e62d206`  
		Last Modified: Wed, 29 Mar 2023 22:03:11 GMT  
		Size: 6.2 MB (6211617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e2093bd79c7edc07287626340a770f377039d0c28f65782d0aed46ed62ef7c`  
		Last Modified: Wed, 29 Mar 2023 22:03:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1dec79611f531d445ddb24ef322318ba9d758c57d9e10396d752658c52f747`  
		Last Modified: Wed, 29 Mar 2023 22:03:10 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3f9ce0715ec46219cae98741924a2e9ef4fbd5cd670d313dbec0c417400d39`  
		Last Modified: Wed, 29 Mar 2023 22:03:10 GMT  
		Size: 6.4 KB (6440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ee4ee039c462fa847783f32633966c0fe6947248eca56b7c35b742e865596472
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66150114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:193c86b0009ec4e7f7f54f88d5213d7dfb37b7f2e260c23c93636bdbffb0c7da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 04:17:15 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 30 Mar 2023 04:17:16 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 30 Mar 2023 04:17:42 GMT
ENV INFLUXDB_VERSION=2.6.1
# Thu, 30 Mar 2023 04:17:46 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 30 Mar 2023 04:17:46 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Thu, 30 Mar 2023 04:17:48 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 30 Mar 2023 04:17:48 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 30 Mar 2023 04:17:48 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 30 Mar 2023 04:17:48 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 30 Mar 2023 04:17:48 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 30 Mar 2023 04:17:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 04:17:49 GMT
CMD ["influxd"]
# Thu, 30 Mar 2023 04:17:49 GMT
EXPOSE 8086
# Thu, 30 Mar 2023 04:17:49 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 30 Mar 2023 04:17:49 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 30 Mar 2023 04:17:49 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 30 Mar 2023 04:17:49 GMT
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
	-	`sha256:73b6f835aacf2662a2b94c43a8ea49fa6bb22e7462d8ac83f92e9fcb65b3adf4`  
		Last Modified: Thu, 30 Mar 2023 04:18:06 GMT  
		Size: 12.0 MB (12027921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16b3409528a44a440ba66163e99ee9e4c43bc43aa2a65788460f2007c77cc47`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8069e6f5b40dc3a481f27e6b9cd9683635ad4706e6cf40e8bb7f91f1ec0c0c6`  
		Last Modified: Thu, 30 Mar 2023 04:18:33 GMT  
		Size: 45.1 MB (45145855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e33d27d7ae6e2689df7f613565e3f228fb3f31e857c12ab7ce5d99043ec28e`  
		Last Modified: Thu, 30 Mar 2023 04:18:30 GMT  
		Size: 5.7 MB (5705962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59d6829fb6ef1e27307189d7b43692e46ece823a98e909ce715dbf75925c80f`  
		Last Modified: Thu, 30 Mar 2023 04:18:29 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8520cd6bff44fdf9b485bea4d6ddde01727bd01eff2c77cdaafd5055ede6a4f0`  
		Last Modified: Thu, 30 Mar 2023 04:18:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1025a916b3c0633180eceb173ac7b89a1e6e618ffc81884bccb7be67ed2e1715`  
		Last Modified: Thu, 30 Mar 2023 04:18:29 GMT  
		Size: 6.4 KB (6441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6.1`

```console
$ docker pull influxdb@sha256:c3431c48e0ddf212ef899ac39034e7b3bacb90a6f4d87b698162ca985041caa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6.1` - linux; amd64

```console
$ docker pull influxdb@sha256:62bb8be55010a76e14e3b11079cd4003e428ae90ec60497782e586dd9dbda94d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.8 MB (98844194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d51928ea51ac6919522f26ae831e0a2afb7cd661fd7ab16fc847b1ddf0cad62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:48:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:48:52 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 01:48:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 01:48:53 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 01:48:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 01:49:09 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 12 Apr 2023 01:49:14 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 01:49:15 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 12 Apr 2023 01:49:17 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 01:49:17 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 01:49:17 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 01:49:17 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 01:49:17 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 01:49:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:49:18 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 01:49:18 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 01:49:18 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 01:49:18 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 01:49:18 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 01:49:18 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631d89e80e4efea8f2c84cb5859b809336e7f53594b8db437806fb3129cf21d`  
		Last Modified: Wed, 12 Apr 2023 01:50:14 GMT  
		Size: 6.3 MB (6327895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60742865a130d899cb9320c3a041fe9b11b34ade8ac793a1bc1c83f6501a4f65`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 7.0 MB (7049185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f3017aa8d7ad8894b072504c2c5cb8b438869314a672ebbaf85313121a3da6`  
		Last Modified: Wed, 12 Apr 2023 01:50:11 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f60e0bc8b1363351a48dc6cffc215f18c8f46611920aca91d34d7fa97b71d`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 982.0 KB (982037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1b9bc550809addbcb98ad55da16980ad44d965c58669536593eca8ae569aba`  
		Last Modified: Wed, 12 Apr 2023 01:50:29 GMT  
		Size: 46.8 MB (46844107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fe08a3a2859345f346424985678900248af89fa4d792ca18f23bc71913262e`  
		Last Modified: Wed, 12 Apr 2023 01:50:25 GMT  
		Size: 6.2 MB (6211630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e0c85494b984c55e971aa73c1ec6d46d1f762751c469744a2ed5fdbe1eb312`  
		Last Modified: Wed, 12 Apr 2023 01:50:24 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1cbb330ff7c2610b90b69365ed987f63cfb38f9b2a9e46c400a99729b3f870`  
		Last Modified: Wed, 12 Apr 2023 01:50:24 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afeff2769623c61bc9ca643ffae4cf045c82dc9109ef96d16f99c000b8b17a`  
		Last Modified: Wed, 12 Apr 2023 01:50:24 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c445197c39fd9bb3bad57d899e672bbdde186379963d678a939561bac3528466
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94795444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e2fd68c2504e5334898c52d6c813c3efea70ab46849841f8bc658fc91544b44`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:34:08 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:34:09 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 03:34:10 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 03:34:10 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 03:34:12 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 03:34:26 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 12 Apr 2023 03:34:30 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 03:34:31 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 12 Apr 2023 03:34:34 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 03:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 03:34:34 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 03:34:34 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 03:34:34 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 03:34:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 03:34:35 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 03:34:35 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 03:34:35 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 03:34:35 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 03:34:35 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 03:34:35 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b243f57d3a1ebfedb4718e25ead24072a440224c350ebe24f3822295c87282`  
		Last Modified: Wed, 12 Apr 2023 03:35:14 GMT  
		Size: 6.3 MB (6308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9df8ad4ddd6a2b1c0cae9d3204053c8346ee8a6aa7a5d37d8d54273daa21c7`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 6.6 MB (6643035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27a311d7f96094d6c9e8d0f73ebf4f9d1710ef98e86d7fe08576a30d1df33bb`  
		Last Modified: Wed, 12 Apr 2023 03:35:12 GMT  
		Size: 4.1 KB (4120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3784a77e687bbe1d8bef04cb5527d2cc3a956ee846a51a299f412b13ef9e1ee`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 916.9 KB (916933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc4a594750ed3298b8c82984d8146fe252a4118bcd01d88d3a47ac02d55179b`  
		Last Modified: Wed, 12 Apr 2023 03:35:27 GMT  
		Size: 45.1 MB (45145830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482849bdfb23fbd4ef3c8e23dfb775437bfb12d85234b72feee1dcb33a445467`  
		Last Modified: Wed, 12 Apr 2023 03:35:24 GMT  
		Size: 5.7 MB (5705995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe9d0e60fe6e48c74b22456817ca0906c61a5b1231e6c7311658b35c42a0e34`  
		Last Modified: Wed, 12 Apr 2023 03:35:23 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b13c4887b6da1387d739ad24613502771b2b05f734b3f6b6dff8060232288c`  
		Last Modified: Wed, 12 Apr 2023 03:35:23 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b09b4c5bb5580c61b23d4751e3159540abced859dd5a6f6b8dbe535a89ad632`  
		Last Modified: Wed, 12 Apr 2023 03:35:23 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6.1-alpine`

```console
$ docker pull influxdb@sha256:44a366dd7724453547c612a9fef7a00f9dcfbfafa30e6a1fe164f640d492051c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:87b888ae6fd20ba37c52e820792d062565455fd22f1e06c92db70799f0f8f6b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68813553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f293d68a70a77a309865be452fc9105c40052a028062346b3c73286a5e49e25c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:59:54 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 29 Mar 2023 21:59:54 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 29 Mar 2023 22:00:23 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 29 Mar 2023 22:00:27 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 29 Mar 2023 22:00:27 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 29 Mar 2023 22:00:29 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 29 Mar 2023 22:00:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 29 Mar 2023 22:00:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 29 Mar 2023 22:00:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 29 Mar 2023 22:00:29 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 29 Mar 2023 22:00:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:00:29 GMT
CMD ["influxd"]
# Wed, 29 Mar 2023 22:00:30 GMT
EXPOSE 8086
# Wed, 29 Mar 2023 22:00:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 29 Mar 2023 22:00:30 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 29 Mar 2023 22:00:30 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 29 Mar 2023 22:00:30 GMT
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
	-	`sha256:c1afb36336fe98dd703c1041000d89b9bae5d279480c46f77620057018d3e2b2`  
		Last Modified: Wed, 29 Mar 2023 22:02:42 GMT  
		Size: 12.4 MB (12374741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b2ee057b405e8d7b36616d40cb252eca7fb22085cad6642982f54ab0ca2baa`  
		Last Modified: Wed, 29 Mar 2023 22:02:40 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4e244e44c220124d50f4b21f2c127272a1eb13cb3dd1490e1f3e62e888ac51`  
		Last Modified: Wed, 29 Mar 2023 22:03:15 GMT  
		Size: 46.8 MB (46844109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b977b87996ce033faf2c8183c2a398750b2b340a4ca825945b9f618f5e62d206`  
		Last Modified: Wed, 29 Mar 2023 22:03:11 GMT  
		Size: 6.2 MB (6211617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e2093bd79c7edc07287626340a770f377039d0c28f65782d0aed46ed62ef7c`  
		Last Modified: Wed, 29 Mar 2023 22:03:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1dec79611f531d445ddb24ef322318ba9d758c57d9e10396d752658c52f747`  
		Last Modified: Wed, 29 Mar 2023 22:03:10 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3f9ce0715ec46219cae98741924a2e9ef4fbd5cd670d313dbec0c417400d39`  
		Last Modified: Wed, 29 Mar 2023 22:03:10 GMT  
		Size: 6.4 KB (6440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ee4ee039c462fa847783f32633966c0fe6947248eca56b7c35b742e865596472
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66150114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:193c86b0009ec4e7f7f54f88d5213d7dfb37b7f2e260c23c93636bdbffb0c7da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 04:17:15 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 30 Mar 2023 04:17:16 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 30 Mar 2023 04:17:42 GMT
ENV INFLUXDB_VERSION=2.6.1
# Thu, 30 Mar 2023 04:17:46 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 30 Mar 2023 04:17:46 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Thu, 30 Mar 2023 04:17:48 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 30 Mar 2023 04:17:48 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 30 Mar 2023 04:17:48 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 30 Mar 2023 04:17:48 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 30 Mar 2023 04:17:48 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 30 Mar 2023 04:17:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 04:17:49 GMT
CMD ["influxd"]
# Thu, 30 Mar 2023 04:17:49 GMT
EXPOSE 8086
# Thu, 30 Mar 2023 04:17:49 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 30 Mar 2023 04:17:49 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 30 Mar 2023 04:17:49 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 30 Mar 2023 04:17:49 GMT
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
	-	`sha256:73b6f835aacf2662a2b94c43a8ea49fa6bb22e7462d8ac83f92e9fcb65b3adf4`  
		Last Modified: Thu, 30 Mar 2023 04:18:06 GMT  
		Size: 12.0 MB (12027921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16b3409528a44a440ba66163e99ee9e4c43bc43aa2a65788460f2007c77cc47`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8069e6f5b40dc3a481f27e6b9cd9683635ad4706e6cf40e8bb7f91f1ec0c0c6`  
		Last Modified: Thu, 30 Mar 2023 04:18:33 GMT  
		Size: 45.1 MB (45145855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e33d27d7ae6e2689df7f613565e3f228fb3f31e857c12ab7ce5d99043ec28e`  
		Last Modified: Thu, 30 Mar 2023 04:18:30 GMT  
		Size: 5.7 MB (5705962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59d6829fb6ef1e27307189d7b43692e46ece823a98e909ce715dbf75925c80f`  
		Last Modified: Thu, 30 Mar 2023 04:18:29 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8520cd6bff44fdf9b485bea4d6ddde01727bd01eff2c77cdaafd5055ede6a4f0`  
		Last Modified: Thu, 30 Mar 2023 04:18:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1025a916b3c0633180eceb173ac7b89a1e6e618ffc81884bccb7be67ed2e1715`  
		Last Modified: Thu, 30 Mar 2023 04:18:29 GMT  
		Size: 6.4 KB (6441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7`

```console
$ docker pull influxdb@sha256:4b811aa4a47a0e5074466c1320fb0932a760933192112809447d0142ca2773f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7` - linux; amd64

```console
$ docker pull influxdb@sha256:32b2c4d5e6fc96da0f6eb325aacc635964d44844cac95bbdee07e620afdf27e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114869180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7de0f3140b356698d7c7ca47cfbefb1aae55a35a70c3b2d8daaa3f7f0cd20bfe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:48:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:48:52 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 01:48:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 01:48:53 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 01:48:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 01:49:22 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 12 Apr 2023 01:49:27 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 01:49:27 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 12 Apr 2023 01:49:30 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 01:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 01:49:30 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 01:49:31 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 01:49:31 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 01:49:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:49:31 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 01:49:31 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 01:49:31 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 01:49:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 01:49:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 01:49:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631d89e80e4efea8f2c84cb5859b809336e7f53594b8db437806fb3129cf21d`  
		Last Modified: Wed, 12 Apr 2023 01:50:14 GMT  
		Size: 6.3 MB (6327895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60742865a130d899cb9320c3a041fe9b11b34ade8ac793a1bc1c83f6501a4f65`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 7.0 MB (7049185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f3017aa8d7ad8894b072504c2c5cb8b438869314a672ebbaf85313121a3da6`  
		Last Modified: Wed, 12 Apr 2023 01:50:11 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f60e0bc8b1363351a48dc6cffc215f18c8f46611920aca91d34d7fa97b71d`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 982.0 KB (982037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a9890bc19a612aa3936ca8f366ba2458d939c934c58855dfa744e415d8bfed`  
		Last Modified: Wed, 12 Apr 2023 01:50:47 GMT  
		Size: 46.3 MB (46334688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dde9a44430dd3a49742911da50232ecae252a57a169d2feb1074a37cbbcdd72`  
		Last Modified: Wed, 12 Apr 2023 01:50:44 GMT  
		Size: 22.7 MB (22746035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ae2894ff3aea334c8bd14e48affa8db988bf2cd184ed8267df559baf8bf6e9`  
		Last Modified: Wed, 12 Apr 2023 01:50:41 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af0707a6d12c69ffe7602747c319c45ed9b50a6d619f094957f8b13dae7eda5`  
		Last Modified: Wed, 12 Apr 2023 01:50:42 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b6ab443599ec65c641cef83b3437c89422b162898083611511da032533bb75`  
		Last Modified: Wed, 12 Apr 2023 01:50:42 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9777b6331615014935e3c4428ed1de0a38e7df1db6f43d844575dc9d43d132d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109730104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97e29edb242329b633cb94a5fe4686cc1895afccea8f9212807c6341555984d9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:34:08 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:34:09 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 03:34:10 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 03:34:10 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 03:34:12 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 03:34:38 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 12 Apr 2023 03:34:42 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 03:34:42 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 12 Apr 2023 03:34:45 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 03:34:45 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 03:34:45 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 03:34:45 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 03:34:45 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 03:34:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 03:34:46 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 03:34:46 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 03:34:46 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 03:34:46 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 03:34:46 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 03:34:46 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b243f57d3a1ebfedb4718e25ead24072a440224c350ebe24f3822295c87282`  
		Last Modified: Wed, 12 Apr 2023 03:35:14 GMT  
		Size: 6.3 MB (6308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9df8ad4ddd6a2b1c0cae9d3204053c8346ee8a6aa7a5d37d8d54273daa21c7`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 6.6 MB (6643035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27a311d7f96094d6c9e8d0f73ebf4f9d1710ef98e86d7fe08576a30d1df33bb`  
		Last Modified: Wed, 12 Apr 2023 03:35:12 GMT  
		Size: 4.1 KB (4120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3784a77e687bbe1d8bef04cb5527d2cc3a956ee846a51a299f412b13ef9e1ee`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 916.9 KB (916933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b0bd765dbad7244932d0bc6e1b0ae45d24d3ea38107b90f8bff5d9a6f4fa13`  
		Last Modified: Wed, 12 Apr 2023 03:35:39 GMT  
		Size: 44.4 MB (44435735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d0e0d56916614791112b9ad2c4ddf16daba60b57122fa5634311c84b91a8fc`  
		Last Modified: Wed, 12 Apr 2023 03:35:37 GMT  
		Size: 21.4 MB (21350751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12f8122a52d5645972b687700a7ede09c1224947361c97164f26e01e9ac397f`  
		Last Modified: Wed, 12 Apr 2023 03:35:35 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f31e093c31418eb240b0e92b54629abf1428400dc52a2eef1119f4e869b120`  
		Last Modified: Wed, 12 Apr 2023 03:35:35 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d70f9875c06738efaaebb76e4afc48036a744793243623fcbefb6a995becd3`  
		Last Modified: Wed, 12 Apr 2023 03:35:35 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7-alpine`

```console
$ docker pull influxdb@sha256:2f7487fe433cf4bb75526c385e3e0510de1e40c4176c8aca3858c127378d27ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:80c6ef024babe804c026931a32a9da53a0f197e3f9cddb38385321a854ad8dbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.8 MB (84838507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d81b58390e922e93331b46f3e5278c5ebf76030453daa19d53ad57c05962dc32`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:59:54 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 29 Mar 2023 21:59:54 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 05 Apr 2023 21:20:28 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 05 Apr 2023 21:20:32 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 05 Apr 2023 21:20:32 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 05 Apr 2023 21:20:34 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 05 Apr 2023 21:20:34 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 05 Apr 2023 21:20:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 05 Apr 2023 21:20:35 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 05 Apr 2023 21:20:35 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 05 Apr 2023 21:20:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Apr 2023 21:20:35 GMT
CMD ["influxd"]
# Wed, 05 Apr 2023 21:20:35 GMT
EXPOSE 8086
# Wed, 05 Apr 2023 21:20:35 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 05 Apr 2023 21:20:35 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 05 Apr 2023 21:20:35 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 05 Apr 2023 21:20:35 GMT
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
	-	`sha256:c1afb36336fe98dd703c1041000d89b9bae5d279480c46f77620057018d3e2b2`  
		Last Modified: Wed, 29 Mar 2023 22:02:42 GMT  
		Size: 12.4 MB (12374741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b2ee057b405e8d7b36616d40cb252eca7fb22085cad6642982f54ab0ca2baa`  
		Last Modified: Wed, 29 Mar 2023 22:02:40 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad124c02e9466927394363db09e8237c01e074cd7ab74357f0357697daa52b5`  
		Last Modified: Wed, 05 Apr 2023 21:21:31 GMT  
		Size: 46.3 MB (46334638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0dea23ab3557a0906d30572828a920e3255ebcb35b12c018f02a082bbfc259`  
		Last Modified: Wed, 05 Apr 2023 21:21:29 GMT  
		Size: 22.7 MB (22746040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9426dfe208286157840f45d8b1baca25f9cb660145704d2f00c5a2f8d347c9fa`  
		Last Modified: Wed, 05 Apr 2023 21:21:26 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7797b468e623ea798e1c57613918eb26a9e2a87a1c2a0f1b8c2b6b34812ef1`  
		Last Modified: Wed, 05 Apr 2023 21:21:26 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c414db96cd83babf4ed2aaa392facc4fa6715af82e8c3e6a6e3b48895bfa6356`  
		Last Modified: Wed, 05 Apr 2023 21:21:26 GMT  
		Size: 6.4 KB (6442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:006f5e1ba8af7211cd55b0b742279ade8ba591ab3b90fa963db9406cc44bff16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81084753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6be29eac1a5176462dc83c897cd42d11b2491b3c8dfdaee1607b7efebea903`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 04:17:15 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 30 Mar 2023 04:17:16 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 05 Apr 2023 21:40:33 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 05 Apr 2023 21:40:36 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 05 Apr 2023 21:40:36 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 05 Apr 2023 21:40:38 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 05 Apr 2023 21:40:39 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 05 Apr 2023 21:40:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 05 Apr 2023 21:40:39 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 05 Apr 2023 21:40:39 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 05 Apr 2023 21:40:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Apr 2023 21:40:39 GMT
CMD ["influxd"]
# Wed, 05 Apr 2023 21:40:39 GMT
EXPOSE 8086
# Wed, 05 Apr 2023 21:40:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 05 Apr 2023 21:40:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 05 Apr 2023 21:40:39 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 05 Apr 2023 21:40:39 GMT
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
	-	`sha256:73b6f835aacf2662a2b94c43a8ea49fa6bb22e7462d8ac83f92e9fcb65b3adf4`  
		Last Modified: Thu, 30 Mar 2023 04:18:06 GMT  
		Size: 12.0 MB (12027921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16b3409528a44a440ba66163e99ee9e4c43bc43aa2a65788460f2007c77cc47`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2307171e9e88cf15e41e3c512ca6958ba7cd4a0943997f73aef13b995585a48`  
		Last Modified: Wed, 05 Apr 2023 21:41:14 GMT  
		Size: 44.4 MB (44435729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba07f325899c078273a439bb929a761db612748e0e5caeffb128368ed0888b9`  
		Last Modified: Wed, 05 Apr 2023 21:41:12 GMT  
		Size: 21.4 MB (21350727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0958fc96a25897970f15196bce7df128e367670bc337ff487871733934068b0`  
		Last Modified: Wed, 05 Apr 2023 21:41:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249adfe958028dfdb4ece08fd1e5e786cc6289b05146181b808cff0db486bc69`  
		Last Modified: Wed, 05 Apr 2023 21:41:10 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae57acef8e97ce7d021f8f5bc003ae845ab318950ffc6355db05f7ec8563b88`  
		Last Modified: Wed, 05 Apr 2023 21:41:10 GMT  
		Size: 6.4 KB (6440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.0`

```console
$ docker pull influxdb@sha256:4b811aa4a47a0e5074466c1320fb0932a760933192112809447d0142ca2773f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.0` - linux; amd64

```console
$ docker pull influxdb@sha256:32b2c4d5e6fc96da0f6eb325aacc635964d44844cac95bbdee07e620afdf27e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114869180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7de0f3140b356698d7c7ca47cfbefb1aae55a35a70c3b2d8daaa3f7f0cd20bfe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:48:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:48:52 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 01:48:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 01:48:53 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 01:48:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 01:49:22 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 12 Apr 2023 01:49:27 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 01:49:27 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 12 Apr 2023 01:49:30 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 01:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 01:49:30 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 01:49:31 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 01:49:31 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 01:49:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:49:31 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 01:49:31 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 01:49:31 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 01:49:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 01:49:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 01:49:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631d89e80e4efea8f2c84cb5859b809336e7f53594b8db437806fb3129cf21d`  
		Last Modified: Wed, 12 Apr 2023 01:50:14 GMT  
		Size: 6.3 MB (6327895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60742865a130d899cb9320c3a041fe9b11b34ade8ac793a1bc1c83f6501a4f65`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 7.0 MB (7049185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f3017aa8d7ad8894b072504c2c5cb8b438869314a672ebbaf85313121a3da6`  
		Last Modified: Wed, 12 Apr 2023 01:50:11 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f60e0bc8b1363351a48dc6cffc215f18c8f46611920aca91d34d7fa97b71d`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 982.0 KB (982037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a9890bc19a612aa3936ca8f366ba2458d939c934c58855dfa744e415d8bfed`  
		Last Modified: Wed, 12 Apr 2023 01:50:47 GMT  
		Size: 46.3 MB (46334688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dde9a44430dd3a49742911da50232ecae252a57a169d2feb1074a37cbbcdd72`  
		Last Modified: Wed, 12 Apr 2023 01:50:44 GMT  
		Size: 22.7 MB (22746035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ae2894ff3aea334c8bd14e48affa8db988bf2cd184ed8267df559baf8bf6e9`  
		Last Modified: Wed, 12 Apr 2023 01:50:41 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af0707a6d12c69ffe7602747c319c45ed9b50a6d619f094957f8b13dae7eda5`  
		Last Modified: Wed, 12 Apr 2023 01:50:42 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b6ab443599ec65c641cef83b3437c89422b162898083611511da032533bb75`  
		Last Modified: Wed, 12 Apr 2023 01:50:42 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9777b6331615014935e3c4428ed1de0a38e7df1db6f43d844575dc9d43d132d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109730104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97e29edb242329b633cb94a5fe4686cc1895afccea8f9212807c6341555984d9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:34:08 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:34:09 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 03:34:10 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 03:34:10 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 03:34:12 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 03:34:38 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 12 Apr 2023 03:34:42 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 03:34:42 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 12 Apr 2023 03:34:45 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 03:34:45 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 03:34:45 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 03:34:45 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 03:34:45 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 03:34:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 03:34:46 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 03:34:46 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 03:34:46 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 03:34:46 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 03:34:46 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 03:34:46 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b243f57d3a1ebfedb4718e25ead24072a440224c350ebe24f3822295c87282`  
		Last Modified: Wed, 12 Apr 2023 03:35:14 GMT  
		Size: 6.3 MB (6308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9df8ad4ddd6a2b1c0cae9d3204053c8346ee8a6aa7a5d37d8d54273daa21c7`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 6.6 MB (6643035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27a311d7f96094d6c9e8d0f73ebf4f9d1710ef98e86d7fe08576a30d1df33bb`  
		Last Modified: Wed, 12 Apr 2023 03:35:12 GMT  
		Size: 4.1 KB (4120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3784a77e687bbe1d8bef04cb5527d2cc3a956ee846a51a299f412b13ef9e1ee`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 916.9 KB (916933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b0bd765dbad7244932d0bc6e1b0ae45d24d3ea38107b90f8bff5d9a6f4fa13`  
		Last Modified: Wed, 12 Apr 2023 03:35:39 GMT  
		Size: 44.4 MB (44435735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d0e0d56916614791112b9ad2c4ddf16daba60b57122fa5634311c84b91a8fc`  
		Last Modified: Wed, 12 Apr 2023 03:35:37 GMT  
		Size: 21.4 MB (21350751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12f8122a52d5645972b687700a7ede09c1224947361c97164f26e01e9ac397f`  
		Last Modified: Wed, 12 Apr 2023 03:35:35 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f31e093c31418eb240b0e92b54629abf1428400dc52a2eef1119f4e869b120`  
		Last Modified: Wed, 12 Apr 2023 03:35:35 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d70f9875c06738efaaebb76e4afc48036a744793243623fcbefb6a995becd3`  
		Last Modified: Wed, 12 Apr 2023 03:35:35 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.0-alpine`

```console
$ docker pull influxdb@sha256:2f7487fe433cf4bb75526c385e3e0510de1e40c4176c8aca3858c127378d27ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:80c6ef024babe804c026931a32a9da53a0f197e3f9cddb38385321a854ad8dbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.8 MB (84838507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d81b58390e922e93331b46f3e5278c5ebf76030453daa19d53ad57c05962dc32`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:59:54 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 29 Mar 2023 21:59:54 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 05 Apr 2023 21:20:28 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 05 Apr 2023 21:20:32 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 05 Apr 2023 21:20:32 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 05 Apr 2023 21:20:34 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 05 Apr 2023 21:20:34 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 05 Apr 2023 21:20:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 05 Apr 2023 21:20:35 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 05 Apr 2023 21:20:35 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 05 Apr 2023 21:20:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Apr 2023 21:20:35 GMT
CMD ["influxd"]
# Wed, 05 Apr 2023 21:20:35 GMT
EXPOSE 8086
# Wed, 05 Apr 2023 21:20:35 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 05 Apr 2023 21:20:35 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 05 Apr 2023 21:20:35 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 05 Apr 2023 21:20:35 GMT
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
	-	`sha256:c1afb36336fe98dd703c1041000d89b9bae5d279480c46f77620057018d3e2b2`  
		Last Modified: Wed, 29 Mar 2023 22:02:42 GMT  
		Size: 12.4 MB (12374741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b2ee057b405e8d7b36616d40cb252eca7fb22085cad6642982f54ab0ca2baa`  
		Last Modified: Wed, 29 Mar 2023 22:02:40 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad124c02e9466927394363db09e8237c01e074cd7ab74357f0357697daa52b5`  
		Last Modified: Wed, 05 Apr 2023 21:21:31 GMT  
		Size: 46.3 MB (46334638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0dea23ab3557a0906d30572828a920e3255ebcb35b12c018f02a082bbfc259`  
		Last Modified: Wed, 05 Apr 2023 21:21:29 GMT  
		Size: 22.7 MB (22746040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9426dfe208286157840f45d8b1baca25f9cb660145704d2f00c5a2f8d347c9fa`  
		Last Modified: Wed, 05 Apr 2023 21:21:26 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7797b468e623ea798e1c57613918eb26a9e2a87a1c2a0f1b8c2b6b34812ef1`  
		Last Modified: Wed, 05 Apr 2023 21:21:26 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c414db96cd83babf4ed2aaa392facc4fa6715af82e8c3e6a6e3b48895bfa6356`  
		Last Modified: Wed, 05 Apr 2023 21:21:26 GMT  
		Size: 6.4 KB (6442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:006f5e1ba8af7211cd55b0b742279ade8ba591ab3b90fa963db9406cc44bff16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81084753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6be29eac1a5176462dc83c897cd42d11b2491b3c8dfdaee1607b7efebea903`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 04:17:15 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 30 Mar 2023 04:17:16 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 05 Apr 2023 21:40:33 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 05 Apr 2023 21:40:36 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 05 Apr 2023 21:40:36 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 05 Apr 2023 21:40:38 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 05 Apr 2023 21:40:39 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 05 Apr 2023 21:40:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 05 Apr 2023 21:40:39 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 05 Apr 2023 21:40:39 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 05 Apr 2023 21:40:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Apr 2023 21:40:39 GMT
CMD ["influxd"]
# Wed, 05 Apr 2023 21:40:39 GMT
EXPOSE 8086
# Wed, 05 Apr 2023 21:40:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 05 Apr 2023 21:40:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 05 Apr 2023 21:40:39 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 05 Apr 2023 21:40:39 GMT
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
	-	`sha256:73b6f835aacf2662a2b94c43a8ea49fa6bb22e7462d8ac83f92e9fcb65b3adf4`  
		Last Modified: Thu, 30 Mar 2023 04:18:06 GMT  
		Size: 12.0 MB (12027921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16b3409528a44a440ba66163e99ee9e4c43bc43aa2a65788460f2007c77cc47`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2307171e9e88cf15e41e3c512ca6958ba7cd4a0943997f73aef13b995585a48`  
		Last Modified: Wed, 05 Apr 2023 21:41:14 GMT  
		Size: 44.4 MB (44435729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba07f325899c078273a439bb929a761db612748e0e5caeffb128368ed0888b9`  
		Last Modified: Wed, 05 Apr 2023 21:41:12 GMT  
		Size: 21.4 MB (21350727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0958fc96a25897970f15196bce7df128e367670bc337ff487871733934068b0`  
		Last Modified: Wed, 05 Apr 2023 21:41:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249adfe958028dfdb4ece08fd1e5e786cc6289b05146181b808cff0db486bc69`  
		Last Modified: Wed, 05 Apr 2023 21:41:10 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae57acef8e97ce7d021f8f5bc003ae845ab318950ffc6355db05f7ec8563b88`  
		Last Modified: Wed, 05 Apr 2023 21:41:10 GMT  
		Size: 6.4 KB (6440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:2f7487fe433cf4bb75526c385e3e0510de1e40c4176c8aca3858c127378d27ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:80c6ef024babe804c026931a32a9da53a0f197e3f9cddb38385321a854ad8dbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.8 MB (84838507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d81b58390e922e93331b46f3e5278c5ebf76030453daa19d53ad57c05962dc32`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:59:54 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 29 Mar 2023 21:59:54 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 05 Apr 2023 21:20:28 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 05 Apr 2023 21:20:32 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 05 Apr 2023 21:20:32 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 05 Apr 2023 21:20:34 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 05 Apr 2023 21:20:34 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 05 Apr 2023 21:20:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 05 Apr 2023 21:20:35 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 05 Apr 2023 21:20:35 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 05 Apr 2023 21:20:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Apr 2023 21:20:35 GMT
CMD ["influxd"]
# Wed, 05 Apr 2023 21:20:35 GMT
EXPOSE 8086
# Wed, 05 Apr 2023 21:20:35 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 05 Apr 2023 21:20:35 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 05 Apr 2023 21:20:35 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 05 Apr 2023 21:20:35 GMT
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
	-	`sha256:c1afb36336fe98dd703c1041000d89b9bae5d279480c46f77620057018d3e2b2`  
		Last Modified: Wed, 29 Mar 2023 22:02:42 GMT  
		Size: 12.4 MB (12374741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b2ee057b405e8d7b36616d40cb252eca7fb22085cad6642982f54ab0ca2baa`  
		Last Modified: Wed, 29 Mar 2023 22:02:40 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad124c02e9466927394363db09e8237c01e074cd7ab74357f0357697daa52b5`  
		Last Modified: Wed, 05 Apr 2023 21:21:31 GMT  
		Size: 46.3 MB (46334638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0dea23ab3557a0906d30572828a920e3255ebcb35b12c018f02a082bbfc259`  
		Last Modified: Wed, 05 Apr 2023 21:21:29 GMT  
		Size: 22.7 MB (22746040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9426dfe208286157840f45d8b1baca25f9cb660145704d2f00c5a2f8d347c9fa`  
		Last Modified: Wed, 05 Apr 2023 21:21:26 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7797b468e623ea798e1c57613918eb26a9e2a87a1c2a0f1b8c2b6b34812ef1`  
		Last Modified: Wed, 05 Apr 2023 21:21:26 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c414db96cd83babf4ed2aaa392facc4fa6715af82e8c3e6a6e3b48895bfa6356`  
		Last Modified: Wed, 05 Apr 2023 21:21:26 GMT  
		Size: 6.4 KB (6442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:006f5e1ba8af7211cd55b0b742279ade8ba591ab3b90fa963db9406cc44bff16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81084753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6be29eac1a5176462dc83c897cd42d11b2491b3c8dfdaee1607b7efebea903`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 04:17:15 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 30 Mar 2023 04:17:16 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 05 Apr 2023 21:40:33 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 05 Apr 2023 21:40:36 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 05 Apr 2023 21:40:36 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 05 Apr 2023 21:40:38 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 05 Apr 2023 21:40:39 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 05 Apr 2023 21:40:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 05 Apr 2023 21:40:39 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 05 Apr 2023 21:40:39 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 05 Apr 2023 21:40:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Apr 2023 21:40:39 GMT
CMD ["influxd"]
# Wed, 05 Apr 2023 21:40:39 GMT
EXPOSE 8086
# Wed, 05 Apr 2023 21:40:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 05 Apr 2023 21:40:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 05 Apr 2023 21:40:39 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 05 Apr 2023 21:40:39 GMT
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
	-	`sha256:73b6f835aacf2662a2b94c43a8ea49fa6bb22e7462d8ac83f92e9fcb65b3adf4`  
		Last Modified: Thu, 30 Mar 2023 04:18:06 GMT  
		Size: 12.0 MB (12027921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16b3409528a44a440ba66163e99ee9e4c43bc43aa2a65788460f2007c77cc47`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2307171e9e88cf15e41e3c512ca6958ba7cd4a0943997f73aef13b995585a48`  
		Last Modified: Wed, 05 Apr 2023 21:41:14 GMT  
		Size: 44.4 MB (44435729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba07f325899c078273a439bb929a761db612748e0e5caeffb128368ed0888b9`  
		Last Modified: Wed, 05 Apr 2023 21:41:12 GMT  
		Size: 21.4 MB (21350727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0958fc96a25897970f15196bce7df128e367670bc337ff487871733934068b0`  
		Last Modified: Wed, 05 Apr 2023 21:41:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249adfe958028dfdb4ece08fd1e5e786cc6289b05146181b808cff0db486bc69`  
		Last Modified: Wed, 05 Apr 2023 21:41:10 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae57acef8e97ce7d021f8f5bc003ae845ab318950ffc6355db05f7ec8563b88`  
		Last Modified: Wed, 05 Apr 2023 21:41:10 GMT  
		Size: 6.4 KB (6440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:651fb015520279fc2eb70429e5e39a0cb27a00e373270af4abce43e1324d8bf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:d8c700b1e793262594120826f9773525711d5da51c8a507f903a8e52e5eccd57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127804861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:991f6378bce35ee5f4e6068f9d196d026a42957cba592edbe3d8faf0aa0406bc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 14:03:59 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 12 Apr 2023 14:04:05 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 Apr 2023 14:04:05 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 12 Apr 2023 14:04:05 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 14:04:05 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 14:04:06 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 12 Apr 2023 14:04:06 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 Apr 2023 14:04:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 14:04:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cf5d0ed10ace6baeea02705ffa1ffda74ce779efe566c6fe809b8394cc35e2`  
		Last Modified: Wed, 12 Apr 2023 14:05:59 GMT  
		Size: 56.7 MB (56705107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d3b9ddf0193b06f898d957b9b6e124283fcf97ba7145e80b4600cfd6d665bd`  
		Last Modified: Wed, 12 Apr 2023 14:05:52 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437cc0e198df5b2772d7092253d0eef4b36ee456285c417834d11e3c0c1c6582`  
		Last Modified: Wed, 12 Apr 2023 14:05:52 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be58dc3ea55fc0f5be05a6b9f6db5b99ced026fe55b99e291afe6bdefd620e29`  
		Last Modified: Wed, 12 Apr 2023 14:05:52 GMT  
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
$ docker pull influxdb@sha256:4b811aa4a47a0e5074466c1320fb0932a760933192112809447d0142ca2773f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:32b2c4d5e6fc96da0f6eb325aacc635964d44844cac95bbdee07e620afdf27e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114869180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7de0f3140b356698d7c7ca47cfbefb1aae55a35a70c3b2d8daaa3f7f0cd20bfe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:48:51 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:48:52 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 01:48:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 01:48:53 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 01:48:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 01:49:22 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 12 Apr 2023 01:49:27 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 01:49:27 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 12 Apr 2023 01:49:30 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 01:49:30 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 01:49:30 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 01:49:31 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 01:49:31 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 01:49:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 01:49:31 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 01:49:31 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 01:49:31 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 01:49:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 01:49:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 01:49:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631d89e80e4efea8f2c84cb5859b809336e7f53594b8db437806fb3129cf21d`  
		Last Modified: Wed, 12 Apr 2023 01:50:14 GMT  
		Size: 6.3 MB (6327895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60742865a130d899cb9320c3a041fe9b11b34ade8ac793a1bc1c83f6501a4f65`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 7.0 MB (7049185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f3017aa8d7ad8894b072504c2c5cb8b438869314a672ebbaf85313121a3da6`  
		Last Modified: Wed, 12 Apr 2023 01:50:11 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f60e0bc8b1363351a48dc6cffc215f18c8f46611920aca91d34d7fa97b71d`  
		Last Modified: Wed, 12 Apr 2023 01:50:12 GMT  
		Size: 982.0 KB (982037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a9890bc19a612aa3936ca8f366ba2458d939c934c58855dfa744e415d8bfed`  
		Last Modified: Wed, 12 Apr 2023 01:50:47 GMT  
		Size: 46.3 MB (46334688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dde9a44430dd3a49742911da50232ecae252a57a169d2feb1074a37cbbcdd72`  
		Last Modified: Wed, 12 Apr 2023 01:50:44 GMT  
		Size: 22.7 MB (22746035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ae2894ff3aea334c8bd14e48affa8db988bf2cd184ed8267df559baf8bf6e9`  
		Last Modified: Wed, 12 Apr 2023 01:50:41 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af0707a6d12c69ffe7602747c319c45ed9b50a6d619f094957f8b13dae7eda5`  
		Last Modified: Wed, 12 Apr 2023 01:50:42 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b6ab443599ec65c641cef83b3437c89422b162898083611511da032533bb75`  
		Last Modified: Wed, 12 Apr 2023 01:50:42 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9777b6331615014935e3c4428ed1de0a38e7df1db6f43d844575dc9d43d132d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109730104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97e29edb242329b633cb94a5fe4686cc1895afccea8f9212807c6341555984d9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:34:08 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:34:09 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 12 Apr 2023 03:34:10 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 12 Apr 2023 03:34:10 GMT
ENV GOSU_VER=1.12
# Wed, 12 Apr 2023 03:34:12 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 12 Apr 2023 03:34:38 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 12 Apr 2023 03:34:42 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 12 Apr 2023 03:34:42 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 12 Apr 2023 03:34:45 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 12 Apr 2023 03:34:45 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 12 Apr 2023 03:34:45 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 12 Apr 2023 03:34:45 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 12 Apr 2023 03:34:45 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 12 Apr 2023 03:34:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 03:34:46 GMT
CMD ["influxd"]
# Wed, 12 Apr 2023 03:34:46 GMT
EXPOSE 8086
# Wed, 12 Apr 2023 03:34:46 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 12 Apr 2023 03:34:46 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 12 Apr 2023 03:34:46 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 12 Apr 2023 03:34:46 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b243f57d3a1ebfedb4718e25ead24072a440224c350ebe24f3822295c87282`  
		Last Modified: Wed, 12 Apr 2023 03:35:14 GMT  
		Size: 6.3 MB (6308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9df8ad4ddd6a2b1c0cae9d3204053c8346ee8a6aa7a5d37d8d54273daa21c7`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 6.6 MB (6643035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27a311d7f96094d6c9e8d0f73ebf4f9d1710ef98e86d7fe08576a30d1df33bb`  
		Last Modified: Wed, 12 Apr 2023 03:35:12 GMT  
		Size: 4.1 KB (4120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3784a77e687bbe1d8bef04cb5527d2cc3a956ee846a51a299f412b13ef9e1ee`  
		Last Modified: Wed, 12 Apr 2023 03:35:13 GMT  
		Size: 916.9 KB (916933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b0bd765dbad7244932d0bc6e1b0ae45d24d3ea38107b90f8bff5d9a6f4fa13`  
		Last Modified: Wed, 12 Apr 2023 03:35:39 GMT  
		Size: 44.4 MB (44435735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d0e0d56916614791112b9ad2c4ddf16daba60b57122fa5634311c84b91a8fc`  
		Last Modified: Wed, 12 Apr 2023 03:35:37 GMT  
		Size: 21.4 MB (21350751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12f8122a52d5645972b687700a7ede09c1224947361c97164f26e01e9ac397f`  
		Last Modified: Wed, 12 Apr 2023 03:35:35 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f31e093c31418eb240b0e92b54629abf1428400dc52a2eef1119f4e869b120`  
		Last Modified: Wed, 12 Apr 2023 03:35:35 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d70f9875c06738efaaebb76e4afc48036a744793243623fcbefb6a995becd3`  
		Last Modified: Wed, 12 Apr 2023 03:35:35 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:8b8e0f30019a3e43168ef1093f15f04f7ea044d1e9d23b27dac170621034abf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:e5abdeaae36b91e4896be90948f0223c58652a82ab9e2c5572ecd148533d9346
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94511353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b5008aee83e3a9cee431e796df5e69d029b9f99106a3ff40fb9fb7bc0faf52`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 14:03:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 12 Apr 2023 14:03:59 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 12 Apr 2023 14:04:16 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 Apr 2023 14:04:16 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 12 Apr 2023 14:04:17 GMT
EXPOSE 8091
# Wed, 12 Apr 2023 14:04:17 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 Apr 2023 14:04:17 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 12 Apr 2023 14:04:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 14:04:17 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b00312931323a7e65b8fcb723e6c767ed0e5b7b5ebca9059ebd8bab99bbf8`  
		Last Modified: Wed, 12 Apr 2023 14:05:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0bb276fc62e020dd98ab120e4174c470a49b8ca3038ec79dea13dce5cb180`  
		Last Modified: Wed, 12 Apr 2023 14:06:13 GMT  
		Size: 23.4 MB (23412806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7ea4ee8b2b00dfcf27aa5da85c49615b0abffe26b0c2aadf01092cccf622c3`  
		Last Modified: Wed, 12 Apr 2023 14:06:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21df78c7760fcc2ae463fe4b3480b417d6c074c71aa2738671e877df5b07964`  
		Last Modified: Wed, 12 Apr 2023 14:06:10 GMT  
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
