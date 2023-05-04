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
$ docker pull influxdb@sha256:2aa953538d84e2ac8c83be23213480e214987a76933f16daeed542d949bcd420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:523932dbfca884827d818940671422fc435607df86f649accb846038e1bae989
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110879473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e547846683dd2f70ddf13795af363dfc8589cb31e336c877a827dc42f87c0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:55 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Thu, 04 May 2023 10:55:57 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:58 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:55:58 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:55:58 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:58 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:58 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:55:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:58 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9346323c3c91678b886bb3d22fc6598bf48e595560dbecadeb577e5ac87d0626`  
		Last Modified: Thu, 04 May 2023 10:57:44 GMT  
		Size: 40.1 MB (40066485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55922205480ceece4b9278d6694a3fd6067cb6a21d391b4460d7e2923a124ca`  
		Last Modified: Thu, 04 May 2023 10:57:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25fdf0dba9152f960a29713d9b3fa3ff3da496a19ed4d95d73ff9dddcfe67dee`  
		Last Modified: Thu, 04 May 2023 10:57:38 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73718238f4e7f4e3619d7905d75ad7ca6c9b3a03520dc2b1c3098bc7d5e9741d`  
		Last Modified: Thu, 04 May 2023 10:57:38 GMT  
		Size: 1.3 KB (1279 bytes)  
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
$ docker pull influxdb@sha256:6b0db1d7c3a2f118dc1a4f734d51ccc88b6f4022a8b9e1d35fbf1eb41352639c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:294d22f57af7a62bf2116fa2ab2ba049bdabf2ec3729a9287610de38d2f51e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91045826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d369d028340d33beaafdf728ed4b2fee4c2dc2b37f989ac021bc8d9a03f62205`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:55 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Thu, 04 May 2023 10:56:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:56:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 04 May 2023 10:56:04 GMT
EXPOSE 8091
# Thu, 04 May 2023 10:56:04 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:56:04 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 04 May 2023 10:56:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:56:05 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c27432c6e754395e5c2bb5156e459a9b2451dd46f43efab64e32baff4bcafda`  
		Last Modified: Thu, 04 May 2023 10:57:55 GMT  
		Size: 20.2 MB (20234038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f39ecb47fc0a05aaa374617aa21187526e8ac1beae11149ac2ef172d00cace`  
		Last Modified: Thu, 04 May 2023 10:57:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eec407f23a2d817f568db0ba23d833dd177b582595f54157404bd5db717e64`  
		Last Modified: Thu, 04 May 2023 10:57:52 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:2aa953538d84e2ac8c83be23213480e214987a76933f16daeed542d949bcd420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.3-data` - linux; amd64

```console
$ docker pull influxdb@sha256:523932dbfca884827d818940671422fc435607df86f649accb846038e1bae989
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110879473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e547846683dd2f70ddf13795af363dfc8589cb31e336c877a827dc42f87c0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:55 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Thu, 04 May 2023 10:55:57 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:58 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:55:58 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:55:58 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:58 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:58 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:55:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:58 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9346323c3c91678b886bb3d22fc6598bf48e595560dbecadeb577e5ac87d0626`  
		Last Modified: Thu, 04 May 2023 10:57:44 GMT  
		Size: 40.1 MB (40066485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55922205480ceece4b9278d6694a3fd6067cb6a21d391b4460d7e2923a124ca`  
		Last Modified: Thu, 04 May 2023 10:57:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25fdf0dba9152f960a29713d9b3fa3ff3da496a19ed4d95d73ff9dddcfe67dee`  
		Last Modified: Thu, 04 May 2023 10:57:38 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73718238f4e7f4e3619d7905d75ad7ca6c9b3a03520dc2b1c3098bc7d5e9741d`  
		Last Modified: Thu, 04 May 2023 10:57:38 GMT  
		Size: 1.3 KB (1279 bytes)  
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
$ docker pull influxdb@sha256:6b0db1d7c3a2f118dc1a4f734d51ccc88b6f4022a8b9e1d35fbf1eb41352639c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.3-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:294d22f57af7a62bf2116fa2ab2ba049bdabf2ec3729a9287610de38d2f51e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91045826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d369d028340d33beaafdf728ed4b2fee4c2dc2b37f989ac021bc8d9a03f62205`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:55 GMT
ENV INFLUXDB_VERSION=1.10.3-c1.10.3
# Thu, 04 May 2023 10:56:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:56:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 04 May 2023 10:56:04 GMT
EXPOSE 8091
# Thu, 04 May 2023 10:56:04 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:56:04 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 04 May 2023 10:56:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:56:05 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c27432c6e754395e5c2bb5156e459a9b2451dd46f43efab64e32baff4bcafda`  
		Last Modified: Thu, 04 May 2023 10:57:55 GMT  
		Size: 20.2 MB (20234038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f39ecb47fc0a05aaa374617aa21187526e8ac1beae11149ac2ef172d00cace`  
		Last Modified: Thu, 04 May 2023 10:57:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eec407f23a2d817f568db0ba23d833dd177b582595f54157404bd5db717e64`  
		Last Modified: Thu, 04 May 2023 10:57:52 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:89bd72ed93c7c2f23f663e968c82234d3c8520d3979018b55cd5e629dd3cc628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:59cb9b20e8185541601de1bfa709517720eb5fee8bdb7ad205aad30de3be1f03
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125698683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94160f7806725540a3d1fb7bc87cd9054bd3801d1df2cc472c09a4ebfc537c11`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:13 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 04 May 2023 10:55:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 04 May 2023 10:55:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:55:18 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:55:18 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:18 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:18 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:55:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:18 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8074b4fc9360904663722477d717c4589a0b36ea709da96c2c7c1102c5b1127`  
		Last Modified: Thu, 04 May 2023 10:56:36 GMT  
		Size: 54.9 MB (54885754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a913b47223309e1aa25838df64b8aa6af7aa52012160cef70f72e832534ec9c1`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8265b2cf7ab8b2a059fa6bdacd7801b91f767ab02fba508da9c74a8aff5ed8`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9037f1aeb9df3c66862416f5fd8453b21cfefb392c9c5c1b925316492dae0af8`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:9c26bbd4d3a2b48e79b8db94343c015f8c3a66d3f1ddabb9beeb27c0c7d618be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116695201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10df6331d080e96fd32ed2abc3dd215e5025bfa84f55b95842a2f70367358227`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:47:46 GMT
ADD file:668ced72eb3825a6cfd123f77fed6c64b8ad5bf1f4aa8e78ede9512198ca65ad in / 
# Tue, 02 May 2023 23:47:47 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:53:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:35:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:35:45 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 04 May 2023 10:35:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 04 May 2023 10:35:51 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:35:51 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:35:51 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:35:51 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 04 May 2023 10:35:51 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:35:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:35:51 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:755944445ece6eac276e067f465680b57daac59a0ed9ce97e7c501f1cde8621d`  
		Last Modified: Tue, 02 May 2023 23:51:06 GMT  
		Size: 50.2 MB (50210011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979fe7914af9b87a93e67c054d2be5b1a2a0b052f4257f06ce7dc8c03570892`  
		Last Modified: Wed, 03 May 2023 22:09:00 GMT  
		Size: 14.9 MB (14868556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36eb1b4119fb61734fedb88132ee136d6f9af8e24a05c82397066851fd3318d3`  
		Last Modified: Thu, 04 May 2023 10:35:59 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e43c16448d13fe57e419fcd24e73d533ef686a4707ef7d4e6ce099bc870c5`  
		Last Modified: Thu, 04 May 2023 10:36:05 GMT  
		Size: 51.6 MB (51613122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685def524101cb24a0d77347a59d5d67094fb692855776f7f8b1d6d9a92f1e57`  
		Last Modified: Thu, 04 May 2023 10:35:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8271e7c0a37cd5865d440fe92c8404ee32d34e27543be4349e1afd6be1cdc9d4`  
		Last Modified: Thu, 04 May 2023 10:35:58 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4637f29df9d50e85ccce52412f39f968da5538963706904d95860985344ddb`  
		Last Modified: Thu, 04 May 2023 10:35:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:1c9d4a4aa80bd4049e479fa0924d2e7cd881677650ddcc8193a72e2d949a97a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120673061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e1c39bb032cafbabf88e2405503cd14e87548320a7aa28c2d7f6241fb446da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 03 May 2023 00:22:41 GMT
ADD file:f930fdb659332a615b0042ca415d6d7feda9ba6b2f58222e3e5bbed326db4d40 in / 
# Wed, 03 May 2023 00:22:42 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 04:34:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 04:34:51 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 04 May 2023 04:34:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 04 May 2023 04:34:55 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 04:34:55 GMT
EXPOSE 8086
# Thu, 04 May 2023 04:34:55 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 04:34:55 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 04 May 2023 04:34:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 04:34:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 04:34:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d677c78be691f8dcbe9d44ce576b97ad205b3dd78557dc62794e59eb19553ee9`  
		Last Modified: Wed, 03 May 2023 00:25:31 GMT  
		Size: 53.7 MB (53692705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73587d290df17347645f166c8385f0a2d320a31f4803658f619f2887a5d88faf`  
		Last Modified: Wed, 03 May 2023 17:36:59 GMT  
		Size: 15.7 MB (15746737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d851f9a7345aeb4976d1bb354959b9efb60a1c9675ef989e9536b365980ded7a`  
		Last Modified: Thu, 04 May 2023 04:35:06 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4720f84b822f8b333a09ef28e6c5df5f974cdff5b63808a379a793b4557d5f63`  
		Last Modified: Thu, 04 May 2023 04:35:10 GMT  
		Size: 51.2 MB (51230106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e273928f38f715d6b7f259105f285efd2709ae3fd3c1485052e742c9eb9906`  
		Last Modified: Thu, 04 May 2023 04:35:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfde179cb264f3987bad30b9826a76dcf57dd79a357a1dc7783e432ea4df904e`  
		Last Modified: Thu, 04 May 2023 04:35:05 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a1dbd10fcd916ad293e2eeb389bb210546b9da9f67314f4dbf1aa98879133`  
		Last Modified: Thu, 04 May 2023 04:35:05 GMT  
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
$ docker pull influxdb@sha256:ca98b623d9512ed8ed9274058d4e078109f07fc55f143ff3511a9d41af6692cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:9d884ada1b799a356c9ffcaa53aa2914fd8c5a1cfe5be6f80abbd7e330d6bf10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127518125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1538bfce69e3dc5bb370450b2ce9d78c643f50898c50b5e43e686d706527d5fc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:22 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 04 May 2023 10:55:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:30 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:55:30 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:55:30 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:55:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ad4359c5f3d8340b96395986520fd3a347167a51b7033e3415ca92b76cf7b1`  
		Last Modified: Thu, 04 May 2023 10:56:52 GMT  
		Size: 56.7 MB (56705136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905dcfeb634b16d5b59f824b3d967725f2e95ad71d0ca7edec1101625fe6f005`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d9fad405d2820272db336a50bae1d55e209c05db0b62e569db1bfcc3e7cecc`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000dd25bf5c3dd19ffcb1235ebc0243195891dba177dadda8430f6d6b4a2e330`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
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
$ docker pull influxdb@sha256:1818dc3a1014ff8bc213b5c5c681328888abec46f3d4474e5135bee3b70d6f36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:f0603d40ad7756af805eab578df632b498915815db7c4a5cbfcb3da0bb3df3ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94224599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fe6dc3badf2bd640104ad7f14bf852f0f9f759cf005ab0204d363bf28060ad5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:22 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 04 May 2023 10:55:37 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:37 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 04 May 2023 10:55:37 GMT
EXPOSE 8091
# Thu, 04 May 2023 10:55:37 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:38 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:38 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0368ac17311eed9aa2f8af4609296812671e408e74467e8a3780f1b6c96647f`  
		Last Modified: Thu, 04 May 2023 10:57:05 GMT  
		Size: 23.4 MB (23412812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957182bf465a16a9c61a29d31942940468a7088fdf3edc6bc6fb48df5c0668e0`  
		Last Modified: Thu, 04 May 2023 10:57:02 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756b9e95001e2a1351853e2c1fe60b068c14e181fd926b78f4d49961880c71ee`  
		Last Modified: Thu, 04 May 2023 10:57:02 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:89bd72ed93c7c2f23f663e968c82234d3c8520d3979018b55cd5e629dd3cc628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:59cb9b20e8185541601de1bfa709517720eb5fee8bdb7ad205aad30de3be1f03
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125698683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94160f7806725540a3d1fb7bc87cd9054bd3801d1df2cc472c09a4ebfc537c11`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:13 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 04 May 2023 10:55:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 04 May 2023 10:55:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:55:18 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:55:18 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:18 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:18 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:55:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:18 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8074b4fc9360904663722477d717c4589a0b36ea709da96c2c7c1102c5b1127`  
		Last Modified: Thu, 04 May 2023 10:56:36 GMT  
		Size: 54.9 MB (54885754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a913b47223309e1aa25838df64b8aa6af7aa52012160cef70f72e832534ec9c1`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8265b2cf7ab8b2a059fa6bdacd7801b91f767ab02fba508da9c74a8aff5ed8`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9037f1aeb9df3c66862416f5fd8453b21cfefb392c9c5c1b925316492dae0af8`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:9c26bbd4d3a2b48e79b8db94343c015f8c3a66d3f1ddabb9beeb27c0c7d618be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116695201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10df6331d080e96fd32ed2abc3dd215e5025bfa84f55b95842a2f70367358227`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:47:46 GMT
ADD file:668ced72eb3825a6cfd123f77fed6c64b8ad5bf1f4aa8e78ede9512198ca65ad in / 
# Tue, 02 May 2023 23:47:47 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:53:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:35:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:35:45 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 04 May 2023 10:35:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 04 May 2023 10:35:51 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:35:51 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:35:51 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:35:51 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 04 May 2023 10:35:51 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:35:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:35:51 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:755944445ece6eac276e067f465680b57daac59a0ed9ce97e7c501f1cde8621d`  
		Last Modified: Tue, 02 May 2023 23:51:06 GMT  
		Size: 50.2 MB (50210011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979fe7914af9b87a93e67c054d2be5b1a2a0b052f4257f06ce7dc8c03570892`  
		Last Modified: Wed, 03 May 2023 22:09:00 GMT  
		Size: 14.9 MB (14868556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36eb1b4119fb61734fedb88132ee136d6f9af8e24a05c82397066851fd3318d3`  
		Last Modified: Thu, 04 May 2023 10:35:59 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e43c16448d13fe57e419fcd24e73d533ef686a4707ef7d4e6ce099bc870c5`  
		Last Modified: Thu, 04 May 2023 10:36:05 GMT  
		Size: 51.6 MB (51613122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685def524101cb24a0d77347a59d5d67094fb692855776f7f8b1d6d9a92f1e57`  
		Last Modified: Thu, 04 May 2023 10:35:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8271e7c0a37cd5865d440fe92c8404ee32d34e27543be4349e1afd6be1cdc9d4`  
		Last Modified: Thu, 04 May 2023 10:35:58 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4637f29df9d50e85ccce52412f39f968da5538963706904d95860985344ddb`  
		Last Modified: Thu, 04 May 2023 10:35:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:1c9d4a4aa80bd4049e479fa0924d2e7cd881677650ddcc8193a72e2d949a97a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120673061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e1c39bb032cafbabf88e2405503cd14e87548320a7aa28c2d7f6241fb446da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 03 May 2023 00:22:41 GMT
ADD file:f930fdb659332a615b0042ca415d6d7feda9ba6b2f58222e3e5bbed326db4d40 in / 
# Wed, 03 May 2023 00:22:42 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 04:34:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 04:34:51 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 04 May 2023 04:34:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 04 May 2023 04:34:55 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 04:34:55 GMT
EXPOSE 8086
# Thu, 04 May 2023 04:34:55 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 04:34:55 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 04 May 2023 04:34:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 04:34:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 04:34:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d677c78be691f8dcbe9d44ce576b97ad205b3dd78557dc62794e59eb19553ee9`  
		Last Modified: Wed, 03 May 2023 00:25:31 GMT  
		Size: 53.7 MB (53692705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73587d290df17347645f166c8385f0a2d320a31f4803658f619f2887a5d88faf`  
		Last Modified: Wed, 03 May 2023 17:36:59 GMT  
		Size: 15.7 MB (15746737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d851f9a7345aeb4976d1bb354959b9efb60a1c9675ef989e9536b365980ded7a`  
		Last Modified: Thu, 04 May 2023 04:35:06 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4720f84b822f8b333a09ef28e6c5df5f974cdff5b63808a379a793b4557d5f63`  
		Last Modified: Thu, 04 May 2023 04:35:10 GMT  
		Size: 51.2 MB (51230106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e273928f38f715d6b7f259105f285efd2709ae3fd3c1485052e742c9eb9906`  
		Last Modified: Thu, 04 May 2023 04:35:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfde179cb264f3987bad30b9826a76dcf57dd79a357a1dc7783e432ea4df904e`  
		Last Modified: Thu, 04 May 2023 04:35:05 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a1dbd10fcd916ad293e2eeb389bb210546b9da9f67314f4dbf1aa98879133`  
		Last Modified: Thu, 04 May 2023 04:35:05 GMT  
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
$ docker pull influxdb@sha256:ca98b623d9512ed8ed9274058d4e078109f07fc55f143ff3511a9d41af6692cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:9d884ada1b799a356c9ffcaa53aa2914fd8c5a1cfe5be6f80abbd7e330d6bf10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127518125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1538bfce69e3dc5bb370450b2ce9d78c643f50898c50b5e43e686d706527d5fc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:22 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 04 May 2023 10:55:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:30 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:55:30 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:55:30 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:55:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ad4359c5f3d8340b96395986520fd3a347167a51b7033e3415ca92b76cf7b1`  
		Last Modified: Thu, 04 May 2023 10:56:52 GMT  
		Size: 56.7 MB (56705136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905dcfeb634b16d5b59f824b3d967725f2e95ad71d0ca7edec1101625fe6f005`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d9fad405d2820272db336a50bae1d55e209c05db0b62e569db1bfcc3e7cecc`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000dd25bf5c3dd19ffcb1235ebc0243195891dba177dadda8430f6d6b4a2e330`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
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
$ docker pull influxdb@sha256:1818dc3a1014ff8bc213b5c5c681328888abec46f3d4474e5135bee3b70d6f36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:f0603d40ad7756af805eab578df632b498915815db7c4a5cbfcb3da0bb3df3ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94224599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fe6dc3badf2bd640104ad7f14bf852f0f9f759cf005ab0204d363bf28060ad5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:22 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 04 May 2023 10:55:37 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:37 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 04 May 2023 10:55:37 GMT
EXPOSE 8091
# Thu, 04 May 2023 10:55:37 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:38 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:38 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0368ac17311eed9aa2f8af4609296812671e408e74467e8a3780f1b6c96647f`  
		Last Modified: Thu, 04 May 2023 10:57:05 GMT  
		Size: 23.4 MB (23412812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957182bf465a16a9c61a29d31942940468a7088fdf3edc6bc6fb48df5c0668e0`  
		Last Modified: Thu, 04 May 2023 10:57:02 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756b9e95001e2a1351853e2c1fe60b068c14e181fd926b78f4d49961880c71ee`  
		Last Modified: Thu, 04 May 2023 10:57:02 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:28ab0c59362aa6f99797a4bcb4949861677a03858c219b813fc22dfeec8568de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:d9a7dbfdfac5c7a0a00f42e4d7699488783c0b15d49733f37f151cd62e7805a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.0 MB (103980662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2821ebf4e0af48142b732840cf14bf2c54973d49172ce141fdefb11a5da29f85`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:41 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Thu, 04 May 2023 10:55:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:44 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:55:44 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:55:44 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:44 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:44 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:55:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:45 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0c19c2e9d2c6901356ab24b7f7ff1fba677ec49d0272346c2d693f9273490b`  
		Last Modified: Thu, 04 May 2023 10:57:20 GMT  
		Size: 33.2 MB (33167673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b577730df90474c0bfb1bc15a1ebb080fbbb2399d5430b1e79cb8d2f885338b`  
		Last Modified: Thu, 04 May 2023 10:57:15 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c6c4c27b14ab56cf13fb6a65625d0d6bd55f065fd6f2438c58b2968cf8fa4b`  
		Last Modified: Thu, 04 May 2023 10:57:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c662c5b8b688f0acf02f0d6e2b18598cf93796830fdb97fdb0506c76ea8a16bc`  
		Last Modified: Thu, 04 May 2023 10:57:15 GMT  
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
$ docker pull influxdb@sha256:f5564ce33121d34088cd6ce7a5a14445643d3bbe9a3f793d20f0804cfbef9cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:e2849332f57535145991fc5b04dbc1eff7d771d7fc407098f130505688f67535
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83426327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ead763b0ef4c285cca52f0cd0c384adb2959dd1db5c95b08e8209baf7580ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:41 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Thu, 04 May 2023 10:55:50 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:50 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 04 May 2023 10:55:50 GMT
EXPOSE 8091
# Thu, 04 May 2023 10:55:50 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:50 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:51 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161ba075110ba2594d26c2f91687704d75a37a3aa54fbff9a9d44a0e2b8a30f3`  
		Last Modified: Thu, 04 May 2023 10:57:30 GMT  
		Size: 12.6 MB (12614545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0cec774b5bb6797d1b7171912c48339464cb47c7da9baf45434a037f4df5de`  
		Last Modified: Thu, 04 May 2023 10:57:28 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39144a358807be42355a4f4ee4c2ce716f63ff331e89092b609b74d690a99f3`  
		Last Modified: Thu, 04 May 2023 10:57:28 GMT  
		Size: 375.0 B  
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
$ docker pull influxdb@sha256:28ab0c59362aa6f99797a4bcb4949861677a03858c219b813fc22dfeec8568de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:d9a7dbfdfac5c7a0a00f42e4d7699488783c0b15d49733f37f151cd62e7805a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.0 MB (103980662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2821ebf4e0af48142b732840cf14bf2c54973d49172ce141fdefb11a5da29f85`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:41 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Thu, 04 May 2023 10:55:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:44 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:55:44 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:55:44 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:44 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:44 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:55:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:45 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0c19c2e9d2c6901356ab24b7f7ff1fba677ec49d0272346c2d693f9273490b`  
		Last Modified: Thu, 04 May 2023 10:57:20 GMT  
		Size: 33.2 MB (33167673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b577730df90474c0bfb1bc15a1ebb080fbbb2399d5430b1e79cb8d2f885338b`  
		Last Modified: Thu, 04 May 2023 10:57:15 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c6c4c27b14ab56cf13fb6a65625d0d6bd55f065fd6f2438c58b2968cf8fa4b`  
		Last Modified: Thu, 04 May 2023 10:57:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c662c5b8b688f0acf02f0d6e2b18598cf93796830fdb97fdb0506c76ea8a16bc`  
		Last Modified: Thu, 04 May 2023 10:57:15 GMT  
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
$ docker pull influxdb@sha256:f5564ce33121d34088cd6ce7a5a14445643d3bbe9a3f793d20f0804cfbef9cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:e2849332f57535145991fc5b04dbc1eff7d771d7fc407098f130505688f67535
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83426327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ead763b0ef4c285cca52f0cd0c384adb2959dd1db5c95b08e8209baf7580ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:41 GMT
ENV INFLUXDB_VERSION=1.9.11-c1.9.11
# Thu, 04 May 2023 10:55:50 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:50 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 04 May 2023 10:55:50 GMT
EXPOSE 8091
# Thu, 04 May 2023 10:55:50 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:50 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:51 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161ba075110ba2594d26c2f91687704d75a37a3aa54fbff9a9d44a0e2b8a30f3`  
		Last Modified: Thu, 04 May 2023 10:57:30 GMT  
		Size: 12.6 MB (12614545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0cec774b5bb6797d1b7171912c48339464cb47c7da9baf45434a037f4df5de`  
		Last Modified: Thu, 04 May 2023 10:57:28 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39144a358807be42355a4f4ee4c2ce716f63ff331e89092b609b74d690a99f3`  
		Last Modified: Thu, 04 May 2023 10:57:28 GMT  
		Size: 375.0 B  
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
$ docker pull influxdb@sha256:c329d32475b1da4205df2e66408ef46689bc77198ecb72f7e87924e7cd109c9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7` - linux; amd64

```console
$ docker pull influxdb@sha256:11b8f3ad1e8a41a028b2de4b9a0466a57df7a25386bfd347d220ccca1a75b4dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114621478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ca18052b424265e2afadad6d256121ef833fc3a7ca8e77a14832a2aa1d8218`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 12:40:19 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:40:20 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 03 May 2023 12:40:20 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 03 May 2023 12:40:21 GMT
ENV GOSU_VER=1.12
# Wed, 03 May 2023 12:40:23 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 03 May 2023 12:40:23 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 03 May 2023 12:40:27 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 03 May 2023 12:40:27 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 03 May 2023 12:40:29 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 03 May 2023 12:40:30 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 03 May 2023 12:40:30 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 03 May 2023 12:40:30 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 03 May 2023 12:40:30 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Wed, 03 May 2023 12:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 12:40:30 GMT
CMD ["influxd"]
# Wed, 03 May 2023 12:40:30 GMT
EXPOSE 8086
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 03 May 2023 12:40:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0794cf0495a3caa74a71b6504803db62386b162e0862936e7094165af35a7ca2`  
		Last Modified: Wed, 03 May 2023 12:42:34 GMT  
		Size: 6.3 MB (6327884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4f7028e33b7b5de9c755a27c3e9ea1cf7d9913cb6c9b5cfcac31cd9a447a8`  
		Last Modified: Wed, 03 May 2023 12:42:33 GMT  
		Size: 6.4 MB (6434104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf91486cf86efc213e9b76cad5e74d49d01dc78896657c3d004b559198f73be`  
		Last Modified: Wed, 03 May 2023 12:42:31 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91daaa2fee4ceb2f269b802c20828e0ac42083951c9fcc9ed0e3c4dc42153f6`  
		Last Modified: Wed, 03 May 2023 12:42:32 GMT  
		Size: 982.0 KB (982049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fdcd2c51969abd5037cc3d56c63e90bc690dde62815fd99efb0efb695b0e52`  
		Last Modified: Wed, 03 May 2023 12:42:35 GMT  
		Size: 46.3 MB (46334322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46a6f45402719e52e80ca1165e7f375999ec943f1e31d5c15ac0f5cc0ef1569`  
		Last Modified: Wed, 03 May 2023 12:42:32 GMT  
		Size: 23.1 MB (23128344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c1d04df637a1edfea8b7f4a66691694104d136429b8fde52098203255c22a1`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a0962e3a5b231760a56a750fbb7f02fa94037b65c765177e10391997d8edf0`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bcae2cf40e36863a533dc1b6c6b622312e7460093175b16b1622fb656f721c`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:730cf48a80b760051f40f0493255d88b1feee636fb867f0270a859e0d1034024
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109341764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2658e03c9acab92c54f70cafdc1e334fd5b5e9b8ab8669c00f0d6fb971ccf41d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 14:08:58 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 14:08:59 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 03 May 2023 14:09:00 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 03 May 2023 14:09:00 GMT
ENV GOSU_VER=1.12
# Wed, 03 May 2023 14:09:03 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 03 May 2023 14:09:03 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 03 May 2023 14:09:07 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 03 May 2023 14:09:08 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 03 May 2023 14:09:10 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 03 May 2023 14:09:11 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 03 May 2023 14:09:11 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 03 May 2023 14:09:11 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 03 May 2023 14:09:11 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Wed, 03 May 2023 14:09:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 14:09:11 GMT
CMD ["influxd"]
# Wed, 03 May 2023 14:09:11 GMT
EXPOSE 8086
# Wed, 03 May 2023 14:09:11 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 03 May 2023 14:09:11 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 03 May 2023 14:09:11 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 03 May 2023 14:09:11 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e980dde75d021cfed4b514b5ddd40b560b30e874d1f291ec4ab9598ad38d167`  
		Last Modified: Wed, 03 May 2023 14:09:43 GMT  
		Size: 6.3 MB (6308694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfd9ebb6ce6e83f63bc6beddd6136d57d19e4e582ebc978fb253e1aa9c8ca74`  
		Last Modified: Wed, 03 May 2023 14:09:41 GMT  
		Size: 6.0 MB (5953758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fb470a28ffe2ce11824d35ac17f32b9b06686daa52fdd64cdfa72c6546d554`  
		Last Modified: Wed, 03 May 2023 14:09:40 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b6a269269bf191ab56376b65cd467d20c9da4013fdcef13216cdf39e211224`  
		Last Modified: Wed, 03 May 2023 14:09:41 GMT  
		Size: 916.9 KB (916932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8cedefc667f7abbd48444542f176680f9801190f8d1d0a99546e1093d298eb`  
		Last Modified: Wed, 03 May 2023 14:09:42 GMT  
		Size: 44.4 MB (44435818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6b3fb5f737c93b7a8782ac947e6be06aed507cca80cb5fe1f7a0355b0cca28`  
		Last Modified: Wed, 03 May 2023 14:09:40 GMT  
		Size: 21.7 MB (21662571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d02413eed321b52ccc5bbc46933726ae7fa5ef6f41fd3e1055d13d0d495e3dd`  
		Last Modified: Wed, 03 May 2023 14:09:38 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27eb8cdfc21e2b71bad9dbad6d510d6f9e9583780d3a4f964676dc4de157c331`  
		Last Modified: Wed, 03 May 2023 14:09:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cd6ae8950cf597abab315d9234da4d4b29e874707ba7300c0e8469bdf54b1a`  
		Last Modified: Wed, 03 May 2023 14:09:38 GMT  
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
$ docker pull influxdb@sha256:c329d32475b1da4205df2e66408ef46689bc77198ecb72f7e87924e7cd109c9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.1` - linux; amd64

```console
$ docker pull influxdb@sha256:11b8f3ad1e8a41a028b2de4b9a0466a57df7a25386bfd347d220ccca1a75b4dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114621478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ca18052b424265e2afadad6d256121ef833fc3a7ca8e77a14832a2aa1d8218`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 12:40:19 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:40:20 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 03 May 2023 12:40:20 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 03 May 2023 12:40:21 GMT
ENV GOSU_VER=1.12
# Wed, 03 May 2023 12:40:23 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 03 May 2023 12:40:23 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 03 May 2023 12:40:27 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 03 May 2023 12:40:27 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 03 May 2023 12:40:29 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 03 May 2023 12:40:30 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 03 May 2023 12:40:30 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 03 May 2023 12:40:30 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 03 May 2023 12:40:30 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Wed, 03 May 2023 12:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 12:40:30 GMT
CMD ["influxd"]
# Wed, 03 May 2023 12:40:30 GMT
EXPOSE 8086
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 03 May 2023 12:40:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0794cf0495a3caa74a71b6504803db62386b162e0862936e7094165af35a7ca2`  
		Last Modified: Wed, 03 May 2023 12:42:34 GMT  
		Size: 6.3 MB (6327884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4f7028e33b7b5de9c755a27c3e9ea1cf7d9913cb6c9b5cfcac31cd9a447a8`  
		Last Modified: Wed, 03 May 2023 12:42:33 GMT  
		Size: 6.4 MB (6434104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf91486cf86efc213e9b76cad5e74d49d01dc78896657c3d004b559198f73be`  
		Last Modified: Wed, 03 May 2023 12:42:31 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91daaa2fee4ceb2f269b802c20828e0ac42083951c9fcc9ed0e3c4dc42153f6`  
		Last Modified: Wed, 03 May 2023 12:42:32 GMT  
		Size: 982.0 KB (982049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fdcd2c51969abd5037cc3d56c63e90bc690dde62815fd99efb0efb695b0e52`  
		Last Modified: Wed, 03 May 2023 12:42:35 GMT  
		Size: 46.3 MB (46334322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46a6f45402719e52e80ca1165e7f375999ec943f1e31d5c15ac0f5cc0ef1569`  
		Last Modified: Wed, 03 May 2023 12:42:32 GMT  
		Size: 23.1 MB (23128344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c1d04df637a1edfea8b7f4a66691694104d136429b8fde52098203255c22a1`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a0962e3a5b231760a56a750fbb7f02fa94037b65c765177e10391997d8edf0`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bcae2cf40e36863a533dc1b6c6b622312e7460093175b16b1622fb656f721c`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:730cf48a80b760051f40f0493255d88b1feee636fb867f0270a859e0d1034024
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109341764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2658e03c9acab92c54f70cafdc1e334fd5b5e9b8ab8669c00f0d6fb971ccf41d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 14:08:58 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 14:08:59 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 03 May 2023 14:09:00 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 03 May 2023 14:09:00 GMT
ENV GOSU_VER=1.12
# Wed, 03 May 2023 14:09:03 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 03 May 2023 14:09:03 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 03 May 2023 14:09:07 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 03 May 2023 14:09:08 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 03 May 2023 14:09:10 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 03 May 2023 14:09:11 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 03 May 2023 14:09:11 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 03 May 2023 14:09:11 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 03 May 2023 14:09:11 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Wed, 03 May 2023 14:09:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 14:09:11 GMT
CMD ["influxd"]
# Wed, 03 May 2023 14:09:11 GMT
EXPOSE 8086
# Wed, 03 May 2023 14:09:11 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 03 May 2023 14:09:11 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 03 May 2023 14:09:11 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 03 May 2023 14:09:11 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e980dde75d021cfed4b514b5ddd40b560b30e874d1f291ec4ab9598ad38d167`  
		Last Modified: Wed, 03 May 2023 14:09:43 GMT  
		Size: 6.3 MB (6308694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfd9ebb6ce6e83f63bc6beddd6136d57d19e4e582ebc978fb253e1aa9c8ca74`  
		Last Modified: Wed, 03 May 2023 14:09:41 GMT  
		Size: 6.0 MB (5953758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fb470a28ffe2ce11824d35ac17f32b9b06686daa52fdd64cdfa72c6546d554`  
		Last Modified: Wed, 03 May 2023 14:09:40 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b6a269269bf191ab56376b65cd467d20c9da4013fdcef13216cdf39e211224`  
		Last Modified: Wed, 03 May 2023 14:09:41 GMT  
		Size: 916.9 KB (916932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8cedefc667f7abbd48444542f176680f9801190f8d1d0a99546e1093d298eb`  
		Last Modified: Wed, 03 May 2023 14:09:42 GMT  
		Size: 44.4 MB (44435818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6b3fb5f737c93b7a8782ac947e6be06aed507cca80cb5fe1f7a0355b0cca28`  
		Last Modified: Wed, 03 May 2023 14:09:40 GMT  
		Size: 21.7 MB (21662571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d02413eed321b52ccc5bbc46933726ae7fa5ef6f41fd3e1055d13d0d495e3dd`  
		Last Modified: Wed, 03 May 2023 14:09:38 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27eb8cdfc21e2b71bad9dbad6d510d6f9e9583780d3a4f964676dc4de157c331`  
		Last Modified: Wed, 03 May 2023 14:09:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cd6ae8950cf597abab315d9234da4d4b29e874707ba7300c0e8469bdf54b1a`  
		Last Modified: Wed, 03 May 2023 14:09:38 GMT  
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
$ docker pull influxdb@sha256:ca98b623d9512ed8ed9274058d4e078109f07fc55f143ff3511a9d41af6692cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:9d884ada1b799a356c9ffcaa53aa2914fd8c5a1cfe5be6f80abbd7e330d6bf10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127518125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1538bfce69e3dc5bb370450b2ce9d78c643f50898c50b5e43e686d706527d5fc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:22 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 04 May 2023 10:55:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:30 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:55:30 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:55:30 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:55:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ad4359c5f3d8340b96395986520fd3a347167a51b7033e3415ca92b76cf7b1`  
		Last Modified: Thu, 04 May 2023 10:56:52 GMT  
		Size: 56.7 MB (56705136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905dcfeb634b16d5b59f824b3d967725f2e95ad71d0ca7edec1101625fe6f005`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d9fad405d2820272db336a50bae1d55e209c05db0b62e569db1bfcc3e7cecc`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000dd25bf5c3dd19ffcb1235ebc0243195891dba177dadda8430f6d6b4a2e330`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
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
$ docker pull influxdb@sha256:c329d32475b1da4205df2e66408ef46689bc77198ecb72f7e87924e7cd109c9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:11b8f3ad1e8a41a028b2de4b9a0466a57df7a25386bfd347d220ccca1a75b4dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114621478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ca18052b424265e2afadad6d256121ef833fc3a7ca8e77a14832a2aa1d8218`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 12:40:19 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:40:20 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 03 May 2023 12:40:20 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 03 May 2023 12:40:21 GMT
ENV GOSU_VER=1.12
# Wed, 03 May 2023 12:40:23 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 03 May 2023 12:40:23 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 03 May 2023 12:40:27 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 03 May 2023 12:40:27 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 03 May 2023 12:40:29 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 03 May 2023 12:40:30 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 03 May 2023 12:40:30 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 03 May 2023 12:40:30 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 03 May 2023 12:40:30 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Wed, 03 May 2023 12:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 12:40:30 GMT
CMD ["influxd"]
# Wed, 03 May 2023 12:40:30 GMT
EXPOSE 8086
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 03 May 2023 12:40:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0794cf0495a3caa74a71b6504803db62386b162e0862936e7094165af35a7ca2`  
		Last Modified: Wed, 03 May 2023 12:42:34 GMT  
		Size: 6.3 MB (6327884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4f7028e33b7b5de9c755a27c3e9ea1cf7d9913cb6c9b5cfcac31cd9a447a8`  
		Last Modified: Wed, 03 May 2023 12:42:33 GMT  
		Size: 6.4 MB (6434104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf91486cf86efc213e9b76cad5e74d49d01dc78896657c3d004b559198f73be`  
		Last Modified: Wed, 03 May 2023 12:42:31 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91daaa2fee4ceb2f269b802c20828e0ac42083951c9fcc9ed0e3c4dc42153f6`  
		Last Modified: Wed, 03 May 2023 12:42:32 GMT  
		Size: 982.0 KB (982049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fdcd2c51969abd5037cc3d56c63e90bc690dde62815fd99efb0efb695b0e52`  
		Last Modified: Wed, 03 May 2023 12:42:35 GMT  
		Size: 46.3 MB (46334322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46a6f45402719e52e80ca1165e7f375999ec943f1e31d5c15ac0f5cc0ef1569`  
		Last Modified: Wed, 03 May 2023 12:42:32 GMT  
		Size: 23.1 MB (23128344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c1d04df637a1edfea8b7f4a66691694104d136429b8fde52098203255c22a1`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a0962e3a5b231760a56a750fbb7f02fa94037b65c765177e10391997d8edf0`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bcae2cf40e36863a533dc1b6c6b622312e7460093175b16b1622fb656f721c`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:730cf48a80b760051f40f0493255d88b1feee636fb867f0270a859e0d1034024
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109341764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2658e03c9acab92c54f70cafdc1e334fd5b5e9b8ab8669c00f0d6fb971ccf41d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 14:08:58 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 14:08:59 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 03 May 2023 14:09:00 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 03 May 2023 14:09:00 GMT
ENV GOSU_VER=1.12
# Wed, 03 May 2023 14:09:03 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 03 May 2023 14:09:03 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 03 May 2023 14:09:07 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 03 May 2023 14:09:08 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 03 May 2023 14:09:10 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 03 May 2023 14:09:11 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 03 May 2023 14:09:11 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 03 May 2023 14:09:11 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 03 May 2023 14:09:11 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Wed, 03 May 2023 14:09:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 14:09:11 GMT
CMD ["influxd"]
# Wed, 03 May 2023 14:09:11 GMT
EXPOSE 8086
# Wed, 03 May 2023 14:09:11 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 03 May 2023 14:09:11 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 03 May 2023 14:09:11 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 03 May 2023 14:09:11 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e980dde75d021cfed4b514b5ddd40b560b30e874d1f291ec4ab9598ad38d167`  
		Last Modified: Wed, 03 May 2023 14:09:43 GMT  
		Size: 6.3 MB (6308694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfd9ebb6ce6e83f63bc6beddd6136d57d19e4e582ebc978fb253e1aa9c8ca74`  
		Last Modified: Wed, 03 May 2023 14:09:41 GMT  
		Size: 6.0 MB (5953758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fb470a28ffe2ce11824d35ac17f32b9b06686daa52fdd64cdfa72c6546d554`  
		Last Modified: Wed, 03 May 2023 14:09:40 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b6a269269bf191ab56376b65cd467d20c9da4013fdcef13216cdf39e211224`  
		Last Modified: Wed, 03 May 2023 14:09:41 GMT  
		Size: 916.9 KB (916932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8cedefc667f7abbd48444542f176680f9801190f8d1d0a99546e1093d298eb`  
		Last Modified: Wed, 03 May 2023 14:09:42 GMT  
		Size: 44.4 MB (44435818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6b3fb5f737c93b7a8782ac947e6be06aed507cca80cb5fe1f7a0355b0cca28`  
		Last Modified: Wed, 03 May 2023 14:09:40 GMT  
		Size: 21.7 MB (21662571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d02413eed321b52ccc5bbc46933726ae7fa5ef6f41fd3e1055d13d0d495e3dd`  
		Last Modified: Wed, 03 May 2023 14:09:38 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27eb8cdfc21e2b71bad9dbad6d510d6f9e9583780d3a4f964676dc4de157c331`  
		Last Modified: Wed, 03 May 2023 14:09:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cd6ae8950cf597abab315d9234da4d4b29e874707ba7300c0e8469bdf54b1a`  
		Last Modified: Wed, 03 May 2023 14:09:38 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:1818dc3a1014ff8bc213b5c5c681328888abec46f3d4474e5135bee3b70d6f36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:f0603d40ad7756af805eab578df632b498915815db7c4a5cbfcb3da0bb3df3ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94224599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fe6dc3badf2bd640104ad7f14bf852f0f9f759cf005ab0204d363bf28060ad5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:22 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 04 May 2023 10:55:37 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:37 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 04 May 2023 10:55:37 GMT
EXPOSE 8091
# Thu, 04 May 2023 10:55:37 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:38 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:38 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0368ac17311eed9aa2f8af4609296812671e408e74467e8a3780f1b6c96647f`  
		Last Modified: Thu, 04 May 2023 10:57:05 GMT  
		Size: 23.4 MB (23412812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957182bf465a16a9c61a29d31942940468a7088fdf3edc6bc6fb48df5c0668e0`  
		Last Modified: Thu, 04 May 2023 10:57:02 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756b9e95001e2a1351853e2c1fe60b068c14e181fd926b78f4d49961880c71ee`  
		Last Modified: Thu, 04 May 2023 10:57:02 GMT  
		Size: 374.0 B  
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
