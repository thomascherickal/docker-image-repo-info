<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `influxdb`

-	[`influxdb:1.10-data`](#influxdb110-data)
-	[`influxdb:1.10-data-alpine`](#influxdb110-data-alpine)
-	[`influxdb:1.10-meta`](#influxdb110-meta)
-	[`influxdb:1.10-meta-alpine`](#influxdb110-meta-alpine)
-	[`influxdb:1.10.4-data`](#influxdb1104-data)
-	[`influxdb:1.10.4-data-alpine`](#influxdb1104-data-alpine)
-	[`influxdb:1.10.4-meta`](#influxdb1104-meta)
-	[`influxdb:1.10.4-meta-alpine`](#influxdb1104-meta-alpine)
-	[`influxdb:1.11-data`](#influxdb111-data)
-	[`influxdb:1.11-data-alpine`](#influxdb111-data-alpine)
-	[`influxdb:1.11-meta`](#influxdb111-meta)
-	[`influxdb:1.11-meta-alpine`](#influxdb111-meta-alpine)
-	[`influxdb:1.11.1-data`](#influxdb1111-data)
-	[`influxdb:1.11.1-data-alpine`](#influxdb1111-data-alpine)
-	[`influxdb:1.11.1-meta`](#influxdb1111-meta)
-	[`influxdb:1.11.1-meta-alpine`](#influxdb1111-meta-alpine)
-	[`influxdb:1.8`](#influxdb18)
-	[`influxdb:1.8-alpine`](#influxdb18-alpine)
-	[`influxdb:1.8.10`](#influxdb1810)
-	[`influxdb:1.8.10-alpine`](#influxdb1810-alpine)
-	[`influxdb:1.9-data`](#influxdb19-data)
-	[`influxdb:1.9-data-alpine`](#influxdb19-data-alpine)
-	[`influxdb:1.9-meta`](#influxdb19-meta)
-	[`influxdb:1.9-meta-alpine`](#influxdb19-meta-alpine)
-	[`influxdb:1.9.12-data`](#influxdb1912-data)
-	[`influxdb:1.9.12-data-alpine`](#influxdb1912-data-alpine)
-	[`influxdb:1.9.12-meta`](#influxdb1912-meta)
-	[`influxdb:1.9.12-meta-alpine`](#influxdb1912-meta-alpine)
-	[`influxdb:2.7`](#influxdb27)
-	[`influxdb:2.7-alpine`](#influxdb27-alpine)
-	[`influxdb:2.7.1`](#influxdb271)
-	[`influxdb:2.7.1-alpine`](#influxdb271-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:latest`](#influxdblatest)

## `influxdb:1.10-data`

```console
$ docker pull influxdb@sha256:d876d875bb00790afc5b80d238477532d9c053d414d453b5f86c71beaa0db5c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:1ed654656b52b7e3db7af38dfe29cea5c88ad421ac4519385e4a798bf7aabbed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110891839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:513ae68c431c904c5d39015ad406a6097124a787879b291903b5e6ec838b314b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:17 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Fri, 28 Jul 2023 03:52:20 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:20 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 28 Jul 2023 03:52:21 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:52:21 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:21 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:21 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 28 Jul 2023 03:52:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:21 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ca65cd3a94fa3e9188b04d5ef647f829d1c12bca5babb7e4ccc06ea95eea0d`  
		Last Modified: Fri, 28 Jul 2023 03:54:32 GMT  
		Size: 40.1 MB (40072097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffba3ed157d3b4c79ef23348350e333a78dcc77fad805ddfc293c7c0ee2f587`  
		Last Modified: Fri, 28 Jul 2023 03:54:26 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0585ff6c90b6dc04b31bdf271c3ac24e8717ec87c3120d2dc48080d13d169604`  
		Last Modified: Fri, 28 Jul 2023 03:54:27 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06d1509aa5e915b6de9a0c9a47271c25f18cdd89e1225cb50f9f7576a9c6db9`  
		Last Modified: Fri, 28 Jul 2023 03:54:27 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-data-alpine`

```console
$ docker pull influxdb@sha256:55b951175bd892dc4e58d2f60cf3168b8f128d69c83fe3776fcc9fcb017fd6be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:17b443b6ddcea807735ab60273b6c3e52d57a95ba809152452055a3e8b810a92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44880968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5f9706688ef79d531421a63ba209a4f24ec350963e193c48fccd268b19a4ead`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 27 Jul 2023 21:01:40 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Thu, 27 Jul 2023 21:01:46 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 27 Jul 2023 21:01:47 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 27 Jul 2023 21:01:47 GMT
EXPOSE 8086
# Thu, 27 Jul 2023 21:01:47 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 Jul 2023 21:01:47 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 27 Jul 2023 21:01:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 27 Jul 2023 21:01:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jul 2023 21:01:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01890aee6f6dca82a4ab58dbc86389879f1ae7bf4cd5a19a291911c6f885ef13`  
		Last Modified: Thu, 27 Jul 2023 21:03:58 GMT  
		Size: 40.0 MB (40031779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503d784a4b36e16b9d2c1475b2df9d2e4c94bf7f0f6144a39eb63b0023e232e1`  
		Last Modified: Thu, 27 Jul 2023 21:03:52 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691989debe8d1afb6e1fe0cbbd6961a005b93b46e6c8827f23a26ab3d3ec41bb`  
		Last Modified: Thu, 27 Jul 2023 21:03:52 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a3ead3a50c54b100f3e748ee34d64841541a28626738a01f556774156a1490`  
		Last Modified: Thu, 27 Jul 2023 21:03:52 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta`

```console
$ docker pull influxdb@sha256:92309d1706807b2f346c9a60a911b053870e44157865fc372e65b36d821e2ded
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:5c640a35dbd7aa46541a60cf48c7864f780708a18a737f43af2eb49d494757e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91056807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29c537671bb32d8358e99382e5f9ea4c740f71c5563a0de33de1488a46b8716`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:17 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Fri, 28 Jul 2023 03:52:28 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:28 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 28 Jul 2023 03:52:28 GMT
EXPOSE 8091
# Fri, 28 Jul 2023 03:52:28 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:29 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:29 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1828237fedd665b4af9b5595e0adf188d4b43613dc6881f9e7744cce2ae337`  
		Last Modified: Fri, 28 Jul 2023 03:54:46 GMT  
		Size: 20.2 MB (20238270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e9b8a1dfc88dd26ba9b365f358856d48395de7229fd596238c1651ff983d58`  
		Last Modified: Fri, 28 Jul 2023 03:54:43 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291787ebfec6593353457e8edbdd6ebcd14db463b4333ccb8385cd6d4bf55618`  
		Last Modified: Fri, 28 Jul 2023 03:54:43 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta-alpine`

```console
$ docker pull influxdb@sha256:466c82aa3f393c9677f5e3afd04ebe12d8e86824b801ee9fb9a34fa41cbcbd68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:078cf6ddc8ea1d2a51bd32736b3a708fd2b7b199fab8b6344af8cda36a5941c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25054484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c225f742ad37870830972503e9cd6bf37d165cd7f8f3f694c8caa3b8ce249d01`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 27 Jul 2023 21:01:40 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Thu, 27 Jul 2023 21:02:01 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 27 Jul 2023 21:02:02 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 27 Jul 2023 21:02:02 GMT
EXPOSE 8091
# Thu, 27 Jul 2023 21:02:02 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 Jul 2023 21:02:02 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 27 Jul 2023 21:02:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jul 2023 21:02:02 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3cef12b3e50dbf8cc97e0c7cae53c9ec9ad2cfe11f9f8f004b583133d8288f`  
		Last Modified: Thu, 27 Jul 2023 21:04:22 GMT  
		Size: 20.2 MB (20206499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcbda364ee258174cc9ee35d77a5a01dfcc3e736dde24459657e253b455589e`  
		Last Modified: Thu, 27 Jul 2023 21:04:19 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4debecc86bf39f0fe9e4b4d85b14cc7ac07e45a2f7bbffa312aa05edb28e4`  
		Last Modified: Thu, 27 Jul 2023 21:04:19 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.4-data`

```console
$ docker pull influxdb@sha256:d876d875bb00790afc5b80d238477532d9c053d414d453b5f86c71beaa0db5c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.4-data` - linux; amd64

```console
$ docker pull influxdb@sha256:1ed654656b52b7e3db7af38dfe29cea5c88ad421ac4519385e4a798bf7aabbed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110891839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:513ae68c431c904c5d39015ad406a6097124a787879b291903b5e6ec838b314b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:17 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Fri, 28 Jul 2023 03:52:20 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:20 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 28 Jul 2023 03:52:21 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:52:21 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:21 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:21 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 28 Jul 2023 03:52:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:21 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ca65cd3a94fa3e9188b04d5ef647f829d1c12bca5babb7e4ccc06ea95eea0d`  
		Last Modified: Fri, 28 Jul 2023 03:54:32 GMT  
		Size: 40.1 MB (40072097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffba3ed157d3b4c79ef23348350e333a78dcc77fad805ddfc293c7c0ee2f587`  
		Last Modified: Fri, 28 Jul 2023 03:54:26 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0585ff6c90b6dc04b31bdf271c3ac24e8717ec87c3120d2dc48080d13d169604`  
		Last Modified: Fri, 28 Jul 2023 03:54:27 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06d1509aa5e915b6de9a0c9a47271c25f18cdd89e1225cb50f9f7576a9c6db9`  
		Last Modified: Fri, 28 Jul 2023 03:54:27 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.4-data-alpine`

```console
$ docker pull influxdb@sha256:55b951175bd892dc4e58d2f60cf3168b8f128d69c83fe3776fcc9fcb017fd6be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.4-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:17b443b6ddcea807735ab60273b6c3e52d57a95ba809152452055a3e8b810a92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44880968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5f9706688ef79d531421a63ba209a4f24ec350963e193c48fccd268b19a4ead`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 27 Jul 2023 21:01:40 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Thu, 27 Jul 2023 21:01:46 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 27 Jul 2023 21:01:47 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 27 Jul 2023 21:01:47 GMT
EXPOSE 8086
# Thu, 27 Jul 2023 21:01:47 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 Jul 2023 21:01:47 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 27 Jul 2023 21:01:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 27 Jul 2023 21:01:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jul 2023 21:01:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01890aee6f6dca82a4ab58dbc86389879f1ae7bf4cd5a19a291911c6f885ef13`  
		Last Modified: Thu, 27 Jul 2023 21:03:58 GMT  
		Size: 40.0 MB (40031779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503d784a4b36e16b9d2c1475b2df9d2e4c94bf7f0f6144a39eb63b0023e232e1`  
		Last Modified: Thu, 27 Jul 2023 21:03:52 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691989debe8d1afb6e1fe0cbbd6961a005b93b46e6c8827f23a26ab3d3ec41bb`  
		Last Modified: Thu, 27 Jul 2023 21:03:52 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a3ead3a50c54b100f3e748ee34d64841541a28626738a01f556774156a1490`  
		Last Modified: Thu, 27 Jul 2023 21:03:52 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.4-meta`

```console
$ docker pull influxdb@sha256:92309d1706807b2f346c9a60a911b053870e44157865fc372e65b36d821e2ded
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.4-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:5c640a35dbd7aa46541a60cf48c7864f780708a18a737f43af2eb49d494757e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91056807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29c537671bb32d8358e99382e5f9ea4c740f71c5563a0de33de1488a46b8716`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:17 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Fri, 28 Jul 2023 03:52:28 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:28 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 28 Jul 2023 03:52:28 GMT
EXPOSE 8091
# Fri, 28 Jul 2023 03:52:28 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:29 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:29 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1828237fedd665b4af9b5595e0adf188d4b43613dc6881f9e7744cce2ae337`  
		Last Modified: Fri, 28 Jul 2023 03:54:46 GMT  
		Size: 20.2 MB (20238270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e9b8a1dfc88dd26ba9b365f358856d48395de7229fd596238c1651ff983d58`  
		Last Modified: Fri, 28 Jul 2023 03:54:43 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291787ebfec6593353457e8edbdd6ebcd14db463b4333ccb8385cd6d4bf55618`  
		Last Modified: Fri, 28 Jul 2023 03:54:43 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.4-meta-alpine`

```console
$ docker pull influxdb@sha256:466c82aa3f393c9677f5e3afd04ebe12d8e86824b801ee9fb9a34fa41cbcbd68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.4-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:078cf6ddc8ea1d2a51bd32736b3a708fd2b7b199fab8b6344af8cda36a5941c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25054484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c225f742ad37870830972503e9cd6bf37d165cd7f8f3f694c8caa3b8ce249d01`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 27 Jul 2023 21:01:40 GMT
ENV INFLUXDB_VERSION=1.10.4-c1.10.4
# Thu, 27 Jul 2023 21:02:01 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 27 Jul 2023 21:02:02 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 27 Jul 2023 21:02:02 GMT
EXPOSE 8091
# Thu, 27 Jul 2023 21:02:02 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 Jul 2023 21:02:02 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 27 Jul 2023 21:02:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jul 2023 21:02:02 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3cef12b3e50dbf8cc97e0c7cae53c9ec9ad2cfe11f9f8f004b583133d8288f`  
		Last Modified: Thu, 27 Jul 2023 21:04:22 GMT  
		Size: 20.2 MB (20206499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcbda364ee258174cc9ee35d77a5a01dfcc3e736dde24459657e253b455589e`  
		Last Modified: Thu, 27 Jul 2023 21:04:19 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4debecc86bf39f0fe9e4b4d85b14cc7ac07e45a2f7bbffa312aa05edb28e4`  
		Last Modified: Thu, 27 Jul 2023 21:04:19 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-data`

```console
$ docker pull influxdb@sha256:6f3f4643335b8f7c13981cf284fcdd5d2d3ab3c47b2f9ef3d8e5134222f2ab39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:b5f741fe90b91e2ad0eb1fc9b2449d1d2046fd5b3601a629d204b9a91674fdbd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110977821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf191547950316b0e157e1014e7a3ddb2bd865fd78b8f8f0d9cafc46c04cd242`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:34 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Fri, 28 Jul 2023 03:52:39 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:39 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 28 Jul 2023 03:52:39 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:52:39 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:39 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 28 Jul 2023 03:52:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:39 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0269a316fa0ffaa7c2560ed4167fb9b3d02c061cb38142a688452d19c6432c7f`  
		Last Modified: Fri, 28 Jul 2023 03:55:01 GMT  
		Size: 40.2 MB (40158080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87256231b67dcf9e0ff47a951134f66072897454d8e3a784f1b8f45dd9dfc167`  
		Last Modified: Fri, 28 Jul 2023 03:54:55 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6854ea14a23716df63291e919f41765dc65f6f84f1537fe00aadd6610566851d`  
		Last Modified: Fri, 28 Jul 2023 03:54:55 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a8c60ef7e6d333bbd271003abce09891821abca1bc9c7f3ec8b6cdddca1f13`  
		Last Modified: Fri, 28 Jul 2023 03:54:55 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-data-alpine`

```console
$ docker pull influxdb@sha256:a93dfd57ff7fdd56e03e5250256c08d3dcc6c48dd1e3e7ca387ea0c1bb84344d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:e710348181c4b53c4fd307d3e4d901d2dbed8bd6a145aac41ed587543b99fb8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44963986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b4314ae3c76629ce8c10da35768ff45a22e1a2cf4244b6f316f63a883a3ed3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 20 Jul 2023 00:20:15 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Thu, 20 Jul 2023 00:20:22 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 20 Jul 2023 00:20:22 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 20 Jul 2023 00:20:22 GMT
EXPOSE 8086
# Thu, 20 Jul 2023 00:20:22 GMT
VOLUME [/var/lib/influxdb]
# Thu, 20 Jul 2023 00:20:22 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 20 Jul 2023 00:20:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 20 Jul 2023 00:20:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Jul 2023 00:20:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b29410c5bc89257806e1c39bbf3f2d5a3279d85622495a0905a92c99e350b27`  
		Last Modified: Thu, 20 Jul 2023 00:21:44 GMT  
		Size: 40.1 MB (40114797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e51023e2cf1ed7bf9f1d0f56b42b63b2544cafc4d0ee29ea3f8b566a52ec7b`  
		Last Modified: Thu, 20 Jul 2023 00:21:38 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f281932b19f3a5b165b20e64ffb8a6b695db78221b6309ba0bfcb30f9b8f8746`  
		Last Modified: Thu, 20 Jul 2023 00:21:38 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388e9a783448507a31c6aede84b3e6a895f3804479278cc7a2d7cebd155726b8`  
		Last Modified: Thu, 20 Jul 2023 00:21:38 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-meta`

```console
$ docker pull influxdb@sha256:dffb12729bf4183a6ebce0d1158257bf431ad99cdf194be6ace231749c487b87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:a0e35fc3c52d1388cb5e233507cd74ec12072af361919ee2f6546ec1acbe7662
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91067591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6e27c667d4ab3b814aa3e8ef3674a91df396c3121834a354657b350d8c9367`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:34 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Fri, 28 Jul 2023 03:52:48 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:48 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 28 Jul 2023 03:52:48 GMT
EXPOSE 8091
# Fri, 28 Jul 2023 03:52:49 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:49 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:49 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acfcbba43f329427e2ef2f514be96908ebb7c7b2e22a4986f32cfaf826d396b`  
		Last Modified: Fri, 28 Jul 2023 03:55:13 GMT  
		Size: 20.2 MB (20249057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8abc82b9a203802f359210a2c4786d500c590aa2d3b8827931691fad98bc057`  
		Last Modified: Fri, 28 Jul 2023 03:55:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d710e9a6fc4c687e071618a51beab780108d3c7c5dcb691d0e8f92234779d6`  
		Last Modified: Fri, 28 Jul 2023 03:55:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-meta-alpine`

```console
$ docker pull influxdb@sha256:9a26d49d2b0e4b0134842f471813cd6745b578a61f7ad480bf57c3f2d0588dab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9417d71ff8f5d8ba8cf78489b7ebc7d59fa1433008a25c93dc9491723a66cbd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25060326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48cfa2958fd500359c86e523c818c684c702282e1ed449b875f17614de4f6531`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 20 Jul 2023 00:20:15 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Thu, 20 Jul 2023 00:20:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 20 Jul 2023 00:20:37 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 20 Jul 2023 00:20:37 GMT
EXPOSE 8091
# Thu, 20 Jul 2023 00:20:37 GMT
VOLUME [/var/lib/influxdb]
# Thu, 20 Jul 2023 00:20:37 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 20 Jul 2023 00:20:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Jul 2023 00:20:37 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36bf6dd7f3f9430fabac56f6f7031fb9077c9e996b1f5572013b386b6ccaa56`  
		Last Modified: Thu, 20 Jul 2023 00:22:09 GMT  
		Size: 20.2 MB (20212340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d883d97c255e0ccc6d631959859bf0b884590bc08aedb55340fadb5b904c75c8`  
		Last Modified: Thu, 20 Jul 2023 00:22:06 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e717e0af6b153ce3aaa85bafd5c0c6ab43d0a0e6e64286e9b04faed43d37e371`  
		Last Modified: Thu, 20 Jul 2023 00:22:06 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.1-data`

```console
$ docker pull influxdb@sha256:6f3f4643335b8f7c13981cf284fcdd5d2d3ab3c47b2f9ef3d8e5134222f2ab39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.1-data` - linux; amd64

```console
$ docker pull influxdb@sha256:b5f741fe90b91e2ad0eb1fc9b2449d1d2046fd5b3601a629d204b9a91674fdbd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110977821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf191547950316b0e157e1014e7a3ddb2bd865fd78b8f8f0d9cafc46c04cd242`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:34 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Fri, 28 Jul 2023 03:52:39 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:39 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 28 Jul 2023 03:52:39 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:52:39 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:39 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 28 Jul 2023 03:52:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:39 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0269a316fa0ffaa7c2560ed4167fb9b3d02c061cb38142a688452d19c6432c7f`  
		Last Modified: Fri, 28 Jul 2023 03:55:01 GMT  
		Size: 40.2 MB (40158080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87256231b67dcf9e0ff47a951134f66072897454d8e3a784f1b8f45dd9dfc167`  
		Last Modified: Fri, 28 Jul 2023 03:54:55 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6854ea14a23716df63291e919f41765dc65f6f84f1537fe00aadd6610566851d`  
		Last Modified: Fri, 28 Jul 2023 03:54:55 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a8c60ef7e6d333bbd271003abce09891821abca1bc9c7f3ec8b6cdddca1f13`  
		Last Modified: Fri, 28 Jul 2023 03:54:55 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.1-data-alpine`

```console
$ docker pull influxdb@sha256:a93dfd57ff7fdd56e03e5250256c08d3dcc6c48dd1e3e7ca387ea0c1bb84344d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.1-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:e710348181c4b53c4fd307d3e4d901d2dbed8bd6a145aac41ed587543b99fb8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44963986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b4314ae3c76629ce8c10da35768ff45a22e1a2cf4244b6f316f63a883a3ed3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 20 Jul 2023 00:20:15 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Thu, 20 Jul 2023 00:20:22 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 20 Jul 2023 00:20:22 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 20 Jul 2023 00:20:22 GMT
EXPOSE 8086
# Thu, 20 Jul 2023 00:20:22 GMT
VOLUME [/var/lib/influxdb]
# Thu, 20 Jul 2023 00:20:22 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 20 Jul 2023 00:20:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 20 Jul 2023 00:20:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Jul 2023 00:20:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b29410c5bc89257806e1c39bbf3f2d5a3279d85622495a0905a92c99e350b27`  
		Last Modified: Thu, 20 Jul 2023 00:21:44 GMT  
		Size: 40.1 MB (40114797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e51023e2cf1ed7bf9f1d0f56b42b63b2544cafc4d0ee29ea3f8b566a52ec7b`  
		Last Modified: Thu, 20 Jul 2023 00:21:38 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f281932b19f3a5b165b20e64ffb8a6b695db78221b6309ba0bfcb30f9b8f8746`  
		Last Modified: Thu, 20 Jul 2023 00:21:38 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388e9a783448507a31c6aede84b3e6a895f3804479278cc7a2d7cebd155726b8`  
		Last Modified: Thu, 20 Jul 2023 00:21:38 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.1-meta`

```console
$ docker pull influxdb@sha256:dffb12729bf4183a6ebce0d1158257bf431ad99cdf194be6ace231749c487b87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.1-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:a0e35fc3c52d1388cb5e233507cd74ec12072af361919ee2f6546ec1acbe7662
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91067591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6e27c667d4ab3b814aa3e8ef3674a91df396c3121834a354657b350d8c9367`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:34 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Fri, 28 Jul 2023 03:52:48 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:48 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 28 Jul 2023 03:52:48 GMT
EXPOSE 8091
# Fri, 28 Jul 2023 03:52:49 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:49 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:49 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acfcbba43f329427e2ef2f514be96908ebb7c7b2e22a4986f32cfaf826d396b`  
		Last Modified: Fri, 28 Jul 2023 03:55:13 GMT  
		Size: 20.2 MB (20249057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8abc82b9a203802f359210a2c4786d500c590aa2d3b8827931691fad98bc057`  
		Last Modified: Fri, 28 Jul 2023 03:55:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d710e9a6fc4c687e071618a51beab780108d3c7c5dcb691d0e8f92234779d6`  
		Last Modified: Fri, 28 Jul 2023 03:55:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.1-meta-alpine`

```console
$ docker pull influxdb@sha256:9a26d49d2b0e4b0134842f471813cd6745b578a61f7ad480bf57c3f2d0588dab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.1-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9417d71ff8f5d8ba8cf78489b7ebc7d59fa1433008a25c93dc9491723a66cbd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25060326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48cfa2958fd500359c86e523c818c684c702282e1ed449b875f17614de4f6531`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 20 Jul 2023 00:20:15 GMT
ENV INFLUXDB_VERSION=1.11.1-c1.11.1
# Thu, 20 Jul 2023 00:20:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/fs/usr/bin/* &&     cp -a /usr/src/influxdb-*/fs/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 20 Jul 2023 00:20:37 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 20 Jul 2023 00:20:37 GMT
EXPOSE 8091
# Thu, 20 Jul 2023 00:20:37 GMT
VOLUME [/var/lib/influxdb]
# Thu, 20 Jul 2023 00:20:37 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 20 Jul 2023 00:20:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Jul 2023 00:20:37 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36bf6dd7f3f9430fabac56f6f7031fb9077c9e996b1f5572013b386b6ccaa56`  
		Last Modified: Thu, 20 Jul 2023 00:22:09 GMT  
		Size: 20.2 MB (20212340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d883d97c255e0ccc6d631959859bf0b884590bc08aedb55340fadb5b904c75c8`  
		Last Modified: Thu, 20 Jul 2023 00:22:06 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e717e0af6b153ce3aaa85bafd5c0c6ab43d0a0e6e64286e9b04faed43d37e371`  
		Last Modified: Thu, 20 Jul 2023 00:22:06 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:eb54772d8020976789edfa6166f8f06b8d5c5a3f88fd363875fc89f1077eae6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:7acc3c96105d766242f5b9d8543b05f9a10f5deafb96690d9ee0561169ebf8b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125705441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51e1f216e151f658595d2f0cc75e9304f65e59c352b13a70863a0fdc371bcf53`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:51:51 GMT
ENV INFLUXDB_VERSION=1.8.10
# Fri, 28 Jul 2023 03:51:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 28 Jul 2023 03:51:55 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 28 Jul 2023 03:51:55 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:51:55 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:51:55 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:51:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 28 Jul 2023 03:51:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:51:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1a298636eb3bde590374108f7966d193f8a0b9be95a00ea221e4b94a30ec80`  
		Last Modified: Fri, 28 Jul 2023 03:53:52 GMT  
		Size: 54.9 MB (54885762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb4d0c0df2de6db2fd8079de2233fe87f41de95f4abe4be80c7d7a7875fc055`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d443149d146d270e0ee71ae117dc2a9505b637f92f08abfa84beb831696b379`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e80ab76a9dfd2ecad22e645fafd762b64c3c20c84e3d5c6716649c2d6ec6d5`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:0a036eba7fe9f72e98fda4aa3df627410694d97530d4756bf58231d7de24c320
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116703577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13406140c51f4b378e53d35df886482e6770377f7b74653583ec76e4e67bfa84`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 00:14:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Jul 2023 00:14:51 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 05 Jul 2023 00:14:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 05 Jul 2023 00:14:57 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 05 Jul 2023 00:14:57 GMT
EXPOSE 8086
# Wed, 05 Jul 2023 00:14:57 GMT
VOLUME [/var/lib/influxdb]
# Wed, 05 Jul 2023 00:14:57 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 05 Jul 2023 00:14:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 05 Jul 2023 00:14:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jul 2023 00:14:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3298e3eb46a8e282087fc6fd8ab99b552e49c6bc255f2bc10cace34828cc20`  
		Last Modified: Wed, 05 Jul 2023 00:15:05 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb287d00d1eb9b1096105af577c39f10b097ff7bcfa0db7c7f8784aef0b4c0f6`  
		Last Modified: Wed, 05 Jul 2023 00:15:12 GMT  
		Size: 51.6 MB (51613160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4d4a98b8f099e9122c82f95f33fcc6790175fb9a20a2c23259fd0705d4837f`  
		Last Modified: Wed, 05 Jul 2023 00:15:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ac60331b74fadc693b9012521173724e2115b40b2b917f20a934758943883f`  
		Last Modified: Wed, 05 Jul 2023 00:15:06 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da368b3d6bc6758e1f53bb3a4075712a17229ac94626706894e852d0458704ab`  
		Last Modified: Wed, 05 Jul 2023 00:15:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:792cc15c03f97d8988941153b4c8754d48f2215c81edf1db6eaa682287e48287
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120684888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39d770b970d5474ba030f82e29c2f37b6959eda613d2b3a19f82d875df7de086`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:38:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:38:47 GMT
ENV INFLUXDB_VERSION=1.8.10
# Fri, 28 Jul 2023 03:38:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 28 Jul 2023 03:38:51 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 28 Jul 2023 03:38:51 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:38:51 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:38:52 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:38:52 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 28 Jul 2023 03:38:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:38:52 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129433af71820f1d641a8a2330c4e8bbdf7aaaf73add50b89fad6cebabc6790f`  
		Last Modified: Fri, 28 Jul 2023 03:39:25 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e5a9d6ec6c4100c596800959e0a05c911bba36126734b63ce3636c2a26a8f0`  
		Last Modified: Fri, 28 Jul 2023 03:39:30 GMT  
		Size: 51.2 MB (51230046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185dbb3914eff73a0e2cbaf66fc459b725d2f6d7c628082e9a3c238fb3bf9e01`  
		Last Modified: Fri, 28 Jul 2023 03:39:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ea9f78ca8b214b27bc1bbb5b078ab0bb1c01265ebee1eb86559d76fa68fd0b`  
		Last Modified: Fri, 28 Jul 2023 03:39:25 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f3f245d7a01e0d71b637a9d7dc6599dcdb052a3e8553e86e5ea4e4ca22d9db`  
		Last Modified: Fri, 28 Jul 2023 03:39:25 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:4a893daadfa691938bcc95638ce23f177c42dbe9915570ba5f675e8346d5ab3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:74ec25adca471e51feb1c40672107bd70abea8544f1595aa68b8201352e6bf5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59495786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3cbcc60a3dfc6dec30fbe4403c09686f4224a32c3ac7faa0c54862c89955a4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 00:09:37 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 15 Jun 2023 00:09:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 00:09:43 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 15 Jun 2023 00:09:43 GMT
EXPOSE 8086
# Thu, 15 Jun 2023 00:09:43 GMT
VOLUME [/var/lib/influxdb]
# Thu, 15 Jun 2023 00:09:44 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 15 Jun 2023 00:09:44 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 15 Jun 2023 00:09:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 00:09:44 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1050660ed794c344720bf8f1026dda21e49ef75f13699c2d552063b989bd95f`  
		Last Modified: Thu, 15 Jun 2023 00:11:52 GMT  
		Size: 54.6 MB (54646654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9229e296cf31a69598b08fb8d59c82d4d67f32ef9a4c1d4c91c14dcdd6182372`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05be0276d3c4e073717df68ae85d811276a911271f0f6a52036074834bc9492`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f755f139a4a19bd5c1d2744f7007dc5563853aafb641c76a32221bb3f3977584`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10`

```console
$ docker pull influxdb@sha256:eb54772d8020976789edfa6166f8f06b8d5c5a3f88fd363875fc89f1077eae6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:7acc3c96105d766242f5b9d8543b05f9a10f5deafb96690d9ee0561169ebf8b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125705441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51e1f216e151f658595d2f0cc75e9304f65e59c352b13a70863a0fdc371bcf53`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:51:51 GMT
ENV INFLUXDB_VERSION=1.8.10
# Fri, 28 Jul 2023 03:51:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 28 Jul 2023 03:51:55 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 28 Jul 2023 03:51:55 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:51:55 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:51:55 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:51:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 28 Jul 2023 03:51:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:51:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1a298636eb3bde590374108f7966d193f8a0b9be95a00ea221e4b94a30ec80`  
		Last Modified: Fri, 28 Jul 2023 03:53:52 GMT  
		Size: 54.9 MB (54885762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb4d0c0df2de6db2fd8079de2233fe87f41de95f4abe4be80c7d7a7875fc055`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d443149d146d270e0ee71ae117dc2a9505b637f92f08abfa84beb831696b379`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e80ab76a9dfd2ecad22e645fafd762b64c3c20c84e3d5c6716649c2d6ec6d5`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:0a036eba7fe9f72e98fda4aa3df627410694d97530d4756bf58231d7de24c320
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116703577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13406140c51f4b378e53d35df886482e6770377f7b74653583ec76e4e67bfa84`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 00:14:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Jul 2023 00:14:51 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 05 Jul 2023 00:14:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 05 Jul 2023 00:14:57 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 05 Jul 2023 00:14:57 GMT
EXPOSE 8086
# Wed, 05 Jul 2023 00:14:57 GMT
VOLUME [/var/lib/influxdb]
# Wed, 05 Jul 2023 00:14:57 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 05 Jul 2023 00:14:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 05 Jul 2023 00:14:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jul 2023 00:14:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3298e3eb46a8e282087fc6fd8ab99b552e49c6bc255f2bc10cace34828cc20`  
		Last Modified: Wed, 05 Jul 2023 00:15:05 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb287d00d1eb9b1096105af577c39f10b097ff7bcfa0db7c7f8784aef0b4c0f6`  
		Last Modified: Wed, 05 Jul 2023 00:15:12 GMT  
		Size: 51.6 MB (51613160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4d4a98b8f099e9122c82f95f33fcc6790175fb9a20a2c23259fd0705d4837f`  
		Last Modified: Wed, 05 Jul 2023 00:15:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ac60331b74fadc693b9012521173724e2115b40b2b917f20a934758943883f`  
		Last Modified: Wed, 05 Jul 2023 00:15:06 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da368b3d6bc6758e1f53bb3a4075712a17229ac94626706894e852d0458704ab`  
		Last Modified: Wed, 05 Jul 2023 00:15:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:792cc15c03f97d8988941153b4c8754d48f2215c81edf1db6eaa682287e48287
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120684888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39d770b970d5474ba030f82e29c2f37b6959eda613d2b3a19f82d875df7de086`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:38:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:38:47 GMT
ENV INFLUXDB_VERSION=1.8.10
# Fri, 28 Jul 2023 03:38:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 28 Jul 2023 03:38:51 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 28 Jul 2023 03:38:51 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:38:51 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:38:52 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:38:52 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 28 Jul 2023 03:38:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:38:52 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129433af71820f1d641a8a2330c4e8bbdf7aaaf73add50b89fad6cebabc6790f`  
		Last Modified: Fri, 28 Jul 2023 03:39:25 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e5a9d6ec6c4100c596800959e0a05c911bba36126734b63ce3636c2a26a8f0`  
		Last Modified: Fri, 28 Jul 2023 03:39:30 GMT  
		Size: 51.2 MB (51230046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185dbb3914eff73a0e2cbaf66fc459b725d2f6d7c628082e9a3c238fb3bf9e01`  
		Last Modified: Fri, 28 Jul 2023 03:39:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ea9f78ca8b214b27bc1bbb5b078ab0bb1c01265ebee1eb86559d76fa68fd0b`  
		Last Modified: Fri, 28 Jul 2023 03:39:25 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f3f245d7a01e0d71b637a9d7dc6599dcdb052a3e8553e86e5ea4e4ca22d9db`  
		Last Modified: Fri, 28 Jul 2023 03:39:25 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-alpine`

```console
$ docker pull influxdb@sha256:4a893daadfa691938bcc95638ce23f177c42dbe9915570ba5f675e8346d5ab3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:74ec25adca471e51feb1c40672107bd70abea8544f1595aa68b8201352e6bf5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59495786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3cbcc60a3dfc6dec30fbe4403c09686f4224a32c3ac7faa0c54862c89955a4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 00:09:37 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 15 Jun 2023 00:09:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 00:09:43 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 15 Jun 2023 00:09:43 GMT
EXPOSE 8086
# Thu, 15 Jun 2023 00:09:43 GMT
VOLUME [/var/lib/influxdb]
# Thu, 15 Jun 2023 00:09:44 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 15 Jun 2023 00:09:44 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 15 Jun 2023 00:09:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 00:09:44 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1050660ed794c344720bf8f1026dda21e49ef75f13699c2d552063b989bd95f`  
		Last Modified: Thu, 15 Jun 2023 00:11:52 GMT  
		Size: 54.6 MB (54646654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9229e296cf31a69598b08fb8d59c82d4d67f32ef9a4c1d4c91c14dcdd6182372`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05be0276d3c4e073717df68ae85d811276a911271f0f6a52036074834bc9492`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f755f139a4a19bd5c1d2744f7007dc5563853aafb641c76a32221bb3f3977584`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data`

```console
$ docker pull influxdb@sha256:bf4f2e8affa4859376422af85dacfef65a856d2355c31a1202f7665191e749fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:b59a8ebe489ac985be3a1857c3467971cf59f48ab75fe68ee8f4bfa650ade443
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.0 MB (103995589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5976a08a8ea2c826140377f2c46a8899caac138d4ed9b96c661cc07e52c2d2c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:01 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Fri, 28 Jul 2023 03:52:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:04 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 28 Jul 2023 03:52:04 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:52:04 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:04 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:04 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 28 Jul 2023 03:52:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:05 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9336d602b0f0150e8ec2627d182005ef2b789be5e3dea018c1e554b1b401c9e8`  
		Last Modified: Fri, 28 Jul 2023 03:54:06 GMT  
		Size: 33.2 MB (33175851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8110f41f8fe5003410f3949061a75efbd9d3a195591cf86196d690ae1b2db236`  
		Last Modified: Fri, 28 Jul 2023 03:54:01 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b336a24c331465c424e3f47322fcaa6596bd7057d60b4222fad2d75f97121b73`  
		Last Modified: Fri, 28 Jul 2023 03:54:01 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0ee18130a4f35b17fce8cd7449fbaf638ff556fb0959bd4282b8da3ffccdb`  
		Last Modified: Fri, 28 Jul 2023 03:54:01 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:9809f77f91e46dec77016f5a4ad488f7a0971106774f2e53c084edc276e0e235
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:647568e501deb302e7f6ae4cec8b5e5eb64d5888253b5fdd8fa75ebe323f316c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37983879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af18ee8bbc00ce46d09b7cccc5f3345662736797411904717b1fb9e537167cc8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 27 Jul 2023 21:01:06 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Thu, 27 Jul 2023 21:01:13 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 27 Jul 2023 21:01:13 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 27 Jul 2023 21:01:14 GMT
EXPOSE 8086
# Thu, 27 Jul 2023 21:01:14 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 Jul 2023 21:01:14 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 27 Jul 2023 21:01:14 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 27 Jul 2023 21:01:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jul 2023 21:01:14 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae37b9f08a90cea295c2b38668cb1ffb2f383d1fd699c9f54adf0cbbe81d4b5`  
		Last Modified: Thu, 27 Jul 2023 21:03:08 GMT  
		Size: 33.1 MB (33134690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e547dee21cb8a6d8f746077c6cf6c5d9e38995695fb4e4ffcb3bf2eda8156e`  
		Last Modified: Thu, 27 Jul 2023 21:03:03 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76585895adac24ab7752e59e409862dc74cf0818146c58b07d0de098675a3a5e`  
		Last Modified: Thu, 27 Jul 2023 21:03:03 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ad9d272774164de2a304dffbfcbc1f3ab38ef20453e1dde4c98156d3671836`  
		Last Modified: Thu, 27 Jul 2023 21:03:03 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:e5b72a5ba963fe9cbecb43fcea59a205741f45628c35e650b2999836d1169329
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:20aa1f46ac8d69e8539770bf1aeefef5a8c405fdd23fd4593c6adac15ae6ed53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83436022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66cc97881713bce3ed3a5557e5e4cbfb20aeda833fc2c79a87845df9da442d35`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:01 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Fri, 28 Jul 2023 03:52:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:12 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 28 Jul 2023 03:52:12 GMT
EXPOSE 8091
# Fri, 28 Jul 2023 03:52:12 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:12 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:12 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0116e4b544bb0c33a16150de6512d0200c98e5957863904454b0c463bb219e29`  
		Last Modified: Fri, 28 Jul 2023 03:54:18 GMT  
		Size: 12.6 MB (12617490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba19f65130b8d7428afdd3933fbbe2af77dbb9a7432d512e7b4ff09d5dc7994`  
		Last Modified: Fri, 28 Jul 2023 03:54:16 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cedf9689810235d6b99df594fda2843e4a4518e0df40ef62fe98d9fc48c38d0`  
		Last Modified: Fri, 28 Jul 2023 03:54:16 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:41ab5924616f2de5e84f517a26761b58c2e711aa8f6bbd9504e60bc239993a96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:e3b2c203b40931574622cc9d82296d2a66439a3dc008c731627a632c1e0433c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17429693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c13ed2509e03203f9846af87130aefb88534af15b7b66a58c5dce9c8d6027b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 27 Jul 2023 21:01:06 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Thu, 27 Jul 2023 21:01:28 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 27 Jul 2023 21:01:28 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 27 Jul 2023 21:01:28 GMT
EXPOSE 8091
# Thu, 27 Jul 2023 21:01:28 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 Jul 2023 21:01:28 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 27 Jul 2023 21:01:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jul 2023 21:01:28 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7588ec7447c93ddc97ad3aa52e4c8091a32172390b9d95373af9d3bacb8bf280`  
		Last Modified: Thu, 27 Jul 2023 21:03:28 GMT  
		Size: 12.6 MB (12581708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f103f73d248b9c924f4d2bbbb4173a0e8d587d0d9979692731b90257e3a949bf`  
		Last Modified: Thu, 27 Jul 2023 21:03:27 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22d6e5265f66dd6b1aed49ef3ecbce0fb88fb30d577b1e061485adc88043a22`  
		Last Modified: Thu, 27 Jul 2023 21:03:27 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.12-data`

```console
$ docker pull influxdb@sha256:bf4f2e8affa4859376422af85dacfef65a856d2355c31a1202f7665191e749fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.12-data` - linux; amd64

```console
$ docker pull influxdb@sha256:b59a8ebe489ac985be3a1857c3467971cf59f48ab75fe68ee8f4bfa650ade443
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.0 MB (103995589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5976a08a8ea2c826140377f2c46a8899caac138d4ed9b96c661cc07e52c2d2c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:01 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Fri, 28 Jul 2023 03:52:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:04 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 28 Jul 2023 03:52:04 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:52:04 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:04 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:04 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 28 Jul 2023 03:52:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:05 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9336d602b0f0150e8ec2627d182005ef2b789be5e3dea018c1e554b1b401c9e8`  
		Last Modified: Fri, 28 Jul 2023 03:54:06 GMT  
		Size: 33.2 MB (33175851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8110f41f8fe5003410f3949061a75efbd9d3a195591cf86196d690ae1b2db236`  
		Last Modified: Fri, 28 Jul 2023 03:54:01 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b336a24c331465c424e3f47322fcaa6596bd7057d60b4222fad2d75f97121b73`  
		Last Modified: Fri, 28 Jul 2023 03:54:01 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0ee18130a4f35b17fce8cd7449fbaf638ff556fb0959bd4282b8da3ffccdb`  
		Last Modified: Fri, 28 Jul 2023 03:54:01 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.12-data-alpine`

```console
$ docker pull influxdb@sha256:9809f77f91e46dec77016f5a4ad488f7a0971106774f2e53c084edc276e0e235
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.12-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:647568e501deb302e7f6ae4cec8b5e5eb64d5888253b5fdd8fa75ebe323f316c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37983879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af18ee8bbc00ce46d09b7cccc5f3345662736797411904717b1fb9e537167cc8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 27 Jul 2023 21:01:06 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Thu, 27 Jul 2023 21:01:13 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 27 Jul 2023 21:01:13 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 27 Jul 2023 21:01:14 GMT
EXPOSE 8086
# Thu, 27 Jul 2023 21:01:14 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 Jul 2023 21:01:14 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 27 Jul 2023 21:01:14 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 27 Jul 2023 21:01:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jul 2023 21:01:14 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae37b9f08a90cea295c2b38668cb1ffb2f383d1fd699c9f54adf0cbbe81d4b5`  
		Last Modified: Thu, 27 Jul 2023 21:03:08 GMT  
		Size: 33.1 MB (33134690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e547dee21cb8a6d8f746077c6cf6c5d9e38995695fb4e4ffcb3bf2eda8156e`  
		Last Modified: Thu, 27 Jul 2023 21:03:03 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76585895adac24ab7752e59e409862dc74cf0818146c58b07d0de098675a3a5e`  
		Last Modified: Thu, 27 Jul 2023 21:03:03 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ad9d272774164de2a304dffbfcbc1f3ab38ef20453e1dde4c98156d3671836`  
		Last Modified: Thu, 27 Jul 2023 21:03:03 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.12-meta`

```console
$ docker pull influxdb@sha256:e5b72a5ba963fe9cbecb43fcea59a205741f45628c35e650b2999836d1169329
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.12-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:20aa1f46ac8d69e8539770bf1aeefef5a8c405fdd23fd4593c6adac15ae6ed53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83436022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66cc97881713bce3ed3a5557e5e4cbfb20aeda833fc2c79a87845df9da442d35`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:51:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 03:52:01 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Fri, 28 Jul 2023 03:52:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 28 Jul 2023 03:52:12 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 28 Jul 2023 03:52:12 GMT
EXPOSE 8091
# Fri, 28 Jul 2023 03:52:12 GMT
VOLUME [/var/lib/influxdb]
# Fri, 28 Jul 2023 03:52:12 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:52:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:52:12 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8330944056b6487b521520b1a309adf408c92209472bdbba8e83dc38cf000b`  
		Last Modified: Fri, 28 Jul 2023 03:53:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0116e4b544bb0c33a16150de6512d0200c98e5957863904454b0c463bb219e29`  
		Last Modified: Fri, 28 Jul 2023 03:54:18 GMT  
		Size: 12.6 MB (12617490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba19f65130b8d7428afdd3933fbbe2af77dbb9a7432d512e7b4ff09d5dc7994`  
		Last Modified: Fri, 28 Jul 2023 03:54:16 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cedf9689810235d6b99df594fda2843e4a4518e0df40ef62fe98d9fc48c38d0`  
		Last Modified: Fri, 28 Jul 2023 03:54:16 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.12-meta-alpine`

```console
$ docker pull influxdb@sha256:41ab5924616f2de5e84f517a26761b58c2e711aa8f6bbd9504e60bc239993a96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.12-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:e3b2c203b40931574622cc9d82296d2a66439a3dc008c731627a632c1e0433c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17429693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c13ed2509e03203f9846af87130aefb88534af15b7b66a58c5dce9c8d6027b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:09:37 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 27 Jul 2023 21:01:06 GMT
ENV INFLUXDB_VERSION=1.9.12-c1.9.12
# Thu, 27 Jul 2023 21:01:28 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 27 Jul 2023 21:01:28 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 27 Jul 2023 21:01:28 GMT
EXPOSE 8091
# Thu, 27 Jul 2023 21:01:28 GMT
VOLUME [/var/lib/influxdb]
# Thu, 27 Jul 2023 21:01:28 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 27 Jul 2023 21:01:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jul 2023 21:01:28 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777733a36019c90975436d08f29c75a0e8bdb7a267141dc5334b3c8b56ba18b5`  
		Last Modified: Thu, 15 Jun 2023 00:11:45 GMT  
		Size: 1.5 MB (1472400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7588ec7447c93ddc97ad3aa52e4c8091a32172390b9d95373af9d3bacb8bf280`  
		Last Modified: Thu, 27 Jul 2023 21:03:28 GMT  
		Size: 12.6 MB (12581708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f103f73d248b9c924f4d2bbbb4173a0e8d587d0d9979692731b90257e3a949bf`  
		Last Modified: Thu, 27 Jul 2023 21:03:27 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22d6e5265f66dd6b1aed49ef3ecbce0fb88fb30d577b1e061485adc88043a22`  
		Last Modified: Thu, 27 Jul 2023 21:03:27 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7`

```console
$ docker pull influxdb@sha256:d7ebb72e456bb865aeb56a036c0568e5101d63192f862fd1aa4e9c2fe6147d03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7` - linux; amd64

```console
$ docker pull influxdb@sha256:1838836254a474d10f8400e15c562ca5f832c1073270a7cf79fd7454d9ebc014
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114639473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b36d12738189d8020349ee0843af1bb7dc878bb79a45bdfb8abbb8c789fd6ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:53:00 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:53:01 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Jul 2023 03:53:02 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Fri, 28 Jul 2023 03:53:02 GMT
ENV GOSU_VER=1.12
# Fri, 28 Jul 2023 03:53:05 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Fri, 28 Jul 2023 03:53:05 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Jul 2023 03:53:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Jul 2023 03:53:08 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Jul 2023 03:53:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Jul 2023 03:53:11 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Jul 2023 03:53:11 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Jul 2023 03:53:11 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Jul 2023 03:53:11 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:53:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:53:12 GMT
CMD ["influxd"]
# Fri, 28 Jul 2023 03:53:12 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Jul 2023 03:53:12 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c856600570b3e8899338e040b207edb1edf918e2f432d172e7c2d7c7711cf54`  
		Last Modified: Fri, 28 Jul 2023 03:55:28 GMT  
		Size: 6.3 MB (6327879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcecbec27943f040bac0f4c870b267decadf6cf5ef35377709951978b5ad07e`  
		Last Modified: Fri, 28 Jul 2023 03:55:26 GMT  
		Size: 6.4 MB (6434101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f2e28ccd0d15763d6e5cc9aa775a980c328a5c4169da74ac67e5be373618ce`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d716e4775561a7cbcd4ff11201c60ffcfcf71f9d9449f17b1dd7edb9561240`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 986.0 KB (986004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbcd38ba0cde636731c1e6fb50c227e90d58b771250494e0d51e7d112dabfca6`  
		Last Modified: Fri, 28 Jul 2023 03:55:28 GMT  
		Size: 46.3 MB (46334285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d59db4f14987c78976a827eefb8fff5b9e041b2f8a949158a34cb59324340bd`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 23.1 MB (23128349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f7ca5eb043f964a733d65e3663217a8dd57e05c38db1dc144e832907d3a393`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45e929d4c8d8366919fa009f30a42250c0ad7296c2e2618236863d7c4058ee5`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249e42eb63e85ab22dfd19ff8e32bd8f851e947eb87a90896cdf87419b81a703`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a7ce35b71b89218687209d08387415c6fd46fcab2cf2e88d3565bb743b15f0d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.4 MB (109356501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaf3349d3cdff14ca2ddda721d19071ec4ca1b24c46320cc922c3f37647ee62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:39:00 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:39:01 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Jul 2023 03:39:02 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Fri, 28 Jul 2023 03:39:02 GMT
ENV GOSU_VER=1.12
# Fri, 28 Jul 2023 03:39:04 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Fri, 28 Jul 2023 03:39:04 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Jul 2023 03:39:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Jul 2023 03:39:08 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Jul 2023 03:39:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Jul 2023 03:39:11 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Jul 2023 03:39:11 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Jul 2023 03:39:11 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Jul 2023 03:39:11 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:39:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:39:12 GMT
CMD ["influxd"]
# Fri, 28 Jul 2023 03:39:12 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Jul 2023 03:39:12 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac205f561e969edd084e6d4d75c4df5abee0eb6c7118268b7aa992fa9f77ea55`  
		Last Modified: Fri, 28 Jul 2023 03:39:43 GMT  
		Size: 6.3 MB (6308722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b5dc0299ed71c049212b9e0bcffec4e1e356fdb96f1271d2c942761106a512`  
		Last Modified: Fri, 28 Jul 2023 03:39:41 GMT  
		Size: 6.0 MB (5953767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0add7db58fdd1110f5835913a59f75f54a51838dcc82e57abe402a4008f1bbfb`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 4.1 KB (4119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ecad330e1544d9821b3b317eac5f9c6e1a3c3d4ea2c13a6c4168566a590bdf`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 921.5 KB (921481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef78635da685d858c3c6e47eafaa8b38f930d66a6268ed4ac2b0cdfca4f6370f`  
		Last Modified: Fri, 28 Jul 2023 03:39:42 GMT  
		Size: 44.4 MB (44435850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e517c72b8b39e3045970fe57e8b1c2156856199598109fd8bbe70cd5fa09b71`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 21.7 MB (21662584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb59ddc55e6888e46120c967f51de5dcb7e3aaf990180cce7ca6aa8473c7091a`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7a6621084b5af4a1eb1151d31c94d38d395376114f8659027af2a24dede674`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc1473a02bf03ce6f291ffa11958d92504b2a0be69b89e96bb15a107fb8dd07`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7-alpine`

```console
$ docker pull influxdb@sha256:4d568d965cd911228f05e0a40598392dceda72887a63012c9aac3aab292657ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:2b8b0fbaebfb0e19b05cd214642a31b311245823bab24ca6b443f71864569dda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87866632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9853621868fb18702352e0cd3b3770baf4af570e1f2c95e8700a8e5e765ac527`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:11:03 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Thu, 15 Jun 2023 00:11:04 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 15 Jun 2023 00:11:05 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 15 Jun 2023 00:11:05 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 15 Jun 2023 00:11:09 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 15 Jun 2023 00:11:09 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 15 Jun 2023 00:11:12 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 15 Jun 2023 00:11:12 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 15 Jun 2023 00:11:12 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 15 Jun 2023 00:11:12 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 15 Jun 2023 00:11:13 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 15 Jun 2023 00:11:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 00:11:13 GMT
CMD ["influxd"]
# Thu, 15 Jun 2023 00:11:13 GMT
EXPOSE 8086
# Thu, 15 Jun 2023 00:11:13 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 15 Jun 2023 00:11:13 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 15 Jun 2023 00:11:13 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 15 Jun 2023 00:11:13 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78754065b20ae6d3b7ba9f802844991196b8f7af4a626b89e0a9f8887459794a`  
		Last Modified: Thu, 15 Jun 2023 00:13:43 GMT  
		Size: 8.6 MB (8586471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784adfd18b93d80908e7d68fd08a5487f4d2ea37dabc19bc2079c8a743459dd2`  
		Last Modified: Thu, 15 Jun 2023 00:13:43 GMT  
		Size: 6.4 MB (6434109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755a91636fbe2e94f94fd3c29ae489b6852881cdf1c2af82201bc325193fc69f`  
		Last Modified: Thu, 15 Jun 2023 00:13:42 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f15a48968976982f9967d24d4b320219044597d8e0750796568ac369a48fdf`  
		Last Modified: Thu, 15 Jun 2023 00:13:45 GMT  
		Size: 46.3 MB (46334298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5248fb28439a50a4195c753c77de97f3c41fabe4787f6e397fea0aebe5cb06`  
		Last Modified: Thu, 15 Jun 2023 00:13:42 GMT  
		Size: 23.1 MB (23128351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d09527bf9a6414867bfbdb12e2f60994cdb5df2736d90abc7a9928f2d44b28f`  
		Last Modified: Thu, 15 Jun 2023 00:13:40 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b4379b18412029fed5325d7b521b27f83d7527e61fd3efabe8fe1954cdbbe7`  
		Last Modified: Thu, 15 Jun 2023 00:13:40 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfe0fc3652c098c4303d9a42599673a4d804148b2725687164440e95be40c80`  
		Last Modified: Thu, 15 Jun 2023 00:13:40 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c940acac472154fc9b544ec9015ee7c648808bd2232891d83db1892d5a7fbd80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83829884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8416c488c7caf6a50b470427fb3a06531810eaa275b96e6029d4ed99faad42dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 03:02:53 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Thu, 15 Jun 2023 03:02:55 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 15 Jun 2023 03:02:55 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 15 Jun 2023 03:02:55 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 15 Jun 2023 03:02:59 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 15 Jun 2023 03:02:59 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 15 Jun 2023 03:03:02 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 15 Jun 2023 03:03:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 15 Jun 2023 03:03:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 15 Jun 2023 03:03:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 15 Jun 2023 03:03:02 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 15 Jun 2023 03:03:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 03:03:03 GMT
CMD ["influxd"]
# Thu, 15 Jun 2023 03:03:03 GMT
EXPOSE 8086
# Thu, 15 Jun 2023 03:03:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 15 Jun 2023 03:03:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 15 Jun 2023 03:03:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 15 Jun 2023 03:03:03 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1a2425562f802e23ddf4aee96a7dad6c211bf662002b533807008a7eb065bc`  
		Last Modified: Thu, 15 Jun 2023 03:03:18 GMT  
		Size: 8.5 MB (8507874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919059c26e31120b5e8c81fe5caa306a90d284935d5f412fc192ff042c8d988e`  
		Last Modified: Thu, 15 Jun 2023 03:03:18 GMT  
		Size: 6.0 MB (5953765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfaa1621bf080bca6ee5c1bd0b402c8a2d051b7a77a4a47efbc2b96ed112b67d`  
		Last Modified: Thu, 15 Jun 2023 03:03:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96279d1fff0acc79afad67b887af3318005301c23c93d0dd9b54e686e9998d3`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 44.4 MB (44435833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d6fd5df8ccc6f553f9704636d4df791bede9c9627026c248032931503fc281`  
		Last Modified: Thu, 15 Jun 2023 03:03:17 GMT  
		Size: 21.7 MB (21662583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4ae790f663637d782ad8887c60bafe88a5040189ce075f3b02d58f59889ccf`  
		Last Modified: Thu, 15 Jun 2023 03:03:15 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7df868318f3946bbdade780f3aa55e20001893ab4a43f9dfb110ac6058e2a0a`  
		Last Modified: Thu, 15 Jun 2023 03:03:15 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42464989a2c662e384a94aabfed542f544ab1ef6969203229e89cf773a247045`  
		Last Modified: Thu, 15 Jun 2023 03:03:15 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.1`

```console
$ docker pull influxdb@sha256:d7ebb72e456bb865aeb56a036c0568e5101d63192f862fd1aa4e9c2fe6147d03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.1` - linux; amd64

```console
$ docker pull influxdb@sha256:1838836254a474d10f8400e15c562ca5f832c1073270a7cf79fd7454d9ebc014
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114639473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b36d12738189d8020349ee0843af1bb7dc878bb79a45bdfb8abbb8c789fd6ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:53:00 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:53:01 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Jul 2023 03:53:02 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Fri, 28 Jul 2023 03:53:02 GMT
ENV GOSU_VER=1.12
# Fri, 28 Jul 2023 03:53:05 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Fri, 28 Jul 2023 03:53:05 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Jul 2023 03:53:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Jul 2023 03:53:08 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Jul 2023 03:53:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Jul 2023 03:53:11 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Jul 2023 03:53:11 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Jul 2023 03:53:11 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Jul 2023 03:53:11 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:53:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:53:12 GMT
CMD ["influxd"]
# Fri, 28 Jul 2023 03:53:12 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Jul 2023 03:53:12 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c856600570b3e8899338e040b207edb1edf918e2f432d172e7c2d7c7711cf54`  
		Last Modified: Fri, 28 Jul 2023 03:55:28 GMT  
		Size: 6.3 MB (6327879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcecbec27943f040bac0f4c870b267decadf6cf5ef35377709951978b5ad07e`  
		Last Modified: Fri, 28 Jul 2023 03:55:26 GMT  
		Size: 6.4 MB (6434101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f2e28ccd0d15763d6e5cc9aa775a980c328a5c4169da74ac67e5be373618ce`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d716e4775561a7cbcd4ff11201c60ffcfcf71f9d9449f17b1dd7edb9561240`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 986.0 KB (986004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbcd38ba0cde636731c1e6fb50c227e90d58b771250494e0d51e7d112dabfca6`  
		Last Modified: Fri, 28 Jul 2023 03:55:28 GMT  
		Size: 46.3 MB (46334285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d59db4f14987c78976a827eefb8fff5b9e041b2f8a949158a34cb59324340bd`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 23.1 MB (23128349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f7ca5eb043f964a733d65e3663217a8dd57e05c38db1dc144e832907d3a393`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45e929d4c8d8366919fa009f30a42250c0ad7296c2e2618236863d7c4058ee5`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249e42eb63e85ab22dfd19ff8e32bd8f851e947eb87a90896cdf87419b81a703`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a7ce35b71b89218687209d08387415c6fd46fcab2cf2e88d3565bb743b15f0d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.4 MB (109356501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaf3349d3cdff14ca2ddda721d19071ec4ca1b24c46320cc922c3f37647ee62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:39:00 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:39:01 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Jul 2023 03:39:02 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Fri, 28 Jul 2023 03:39:02 GMT
ENV GOSU_VER=1.12
# Fri, 28 Jul 2023 03:39:04 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Fri, 28 Jul 2023 03:39:04 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Jul 2023 03:39:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Jul 2023 03:39:08 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Jul 2023 03:39:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Jul 2023 03:39:11 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Jul 2023 03:39:11 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Jul 2023 03:39:11 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Jul 2023 03:39:11 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:39:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:39:12 GMT
CMD ["influxd"]
# Fri, 28 Jul 2023 03:39:12 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Jul 2023 03:39:12 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac205f561e969edd084e6d4d75c4df5abee0eb6c7118268b7aa992fa9f77ea55`  
		Last Modified: Fri, 28 Jul 2023 03:39:43 GMT  
		Size: 6.3 MB (6308722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b5dc0299ed71c049212b9e0bcffec4e1e356fdb96f1271d2c942761106a512`  
		Last Modified: Fri, 28 Jul 2023 03:39:41 GMT  
		Size: 6.0 MB (5953767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0add7db58fdd1110f5835913a59f75f54a51838dcc82e57abe402a4008f1bbfb`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 4.1 KB (4119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ecad330e1544d9821b3b317eac5f9c6e1a3c3d4ea2c13a6c4168566a590bdf`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 921.5 KB (921481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef78635da685d858c3c6e47eafaa8b38f930d66a6268ed4ac2b0cdfca4f6370f`  
		Last Modified: Fri, 28 Jul 2023 03:39:42 GMT  
		Size: 44.4 MB (44435850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e517c72b8b39e3045970fe57e8b1c2156856199598109fd8bbe70cd5fa09b71`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 21.7 MB (21662584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb59ddc55e6888e46120c967f51de5dcb7e3aaf990180cce7ca6aa8473c7091a`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7a6621084b5af4a1eb1151d31c94d38d395376114f8659027af2a24dede674`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc1473a02bf03ce6f291ffa11958d92504b2a0be69b89e96bb15a107fb8dd07`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.1-alpine`

```console
$ docker pull influxdb@sha256:4d568d965cd911228f05e0a40598392dceda72887a63012c9aac3aab292657ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:2b8b0fbaebfb0e19b05cd214642a31b311245823bab24ca6b443f71864569dda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87866632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9853621868fb18702352e0cd3b3770baf4af570e1f2c95e8700a8e5e765ac527`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:11:03 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Thu, 15 Jun 2023 00:11:04 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 15 Jun 2023 00:11:05 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 15 Jun 2023 00:11:05 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 15 Jun 2023 00:11:09 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 15 Jun 2023 00:11:09 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 15 Jun 2023 00:11:12 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 15 Jun 2023 00:11:12 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 15 Jun 2023 00:11:12 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 15 Jun 2023 00:11:12 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 15 Jun 2023 00:11:13 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 15 Jun 2023 00:11:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 00:11:13 GMT
CMD ["influxd"]
# Thu, 15 Jun 2023 00:11:13 GMT
EXPOSE 8086
# Thu, 15 Jun 2023 00:11:13 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 15 Jun 2023 00:11:13 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 15 Jun 2023 00:11:13 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 15 Jun 2023 00:11:13 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78754065b20ae6d3b7ba9f802844991196b8f7af4a626b89e0a9f8887459794a`  
		Last Modified: Thu, 15 Jun 2023 00:13:43 GMT  
		Size: 8.6 MB (8586471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784adfd18b93d80908e7d68fd08a5487f4d2ea37dabc19bc2079c8a743459dd2`  
		Last Modified: Thu, 15 Jun 2023 00:13:43 GMT  
		Size: 6.4 MB (6434109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755a91636fbe2e94f94fd3c29ae489b6852881cdf1c2af82201bc325193fc69f`  
		Last Modified: Thu, 15 Jun 2023 00:13:42 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f15a48968976982f9967d24d4b320219044597d8e0750796568ac369a48fdf`  
		Last Modified: Thu, 15 Jun 2023 00:13:45 GMT  
		Size: 46.3 MB (46334298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5248fb28439a50a4195c753c77de97f3c41fabe4787f6e397fea0aebe5cb06`  
		Last Modified: Thu, 15 Jun 2023 00:13:42 GMT  
		Size: 23.1 MB (23128351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d09527bf9a6414867bfbdb12e2f60994cdb5df2736d90abc7a9928f2d44b28f`  
		Last Modified: Thu, 15 Jun 2023 00:13:40 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b4379b18412029fed5325d7b521b27f83d7527e61fd3efabe8fe1954cdbbe7`  
		Last Modified: Thu, 15 Jun 2023 00:13:40 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfe0fc3652c098c4303d9a42599673a4d804148b2725687164440e95be40c80`  
		Last Modified: Thu, 15 Jun 2023 00:13:40 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c940acac472154fc9b544ec9015ee7c648808bd2232891d83db1892d5a7fbd80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83829884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8416c488c7caf6a50b470427fb3a06531810eaa275b96e6029d4ed99faad42dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 03:02:53 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Thu, 15 Jun 2023 03:02:55 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 15 Jun 2023 03:02:55 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 15 Jun 2023 03:02:55 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 15 Jun 2023 03:02:59 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 15 Jun 2023 03:02:59 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 15 Jun 2023 03:03:02 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 15 Jun 2023 03:03:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 15 Jun 2023 03:03:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 15 Jun 2023 03:03:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 15 Jun 2023 03:03:02 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 15 Jun 2023 03:03:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 03:03:03 GMT
CMD ["influxd"]
# Thu, 15 Jun 2023 03:03:03 GMT
EXPOSE 8086
# Thu, 15 Jun 2023 03:03:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 15 Jun 2023 03:03:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 15 Jun 2023 03:03:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 15 Jun 2023 03:03:03 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1a2425562f802e23ddf4aee96a7dad6c211bf662002b533807008a7eb065bc`  
		Last Modified: Thu, 15 Jun 2023 03:03:18 GMT  
		Size: 8.5 MB (8507874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919059c26e31120b5e8c81fe5caa306a90d284935d5f412fc192ff042c8d988e`  
		Last Modified: Thu, 15 Jun 2023 03:03:18 GMT  
		Size: 6.0 MB (5953765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfaa1621bf080bca6ee5c1bd0b402c8a2d051b7a77a4a47efbc2b96ed112b67d`  
		Last Modified: Thu, 15 Jun 2023 03:03:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96279d1fff0acc79afad67b887af3318005301c23c93d0dd9b54e686e9998d3`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 44.4 MB (44435833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d6fd5df8ccc6f553f9704636d4df791bede9c9627026c248032931503fc281`  
		Last Modified: Thu, 15 Jun 2023 03:03:17 GMT  
		Size: 21.7 MB (21662583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4ae790f663637d782ad8887c60bafe88a5040189ce075f3b02d58f59889ccf`  
		Last Modified: Thu, 15 Jun 2023 03:03:15 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7df868318f3946bbdade780f3aa55e20001893ab4a43f9dfb110ac6058e2a0a`  
		Last Modified: Thu, 15 Jun 2023 03:03:15 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42464989a2c662e384a94aabfed542f544ab1ef6969203229e89cf773a247045`  
		Last Modified: Thu, 15 Jun 2023 03:03:15 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:4d568d965cd911228f05e0a40598392dceda72887a63012c9aac3aab292657ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:2b8b0fbaebfb0e19b05cd214642a31b311245823bab24ca6b443f71864569dda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87866632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9853621868fb18702352e0cd3b3770baf4af570e1f2c95e8700a8e5e765ac527`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 00:11:03 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Thu, 15 Jun 2023 00:11:04 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 15 Jun 2023 00:11:05 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 15 Jun 2023 00:11:05 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 15 Jun 2023 00:11:09 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 15 Jun 2023 00:11:09 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 15 Jun 2023 00:11:12 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 15 Jun 2023 00:11:12 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 15 Jun 2023 00:11:12 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 15 Jun 2023 00:11:12 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 15 Jun 2023 00:11:13 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 15 Jun 2023 00:11:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 00:11:13 GMT
CMD ["influxd"]
# Thu, 15 Jun 2023 00:11:13 GMT
EXPOSE 8086
# Thu, 15 Jun 2023 00:11:13 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 15 Jun 2023 00:11:13 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 15 Jun 2023 00:11:13 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 15 Jun 2023 00:11:13 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78754065b20ae6d3b7ba9f802844991196b8f7af4a626b89e0a9f8887459794a`  
		Last Modified: Thu, 15 Jun 2023 00:13:43 GMT  
		Size: 8.6 MB (8586471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784adfd18b93d80908e7d68fd08a5487f4d2ea37dabc19bc2079c8a743459dd2`  
		Last Modified: Thu, 15 Jun 2023 00:13:43 GMT  
		Size: 6.4 MB (6434109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755a91636fbe2e94f94fd3c29ae489b6852881cdf1c2af82201bc325193fc69f`  
		Last Modified: Thu, 15 Jun 2023 00:13:42 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f15a48968976982f9967d24d4b320219044597d8e0750796568ac369a48fdf`  
		Last Modified: Thu, 15 Jun 2023 00:13:45 GMT  
		Size: 46.3 MB (46334298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5248fb28439a50a4195c753c77de97f3c41fabe4787f6e397fea0aebe5cb06`  
		Last Modified: Thu, 15 Jun 2023 00:13:42 GMT  
		Size: 23.1 MB (23128351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d09527bf9a6414867bfbdb12e2f60994cdb5df2736d90abc7a9928f2d44b28f`  
		Last Modified: Thu, 15 Jun 2023 00:13:40 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b4379b18412029fed5325d7b521b27f83d7527e61fd3efabe8fe1954cdbbe7`  
		Last Modified: Thu, 15 Jun 2023 00:13:40 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfe0fc3652c098c4303d9a42599673a4d804148b2725687164440e95be40c80`  
		Last Modified: Thu, 15 Jun 2023 00:13:40 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c940acac472154fc9b544ec9015ee7c648808bd2232891d83db1892d5a7fbd80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83829884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8416c488c7caf6a50b470427fb3a06531810eaa275b96e6029d4ed99faad42dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 03:02:53 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Thu, 15 Jun 2023 03:02:55 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 15 Jun 2023 03:02:55 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 15 Jun 2023 03:02:55 GMT
ENV INFLUXDB_VERSION=2.7.1
# Thu, 15 Jun 2023 03:02:59 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 15 Jun 2023 03:02:59 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 15 Jun 2023 03:03:02 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 15 Jun 2023 03:03:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 15 Jun 2023 03:03:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 15 Jun 2023 03:03:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 15 Jun 2023 03:03:02 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 15 Jun 2023 03:03:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 03:03:03 GMT
CMD ["influxd"]
# Thu, 15 Jun 2023 03:03:03 GMT
EXPOSE 8086
# Thu, 15 Jun 2023 03:03:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 15 Jun 2023 03:03:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 15 Jun 2023 03:03:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 15 Jun 2023 03:03:03 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1a2425562f802e23ddf4aee96a7dad6c211bf662002b533807008a7eb065bc`  
		Last Modified: Thu, 15 Jun 2023 03:03:18 GMT  
		Size: 8.5 MB (8507874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919059c26e31120b5e8c81fe5caa306a90d284935d5f412fc192ff042c8d988e`  
		Last Modified: Thu, 15 Jun 2023 03:03:18 GMT  
		Size: 6.0 MB (5953765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfaa1621bf080bca6ee5c1bd0b402c8a2d051b7a77a4a47efbc2b96ed112b67d`  
		Last Modified: Thu, 15 Jun 2023 03:03:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96279d1fff0acc79afad67b887af3318005301c23c93d0dd9b54e686e9998d3`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 44.4 MB (44435833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d6fd5df8ccc6f553f9704636d4df791bede9c9627026c248032931503fc281`  
		Last Modified: Thu, 15 Jun 2023 03:03:17 GMT  
		Size: 21.7 MB (21662583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4ae790f663637d782ad8887c60bafe88a5040189ce075f3b02d58f59889ccf`  
		Last Modified: Thu, 15 Jun 2023 03:03:15 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7df868318f3946bbdade780f3aa55e20001893ab4a43f9dfb110ac6058e2a0a`  
		Last Modified: Thu, 15 Jun 2023 03:03:15 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42464989a2c662e384a94aabfed542f544ab1ef6969203229e89cf773a247045`  
		Last Modified: Thu, 15 Jun 2023 03:03:15 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:d7ebb72e456bb865aeb56a036c0568e5101d63192f862fd1aa4e9c2fe6147d03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:1838836254a474d10f8400e15c562ca5f832c1073270a7cf79fd7454d9ebc014
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114639473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b36d12738189d8020349ee0843af1bb7dc878bb79a45bdfb8abbb8c789fd6ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:53:00 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:53:01 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Jul 2023 03:53:02 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Fri, 28 Jul 2023 03:53:02 GMT
ENV GOSU_VER=1.12
# Fri, 28 Jul 2023 03:53:05 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Fri, 28 Jul 2023 03:53:05 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Jul 2023 03:53:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Jul 2023 03:53:08 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Jul 2023 03:53:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Jul 2023 03:53:11 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Jul 2023 03:53:11 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Jul 2023 03:53:11 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Jul 2023 03:53:11 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:53:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:53:12 GMT
CMD ["influxd"]
# Fri, 28 Jul 2023 03:53:12 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Jul 2023 03:53:12 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c856600570b3e8899338e040b207edb1edf918e2f432d172e7c2d7c7711cf54`  
		Last Modified: Fri, 28 Jul 2023 03:55:28 GMT  
		Size: 6.3 MB (6327879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcecbec27943f040bac0f4c870b267decadf6cf5ef35377709951978b5ad07e`  
		Last Modified: Fri, 28 Jul 2023 03:55:26 GMT  
		Size: 6.4 MB (6434101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f2e28ccd0d15763d6e5cc9aa775a980c328a5c4169da74ac67e5be373618ce`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d716e4775561a7cbcd4ff11201c60ffcfcf71f9d9449f17b1dd7edb9561240`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 986.0 KB (986004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbcd38ba0cde636731c1e6fb50c227e90d58b771250494e0d51e7d112dabfca6`  
		Last Modified: Fri, 28 Jul 2023 03:55:28 GMT  
		Size: 46.3 MB (46334285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d59db4f14987c78976a827eefb8fff5b9e041b2f8a949158a34cb59324340bd`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 23.1 MB (23128349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f7ca5eb043f964a733d65e3663217a8dd57e05c38db1dc144e832907d3a393`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45e929d4c8d8366919fa009f30a42250c0ad7296c2e2618236863d7c4058ee5`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249e42eb63e85ab22dfd19ff8e32bd8f851e947eb87a90896cdf87419b81a703`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a7ce35b71b89218687209d08387415c6fd46fcab2cf2e88d3565bb743b15f0d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.4 MB (109356501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaf3349d3cdff14ca2ddda721d19071ec4ca1b24c46320cc922c3f37647ee62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:39:00 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:39:01 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Jul 2023 03:39:02 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Fri, 28 Jul 2023 03:39:02 GMT
ENV GOSU_VER=1.12
# Fri, 28 Jul 2023 03:39:04 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Fri, 28 Jul 2023 03:39:04 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Jul 2023 03:39:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Jul 2023 03:39:08 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Jul 2023 03:39:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Jul 2023 03:39:11 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Jul 2023 03:39:11 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Jul 2023 03:39:11 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Jul 2023 03:39:11 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:39:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:39:12 GMT
CMD ["influxd"]
# Fri, 28 Jul 2023 03:39:12 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Jul 2023 03:39:12 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac205f561e969edd084e6d4d75c4df5abee0eb6c7118268b7aa992fa9f77ea55`  
		Last Modified: Fri, 28 Jul 2023 03:39:43 GMT  
		Size: 6.3 MB (6308722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b5dc0299ed71c049212b9e0bcffec4e1e356fdb96f1271d2c942761106a512`  
		Last Modified: Fri, 28 Jul 2023 03:39:41 GMT  
		Size: 6.0 MB (5953767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0add7db58fdd1110f5835913a59f75f54a51838dcc82e57abe402a4008f1bbfb`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 4.1 KB (4119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ecad330e1544d9821b3b317eac5f9c6e1a3c3d4ea2c13a6c4168566a590bdf`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 921.5 KB (921481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef78635da685d858c3c6e47eafaa8b38f930d66a6268ed4ac2b0cdfca4f6370f`  
		Last Modified: Fri, 28 Jul 2023 03:39:42 GMT  
		Size: 44.4 MB (44435850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e517c72b8b39e3045970fe57e8b1c2156856199598109fd8bbe70cd5fa09b71`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 21.7 MB (21662584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb59ddc55e6888e46120c967f51de5dcb7e3aaf990180cce7ca6aa8473c7091a`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7a6621084b5af4a1eb1151d31c94d38d395376114f8659027af2a24dede674`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc1473a02bf03ce6f291ffa11958d92504b2a0be69b89e96bb15a107fb8dd07`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
