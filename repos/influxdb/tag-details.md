<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `influxdb`

-	[`influxdb:1.10-data`](#influxdb110-data)
-	[`influxdb:1.10-data-alpine`](#influxdb110-data-alpine)
-	[`influxdb:1.10-meta`](#influxdb110-meta)
-	[`influxdb:1.10-meta-alpine`](#influxdb110-meta-alpine)
-	[`influxdb:1.10.0-data`](#influxdb1100-data)
-	[`influxdb:1.10.0-data-alpine`](#influxdb1100-data-alpine)
-	[`influxdb:1.10.0-meta`](#influxdb1100-meta)
-	[`influxdb:1.10.0-meta-alpine`](#influxdb1100-meta-alpine)
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
-	[`influxdb:1.9.8-data`](#influxdb198-data)
-	[`influxdb:1.9.8-data-alpine`](#influxdb198-data-alpine)
-	[`influxdb:1.9.8-meta`](#influxdb198-meta)
-	[`influxdb:1.9.8-meta-alpine`](#influxdb198-meta-alpine)
-	[`influxdb:2.4`](#influxdb24)
-	[`influxdb:2.4-alpine`](#influxdb24-alpine)
-	[`influxdb:2.4.0`](#influxdb240)
-	[`influxdb:2.4.0-alpine`](#influxdb240-alpine)
-	[`influxdb:2.5`](#influxdb25)
-	[`influxdb:2.5-alpine`](#influxdb25-alpine)
-	[`influxdb:2.5.1`](#influxdb251)
-	[`influxdb:2.5.1-alpine`](#influxdb251-alpine)
-	[`influxdb:2.6`](#influxdb26)
-	[`influxdb:2.6-alpine`](#influxdb26-alpine)
-	[`influxdb:2.6.0`](#influxdb260)
-	[`influxdb:2.6.0-alpine`](#influxdb260-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.10-data`

```console
$ docker pull influxdb@sha256:fb50f6b5ba0cf150dea51e459d98279f39dc9faaf86a468573a975ee5c69aef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:2c916bf671e06740d9a9b86f89b91f6718c585f111d903cc85833318760524a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101781655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a4029306702f41458200500a8184398d6db6db00dab20275b1671b61d5e1db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 17:00:38 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Tue, 06 Dec 2022 17:00:42 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 06 Dec 2022 17:00:42 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 06 Dec 2022 17:00:42 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 17:00:42 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 17:00:43 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 06 Dec 2022 17:00:43 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 06 Dec 2022 17:00:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:00:43 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23438adec1ce3e5bcf265ca3593bfe8e93e04da1e3ae0bd01f9a46567bada7b5`  
		Last Modified: Tue, 06 Dec 2022 17:03:58 GMT  
		Size: 30.7 MB (30693306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2245df77704ccb2be55e0dd67e13c7b8c333c98d43c1156b985c877d12a7752f`  
		Last Modified: Tue, 06 Dec 2022 17:03:54 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7c1b6d1cdb35736106726c16fb55f2f432c79ea90d581fd9955a742b79817a`  
		Last Modified: Tue, 06 Dec 2022 17:03:53 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3089f1cb6e917a16d1535c50a8f78c29a06a4bd160665077603f461a9d80da`  
		Last Modified: Tue, 06 Dec 2022 17:03:53 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-data-alpine`

```console
$ docker pull influxdb@sha256:97a54cdaa79fde21531561711a49a45d5219e83e251f804ba0d8aaeace153e25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:1b5f43f86c108b08915587a7836e791e4a9d77ed1a83635b55e6ae5d7b3fb58b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34961985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f20e981428ad6caf309ff381c1a14f62f2f9e4ecc629726f557516278fc5f30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:41:05 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 06 Oct 2022 22:41:11 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:41:11 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 06 Oct 2022 22:41:11 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:41:12 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:41:12 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:41:12 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 06 Oct 2022 22:41:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:41:12 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd8ff045fb30dc7039026afa7b842b02209eff1782d50c52626aded0e903d69`  
		Last Modified: Thu, 06 Oct 2022 22:44:40 GMT  
		Size: 30.7 MB (30651262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816d358bef8a0bf29346a7d2ca321c2668410b9c104f5025c20346a1ffed980`  
		Last Modified: Thu, 06 Oct 2022 22:44:35 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108fb18700076955d74033f3a3e842d99e982f694b2ffba5e3b6ec53d6b93cdd`  
		Last Modified: Thu, 06 Oct 2022 22:44:35 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e082e9ca7b8d9e85406af28023733f541b9e792e663ff66da311d3390711b00f`  
		Last Modified: Thu, 06 Oct 2022 22:44:35 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta`

```console
$ docker pull influxdb@sha256:9d0ce83a31efc571787d7e1a260cced02d15cdc77d801d641cfa6567994444c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:2e71177de2e9ede2f764e7631cefa4ed1173891ada16f5f4e6542b8444cff012
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.0 MB (82994345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e65519ce0aa5ae3ec46772de594fc061d1425c18b4b07a174bab622f9c97a9b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 17:00:38 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Tue, 06 Dec 2022 17:00:50 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 06 Dec 2022 17:00:50 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 06 Dec 2022 17:00:50 GMT
EXPOSE 8091
# Tue, 06 Dec 2022 17:00:50 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 17:00:50 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 06 Dec 2022 17:00:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:00:50 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61069ce781bebd3c7a43ba7ac4f482789ab32ded82e424ab8f9d324c315a1a0`  
		Last Modified: Tue, 06 Dec 2022 17:04:10 GMT  
		Size: 11.9 MB (11907199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc96a7ae13dea66c9a71d6130bafc50e8e57820e8becf1fbaa23597338aa3879`  
		Last Modified: Tue, 06 Dec 2022 17:04:08 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce2457daf92b9e7edb9e70b901c8f4a080a1523695ca7420d3437c2855d54ce`  
		Last Modified: Tue, 06 Dec 2022 17:04:08 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta-alpine`

```console
$ docker pull influxdb@sha256:46a7513ea128bd01532c81463c59e069af801f8cd31e157854f7fec901aeae6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:3870d14532d6ab3ef7c1bd7c4faaa75397b44770abbec610bcab034f166c2cdc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16181334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:215f5c4a24b25c6869311fe1fa9505fd0c6366b8894118556571709c0865069d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:41:05 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 06 Oct 2022 22:41:21 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:41:21 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 06 Oct 2022 22:41:21 GMT
EXPOSE 8091
# Thu, 06 Oct 2022 22:41:22 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:41:22 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:41:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:41:22 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0068a3da6be923bef1d4268544334826869f86960167887234f892f6cf4d479`  
		Last Modified: Thu, 06 Oct 2022 22:44:52 GMT  
		Size: 11.9 MB (11871815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8cc9a0c8fbc75118e4bf898decc19f9f1ae6667aa1008dc7aa52aa0cc20877`  
		Last Modified: Thu, 06 Oct 2022 22:44:51 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2995883e4c21340e6643e44cfce84ce331434205ebb233093a8af992b8d03ce5`  
		Last Modified: Thu, 06 Oct 2022 22:44:50 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.0-data`

```console
$ docker pull influxdb@sha256:fb50f6b5ba0cf150dea51e459d98279f39dc9faaf86a468573a975ee5c69aef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.0-data` - linux; amd64

```console
$ docker pull influxdb@sha256:2c916bf671e06740d9a9b86f89b91f6718c585f111d903cc85833318760524a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101781655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a4029306702f41458200500a8184398d6db6db00dab20275b1671b61d5e1db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 17:00:38 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Tue, 06 Dec 2022 17:00:42 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 06 Dec 2022 17:00:42 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 06 Dec 2022 17:00:42 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 17:00:42 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 17:00:43 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 06 Dec 2022 17:00:43 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 06 Dec 2022 17:00:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:00:43 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23438adec1ce3e5bcf265ca3593bfe8e93e04da1e3ae0bd01f9a46567bada7b5`  
		Last Modified: Tue, 06 Dec 2022 17:03:58 GMT  
		Size: 30.7 MB (30693306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2245df77704ccb2be55e0dd67e13c7b8c333c98d43c1156b985c877d12a7752f`  
		Last Modified: Tue, 06 Dec 2022 17:03:54 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7c1b6d1cdb35736106726c16fb55f2f432c79ea90d581fd9955a742b79817a`  
		Last Modified: Tue, 06 Dec 2022 17:03:53 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3089f1cb6e917a16d1535c50a8f78c29a06a4bd160665077603f461a9d80da`  
		Last Modified: Tue, 06 Dec 2022 17:03:53 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.0-data-alpine`

```console
$ docker pull influxdb@sha256:97a54cdaa79fde21531561711a49a45d5219e83e251f804ba0d8aaeace153e25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.0-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:1b5f43f86c108b08915587a7836e791e4a9d77ed1a83635b55e6ae5d7b3fb58b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34961985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f20e981428ad6caf309ff381c1a14f62f2f9e4ecc629726f557516278fc5f30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:41:05 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 06 Oct 2022 22:41:11 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:41:11 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 06 Oct 2022 22:41:11 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:41:12 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:41:12 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:41:12 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 06 Oct 2022 22:41:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:41:12 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd8ff045fb30dc7039026afa7b842b02209eff1782d50c52626aded0e903d69`  
		Last Modified: Thu, 06 Oct 2022 22:44:40 GMT  
		Size: 30.7 MB (30651262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816d358bef8a0bf29346a7d2ca321c2668410b9c104f5025c20346a1ffed980`  
		Last Modified: Thu, 06 Oct 2022 22:44:35 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108fb18700076955d74033f3a3e842d99e982f694b2ffba5e3b6ec53d6b93cdd`  
		Last Modified: Thu, 06 Oct 2022 22:44:35 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e082e9ca7b8d9e85406af28023733f541b9e792e663ff66da311d3390711b00f`  
		Last Modified: Thu, 06 Oct 2022 22:44:35 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.0-meta`

```console
$ docker pull influxdb@sha256:9d0ce83a31efc571787d7e1a260cced02d15cdc77d801d641cfa6567994444c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.0-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:2e71177de2e9ede2f764e7631cefa4ed1173891ada16f5f4e6542b8444cff012
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.0 MB (82994345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e65519ce0aa5ae3ec46772de594fc061d1425c18b4b07a174bab622f9c97a9b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 17:00:38 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Tue, 06 Dec 2022 17:00:50 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 06 Dec 2022 17:00:50 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 06 Dec 2022 17:00:50 GMT
EXPOSE 8091
# Tue, 06 Dec 2022 17:00:50 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 17:00:50 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 06 Dec 2022 17:00:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:00:50 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61069ce781bebd3c7a43ba7ac4f482789ab32ded82e424ab8f9d324c315a1a0`  
		Last Modified: Tue, 06 Dec 2022 17:04:10 GMT  
		Size: 11.9 MB (11907199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc96a7ae13dea66c9a71d6130bafc50e8e57820e8becf1fbaa23597338aa3879`  
		Last Modified: Tue, 06 Dec 2022 17:04:08 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce2457daf92b9e7edb9e70b901c8f4a080a1523695ca7420d3437c2855d54ce`  
		Last Modified: Tue, 06 Dec 2022 17:04:08 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.0-meta-alpine`

```console
$ docker pull influxdb@sha256:46a7513ea128bd01532c81463c59e069af801f8cd31e157854f7fec901aeae6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.0-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:3870d14532d6ab3ef7c1bd7c4faaa75397b44770abbec610bcab034f166c2cdc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16181334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:215f5c4a24b25c6869311fe1fa9505fd0c6366b8894118556571709c0865069d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:41:05 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Thu, 06 Oct 2022 22:41:21 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:41:21 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 06 Oct 2022 22:41:21 GMT
EXPOSE 8091
# Thu, 06 Oct 2022 22:41:22 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:41:22 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:41:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:41:22 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0068a3da6be923bef1d4268544334826869f86960167887234f892f6cf4d479`  
		Last Modified: Thu, 06 Oct 2022 22:44:52 GMT  
		Size: 11.9 MB (11871815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8cc9a0c8fbc75118e4bf898decc19f9f1ae6667aa1008dc7aa52aa0cc20877`  
		Last Modified: Thu, 06 Oct 2022 22:44:51 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2995883e4c21340e6643e44cfce84ce331434205ebb233093a8af992b8d03ce5`  
		Last Modified: Thu, 06 Oct 2022 22:44:50 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:4f1b449205ab29b56e096581227cfe7647090e1d64c8a510d6089c3bf2706ffd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:1ae78492b61983ae9331da8beb3912daf2bed91cd01f293b407f6217769085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125974042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27bb5416e7117f7e62d94057908585104c8d7bc27a31120508d044452b90e3bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 16:59:54 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 06 Dec 2022 16:59:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 06 Dec 2022 16:59:58 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 06 Dec 2022 16:59:59 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 16:59:59 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 16:59:59 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 06 Dec 2022 16:59:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 06 Dec 2022 16:59:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 16:59:59 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5644cc08aefa3a356bbfe4c5d0adc8cf1e05b360f35b477c41b6f531e0dfebe3`  
		Last Modified: Tue, 06 Dec 2022 17:02:44 GMT  
		Size: 54.9 MB (54885754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a7b585ac9d0af01da7581306c9a21de42e9f4d1cb0184ecad86b5af7859e17`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33b15a4a898166bb7b206df89a52a04214d7c89dbd8c20510084fee56c0747`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b88b55586f58a1c612ddb23a171fcd916ede7ead5f9799ee073ac889ec2d411`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:541197d04fd253cf561100aee74c750a03e5ae63591d453b353f00dc7eac9dda
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (116976209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6039cf3a99c363239215b60530c1efe67ac9678d1a36cccacbb23deb2b740db2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:30 GMT
ADD file:72eaf12ec65c98e9cde1654b6adb2b3d19f7d81c13b12801c198f699252b7503 in / 
# Tue, 06 Dec 2022 00:58:31 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:49:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:49:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 20:41:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 20:41:28 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 06 Dec 2022 20:41:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 06 Dec 2022 20:41:33 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 06 Dec 2022 20:41:33 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 20:41:34 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 20:41:34 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 06 Dec 2022 20:41:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 06 Dec 2022 20:41:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 20:41:34 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:58e27900c24f1f8f5b6b5eacbc073583f2372b58e9f5678dfe171b496b9cd71e`  
		Last Modified: Tue, 06 Dec 2022 01:05:33 GMT  
		Size: 50.2 MB (50207085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3975e0b03a66ba4371cf2cae58e77e148d952679dd5fa1e322124604805fc6a2`  
		Last Modified: Tue, 06 Dec 2022 09:59:29 GMT  
		Size: 4.9 MB (4932853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806632ddd1d79b55318482c725338dc97649f22ca0ec8dbdf79cc8be451201eb`  
		Last Modified: Tue, 06 Dec 2022 09:59:30 GMT  
		Size: 10.2 MB (10218527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2dd4bfa6e14ee8d0a05ffdef9e7ea802c2ddf6213839e03805bf83cbcf4695`  
		Last Modified: Tue, 06 Dec 2022 20:41:48 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7902dcb754540ebbcdb7f87d48069f1b6904359f71d4ab378b3674cc5e183d1e`  
		Last Modified: Tue, 06 Dec 2022 20:41:56 GMT  
		Size: 51.6 MB (51613159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1936ffba1d99c0f0496687499437956a585733f42852f7c465d9deb91907f6ff`  
		Last Modified: Tue, 06 Dec 2022 20:41:49 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc0d850537c9c29fea7407483dea5d56c78da357636fea263a1279e19072457`  
		Last Modified: Tue, 06 Dec 2022 20:41:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0cb6c0ceac97bb3d7c86dce7e493d40c49b07ee76b92b9ca71b41802a191e2`  
		Last Modified: Tue, 06 Dec 2022 20:41:48 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:2f497e0d8ad38deeff3bfb7414d8966c61d8ffaf08736598dfc364f7fd140f83
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120939739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2208cb5674e672388834c42c81e28dd508224f1370bd1433788a625440cc2ff3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:06:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 17:34:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 21 Dec 2022 17:34:19 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 21 Dec 2022 17:34:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 21 Dec 2022 17:34:23 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 21 Dec 2022 17:34:23 GMT
EXPOSE 8086
# Wed, 21 Dec 2022 17:34:23 GMT
VOLUME [/var/lib/influxdb]
# Wed, 21 Dec 2022 17:34:23 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 21 Dec 2022 17:34:23 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 21 Dec 2022 17:34:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Dec 2022 17:34:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0470f9572d03767b054118fe19e60a9c7e2510168b3a0868d9ac2953d2def5`  
		Last Modified: Wed, 21 Dec 2022 02:12:40 GMT  
		Size: 5.1 MB (5149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dfcef0545e5bca269c65c0208385c886321a1e0212977299827be5346dfea5`  
		Last Modified: Wed, 21 Dec 2022 02:12:40 GMT  
		Size: 10.9 MB (10873505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679d11cfdf518503a3a8d7aead626261fb2b7ca220c3c3dddc290b86d6d25c1e`  
		Last Modified: Wed, 21 Dec 2022 17:35:48 GMT  
		Size: 2.9 KB (2899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b872061ff402c9ef0821b6284a8475e13d4ee5b72e0e46f520245ad001cb60`  
		Last Modified: Wed, 21 Dec 2022 17:35:53 GMT  
		Size: 51.2 MB (51230051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db62c4d2794c5e6c1d825b73db01dfd972c45ea7ef17dfe97a500dd314e757fa`  
		Last Modified: Wed, 21 Dec 2022 17:35:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be5ca48085cb42c932d44d8ee475c0c746f988e1e7beddb989595317cc91ef`  
		Last Modified: Wed, 21 Dec 2022 17:35:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6483244078527630a70000ff9688d1f0b1c1b6b90fb2b64465f5acf1b7308ff`  
		Last Modified: Wed, 21 Dec 2022 17:35:48 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:d21936aaa13a7b4761da421bba378f0addd1aafa007454fd3d0cb63be3750ceb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:c5d58fac08a6bdf1cb8f3d91921c7a7abb7715a32807a7e25b3b5eebb7f429a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58957254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a20ca475f19e1210ad8ba2c761f769d4eb17901b78a3b03f78679db239de760`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:40:06 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 06 Oct 2022 22:40:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:40:14 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 06 Oct 2022 22:40:14 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:40:14 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:40:14 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:40:15 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 06 Oct 2022 22:40:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:40:15 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b6f6ecc6282fc9eb0bac613bb9bf9b890a3434564e38cfb98df5dae2242a86`  
		Last Modified: Thu, 06 Oct 2022 22:43:19 GMT  
		Size: 54.6 MB (54646588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d34625061a8625de99f662d174b92936f1d39b5ab61895393262420ee5f3ca4`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bf40c5860e1c71b631c1f61541dc9b7e3e6ccf415405a8a3b6d1c390ce083`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7859bec41186dc8c5c1df193da40f96d5c0baa612bb7bb5d4b9bc677beb5ea`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:5d8a14f894d50454dd27b62a219440d577c608dcc5efc3a50df19cbd74e0d52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:8c28b446691639831f01f03e3e3ae472d6cf51d41012f5e2954a4a5a3adb0fb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127793429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7d723685c97cf7eb4980deaff6605bdc0d750becb4ce3eaa702dba866cffa8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 17:00:04 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Tue, 06 Dec 2022 17:00:08 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 06 Dec 2022 17:00:08 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 06 Dec 2022 17:00:09 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 17:00:09 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 17:00:09 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 06 Dec 2022 17:00:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 06 Dec 2022 17:00:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:00:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae95131cb457a9ff37c6cc32fa694fe786421a433187e9df409879438e03ad45`  
		Last Modified: Tue, 06 Dec 2022 17:03:01 GMT  
		Size: 56.7 MB (56705082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b100dbabd0b6c04955eac9f232ac76885d708f02875c649bbf5d5ff6594b7c0c`  
		Last Modified: Tue, 06 Dec 2022 17:02:54 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b46154af8ae949bc0eba50def161dd0207094c21b61fb3689dd8c6f1880d55`  
		Last Modified: Tue, 06 Dec 2022 17:02:54 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ab112ff452ac9d0eb7ecaea0ce0a55c60fca45e6d029b72de217d14ff61a39`  
		Last Modified: Tue, 06 Dec 2022 17:02:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:7bd3639a58705b4e8a844d0031ae348220ce36add6e4cd06de72f2ecf550cd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:7c75c37bc1a924e38c6c1dfd32bc06529ae837a70f8eac0c9d20a6b4b9ad2c3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60814393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf835835b494592c58fe798cbd65be7f2098c2c7c2832d08bae5e48326fb2c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:40:20 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 06 Oct 2022 22:40:29 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:40:29 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 06 Oct 2022 22:40:29 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:40:30 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:40:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:40:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 06 Oct 2022 22:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:40:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce3f09ef3045575d0c8013e9b79575368b4854f9f960ca8ebf623845bc7c4bc`  
		Last Modified: Thu, 06 Oct 2022 22:43:38 GMT  
		Size: 56.5 MB (56503668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722ce550ab9d131d604789b351c758fbcb49c943245aca7e308df39b5699692a`  
		Last Modified: Thu, 06 Oct 2022 22:43:30 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66220e5ba00d4c40fa7c1f459663fa010dd302ffb46b3470cc651e35f9223d19`  
		Last Modified: Thu, 06 Oct 2022 22:43:30 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c327b9a7fb58412fa6ce33a8a8a5fb8d558c4d63454fd1b354a8e08977057b9`  
		Last Modified: Thu, 06 Oct 2022 22:43:30 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:107920d3821003e1c1bdbed734785a929b05ba6e2e202dccd44e954bca53b020
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:536141cb2fc369d3a3a239047bce1a8e3ce62742f3224c7c6275cbbebd69ec25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94499931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ceec4da767278293d67a5a1f4364babd005f6a8d176ea3f12e75c5f305bf5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 17:00:04 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Tue, 06 Dec 2022 17:00:17 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 06 Dec 2022 17:00:17 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 06 Dec 2022 17:00:17 GMT
EXPOSE 8091
# Tue, 06 Dec 2022 17:00:17 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 17:00:17 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 06 Dec 2022 17:00:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:00:17 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bffb67fb84c28ccc643c0f0d4cca77a82c41907cb197d7e0b39f94cbe52301`  
		Last Modified: Tue, 06 Dec 2022 17:03:16 GMT  
		Size: 23.4 MB (23412788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae5240e9f29e22b23228ba9d3b5bcc5dbaf38983b4b0eda57af1b1e61cf065f`  
		Last Modified: Tue, 06 Dec 2022 17:03:13 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd844b9be54263daf80ee9fabbd72b5b44aec54a2e7f5fbed25ecf25778b3c9`  
		Last Modified: Tue, 06 Dec 2022 17:03:13 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:e54c4cb5759595c14e3d8e9e84cf6d500951658b9cd1e5297c978e8516c73c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b0e146b30f81e6588cda723946c2e8b6feca9e6932e57a59585bf5ae43890db4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27602995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2afcdc6818b36dab0a9b82d98969c463aca2b85fd9602d1344baf017917c3c9e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:40:20 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 06 Oct 2022 22:40:39 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:40:40 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 06 Oct 2022 22:40:40 GMT
EXPOSE 8091
# Thu, 06 Oct 2022 22:40:40 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:40:40 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:40:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:40:40 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2888fe258e30ad3d0dfc4c02cb57422a39f38c6535f624bf01a9e1a9fc3215f`  
		Last Modified: Thu, 06 Oct 2022 22:43:54 GMT  
		Size: 23.3 MB (23293473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd62607efcaec46b698b09a7ab3df2c11a01512bdadef6915d63b6ff5d9cdb9`  
		Last Modified: Thu, 06 Oct 2022 22:43:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cea404d4e11d2846f9a5d3ec2b3d200462d5d41e8ac23915813eda3bb3a1fd`  
		Last Modified: Thu, 06 Oct 2022 22:43:52 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10`

```console
$ docker pull influxdb@sha256:4f1b449205ab29b56e096581227cfe7647090e1d64c8a510d6089c3bf2706ffd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:1ae78492b61983ae9331da8beb3912daf2bed91cd01f293b407f6217769085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125974042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27bb5416e7117f7e62d94057908585104c8d7bc27a31120508d044452b90e3bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 16:59:54 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 06 Dec 2022 16:59:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 06 Dec 2022 16:59:58 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 06 Dec 2022 16:59:59 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 16:59:59 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 16:59:59 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 06 Dec 2022 16:59:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 06 Dec 2022 16:59:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 16:59:59 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5644cc08aefa3a356bbfe4c5d0adc8cf1e05b360f35b477c41b6f531e0dfebe3`  
		Last Modified: Tue, 06 Dec 2022 17:02:44 GMT  
		Size: 54.9 MB (54885754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a7b585ac9d0af01da7581306c9a21de42e9f4d1cb0184ecad86b5af7859e17`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33b15a4a898166bb7b206df89a52a04214d7c89dbd8c20510084fee56c0747`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b88b55586f58a1c612ddb23a171fcd916ede7ead5f9799ee073ac889ec2d411`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:541197d04fd253cf561100aee74c750a03e5ae63591d453b353f00dc7eac9dda
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (116976209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6039cf3a99c363239215b60530c1efe67ac9678d1a36cccacbb23deb2b740db2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:30 GMT
ADD file:72eaf12ec65c98e9cde1654b6adb2b3d19f7d81c13b12801c198f699252b7503 in / 
# Tue, 06 Dec 2022 00:58:31 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:49:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:49:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 20:41:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 20:41:28 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 06 Dec 2022 20:41:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 06 Dec 2022 20:41:33 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 06 Dec 2022 20:41:33 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 20:41:34 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 20:41:34 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 06 Dec 2022 20:41:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 06 Dec 2022 20:41:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 20:41:34 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:58e27900c24f1f8f5b6b5eacbc073583f2372b58e9f5678dfe171b496b9cd71e`  
		Last Modified: Tue, 06 Dec 2022 01:05:33 GMT  
		Size: 50.2 MB (50207085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3975e0b03a66ba4371cf2cae58e77e148d952679dd5fa1e322124604805fc6a2`  
		Last Modified: Tue, 06 Dec 2022 09:59:29 GMT  
		Size: 4.9 MB (4932853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806632ddd1d79b55318482c725338dc97649f22ca0ec8dbdf79cc8be451201eb`  
		Last Modified: Tue, 06 Dec 2022 09:59:30 GMT  
		Size: 10.2 MB (10218527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2dd4bfa6e14ee8d0a05ffdef9e7ea802c2ddf6213839e03805bf83cbcf4695`  
		Last Modified: Tue, 06 Dec 2022 20:41:48 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7902dcb754540ebbcdb7f87d48069f1b6904359f71d4ab378b3674cc5e183d1e`  
		Last Modified: Tue, 06 Dec 2022 20:41:56 GMT  
		Size: 51.6 MB (51613159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1936ffba1d99c0f0496687499437956a585733f42852f7c465d9deb91907f6ff`  
		Last Modified: Tue, 06 Dec 2022 20:41:49 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc0d850537c9c29fea7407483dea5d56c78da357636fea263a1279e19072457`  
		Last Modified: Tue, 06 Dec 2022 20:41:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0cb6c0ceac97bb3d7c86dce7e493d40c49b07ee76b92b9ca71b41802a191e2`  
		Last Modified: Tue, 06 Dec 2022 20:41:48 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:2f497e0d8ad38deeff3bfb7414d8966c61d8ffaf08736598dfc364f7fd140f83
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120939739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2208cb5674e672388834c42c81e28dd508224f1370bd1433788a625440cc2ff3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:06:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 17:34:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 21 Dec 2022 17:34:19 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 21 Dec 2022 17:34:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 21 Dec 2022 17:34:23 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 21 Dec 2022 17:34:23 GMT
EXPOSE 8086
# Wed, 21 Dec 2022 17:34:23 GMT
VOLUME [/var/lib/influxdb]
# Wed, 21 Dec 2022 17:34:23 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 21 Dec 2022 17:34:23 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 21 Dec 2022 17:34:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Dec 2022 17:34:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0470f9572d03767b054118fe19e60a9c7e2510168b3a0868d9ac2953d2def5`  
		Last Modified: Wed, 21 Dec 2022 02:12:40 GMT  
		Size: 5.1 MB (5149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dfcef0545e5bca269c65c0208385c886321a1e0212977299827be5346dfea5`  
		Last Modified: Wed, 21 Dec 2022 02:12:40 GMT  
		Size: 10.9 MB (10873505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679d11cfdf518503a3a8d7aead626261fb2b7ca220c3c3dddc290b86d6d25c1e`  
		Last Modified: Wed, 21 Dec 2022 17:35:48 GMT  
		Size: 2.9 KB (2899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b872061ff402c9ef0821b6284a8475e13d4ee5b72e0e46f520245ad001cb60`  
		Last Modified: Wed, 21 Dec 2022 17:35:53 GMT  
		Size: 51.2 MB (51230051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db62c4d2794c5e6c1d825b73db01dfd972c45ea7ef17dfe97a500dd314e757fa`  
		Last Modified: Wed, 21 Dec 2022 17:35:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be5ca48085cb42c932d44d8ee475c0c746f988e1e7beddb989595317cc91ef`  
		Last Modified: Wed, 21 Dec 2022 17:35:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6483244078527630a70000ff9688d1f0b1c1b6b90fb2b64465f5acf1b7308ff`  
		Last Modified: Wed, 21 Dec 2022 17:35:48 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-alpine`

```console
$ docker pull influxdb@sha256:d21936aaa13a7b4761da421bba378f0addd1aafa007454fd3d0cb63be3750ceb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:c5d58fac08a6bdf1cb8f3d91921c7a7abb7715a32807a7e25b3b5eebb7f429a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58957254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a20ca475f19e1210ad8ba2c761f769d4eb17901b78a3b03f78679db239de760`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:40:06 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 06 Oct 2022 22:40:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:40:14 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 06 Oct 2022 22:40:14 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:40:14 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:40:14 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:40:15 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 06 Oct 2022 22:40:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:40:15 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b6f6ecc6282fc9eb0bac613bb9bf9b890a3434564e38cfb98df5dae2242a86`  
		Last Modified: Thu, 06 Oct 2022 22:43:19 GMT  
		Size: 54.6 MB (54646588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d34625061a8625de99f662d174b92936f1d39b5ab61895393262420ee5f3ca4`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bf40c5860e1c71b631c1f61541dc9b7e3e6ccf415405a8a3b6d1c390ce083`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7859bec41186dc8c5c1df193da40f96d5c0baa612bb7bb5d4b9bc677beb5ea`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data`

```console
$ docker pull influxdb@sha256:5d8a14f894d50454dd27b62a219440d577c608dcc5efc3a50df19cbd74e0d52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:8c28b446691639831f01f03e3e3ae472d6cf51d41012f5e2954a4a5a3adb0fb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127793429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7d723685c97cf7eb4980deaff6605bdc0d750becb4ce3eaa702dba866cffa8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 17:00:04 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Tue, 06 Dec 2022 17:00:08 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 06 Dec 2022 17:00:08 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 06 Dec 2022 17:00:09 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 17:00:09 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 17:00:09 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 06 Dec 2022 17:00:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 06 Dec 2022 17:00:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:00:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae95131cb457a9ff37c6cc32fa694fe786421a433187e9df409879438e03ad45`  
		Last Modified: Tue, 06 Dec 2022 17:03:01 GMT  
		Size: 56.7 MB (56705082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b100dbabd0b6c04955eac9f232ac76885d708f02875c649bbf5d5ff6594b7c0c`  
		Last Modified: Tue, 06 Dec 2022 17:02:54 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b46154af8ae949bc0eba50def161dd0207094c21b61fb3689dd8c6f1880d55`  
		Last Modified: Tue, 06 Dec 2022 17:02:54 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ab112ff452ac9d0eb7ecaea0ce0a55c60fca45e6d029b72de217d14ff61a39`  
		Last Modified: Tue, 06 Dec 2022 17:02:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data-alpine`

```console
$ docker pull influxdb@sha256:7bd3639a58705b4e8a844d0031ae348220ce36add6e4cd06de72f2ecf550cd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:7c75c37bc1a924e38c6c1dfd32bc06529ae837a70f8eac0c9d20a6b4b9ad2c3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60814393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf835835b494592c58fe798cbd65be7f2098c2c7c2832d08bae5e48326fb2c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:40:20 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 06 Oct 2022 22:40:29 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:40:29 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 06 Oct 2022 22:40:29 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:40:30 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:40:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:40:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 06 Oct 2022 22:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:40:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce3f09ef3045575d0c8013e9b79575368b4854f9f960ca8ebf623845bc7c4bc`  
		Last Modified: Thu, 06 Oct 2022 22:43:38 GMT  
		Size: 56.5 MB (56503668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722ce550ab9d131d604789b351c758fbcb49c943245aca7e308df39b5699692a`  
		Last Modified: Thu, 06 Oct 2022 22:43:30 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66220e5ba00d4c40fa7c1f459663fa010dd302ffb46b3470cc651e35f9223d19`  
		Last Modified: Thu, 06 Oct 2022 22:43:30 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c327b9a7fb58412fa6ce33a8a8a5fb8d558c4d63454fd1b354a8e08977057b9`  
		Last Modified: Thu, 06 Oct 2022 22:43:30 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta`

```console
$ docker pull influxdb@sha256:107920d3821003e1c1bdbed734785a929b05ba6e2e202dccd44e954bca53b020
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:536141cb2fc369d3a3a239047bce1a8e3ce62742f3224c7c6275cbbebd69ec25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94499931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ceec4da767278293d67a5a1f4364babd005f6a8d176ea3f12e75c5f305bf5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 17:00:04 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Tue, 06 Dec 2022 17:00:17 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 06 Dec 2022 17:00:17 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 06 Dec 2022 17:00:17 GMT
EXPOSE 8091
# Tue, 06 Dec 2022 17:00:17 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 17:00:17 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 06 Dec 2022 17:00:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:00:17 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bffb67fb84c28ccc643c0f0d4cca77a82c41907cb197d7e0b39f94cbe52301`  
		Last Modified: Tue, 06 Dec 2022 17:03:16 GMT  
		Size: 23.4 MB (23412788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae5240e9f29e22b23228ba9d3b5bcc5dbaf38983b4b0eda57af1b1e61cf065f`  
		Last Modified: Tue, 06 Dec 2022 17:03:13 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd844b9be54263daf80ee9fabbd72b5b44aec54a2e7f5fbed25ecf25778b3c9`  
		Last Modified: Tue, 06 Dec 2022 17:03:13 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta-alpine`

```console
$ docker pull influxdb@sha256:e54c4cb5759595c14e3d8e9e84cf6d500951658b9cd1e5297c978e8516c73c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b0e146b30f81e6588cda723946c2e8b6feca9e6932e57a59585bf5ae43890db4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27602995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2afcdc6818b36dab0a9b82d98969c463aca2b85fd9602d1344baf017917c3c9e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:40:20 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 06 Oct 2022 22:40:39 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:40:40 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 06 Oct 2022 22:40:40 GMT
EXPOSE 8091
# Thu, 06 Oct 2022 22:40:40 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:40:40 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:40:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:40:40 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2888fe258e30ad3d0dfc4c02cb57422a39f38c6535f624bf01a9e1a9fc3215f`  
		Last Modified: Thu, 06 Oct 2022 22:43:54 GMT  
		Size: 23.3 MB (23293473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd62607efcaec46b698b09a7ab3df2c11a01512bdadef6915d63b6ff5d9cdb9`  
		Last Modified: Thu, 06 Oct 2022 22:43:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cea404d4e11d2846f9a5d3ec2b3d200462d5d41e8ac23915813eda3bb3a1fd`  
		Last Modified: Thu, 06 Oct 2022 22:43:52 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data`

```console
$ docker pull influxdb@sha256:78857192d3685ceb31d3513bf5a13d8a1f3e9f3a8f9ab1632b58ca7e81b380e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:2d1ce119cfb9cdd0e7261c4fc713ea4087cafd2077efd052276395e01a73a569
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103944637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ede64cfd5a79bb852bcb23a9a4e0083bc0e6b4124f0cfd6b001e39aa0cf36c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 16 Dec 2022 00:22:25 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Fri, 16 Dec 2022 00:22:29 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 16 Dec 2022 00:22:30 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 16 Dec 2022 00:22:30 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:22:30 GMT
VOLUME [/var/lib/influxdb]
# Fri, 16 Dec 2022 00:22:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:22:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 16 Dec 2022 00:22:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:22:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd7874fa5cb5583e8df1e9d0136d838954a698b1959076cc3f521e33f6244f4`  
		Last Modified: Fri, 16 Dec 2022 00:24:37 GMT  
		Size: 32.9 MB (32856291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a7dff4376ffc102e2af2e48a50995b01a03a62afe852551053785cabea8043`  
		Last Modified: Fri, 16 Dec 2022 00:24:32 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968f463bc2fa0b52558e9c70fe66abef6b96babb902b9eec5c7a17b861d1a2d9`  
		Last Modified: Fri, 16 Dec 2022 00:24:32 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726fa617d426ea1fa97cab5c3387c5cf1c1602a52fbb36d21007a40c48e5d075`  
		Last Modified: Fri, 16 Dec 2022 00:24:32 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:655cadea047c1146021e421ebe9175502df66343e897722b91e341f5b6091973
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:27a546fe7a55069535d05c679bc805db3b4affaec603ad54fa9659c962878397
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37123145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8f0d6966cdc4632a2377a230097d2b3625259923f50cbc8258b6a6da2956f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 16 Dec 2022 00:22:33 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Fri, 16 Dec 2022 00:22:40 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 16 Dec 2022 00:22:40 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 16 Dec 2022 00:22:40 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:22:40 GMT
VOLUME [/var/lib/influxdb]
# Fri, 16 Dec 2022 00:22:40 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:22:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 16 Dec 2022 00:22:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:22:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d467f271b203363214b4c57ec4bc37f9775f93df69162287ba068cc15e4c8bb`  
		Last Modified: Fri, 16 Dec 2022 00:24:51 GMT  
		Size: 32.8 MB (32812421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f673ffc3ec79e7c63e11213fbac973c119c3e92b48ffd4b492c1d0ce18bfe58`  
		Last Modified: Fri, 16 Dec 2022 00:24:45 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc19480d99cdb683f69ac99b3316a48274773156ddfc6a53702277749a24aba`  
		Last Modified: Fri, 16 Dec 2022 00:24:45 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a511f7e6c07ae78e6db5b768719fc5b468e9fa98ddf1bb26db3261fba06d54`  
		Last Modified: Fri, 16 Dec 2022 00:24:46 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:8faed92e929e64f4e866e47a561e3c8a2935ce4aac88665733396217edd635e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:8a357f8eca30dbd35a8f984973b0bdaf450d87e98ba5e7d81635988439256460
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83507084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e68e9dc630130875f4723fa61979ca7ab98c744d9aabef11fa126ef4976448`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 16 Dec 2022 00:22:25 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Fri, 16 Dec 2022 00:22:46 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 16 Dec 2022 00:22:46 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 16 Dec 2022 00:22:46 GMT
EXPOSE 8091
# Fri, 16 Dec 2022 00:22:46 GMT
VOLUME [/var/lib/influxdb]
# Fri, 16 Dec 2022 00:22:46 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:22:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:22:47 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cea1687f37f9da4a1cfb45c3d9a60f93a2d0294880f7173733c6696499d6d3`  
		Last Modified: Fri, 16 Dec 2022 00:25:01 GMT  
		Size: 12.4 MB (12419942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ab8b4aeac1ef1d5fa903aac0d8719d08153bd0c660024a66382049e4587a9b`  
		Last Modified: Fri, 16 Dec 2022 00:24:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a4ecf77369ebd0b4e6fe33762b4af1be7b3c4766e2b807575848ebd25a0bbf`  
		Last Modified: Fri, 16 Dec 2022 00:24:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:01581f6f426315f15fc795b7d39add74445cd4088ab753ba4a7852049fc6123c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f41d09f5e79a051ba032e03e18538ee005b5cb661b36cfc828c8cbc8b8f32afb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.7 MB (16691582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45530fd2894d8b981bef0867b213c39cb177d8cd2bdf9e4e04fdcd68ceea819b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 16 Dec 2022 00:22:33 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Fri, 16 Dec 2022 00:22:54 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 16 Dec 2022 00:22:54 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 16 Dec 2022 00:22:54 GMT
EXPOSE 8091
# Fri, 16 Dec 2022 00:22:54 GMT
VOLUME [/var/lib/influxdb]
# Fri, 16 Dec 2022 00:22:54 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:22:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:22:54 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28187feeb066451be3107428783a9426a129c4632918ab4771fac47a005473d2`  
		Last Modified: Fri, 16 Dec 2022 00:25:11 GMT  
		Size: 12.4 MB (12382062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e813ed160996960a9d2e7a216ec670175998d8b8130898d12fbbb434ab1a487`  
		Last Modified: Fri, 16 Dec 2022 00:25:09 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ea000fb94781b2f19b5e368f2debc78e45965845ce207a35460e15cfea1708`  
		Last Modified: Fri, 16 Dec 2022 00:25:09 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.8-data`

```console
$ docker pull influxdb@sha256:78857192d3685ceb31d3513bf5a13d8a1f3e9f3a8f9ab1632b58ca7e81b380e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:2d1ce119cfb9cdd0e7261c4fc713ea4087cafd2077efd052276395e01a73a569
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103944637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ede64cfd5a79bb852bcb23a9a4e0083bc0e6b4124f0cfd6b001e39aa0cf36c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 16 Dec 2022 00:22:25 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Fri, 16 Dec 2022 00:22:29 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 16 Dec 2022 00:22:30 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 16 Dec 2022 00:22:30 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:22:30 GMT
VOLUME [/var/lib/influxdb]
# Fri, 16 Dec 2022 00:22:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:22:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 16 Dec 2022 00:22:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:22:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd7874fa5cb5583e8df1e9d0136d838954a698b1959076cc3f521e33f6244f4`  
		Last Modified: Fri, 16 Dec 2022 00:24:37 GMT  
		Size: 32.9 MB (32856291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a7dff4376ffc102e2af2e48a50995b01a03a62afe852551053785cabea8043`  
		Last Modified: Fri, 16 Dec 2022 00:24:32 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968f463bc2fa0b52558e9c70fe66abef6b96babb902b9eec5c7a17b861d1a2d9`  
		Last Modified: Fri, 16 Dec 2022 00:24:32 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726fa617d426ea1fa97cab5c3387c5cf1c1602a52fbb36d21007a40c48e5d075`  
		Last Modified: Fri, 16 Dec 2022 00:24:32 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.8-data-alpine`

```console
$ docker pull influxdb@sha256:655cadea047c1146021e421ebe9175502df66343e897722b91e341f5b6091973
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:27a546fe7a55069535d05c679bc805db3b4affaec603ad54fa9659c962878397
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37123145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8f0d6966cdc4632a2377a230097d2b3625259923f50cbc8258b6a6da2956f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 16 Dec 2022 00:22:33 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Fri, 16 Dec 2022 00:22:40 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 16 Dec 2022 00:22:40 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 16 Dec 2022 00:22:40 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:22:40 GMT
VOLUME [/var/lib/influxdb]
# Fri, 16 Dec 2022 00:22:40 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:22:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 16 Dec 2022 00:22:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:22:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d467f271b203363214b4c57ec4bc37f9775f93df69162287ba068cc15e4c8bb`  
		Last Modified: Fri, 16 Dec 2022 00:24:51 GMT  
		Size: 32.8 MB (32812421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f673ffc3ec79e7c63e11213fbac973c119c3e92b48ffd4b492c1d0ce18bfe58`  
		Last Modified: Fri, 16 Dec 2022 00:24:45 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc19480d99cdb683f69ac99b3316a48274773156ddfc6a53702277749a24aba`  
		Last Modified: Fri, 16 Dec 2022 00:24:45 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a511f7e6c07ae78e6db5b768719fc5b468e9fa98ddf1bb26db3261fba06d54`  
		Last Modified: Fri, 16 Dec 2022 00:24:46 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.8-meta`

```console
$ docker pull influxdb@sha256:8faed92e929e64f4e866e47a561e3c8a2935ce4aac88665733396217edd635e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:8a357f8eca30dbd35a8f984973b0bdaf450d87e98ba5e7d81635988439256460
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83507084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e68e9dc630130875f4723fa61979ca7ab98c744d9aabef11fa126ef4976448`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 16 Dec 2022 00:22:25 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Fri, 16 Dec 2022 00:22:46 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 16 Dec 2022 00:22:46 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 16 Dec 2022 00:22:46 GMT
EXPOSE 8091
# Fri, 16 Dec 2022 00:22:46 GMT
VOLUME [/var/lib/influxdb]
# Fri, 16 Dec 2022 00:22:46 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:22:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:22:47 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cea1687f37f9da4a1cfb45c3d9a60f93a2d0294880f7173733c6696499d6d3`  
		Last Modified: Fri, 16 Dec 2022 00:25:01 GMT  
		Size: 12.4 MB (12419942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ab8b4aeac1ef1d5fa903aac0d8719d08153bd0c660024a66382049e4587a9b`  
		Last Modified: Fri, 16 Dec 2022 00:24:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a4ecf77369ebd0b4e6fe33762b4af1be7b3c4766e2b807575848ebd25a0bbf`  
		Last Modified: Fri, 16 Dec 2022 00:24:59 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.8-meta-alpine`

```console
$ docker pull influxdb@sha256:01581f6f426315f15fc795b7d39add74445cd4088ab753ba4a7852049fc6123c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f41d09f5e79a051ba032e03e18538ee005b5cb661b36cfc828c8cbc8b8f32afb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.7 MB (16691582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45530fd2894d8b981bef0867b213c39cb177d8cd2bdf9e4e04fdcd68ceea819b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 16 Dec 2022 00:22:33 GMT
ENV INFLUXDB_VERSION=1.9.9-c1.9.9
# Fri, 16 Dec 2022 00:22:54 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 16 Dec 2022 00:22:54 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 16 Dec 2022 00:22:54 GMT
EXPOSE 8091
# Fri, 16 Dec 2022 00:22:54 GMT
VOLUME [/var/lib/influxdb]
# Fri, 16 Dec 2022 00:22:54 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:22:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:22:54 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28187feeb066451be3107428783a9426a129c4632918ab4771fac47a005473d2`  
		Last Modified: Fri, 16 Dec 2022 00:25:11 GMT  
		Size: 12.4 MB (12382062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e813ed160996960a9d2e7a216ec670175998d8b8130898d12fbbb434ab1a487`  
		Last Modified: Fri, 16 Dec 2022 00:25:09 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ea000fb94781b2f19b5e368f2debc78e45965845ce207a35460e15cfea1708`  
		Last Modified: Fri, 16 Dec 2022 00:25:09 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.4`

```console
$ docker pull influxdb@sha256:45b36d6c66e5f07f4bec488f2509b1807e7f6865f707af9940e4830a7f208f94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.4` - linux; amd64

```console
$ docker pull influxdb@sha256:194424d7bb799a751cd52233d284a4d10d55c05349368cdd31bf98c017204573
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261151241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0dd8df80c869f2f2fc9cce5cd079eaef2b28423c9f59e330ed6e0ba2aada10f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:05 GMT
ADD file:00d8a84de32d523b936621886a10683664f38d8ec0846a60511fcf3a99d0e0c4 in / 
# Tue, 06 Dec 2022 01:21:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:15:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:15:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 17:00:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 06 Dec 2022 17:00:55 GMT
ENV GOSU_VER=1.12
# Tue, 06 Dec 2022 17:00:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 06 Dec 2022 17:01:20 GMT
ENV INFLUXDB_VERSION=2.4.0
# Tue, 06 Dec 2022 17:01:27 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 06 Dec 2022 17:01:28 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Tue, 06 Dec 2022 17:01:31 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 06 Dec 2022 17:01:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 06 Dec 2022 17:01:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 06 Dec 2022 17:01:32 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 06 Dec 2022 17:01:32 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Tue, 06 Dec 2022 17:01:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:01:32 GMT
CMD ["influxd"]
# Tue, 06 Dec 2022 17:01:32 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 17:01:33 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 06 Dec 2022 17:01:33 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 06 Dec 2022 17:01:33 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 06 Dec 2022 17:01:33 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0`  
		Last Modified: Tue, 06 Dec 2022 01:25:30 GMT  
		Size: 50.4 MB (50448865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae29f309a72482bf13fbb1a8f4889ab9107fcad0c9fda76586aa55445e93ded`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 7.9 MB (7859378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fca74d99b6532401bfe63d36e1bafb1ac839564d48aa4e6e0a6aa2706a4d12`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 10.0 MB (10001409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f72f7239d05382f875123b7701a9b8f046e57991ac382e3600cae19898be9ab`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b452aa99faf6a110eb189f03d75e819e130542d88549ff9683b32a72f9c1be1`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 961.0 KB (960955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3e4c89f0f3d3cf1146234582919382db2d1571e69b6eb4d8dd2b088ac2b797`  
		Last Modified: Tue, 06 Dec 2022 17:04:56 GMT  
		Size: 185.8 MB (185802095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180ffd28324d2d024fd4fcfd4f30129955f77d304dde43ff7b8fb2b9d2950d72`  
		Last Modified: Tue, 06 Dec 2022 17:04:43 GMT  
		Size: 6.1 MB (6071067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f911df179c6bb988ac6b94bc98d0e66e397b40241406fa4f37e2281b0aa6f3f5`  
		Last Modified: Tue, 06 Dec 2022 17:04:42 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6c2206cee4a34a15707e5fde7df2788ea8a1301c02bda7cbc8b4f815555c71`  
		Last Modified: Tue, 06 Dec 2022 17:04:42 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1e7082f1791c48ad648fb47dc055735c0138783e39a3534ccd2832104b8265`  
		Last Modified: Tue, 06 Dec 2022 17:04:42 GMT  
		Size: 5.1 KB (5131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.4` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4494ea1788c63f5bc7514ebcd52dbec9543d05c6f9b6fbdfc2640f48b19aef73
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255914566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712d5f56dc865367dc6994db5a09be6ac8170951ebe13ebe35f7b934f31b180c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:07:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 17:34:26 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 21 Dec 2022 17:34:26 GMT
ENV GOSU_VER=1.12
# Wed, 21 Dec 2022 17:34:30 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 21 Dec 2022 17:34:30 GMT
ENV INFLUXDB_VERSION=2.4.0
# Wed, 21 Dec 2022 17:34:38 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 21 Dec 2022 17:34:39 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Wed, 21 Dec 2022 17:34:43 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 21 Dec 2022 17:34:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 21 Dec 2022 17:34:44 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 21 Dec 2022 17:34:44 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 21 Dec 2022 17:34:44 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 21 Dec 2022 17:34:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Dec 2022 17:34:44 GMT
CMD ["influxd"]
# Wed, 21 Dec 2022 17:34:44 GMT
EXPOSE 8086
# Wed, 21 Dec 2022 17:34:44 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 21 Dec 2022 17:34:44 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 21 Dec 2022 17:34:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 21 Dec 2022 17:34:44 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2a650584f22c4b0b1ceb1f2afaa0462e3ae41ecb07c7cb82d338e99fc3a9e5`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 7.7 MB (7727254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4859d8b8d8b84e5f11d435628f9c17fbbf42bab8f1e960e9142d545c44a21c`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 10.0 MB (10003411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736da873ef8a7fcc9dbfebb96b5dc7a5b87635d6ba768c0e82074b4f88382c76`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d21b0febed14257c2a26f14a554e1f6dd6c25e80c9cce7fe4b2e82b6168ef9`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40db7781563154fb84c04c5a83a569918fcfcf77a25a48ab165584bc27fc6420`  
		Last Modified: Wed, 21 Dec 2022 17:36:12 GMT  
		Size: 182.4 MB (182445555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33e466ecc111a6dcc0bb32a2aede550b5a2bb9b9115d227545b5cf425f12aaa`  
		Last Modified: Wed, 21 Dec 2022 17:36:03 GMT  
		Size: 5.6 MB (5600702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5775e58af89ba9879c88f48c7477a6df30c0f1e5b3ac5422edf9504a56656682`  
		Last Modified: Wed, 21 Dec 2022 17:36:02 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed98ad2c99bc85357e7d538424756bfce12d5ada8f705e25bbfaea8fb9bd3c3e`  
		Last Modified: Wed, 21 Dec 2022 17:36:02 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e050400a6ae53d7f4280804524b5c8864a907e9063bdd55d9904f9f48b1b89`  
		Last Modified: Wed, 21 Dec 2022 17:36:02 GMT  
		Size: 5.1 KB (5129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.4-alpine`

```console
$ docker pull influxdb@sha256:13938205edd25c78f6450013018c86a4e1fe559a1ad42dbfe2e450c84fc7c1c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.4-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:75ffbf7f6d7ac8ff0c5cc9a79841171592f12cc8700c06f6d69a4aa328849a18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.6 MB (204556973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163f83b4e78480834ba7ca1a67f22aecbbe4eda0b5f826e185334d4d00ad13ef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:41:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 06 Oct 2022 22:41:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 06 Oct 2022 22:42:10 GMT
ENV INFLUXDB_VERSION=2.4.0
# Thu, 06 Oct 2022 22:42:18 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 06 Oct 2022 22:42:19 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Thu, 06 Oct 2022 22:42:22 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 06 Oct 2022 22:42:23 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 06 Oct 2022 22:42:23 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 06 Oct 2022 22:42:23 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 06 Oct 2022 22:42:23 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:42:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:42:23 GMT
CMD ["influxd"]
# Thu, 06 Oct 2022 22:42:23 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:42:23 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 06 Oct 2022 22:42:23 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 06 Oct 2022 22:42:23 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 06 Oct 2022 22:42:24 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46acce005ff6ed730110484cb17e875a1911ffa2be93390133229983acda92ae`  
		Last Modified: Thu, 06 Oct 2022 22:45:07 GMT  
		Size: 9.8 MB (9849353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d46d699caad9f4c3d02e96eb23fe812a5fe94e056d9d00855e190bc4d259fd`  
		Last Modified: Thu, 06 Oct 2022 22:45:05 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3444c163ae388172e02d25763a9b92d1315f19b062f696551ee5f2b443d92a2b`  
		Last Modified: Thu, 06 Oct 2022 22:45:59 GMT  
		Size: 185.8 MB (185802064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204f61998572be91af42495de244b81a1d9a9096d4445fc7f39a540c9d7d5b65`  
		Last Modified: Thu, 06 Oct 2022 22:45:46 GMT  
		Size: 6.1 MB (6071087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1807fc7dfb4a3a92677b8bdcb2c10e30ce2916a94bb17a585afef03b3c47bb82`  
		Last Modified: Thu, 06 Oct 2022 22:45:45 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed75f252c42d8110db798cf0a4adb1ece010f6f54bb6aacf6a7af2634c04268`  
		Last Modified: Thu, 06 Oct 2022 22:45:45 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543eefad640e8f36b7ee14b1296d74581c943ea04d2f1649f3a57768ab5ee1`  
		Last Modified: Thu, 06 Oct 2022 22:45:45 GMT  
		Size: 5.0 KB (5018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.4-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:5b7debfa1302861f167d9c8c337b2cda61b8d3cbf9624e83d037d057de0f9e8d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200450887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c660638720d949f8c74c2e1eefd8a240578a98310ac2d0652a01aae24b1e50f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:47:19 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:47:21 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 10 Nov 2022 21:47:22 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 10 Nov 2022 21:47:44 GMT
ENV INFLUXDB_VERSION=2.4.0
# Thu, 10 Nov 2022 21:47:54 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 10 Nov 2022 21:47:56 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Thu, 10 Nov 2022 21:48:00 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 10 Nov 2022 21:48:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 10 Nov 2022 21:48:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 10 Nov 2022 21:48:01 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 10 Nov 2022 21:48:01 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 10 Nov 2022 21:48:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 10 Nov 2022 21:48:01 GMT
CMD ["influxd"]
# Thu, 10 Nov 2022 21:48:01 GMT
EXPOSE 8086
# Thu, 10 Nov 2022 21:48:01 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 10 Nov 2022 21:48:01 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 10 Nov 2022 21:48:01 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 10 Nov 2022 21:48:01 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dfdc2937073725a58668c13be29b74424cf00be3343640f2a18d1d635615b7`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af93c77cab7bd0584810da0a49358603ff93f64ca58734dc4bb8bdaa864ab92`  
		Last Modified: Thu, 10 Nov 2022 21:48:46 GMT  
		Size: 9.7 MB (9675488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df95e7c08d5f4b61b31e8ce0b013a6f0be89098373306dcac7dfcd5034e73a7d`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28beb875b1b32c624d137d1b4f96f156be1617d81c566aa2e9e5b3af14284d7a`  
		Last Modified: Thu, 10 Nov 2022 21:49:14 GMT  
		Size: 182.4 MB (182445564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98925098435f5f063cc7893d1de29b014f21cf260bad0c2a46e3c8338a873812`  
		Last Modified: Thu, 10 Nov 2022 21:49:05 GMT  
		Size: 5.6 MB (5600706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b912876ab2d7e4cff86e572adc9243480b8ec1818662d96ab8bea6f0260b94`  
		Last Modified: Thu, 10 Nov 2022 21:49:04 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbda8e44cfc02a502ec49be530ba1cd9d195d8a7e71d479568eebad4e8fb2cc`  
		Last Modified: Thu, 10 Nov 2022 21:49:04 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a22b72bf86a33b660d7b94830ba4b1ebe0dd5bd92fa804772f2868df81c62c7`  
		Last Modified: Thu, 10 Nov 2022 21:49:04 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.4.0`

```console
$ docker pull influxdb@sha256:45b36d6c66e5f07f4bec488f2509b1807e7f6865f707af9940e4830a7f208f94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.4.0` - linux; amd64

```console
$ docker pull influxdb@sha256:194424d7bb799a751cd52233d284a4d10d55c05349368cdd31bf98c017204573
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261151241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0dd8df80c869f2f2fc9cce5cd079eaef2b28423c9f59e330ed6e0ba2aada10f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:05 GMT
ADD file:00d8a84de32d523b936621886a10683664f38d8ec0846a60511fcf3a99d0e0c4 in / 
# Tue, 06 Dec 2022 01:21:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:15:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:15:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 17:00:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 06 Dec 2022 17:00:55 GMT
ENV GOSU_VER=1.12
# Tue, 06 Dec 2022 17:00:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 06 Dec 2022 17:01:20 GMT
ENV INFLUXDB_VERSION=2.4.0
# Tue, 06 Dec 2022 17:01:27 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 06 Dec 2022 17:01:28 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Tue, 06 Dec 2022 17:01:31 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 06 Dec 2022 17:01:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 06 Dec 2022 17:01:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 06 Dec 2022 17:01:32 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 06 Dec 2022 17:01:32 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Tue, 06 Dec 2022 17:01:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:01:32 GMT
CMD ["influxd"]
# Tue, 06 Dec 2022 17:01:32 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 17:01:33 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 06 Dec 2022 17:01:33 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 06 Dec 2022 17:01:33 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 06 Dec 2022 17:01:33 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0`  
		Last Modified: Tue, 06 Dec 2022 01:25:30 GMT  
		Size: 50.4 MB (50448865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae29f309a72482bf13fbb1a8f4889ab9107fcad0c9fda76586aa55445e93ded`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 7.9 MB (7859378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fca74d99b6532401bfe63d36e1bafb1ac839564d48aa4e6e0a6aa2706a4d12`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 10.0 MB (10001409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f72f7239d05382f875123b7701a9b8f046e57991ac382e3600cae19898be9ab`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b452aa99faf6a110eb189f03d75e819e130542d88549ff9683b32a72f9c1be1`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 961.0 KB (960955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3e4c89f0f3d3cf1146234582919382db2d1571e69b6eb4d8dd2b088ac2b797`  
		Last Modified: Tue, 06 Dec 2022 17:04:56 GMT  
		Size: 185.8 MB (185802095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180ffd28324d2d024fd4fcfd4f30129955f77d304dde43ff7b8fb2b9d2950d72`  
		Last Modified: Tue, 06 Dec 2022 17:04:43 GMT  
		Size: 6.1 MB (6071067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f911df179c6bb988ac6b94bc98d0e66e397b40241406fa4f37e2281b0aa6f3f5`  
		Last Modified: Tue, 06 Dec 2022 17:04:42 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6c2206cee4a34a15707e5fde7df2788ea8a1301c02bda7cbc8b4f815555c71`  
		Last Modified: Tue, 06 Dec 2022 17:04:42 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1e7082f1791c48ad648fb47dc055735c0138783e39a3534ccd2832104b8265`  
		Last Modified: Tue, 06 Dec 2022 17:04:42 GMT  
		Size: 5.1 KB (5131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.4.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4494ea1788c63f5bc7514ebcd52dbec9543d05c6f9b6fbdfc2640f48b19aef73
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255914566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712d5f56dc865367dc6994db5a09be6ac8170951ebe13ebe35f7b934f31b180c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:07:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 17:34:26 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 21 Dec 2022 17:34:26 GMT
ENV GOSU_VER=1.12
# Wed, 21 Dec 2022 17:34:30 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 21 Dec 2022 17:34:30 GMT
ENV INFLUXDB_VERSION=2.4.0
# Wed, 21 Dec 2022 17:34:38 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 21 Dec 2022 17:34:39 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Wed, 21 Dec 2022 17:34:43 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 21 Dec 2022 17:34:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 21 Dec 2022 17:34:44 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 21 Dec 2022 17:34:44 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 21 Dec 2022 17:34:44 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 21 Dec 2022 17:34:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Dec 2022 17:34:44 GMT
CMD ["influxd"]
# Wed, 21 Dec 2022 17:34:44 GMT
EXPOSE 8086
# Wed, 21 Dec 2022 17:34:44 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 21 Dec 2022 17:34:44 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 21 Dec 2022 17:34:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 21 Dec 2022 17:34:44 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2a650584f22c4b0b1ceb1f2afaa0462e3ae41ecb07c7cb82d338e99fc3a9e5`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 7.7 MB (7727254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4859d8b8d8b84e5f11d435628f9c17fbbf42bab8f1e960e9142d545c44a21c`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 10.0 MB (10003411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736da873ef8a7fcc9dbfebb96b5dc7a5b87635d6ba768c0e82074b4f88382c76`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d21b0febed14257c2a26f14a554e1f6dd6c25e80c9cce7fe4b2e82b6168ef9`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40db7781563154fb84c04c5a83a569918fcfcf77a25a48ab165584bc27fc6420`  
		Last Modified: Wed, 21 Dec 2022 17:36:12 GMT  
		Size: 182.4 MB (182445555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33e466ecc111a6dcc0bb32a2aede550b5a2bb9b9115d227545b5cf425f12aaa`  
		Last Modified: Wed, 21 Dec 2022 17:36:03 GMT  
		Size: 5.6 MB (5600702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5775e58af89ba9879c88f48c7477a6df30c0f1e5b3ac5422edf9504a56656682`  
		Last Modified: Wed, 21 Dec 2022 17:36:02 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed98ad2c99bc85357e7d538424756bfce12d5ada8f705e25bbfaea8fb9bd3c3e`  
		Last Modified: Wed, 21 Dec 2022 17:36:02 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e050400a6ae53d7f4280804524b5c8864a907e9063bdd55d9904f9f48b1b89`  
		Last Modified: Wed, 21 Dec 2022 17:36:02 GMT  
		Size: 5.1 KB (5129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.4.0-alpine`

```console
$ docker pull influxdb@sha256:13938205edd25c78f6450013018c86a4e1fe559a1ad42dbfe2e450c84fc7c1c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.4.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:75ffbf7f6d7ac8ff0c5cc9a79841171592f12cc8700c06f6d69a4aa328849a18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.6 MB (204556973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163f83b4e78480834ba7ca1a67f22aecbbe4eda0b5f826e185334d4d00ad13ef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:41:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 06 Oct 2022 22:41:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 06 Oct 2022 22:42:10 GMT
ENV INFLUXDB_VERSION=2.4.0
# Thu, 06 Oct 2022 22:42:18 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 06 Oct 2022 22:42:19 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Thu, 06 Oct 2022 22:42:22 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 06 Oct 2022 22:42:23 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 06 Oct 2022 22:42:23 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 06 Oct 2022 22:42:23 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 06 Oct 2022 22:42:23 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:42:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:42:23 GMT
CMD ["influxd"]
# Thu, 06 Oct 2022 22:42:23 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:42:23 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 06 Oct 2022 22:42:23 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 06 Oct 2022 22:42:23 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 06 Oct 2022 22:42:24 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46acce005ff6ed730110484cb17e875a1911ffa2be93390133229983acda92ae`  
		Last Modified: Thu, 06 Oct 2022 22:45:07 GMT  
		Size: 9.8 MB (9849353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d46d699caad9f4c3d02e96eb23fe812a5fe94e056d9d00855e190bc4d259fd`  
		Last Modified: Thu, 06 Oct 2022 22:45:05 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3444c163ae388172e02d25763a9b92d1315f19b062f696551ee5f2b443d92a2b`  
		Last Modified: Thu, 06 Oct 2022 22:45:59 GMT  
		Size: 185.8 MB (185802064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204f61998572be91af42495de244b81a1d9a9096d4445fc7f39a540c9d7d5b65`  
		Last Modified: Thu, 06 Oct 2022 22:45:46 GMT  
		Size: 6.1 MB (6071087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1807fc7dfb4a3a92677b8bdcb2c10e30ce2916a94bb17a585afef03b3c47bb82`  
		Last Modified: Thu, 06 Oct 2022 22:45:45 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed75f252c42d8110db798cf0a4adb1ece010f6f54bb6aacf6a7af2634c04268`  
		Last Modified: Thu, 06 Oct 2022 22:45:45 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543eefad640e8f36b7ee14b1296d74581c943ea04d2f1649f3a57768ab5ee1`  
		Last Modified: Thu, 06 Oct 2022 22:45:45 GMT  
		Size: 5.0 KB (5018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.4.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:5b7debfa1302861f167d9c8c337b2cda61b8d3cbf9624e83d037d057de0f9e8d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.5 MB (200450887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c660638720d949f8c74c2e1eefd8a240578a98310ac2d0652a01aae24b1e50f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:47:19 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:47:21 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 10 Nov 2022 21:47:22 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 10 Nov 2022 21:47:44 GMT
ENV INFLUXDB_VERSION=2.4.0
# Thu, 10 Nov 2022 21:47:54 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 10 Nov 2022 21:47:56 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Thu, 10 Nov 2022 21:48:00 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 10 Nov 2022 21:48:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 10 Nov 2022 21:48:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 10 Nov 2022 21:48:01 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 10 Nov 2022 21:48:01 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 10 Nov 2022 21:48:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 10 Nov 2022 21:48:01 GMT
CMD ["influxd"]
# Thu, 10 Nov 2022 21:48:01 GMT
EXPOSE 8086
# Thu, 10 Nov 2022 21:48:01 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 10 Nov 2022 21:48:01 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 10 Nov 2022 21:48:01 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 10 Nov 2022 21:48:01 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dfdc2937073725a58668c13be29b74424cf00be3343640f2a18d1d635615b7`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af93c77cab7bd0584810da0a49358603ff93f64ca58734dc4bb8bdaa864ab92`  
		Last Modified: Thu, 10 Nov 2022 21:48:46 GMT  
		Size: 9.7 MB (9675488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df95e7c08d5f4b61b31e8ce0b013a6f0be89098373306dcac7dfcd5034e73a7d`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28beb875b1b32c624d137d1b4f96f156be1617d81c566aa2e9e5b3af14284d7a`  
		Last Modified: Thu, 10 Nov 2022 21:49:14 GMT  
		Size: 182.4 MB (182445564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98925098435f5f063cc7893d1de29b014f21cf260bad0c2a46e3c8338a873812`  
		Last Modified: Thu, 10 Nov 2022 21:49:05 GMT  
		Size: 5.6 MB (5600706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b912876ab2d7e4cff86e572adc9243480b8ec1818662d96ab8bea6f0260b94`  
		Last Modified: Thu, 10 Nov 2022 21:49:04 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbda8e44cfc02a502ec49be530ba1cd9d195d8a7e71d479568eebad4e8fb2cc`  
		Last Modified: Thu, 10 Nov 2022 21:49:04 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a22b72bf86a33b660d7b94830ba4b1ebe0dd5bd92fa804772f2868df81c62c7`  
		Last Modified: Thu, 10 Nov 2022 21:49:04 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.5`

```console
$ docker pull influxdb@sha256:c7db9b3628a37330676cf6f5d9d51feb1cad948c057ce8ec7aff2c3fc5bfd7f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5` - linux; amd64

```console
$ docker pull influxdb@sha256:1ddc46d69db843cd4e0134e96a1c4e5c449ef4e577288b9e6081b5441397aee4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169818062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe394b6cd7a090cf98d2f317dea7258bc207d6e339abda2f849cfc9ca07a754`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:05 GMT
ADD file:00d8a84de32d523b936621886a10683664f38d8ec0846a60511fcf3a99d0e0c4 in / 
# Tue, 06 Dec 2022 01:21:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:15:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:15:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 17:00:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 06 Dec 2022 17:00:55 GMT
ENV GOSU_VER=1.12
# Tue, 06 Dec 2022 17:00:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 06 Dec 2022 17:01:39 GMT
ENV INFLUXDB_VERSION=2.5.1
# Tue, 06 Dec 2022 17:01:44 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 06 Dec 2022 17:01:45 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Tue, 06 Dec 2022 17:01:48 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 06 Dec 2022 17:01:49 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 06 Dec 2022 17:01:49 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 06 Dec 2022 17:01:49 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 06 Dec 2022 17:01:49 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Tue, 06 Dec 2022 17:01:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:01:50 GMT
CMD ["influxd"]
# Tue, 06 Dec 2022 17:01:50 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 17:01:50 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 06 Dec 2022 17:01:50 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 06 Dec 2022 17:01:50 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 06 Dec 2022 17:01:50 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0`  
		Last Modified: Tue, 06 Dec 2022 01:25:30 GMT  
		Size: 50.4 MB (50448865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae29f309a72482bf13fbb1a8f4889ab9107fcad0c9fda76586aa55445e93ded`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 7.9 MB (7859378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fca74d99b6532401bfe63d36e1bafb1ac839564d48aa4e6e0a6aa2706a4d12`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 10.0 MB (10001409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f72f7239d05382f875123b7701a9b8f046e57991ac382e3600cae19898be9ab`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b452aa99faf6a110eb189f03d75e819e130542d88549ff9683b32a72f9c1be1`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 961.0 KB (960955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa0322b90acec8c2511e2e9c75022912c4f2a645518009cb3601e06dc88c23f`  
		Last Modified: Tue, 06 Dec 2022 17:05:17 GMT  
		Size: 94.4 MB (94434201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4318433ceb72e6aa0e9526cd511dd70ba853e229adbc720f779c1b1947c9309d`  
		Last Modified: Tue, 06 Dec 2022 17:05:08 GMT  
		Size: 6.1 MB (6105782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5112021d11a3101fe7c2f297e4875d700918abc23e28004adab7b2a8329dfaca`  
		Last Modified: Tue, 06 Dec 2022 17:05:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b98b65612c8652c5a00886beda3fcf2152c42de07ac9ca01dd082953ced351`  
		Last Modified: Tue, 06 Dec 2022 17:05:07 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f4c3161f45255b24073c3d5b868854127360ef106f6dd649b8e4971ee87ea8`  
		Last Modified: Tue, 06 Dec 2022 17:05:07 GMT  
		Size: 5.1 KB (5130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:6cda3f0f803a5749848f846a958a4e7d1a271a7ceefe65d8882ab2c1066460d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164548602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18c5c5f2d6923b3c9786a45a0e85937f7d47d77acd868f7a401b95247a82ebb7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:07:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 17:34:26 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 21 Dec 2022 17:34:26 GMT
ENV GOSU_VER=1.12
# Wed, 21 Dec 2022 17:34:30 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 21 Dec 2022 17:34:51 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 21 Dec 2022 17:34:57 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 21 Dec 2022 17:34:58 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 21 Dec 2022 17:35:01 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 21 Dec 2022 17:35:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 21 Dec 2022 17:35:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 21 Dec 2022 17:35:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 21 Dec 2022 17:35:02 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 21 Dec 2022 17:35:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Dec 2022 17:35:02 GMT
CMD ["influxd"]
# Wed, 21 Dec 2022 17:35:02 GMT
EXPOSE 8086
# Wed, 21 Dec 2022 17:35:02 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 21 Dec 2022 17:35:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 21 Dec 2022 17:35:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 21 Dec 2022 17:35:03 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2a650584f22c4b0b1ceb1f2afaa0462e3ae41ecb07c7cb82d338e99fc3a9e5`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 7.7 MB (7727254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4859d8b8d8b84e5f11d435628f9c17fbbf42bab8f1e960e9142d545c44a21c`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 10.0 MB (10003411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736da873ef8a7fcc9dbfebb96b5dc7a5b87635d6ba768c0e82074b4f88382c76`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d21b0febed14257c2a26f14a554e1f6dd6c25e80c9cce7fe4b2e82b6168ef9`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b097931865eecdf79f6df97a734f0df7419eb30ae1eca85e846c372128ebd`  
		Last Modified: Wed, 21 Dec 2022 17:36:29 GMT  
		Size: 91.0 MB (91048398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb0d8decd104f3dc2db7b8e9a8e2c1f93c31b1fe2d300612610ebf745adbde`  
		Last Modified: Wed, 21 Dec 2022 17:36:23 GMT  
		Size: 5.6 MB (5631892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaf8d0ffd5021aa9446c8dbd05bf72c0101d895c4a5dd998232ae9145626414`  
		Last Modified: Wed, 21 Dec 2022 17:36:22 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1254a27ebf1006b4015b8abc5b02a5dfcd3230428139b07e671ba2b4675236`  
		Last Modified: Wed, 21 Dec 2022 17:36:22 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21b70aafc1acf185bdd694bb9086ef542fee786b3faa6cffe5999746f4ac9c9`  
		Last Modified: Wed, 21 Dec 2022 17:36:22 GMT  
		Size: 5.1 KB (5131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.5-alpine`

```console
$ docker pull influxdb@sha256:0cde017d9bc2e77fbb3cdc258cfdaebc2059e8aca8edac61c2f4a290a3a3bc6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:98444f55506bfce0cdaae99b0b3b99832406b5e528b0e783011b3b632bba5c06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113223812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdfeaeb516d50a7f06be060b416648e82117cce88c9526a31f892db9d6bbe140`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:41:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 06 Oct 2022 22:41:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 03 Nov 2022 18:20:45 GMT
ENV INFLUXDB_VERSION=2.5.1
# Thu, 03 Nov 2022 18:20:51 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 03 Nov 2022 18:20:52 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Thu, 03 Nov 2022 18:20:55 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 03 Nov 2022 18:20:55 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 03 Nov 2022 18:20:55 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 03 Nov 2022 18:20:56 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 03 Nov 2022 18:20:56 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 03 Nov 2022 18:20:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Nov 2022 18:20:56 GMT
CMD ["influxd"]
# Thu, 03 Nov 2022 18:20:56 GMT
EXPOSE 8086
# Thu, 03 Nov 2022 18:20:56 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 03 Nov 2022 18:20:56 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 03 Nov 2022 18:20:57 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 03 Nov 2022 18:20:57 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46acce005ff6ed730110484cb17e875a1911ffa2be93390133229983acda92ae`  
		Last Modified: Thu, 06 Oct 2022 22:45:07 GMT  
		Size: 9.8 MB (9849353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d46d699caad9f4c3d02e96eb23fe812a5fe94e056d9d00855e190bc4d259fd`  
		Last Modified: Thu, 06 Oct 2022 22:45:05 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ce778603d20c1dd4c00d95da112dc1bc7f1e716db74371d67c7f73c6180013`  
		Last Modified: Thu, 03 Nov 2022 18:22:44 GMT  
		Size: 94.4 MB (94434194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0236a91e8c3df14e1a3247b21fd414d82f9e93295b9617333c27299bc1919e3d`  
		Last Modified: Thu, 03 Nov 2022 18:22:33 GMT  
		Size: 6.1 MB (6105798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccca15e7be208ada72168e7909d215bcf8c7dde8c61fff7aafa8821f744bf13`  
		Last Modified: Thu, 03 Nov 2022 18:22:32 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1729dd46a82eb3433b20e826a6d550b744e28becba678ccbd482a642be8b56b8`  
		Last Modified: Thu, 03 Nov 2022 18:22:32 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92e991061f4c3cd206501e99c54acf40e3981716a0dabec4493f2c29286f786`  
		Last Modified: Thu, 03 Nov 2022 18:22:32 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:663a897c5b410ce0b7f965dc12c68db15787da25dd0415257c0d87cd5f1ef704
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.1 MB (109084891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a14761fd3500b0fcd3de5fddf6cce53cfd2da91f1090643a18462f6a5fe678d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:47:19 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:47:21 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 10 Nov 2022 21:47:22 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 10 Nov 2022 21:48:05 GMT
ENV INFLUXDB_VERSION=2.5.1
# Thu, 10 Nov 2022 21:48:12 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 10 Nov 2022 21:48:13 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Thu, 10 Nov 2022 21:48:17 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 10 Nov 2022 21:48:17 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 10 Nov 2022 21:48:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 10 Nov 2022 21:48:18 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 10 Nov 2022 21:48:18 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 10 Nov 2022 21:48:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 10 Nov 2022 21:48:18 GMT
CMD ["influxd"]
# Thu, 10 Nov 2022 21:48:18 GMT
EXPOSE 8086
# Thu, 10 Nov 2022 21:48:18 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 10 Nov 2022 21:48:18 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 10 Nov 2022 21:48:18 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 10 Nov 2022 21:48:18 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dfdc2937073725a58668c13be29b74424cf00be3343640f2a18d1d635615b7`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af93c77cab7bd0584810da0a49358603ff93f64ca58734dc4bb8bdaa864ab92`  
		Last Modified: Thu, 10 Nov 2022 21:48:46 GMT  
		Size: 9.7 MB (9675488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df95e7c08d5f4b61b31e8ce0b013a6f0be89098373306dcac7dfcd5034e73a7d`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd5a56b340feceb036c8a2a31285cd0d9d89a53df1d0a6e5777219d1987fb4`  
		Last Modified: Thu, 10 Nov 2022 21:49:32 GMT  
		Size: 91.0 MB (91048366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ced6843bd469064f133fa1d7415d30e28107787aca3786493c1a1b64b1f757`  
		Last Modified: Thu, 10 Nov 2022 21:49:26 GMT  
		Size: 5.6 MB (5631906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcab12af0749e1ca6c41ac9ef038b9abd85d5d12f7a1fded17f8925084ee68d2`  
		Last Modified: Thu, 10 Nov 2022 21:49:25 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995f3f7a9e107eea0d51e2e1e5f519b66091608b3fdc41ac159af3b135a296f1`  
		Last Modified: Thu, 10 Nov 2022 21:49:25 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae572fd8197d4375e9cc62e31ee9400a1afce79b8d53d285bb8354318d3e684c`  
		Last Modified: Thu, 10 Nov 2022 21:49:25 GMT  
		Size: 5.0 KB (5018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.5.1`

```console
$ docker pull influxdb@sha256:c7db9b3628a37330676cf6f5d9d51feb1cad948c057ce8ec7aff2c3fc5bfd7f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5.1` - linux; amd64

```console
$ docker pull influxdb@sha256:1ddc46d69db843cd4e0134e96a1c4e5c449ef4e577288b9e6081b5441397aee4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169818062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe394b6cd7a090cf98d2f317dea7258bc207d6e339abda2f849cfc9ca07a754`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:05 GMT
ADD file:00d8a84de32d523b936621886a10683664f38d8ec0846a60511fcf3a99d0e0c4 in / 
# Tue, 06 Dec 2022 01:21:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:15:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:15:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 17:00:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 06 Dec 2022 17:00:55 GMT
ENV GOSU_VER=1.12
# Tue, 06 Dec 2022 17:00:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 06 Dec 2022 17:01:39 GMT
ENV INFLUXDB_VERSION=2.5.1
# Tue, 06 Dec 2022 17:01:44 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 06 Dec 2022 17:01:45 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Tue, 06 Dec 2022 17:01:48 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 06 Dec 2022 17:01:49 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 06 Dec 2022 17:01:49 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 06 Dec 2022 17:01:49 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 06 Dec 2022 17:01:49 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Tue, 06 Dec 2022 17:01:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:01:50 GMT
CMD ["influxd"]
# Tue, 06 Dec 2022 17:01:50 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 17:01:50 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 06 Dec 2022 17:01:50 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 06 Dec 2022 17:01:50 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 06 Dec 2022 17:01:50 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0`  
		Last Modified: Tue, 06 Dec 2022 01:25:30 GMT  
		Size: 50.4 MB (50448865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae29f309a72482bf13fbb1a8f4889ab9107fcad0c9fda76586aa55445e93ded`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 7.9 MB (7859378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fca74d99b6532401bfe63d36e1bafb1ac839564d48aa4e6e0a6aa2706a4d12`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 10.0 MB (10001409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f72f7239d05382f875123b7701a9b8f046e57991ac382e3600cae19898be9ab`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b452aa99faf6a110eb189f03d75e819e130542d88549ff9683b32a72f9c1be1`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 961.0 KB (960955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa0322b90acec8c2511e2e9c75022912c4f2a645518009cb3601e06dc88c23f`  
		Last Modified: Tue, 06 Dec 2022 17:05:17 GMT  
		Size: 94.4 MB (94434201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4318433ceb72e6aa0e9526cd511dd70ba853e229adbc720f779c1b1947c9309d`  
		Last Modified: Tue, 06 Dec 2022 17:05:08 GMT  
		Size: 6.1 MB (6105782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5112021d11a3101fe7c2f297e4875d700918abc23e28004adab7b2a8329dfaca`  
		Last Modified: Tue, 06 Dec 2022 17:05:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b98b65612c8652c5a00886beda3fcf2152c42de07ac9ca01dd082953ced351`  
		Last Modified: Tue, 06 Dec 2022 17:05:07 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f4c3161f45255b24073c3d5b868854127360ef106f6dd649b8e4971ee87ea8`  
		Last Modified: Tue, 06 Dec 2022 17:05:07 GMT  
		Size: 5.1 KB (5130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:6cda3f0f803a5749848f846a958a4e7d1a271a7ceefe65d8882ab2c1066460d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164548602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18c5c5f2d6923b3c9786a45a0e85937f7d47d77acd868f7a401b95247a82ebb7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:07:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 17:34:26 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 21 Dec 2022 17:34:26 GMT
ENV GOSU_VER=1.12
# Wed, 21 Dec 2022 17:34:30 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 21 Dec 2022 17:34:51 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 21 Dec 2022 17:34:57 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 21 Dec 2022 17:34:58 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 21 Dec 2022 17:35:01 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 21 Dec 2022 17:35:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 21 Dec 2022 17:35:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 21 Dec 2022 17:35:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 21 Dec 2022 17:35:02 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 21 Dec 2022 17:35:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Dec 2022 17:35:02 GMT
CMD ["influxd"]
# Wed, 21 Dec 2022 17:35:02 GMT
EXPOSE 8086
# Wed, 21 Dec 2022 17:35:02 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 21 Dec 2022 17:35:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 21 Dec 2022 17:35:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 21 Dec 2022 17:35:03 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2a650584f22c4b0b1ceb1f2afaa0462e3ae41ecb07c7cb82d338e99fc3a9e5`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 7.7 MB (7727254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4859d8b8d8b84e5f11d435628f9c17fbbf42bab8f1e960e9142d545c44a21c`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 10.0 MB (10003411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736da873ef8a7fcc9dbfebb96b5dc7a5b87635d6ba768c0e82074b4f88382c76`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d21b0febed14257c2a26f14a554e1f6dd6c25e80c9cce7fe4b2e82b6168ef9`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b097931865eecdf79f6df97a734f0df7419eb30ae1eca85e846c372128ebd`  
		Last Modified: Wed, 21 Dec 2022 17:36:29 GMT  
		Size: 91.0 MB (91048398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb0d8decd104f3dc2db7b8e9a8e2c1f93c31b1fe2d300612610ebf745adbde`  
		Last Modified: Wed, 21 Dec 2022 17:36:23 GMT  
		Size: 5.6 MB (5631892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaf8d0ffd5021aa9446c8dbd05bf72c0101d895c4a5dd998232ae9145626414`  
		Last Modified: Wed, 21 Dec 2022 17:36:22 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1254a27ebf1006b4015b8abc5b02a5dfcd3230428139b07e671ba2b4675236`  
		Last Modified: Wed, 21 Dec 2022 17:36:22 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21b70aafc1acf185bdd694bb9086ef542fee786b3faa6cffe5999746f4ac9c9`  
		Last Modified: Wed, 21 Dec 2022 17:36:22 GMT  
		Size: 5.1 KB (5131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.5.1-alpine`

```console
$ docker pull influxdb@sha256:0cde017d9bc2e77fbb3cdc258cfdaebc2059e8aca8edac61c2f4a290a3a3bc6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:98444f55506bfce0cdaae99b0b3b99832406b5e528b0e783011b3b632bba5c06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113223812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdfeaeb516d50a7f06be060b416648e82117cce88c9526a31f892db9d6bbe140`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:41:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 06 Oct 2022 22:41:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 03 Nov 2022 18:20:45 GMT
ENV INFLUXDB_VERSION=2.5.1
# Thu, 03 Nov 2022 18:20:51 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 03 Nov 2022 18:20:52 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Thu, 03 Nov 2022 18:20:55 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 03 Nov 2022 18:20:55 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 03 Nov 2022 18:20:55 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 03 Nov 2022 18:20:56 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 03 Nov 2022 18:20:56 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 03 Nov 2022 18:20:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Nov 2022 18:20:56 GMT
CMD ["influxd"]
# Thu, 03 Nov 2022 18:20:56 GMT
EXPOSE 8086
# Thu, 03 Nov 2022 18:20:56 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 03 Nov 2022 18:20:56 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 03 Nov 2022 18:20:57 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 03 Nov 2022 18:20:57 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46acce005ff6ed730110484cb17e875a1911ffa2be93390133229983acda92ae`  
		Last Modified: Thu, 06 Oct 2022 22:45:07 GMT  
		Size: 9.8 MB (9849353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d46d699caad9f4c3d02e96eb23fe812a5fe94e056d9d00855e190bc4d259fd`  
		Last Modified: Thu, 06 Oct 2022 22:45:05 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ce778603d20c1dd4c00d95da112dc1bc7f1e716db74371d67c7f73c6180013`  
		Last Modified: Thu, 03 Nov 2022 18:22:44 GMT  
		Size: 94.4 MB (94434194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0236a91e8c3df14e1a3247b21fd414d82f9e93295b9617333c27299bc1919e3d`  
		Last Modified: Thu, 03 Nov 2022 18:22:33 GMT  
		Size: 6.1 MB (6105798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccca15e7be208ada72168e7909d215bcf8c7dde8c61fff7aafa8821f744bf13`  
		Last Modified: Thu, 03 Nov 2022 18:22:32 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1729dd46a82eb3433b20e826a6d550b744e28becba678ccbd482a642be8b56b8`  
		Last Modified: Thu, 03 Nov 2022 18:22:32 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92e991061f4c3cd206501e99c54acf40e3981716a0dabec4493f2c29286f786`  
		Last Modified: Thu, 03 Nov 2022 18:22:32 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:663a897c5b410ce0b7f965dc12c68db15787da25dd0415257c0d87cd5f1ef704
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.1 MB (109084891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a14761fd3500b0fcd3de5fddf6cce53cfd2da91f1090643a18462f6a5fe678d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:47:19 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:47:21 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 10 Nov 2022 21:47:22 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 10 Nov 2022 21:48:05 GMT
ENV INFLUXDB_VERSION=2.5.1
# Thu, 10 Nov 2022 21:48:12 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 10 Nov 2022 21:48:13 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Thu, 10 Nov 2022 21:48:17 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 10 Nov 2022 21:48:17 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 10 Nov 2022 21:48:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 10 Nov 2022 21:48:18 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 10 Nov 2022 21:48:18 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 10 Nov 2022 21:48:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 10 Nov 2022 21:48:18 GMT
CMD ["influxd"]
# Thu, 10 Nov 2022 21:48:18 GMT
EXPOSE 8086
# Thu, 10 Nov 2022 21:48:18 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 10 Nov 2022 21:48:18 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 10 Nov 2022 21:48:18 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 10 Nov 2022 21:48:18 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dfdc2937073725a58668c13be29b74424cf00be3343640f2a18d1d635615b7`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af93c77cab7bd0584810da0a49358603ff93f64ca58734dc4bb8bdaa864ab92`  
		Last Modified: Thu, 10 Nov 2022 21:48:46 GMT  
		Size: 9.7 MB (9675488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df95e7c08d5f4b61b31e8ce0b013a6f0be89098373306dcac7dfcd5034e73a7d`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd5a56b340feceb036c8a2a31285cd0d9d89a53df1d0a6e5777219d1987fb4`  
		Last Modified: Thu, 10 Nov 2022 21:49:32 GMT  
		Size: 91.0 MB (91048366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ced6843bd469064f133fa1d7415d30e28107787aca3786493c1a1b64b1f757`  
		Last Modified: Thu, 10 Nov 2022 21:49:26 GMT  
		Size: 5.6 MB (5631906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcab12af0749e1ca6c41ac9ef038b9abd85d5d12f7a1fded17f8925084ee68d2`  
		Last Modified: Thu, 10 Nov 2022 21:49:25 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995f3f7a9e107eea0d51e2e1e5f519b66091608b3fdc41ac159af3b135a296f1`  
		Last Modified: Thu, 10 Nov 2022 21:49:25 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae572fd8197d4375e9cc62e31ee9400a1afce79b8d53d285bb8354318d3e684c`  
		Last Modified: Thu, 10 Nov 2022 21:49:25 GMT  
		Size: 5.0 KB (5018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6`

```console
$ docker pull influxdb@sha256:6efc621cc68615b71d807e910eacc377f6f50422de79085d03add16253dcf5a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6` - linux; amd64

```console
$ docker pull influxdb@sha256:bca158ede8b68ae864b71935c518028b82a9c8802bad623cefe9df0a068ebd89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.9 MB (168874810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1c226db87e0a435f23472b152ab184acbc42350f89803efab5952494c5809e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:05 GMT
ADD file:00d8a84de32d523b936621886a10683664f38d8ec0846a60511fcf3a99d0e0c4 in / 
# Tue, 06 Dec 2022 01:21:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:15:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:15:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 17:00:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 06 Dec 2022 17:00:55 GMT
ENV GOSU_VER=1.12
# Tue, 06 Dec 2022 17:00:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Fri, 16 Dec 2022 00:23:15 GMT
ENV INFLUXDB_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:21 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 16 Dec 2022 00:23:21 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:24 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 16 Dec 2022 00:23:25 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 16 Dec 2022 00:23:25 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 16 Dec 2022 00:23:25 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 16 Dec 2022 00:23:25 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Fri, 16 Dec 2022 00:23:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:23:25 GMT
CMD ["influxd"]
# Fri, 16 Dec 2022 00:23:26 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:23:26 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 16 Dec 2022 00:23:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 16 Dec 2022 00:23:26 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 16 Dec 2022 00:23:26 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0`  
		Last Modified: Tue, 06 Dec 2022 01:25:30 GMT  
		Size: 50.4 MB (50448865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae29f309a72482bf13fbb1a8f4889ab9107fcad0c9fda76586aa55445e93ded`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 7.9 MB (7859378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fca74d99b6532401bfe63d36e1bafb1ac839564d48aa4e6e0a6aa2706a4d12`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 10.0 MB (10001409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f72f7239d05382f875123b7701a9b8f046e57991ac382e3600cae19898be9ab`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b452aa99faf6a110eb189f03d75e819e130542d88549ff9683b32a72f9c1be1`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 961.0 KB (960955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635166a7c0c120985669f335069fe29d36f8fcee4428f7fdd8ff5cdc86817957`  
		Last Modified: Fri, 16 Dec 2022 00:25:36 GMT  
		Size: 93.5 MB (93490547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8604ca7ede783db92247ea054bd3835357d16d60e0a89d07b13868ad8e8df786`  
		Last Modified: Fri, 16 Dec 2022 00:25:26 GMT  
		Size: 6.1 MB (6106184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9add9c5ef692a0519d4f8fc593c479aed010901de975280b780c2de72b885325`  
		Last Modified: Fri, 16 Dec 2022 00:25:25 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f57534d09bf184069894643dcd7e9bb6c6f9b037b97603a6157d9e160ea421`  
		Last Modified: Fri, 16 Dec 2022 00:25:25 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ca38a3cde39ecd033ca9a1fc04b7109142cd3433ddeeb2f9b317ba34d96e4f`  
		Last Modified: Fri, 16 Dec 2022 00:25:25 GMT  
		Size: 5.1 KB (5130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:dce33083b376d70d522d4c9bcacb161126e941fe2843653468c96f4cd30a5259
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.6 MB (163594927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb3e360f1d07719caa8d11b70c563218f3d1565b18c6d594ca8439d19e446a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:07:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 17:34:26 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 21 Dec 2022 17:34:26 GMT
ENV GOSU_VER=1.12
# Wed, 21 Dec 2022 17:34:30 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 21 Dec 2022 17:35:09 GMT
ENV INFLUXDB_VERSION=2.6.0
# Wed, 21 Dec 2022 17:35:19 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 21 Dec 2022 17:35:20 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Wed, 21 Dec 2022 17:35:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 21 Dec 2022 17:35:23 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 21 Dec 2022 17:35:23 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 21 Dec 2022 17:35:23 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 21 Dec 2022 17:35:23 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 21 Dec 2022 17:35:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Dec 2022 17:35:24 GMT
CMD ["influxd"]
# Wed, 21 Dec 2022 17:35:24 GMT
EXPOSE 8086
# Wed, 21 Dec 2022 17:35:24 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 21 Dec 2022 17:35:24 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 21 Dec 2022 17:35:24 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 21 Dec 2022 17:35:24 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2a650584f22c4b0b1ceb1f2afaa0462e3ae41ecb07c7cb82d338e99fc3a9e5`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 7.7 MB (7727254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4859d8b8d8b84e5f11d435628f9c17fbbf42bab8f1e960e9142d545c44a21c`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 10.0 MB (10003411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736da873ef8a7fcc9dbfebb96b5dc7a5b87635d6ba768c0e82074b4f88382c76`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d21b0febed14257c2a26f14a554e1f6dd6c25e80c9cce7fe4b2e82b6168ef9`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb8383a95195d27a08b756f8ef636b60f6b7a7ad42818e2bcef38c87c07382e`  
		Last Modified: Wed, 21 Dec 2022 17:36:45 GMT  
		Size: 90.1 MB (90094082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3ad3e99fadc31f36ea5013275c8a61db4b4b420f6876d45943ca324bf62329`  
		Last Modified: Wed, 21 Dec 2022 17:36:39 GMT  
		Size: 5.6 MB (5632535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80b883f9de0c8dcf9f162683c641295a44259e95c389fc1207a6c1ada340022`  
		Last Modified: Wed, 21 Dec 2022 17:36:38 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dffd1dd6f12ff7bccff7fdf11daa70b8682c42bb88625a0bdfd7ca8f9e887c4`  
		Last Modified: Wed, 21 Dec 2022 17:36:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65317a6e67aa8f8ad0b46fd831052cab8ef6d5cf99b30254d5fae9b1c3de7483`  
		Last Modified: Wed, 21 Dec 2022 17:36:38 GMT  
		Size: 5.1 KB (5129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6-alpine`

```console
$ docker pull influxdb@sha256:7449950f26b6a48911b2e9ca205020fbec9f5f31b880d3a3cb09f021439903d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:af27abadb0a5e58b01e58806a02aca8c46d4c2b0823d6077d13de7ade017e9a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112280552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5be9c8729a3133e803f1863821aec725d5e64235c0edf21559ea2cc65d5028be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:41:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 06 Oct 2022 22:41:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 16 Dec 2022 00:23:29 GMT
ENV INFLUXDB_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:35 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 16 Dec 2022 00:23:35 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:38 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 16 Dec 2022 00:23:39 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 16 Dec 2022 00:23:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 16 Dec 2022 00:23:39 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 16 Dec 2022 00:23:39 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:23:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:23:39 GMT
CMD ["influxd"]
# Fri, 16 Dec 2022 00:23:39 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:23:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 16 Dec 2022 00:23:40 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 16 Dec 2022 00:23:40 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 16 Dec 2022 00:23:40 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46acce005ff6ed730110484cb17e875a1911ffa2be93390133229983acda92ae`  
		Last Modified: Thu, 06 Oct 2022 22:45:07 GMT  
		Size: 9.8 MB (9849353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d46d699caad9f4c3d02e96eb23fe812a5fe94e056d9d00855e190bc4d259fd`  
		Last Modified: Thu, 06 Oct 2022 22:45:05 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973b9c614460e48bb8198b84bfa8bc5f19839094be66ac5c89acc99d9d5a483b`  
		Last Modified: Fri, 16 Dec 2022 00:25:58 GMT  
		Size: 93.5 MB (93490538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4063f2d6ed001de86dee1ce0b264f010f104e3e55e412752356f05258fafdea9`  
		Last Modified: Fri, 16 Dec 2022 00:25:48 GMT  
		Size: 6.1 MB (6106195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd72b52e28b4bf77a36de4b4e46f7201aa582f646eb004ff8b87690be7df9699`  
		Last Modified: Fri, 16 Dec 2022 00:25:47 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e24783d4ea7cc6864d852c0c6c7073969c3a21c801436a05b45402c23d9d1c0`  
		Last Modified: Fri, 16 Dec 2022 00:25:47 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b58cd1820a5b849a855f02a5bfb3ce5cf53958c9d16fccabc2ead69a88e7d4`  
		Last Modified: Fri, 16 Dec 2022 00:25:47 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a9c388606524a2ba78ed0e98e1432af0a02bbc1b32ed601c9c02be29506e848f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.1 MB (108131267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd7a9f762016c9573b382c8931b62cb9e93d782f45088561e54ae2ae0d89ae6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:47:19 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:47:21 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 10 Nov 2022 21:47:22 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 16 Dec 2022 00:44:15 GMT
ENV INFLUXDB_VERSION=2.6.0
# Fri, 16 Dec 2022 00:44:20 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 16 Dec 2022 00:44:21 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Fri, 16 Dec 2022 00:44:24 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 16 Dec 2022 00:44:24 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 16 Dec 2022 00:44:24 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 16 Dec 2022 00:44:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 16 Dec 2022 00:44:24 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:44:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:44:25 GMT
CMD ["influxd"]
# Fri, 16 Dec 2022 00:44:25 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:44:25 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 16 Dec 2022 00:44:25 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 16 Dec 2022 00:44:25 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 16 Dec 2022 00:44:25 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dfdc2937073725a58668c13be29b74424cf00be3343640f2a18d1d635615b7`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af93c77cab7bd0584810da0a49358603ff93f64ca58734dc4bb8bdaa864ab92`  
		Last Modified: Thu, 10 Nov 2022 21:48:46 GMT  
		Size: 9.7 MB (9675488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df95e7c08d5f4b61b31e8ce0b013a6f0be89098373306dcac7dfcd5034e73a7d`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3587595dae25d5ff29eb0184b6a05414961684f8929e0646771a07fc1b417`  
		Last Modified: Fri, 16 Dec 2022 00:45:18 GMT  
		Size: 90.1 MB (90094113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be43e0f034f8a66e71dfdc2efc75be12aebf682bae6baff1c2bbe8fcc0643a0`  
		Last Modified: Fri, 16 Dec 2022 00:45:11 GMT  
		Size: 5.6 MB (5632536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1174b5b5f6609d1907ed6ffd3331d8aa05ebf030eaef79d3965598e031990d`  
		Last Modified: Fri, 16 Dec 2022 00:45:10 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bd7ed476247ce1cd50e9a4f5ea4fecb24df63489d53c7f30d5c8f5e71391eb`  
		Last Modified: Fri, 16 Dec 2022 00:45:10 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b83f1d45f7ca18f99c8c7bfa68c76141af3e3cd4ff004cb3e7f38dc58938bf`  
		Last Modified: Fri, 16 Dec 2022 00:45:10 GMT  
		Size: 5.0 KB (5019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6.0`

```console
$ docker pull influxdb@sha256:6efc621cc68615b71d807e910eacc377f6f50422de79085d03add16253dcf5a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6.0` - linux; amd64

```console
$ docker pull influxdb@sha256:bca158ede8b68ae864b71935c518028b82a9c8802bad623cefe9df0a068ebd89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.9 MB (168874810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1c226db87e0a435f23472b152ab184acbc42350f89803efab5952494c5809e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:05 GMT
ADD file:00d8a84de32d523b936621886a10683664f38d8ec0846a60511fcf3a99d0e0c4 in / 
# Tue, 06 Dec 2022 01:21:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:15:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:15:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 17:00:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 06 Dec 2022 17:00:55 GMT
ENV GOSU_VER=1.12
# Tue, 06 Dec 2022 17:00:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Fri, 16 Dec 2022 00:23:15 GMT
ENV INFLUXDB_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:21 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 16 Dec 2022 00:23:21 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:24 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 16 Dec 2022 00:23:25 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 16 Dec 2022 00:23:25 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 16 Dec 2022 00:23:25 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 16 Dec 2022 00:23:25 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Fri, 16 Dec 2022 00:23:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:23:25 GMT
CMD ["influxd"]
# Fri, 16 Dec 2022 00:23:26 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:23:26 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 16 Dec 2022 00:23:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 16 Dec 2022 00:23:26 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 16 Dec 2022 00:23:26 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0`  
		Last Modified: Tue, 06 Dec 2022 01:25:30 GMT  
		Size: 50.4 MB (50448865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae29f309a72482bf13fbb1a8f4889ab9107fcad0c9fda76586aa55445e93ded`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 7.9 MB (7859378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fca74d99b6532401bfe63d36e1bafb1ac839564d48aa4e6e0a6aa2706a4d12`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 10.0 MB (10001409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f72f7239d05382f875123b7701a9b8f046e57991ac382e3600cae19898be9ab`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b452aa99faf6a110eb189f03d75e819e130542d88549ff9683b32a72f9c1be1`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 961.0 KB (960955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635166a7c0c120985669f335069fe29d36f8fcee4428f7fdd8ff5cdc86817957`  
		Last Modified: Fri, 16 Dec 2022 00:25:36 GMT  
		Size: 93.5 MB (93490547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8604ca7ede783db92247ea054bd3835357d16d60e0a89d07b13868ad8e8df786`  
		Last Modified: Fri, 16 Dec 2022 00:25:26 GMT  
		Size: 6.1 MB (6106184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9add9c5ef692a0519d4f8fc593c479aed010901de975280b780c2de72b885325`  
		Last Modified: Fri, 16 Dec 2022 00:25:25 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f57534d09bf184069894643dcd7e9bb6c6f9b037b97603a6157d9e160ea421`  
		Last Modified: Fri, 16 Dec 2022 00:25:25 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ca38a3cde39ecd033ca9a1fc04b7109142cd3433ddeeb2f9b317ba34d96e4f`  
		Last Modified: Fri, 16 Dec 2022 00:25:25 GMT  
		Size: 5.1 KB (5130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:dce33083b376d70d522d4c9bcacb161126e941fe2843653468c96f4cd30a5259
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.6 MB (163594927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb3e360f1d07719caa8d11b70c563218f3d1565b18c6d594ca8439d19e446a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:07:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 17:34:26 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 21 Dec 2022 17:34:26 GMT
ENV GOSU_VER=1.12
# Wed, 21 Dec 2022 17:34:30 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 21 Dec 2022 17:35:09 GMT
ENV INFLUXDB_VERSION=2.6.0
# Wed, 21 Dec 2022 17:35:19 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 21 Dec 2022 17:35:20 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Wed, 21 Dec 2022 17:35:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 21 Dec 2022 17:35:23 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 21 Dec 2022 17:35:23 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 21 Dec 2022 17:35:23 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 21 Dec 2022 17:35:23 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 21 Dec 2022 17:35:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Dec 2022 17:35:24 GMT
CMD ["influxd"]
# Wed, 21 Dec 2022 17:35:24 GMT
EXPOSE 8086
# Wed, 21 Dec 2022 17:35:24 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 21 Dec 2022 17:35:24 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 21 Dec 2022 17:35:24 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 21 Dec 2022 17:35:24 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2a650584f22c4b0b1ceb1f2afaa0462e3ae41ecb07c7cb82d338e99fc3a9e5`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 7.7 MB (7727254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4859d8b8d8b84e5f11d435628f9c17fbbf42bab8f1e960e9142d545c44a21c`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 10.0 MB (10003411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736da873ef8a7fcc9dbfebb96b5dc7a5b87635d6ba768c0e82074b4f88382c76`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d21b0febed14257c2a26f14a554e1f6dd6c25e80c9cce7fe4b2e82b6168ef9`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb8383a95195d27a08b756f8ef636b60f6b7a7ad42818e2bcef38c87c07382e`  
		Last Modified: Wed, 21 Dec 2022 17:36:45 GMT  
		Size: 90.1 MB (90094082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3ad3e99fadc31f36ea5013275c8a61db4b4b420f6876d45943ca324bf62329`  
		Last Modified: Wed, 21 Dec 2022 17:36:39 GMT  
		Size: 5.6 MB (5632535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80b883f9de0c8dcf9f162683c641295a44259e95c389fc1207a6c1ada340022`  
		Last Modified: Wed, 21 Dec 2022 17:36:38 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dffd1dd6f12ff7bccff7fdf11daa70b8682c42bb88625a0bdfd7ca8f9e887c4`  
		Last Modified: Wed, 21 Dec 2022 17:36:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65317a6e67aa8f8ad0b46fd831052cab8ef6d5cf99b30254d5fae9b1c3de7483`  
		Last Modified: Wed, 21 Dec 2022 17:36:38 GMT  
		Size: 5.1 KB (5129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.6.0-alpine`

```console
$ docker pull influxdb@sha256:7449950f26b6a48911b2e9ca205020fbec9f5f31b880d3a3cb09f021439903d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.6.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:af27abadb0a5e58b01e58806a02aca8c46d4c2b0823d6077d13de7ade017e9a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112280552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5be9c8729a3133e803f1863821aec725d5e64235c0edf21559ea2cc65d5028be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:41:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 06 Oct 2022 22:41:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 16 Dec 2022 00:23:29 GMT
ENV INFLUXDB_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:35 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 16 Dec 2022 00:23:35 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:38 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 16 Dec 2022 00:23:39 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 16 Dec 2022 00:23:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 16 Dec 2022 00:23:39 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 16 Dec 2022 00:23:39 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:23:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:23:39 GMT
CMD ["influxd"]
# Fri, 16 Dec 2022 00:23:39 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:23:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 16 Dec 2022 00:23:40 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 16 Dec 2022 00:23:40 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 16 Dec 2022 00:23:40 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46acce005ff6ed730110484cb17e875a1911ffa2be93390133229983acda92ae`  
		Last Modified: Thu, 06 Oct 2022 22:45:07 GMT  
		Size: 9.8 MB (9849353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d46d699caad9f4c3d02e96eb23fe812a5fe94e056d9d00855e190bc4d259fd`  
		Last Modified: Thu, 06 Oct 2022 22:45:05 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973b9c614460e48bb8198b84bfa8bc5f19839094be66ac5c89acc99d9d5a483b`  
		Last Modified: Fri, 16 Dec 2022 00:25:58 GMT  
		Size: 93.5 MB (93490538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4063f2d6ed001de86dee1ce0b264f010f104e3e55e412752356f05258fafdea9`  
		Last Modified: Fri, 16 Dec 2022 00:25:48 GMT  
		Size: 6.1 MB (6106195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd72b52e28b4bf77a36de4b4e46f7201aa582f646eb004ff8b87690be7df9699`  
		Last Modified: Fri, 16 Dec 2022 00:25:47 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e24783d4ea7cc6864d852c0c6c7073969c3a21c801436a05b45402c23d9d1c0`  
		Last Modified: Fri, 16 Dec 2022 00:25:47 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b58cd1820a5b849a855f02a5bfb3ce5cf53958c9d16fccabc2ead69a88e7d4`  
		Last Modified: Fri, 16 Dec 2022 00:25:47 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.6.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a9c388606524a2ba78ed0e98e1432af0a02bbc1b32ed601c9c02be29506e848f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.1 MB (108131267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd7a9f762016c9573b382c8931b62cb9e93d782f45088561e54ae2ae0d89ae6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:47:19 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:47:21 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 10 Nov 2022 21:47:22 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 16 Dec 2022 00:44:15 GMT
ENV INFLUXDB_VERSION=2.6.0
# Fri, 16 Dec 2022 00:44:20 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 16 Dec 2022 00:44:21 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Fri, 16 Dec 2022 00:44:24 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 16 Dec 2022 00:44:24 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 16 Dec 2022 00:44:24 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 16 Dec 2022 00:44:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 16 Dec 2022 00:44:24 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:44:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:44:25 GMT
CMD ["influxd"]
# Fri, 16 Dec 2022 00:44:25 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:44:25 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 16 Dec 2022 00:44:25 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 16 Dec 2022 00:44:25 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 16 Dec 2022 00:44:25 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dfdc2937073725a58668c13be29b74424cf00be3343640f2a18d1d635615b7`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af93c77cab7bd0584810da0a49358603ff93f64ca58734dc4bb8bdaa864ab92`  
		Last Modified: Thu, 10 Nov 2022 21:48:46 GMT  
		Size: 9.7 MB (9675488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df95e7c08d5f4b61b31e8ce0b013a6f0be89098373306dcac7dfcd5034e73a7d`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3587595dae25d5ff29eb0184b6a05414961684f8929e0646771a07fc1b417`  
		Last Modified: Fri, 16 Dec 2022 00:45:18 GMT  
		Size: 90.1 MB (90094113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be43e0f034f8a66e71dfdc2efc75be12aebf682bae6baff1c2bbe8fcc0643a0`  
		Last Modified: Fri, 16 Dec 2022 00:45:11 GMT  
		Size: 5.6 MB (5632536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1174b5b5f6609d1907ed6ffd3331d8aa05ebf030eaef79d3965598e031990d`  
		Last Modified: Fri, 16 Dec 2022 00:45:10 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bd7ed476247ce1cd50e9a4f5ea4fecb24df63489d53c7f30d5c8f5e71391eb`  
		Last Modified: Fri, 16 Dec 2022 00:45:10 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b83f1d45f7ca18f99c8c7bfa68c76141af3e3cd4ff004cb3e7f38dc58938bf`  
		Last Modified: Fri, 16 Dec 2022 00:45:10 GMT  
		Size: 5.0 KB (5019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:7449950f26b6a48911b2e9ca205020fbec9f5f31b880d3a3cb09f021439903d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:af27abadb0a5e58b01e58806a02aca8c46d4c2b0823d6077d13de7ade017e9a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112280552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5be9c8729a3133e803f1863821aec725d5e64235c0edf21559ea2cc65d5028be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:41:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 06 Oct 2022 22:41:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 16 Dec 2022 00:23:29 GMT
ENV INFLUXDB_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:35 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 16 Dec 2022 00:23:35 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:38 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 16 Dec 2022 00:23:39 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 16 Dec 2022 00:23:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 16 Dec 2022 00:23:39 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 16 Dec 2022 00:23:39 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:23:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:23:39 GMT
CMD ["influxd"]
# Fri, 16 Dec 2022 00:23:39 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:23:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 16 Dec 2022 00:23:40 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 16 Dec 2022 00:23:40 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 16 Dec 2022 00:23:40 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46acce005ff6ed730110484cb17e875a1911ffa2be93390133229983acda92ae`  
		Last Modified: Thu, 06 Oct 2022 22:45:07 GMT  
		Size: 9.8 MB (9849353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d46d699caad9f4c3d02e96eb23fe812a5fe94e056d9d00855e190bc4d259fd`  
		Last Modified: Thu, 06 Oct 2022 22:45:05 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973b9c614460e48bb8198b84bfa8bc5f19839094be66ac5c89acc99d9d5a483b`  
		Last Modified: Fri, 16 Dec 2022 00:25:58 GMT  
		Size: 93.5 MB (93490538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4063f2d6ed001de86dee1ce0b264f010f104e3e55e412752356f05258fafdea9`  
		Last Modified: Fri, 16 Dec 2022 00:25:48 GMT  
		Size: 6.1 MB (6106195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd72b52e28b4bf77a36de4b4e46f7201aa582f646eb004ff8b87690be7df9699`  
		Last Modified: Fri, 16 Dec 2022 00:25:47 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e24783d4ea7cc6864d852c0c6c7073969c3a21c801436a05b45402c23d9d1c0`  
		Last Modified: Fri, 16 Dec 2022 00:25:47 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b58cd1820a5b849a855f02a5bfb3ce5cf53958c9d16fccabc2ead69a88e7d4`  
		Last Modified: Fri, 16 Dec 2022 00:25:47 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a9c388606524a2ba78ed0e98e1432af0a02bbc1b32ed601c9c02be29506e848f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.1 MB (108131267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd7a9f762016c9573b382c8931b62cb9e93d782f45088561e54ae2ae0d89ae6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:47:19 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:47:21 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts su-exec &&     update-ca-certificates
# Thu, 10 Nov 2022 21:47:22 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 16 Dec 2022 00:44:15 GMT
ENV INFLUXDB_VERSION=2.6.0
# Fri, 16 Dec 2022 00:44:20 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 16 Dec 2022 00:44:21 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Fri, 16 Dec 2022 00:44:24 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 16 Dec 2022 00:44:24 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 16 Dec 2022 00:44:24 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 16 Dec 2022 00:44:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 16 Dec 2022 00:44:24 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Fri, 16 Dec 2022 00:44:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:44:25 GMT
CMD ["influxd"]
# Fri, 16 Dec 2022 00:44:25 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:44:25 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 16 Dec 2022 00:44:25 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 16 Dec 2022 00:44:25 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 16 Dec 2022 00:44:25 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dfdc2937073725a58668c13be29b74424cf00be3343640f2a18d1d635615b7`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af93c77cab7bd0584810da0a49358603ff93f64ca58734dc4bb8bdaa864ab92`  
		Last Modified: Thu, 10 Nov 2022 21:48:46 GMT  
		Size: 9.7 MB (9675488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df95e7c08d5f4b61b31e8ce0b013a6f0be89098373306dcac7dfcd5034e73a7d`  
		Last Modified: Thu, 10 Nov 2022 21:48:44 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3587595dae25d5ff29eb0184b6a05414961684f8929e0646771a07fc1b417`  
		Last Modified: Fri, 16 Dec 2022 00:45:18 GMT  
		Size: 90.1 MB (90094113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be43e0f034f8a66e71dfdc2efc75be12aebf682bae6baff1c2bbe8fcc0643a0`  
		Last Modified: Fri, 16 Dec 2022 00:45:11 GMT  
		Size: 5.6 MB (5632536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1174b5b5f6609d1907ed6ffd3331d8aa05ebf030eaef79d3965598e031990d`  
		Last Modified: Fri, 16 Dec 2022 00:45:10 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bd7ed476247ce1cd50e9a4f5ea4fecb24df63489d53c7f30d5c8f5e71391eb`  
		Last Modified: Fri, 16 Dec 2022 00:45:10 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b83f1d45f7ca18f99c8c7bfa68c76141af3e3cd4ff004cb3e7f38dc58938bf`  
		Last Modified: Fri, 16 Dec 2022 00:45:10 GMT  
		Size: 5.0 KB (5019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:5d8a14f894d50454dd27b62a219440d577c608dcc5efc3a50df19cbd74e0d52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:8c28b446691639831f01f03e3e3ae472d6cf51d41012f5e2954a4a5a3adb0fb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127793429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7d723685c97cf7eb4980deaff6605bdc0d750becb4ce3eaa702dba866cffa8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 17:00:04 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Tue, 06 Dec 2022 17:00:08 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 06 Dec 2022 17:00:08 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 06 Dec 2022 17:00:09 GMT
EXPOSE 8086
# Tue, 06 Dec 2022 17:00:09 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 17:00:09 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 06 Dec 2022 17:00:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 06 Dec 2022 17:00:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:00:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae95131cb457a9ff37c6cc32fa694fe786421a433187e9df409879438e03ad45`  
		Last Modified: Tue, 06 Dec 2022 17:03:01 GMT  
		Size: 56.7 MB (56705082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b100dbabd0b6c04955eac9f232ac76885d708f02875c649bbf5d5ff6594b7c0c`  
		Last Modified: Tue, 06 Dec 2022 17:02:54 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b46154af8ae949bc0eba50def161dd0207094c21b61fb3689dd8c6f1880d55`  
		Last Modified: Tue, 06 Dec 2022 17:02:54 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ab112ff452ac9d0eb7ecaea0ce0a55c60fca45e6d029b72de217d14ff61a39`  
		Last Modified: Tue, 06 Dec 2022 17:02:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:7bd3639a58705b4e8a844d0031ae348220ce36add6e4cd06de72f2ecf550cd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:7c75c37bc1a924e38c6c1dfd32bc06529ae837a70f8eac0c9d20a6b4b9ad2c3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60814393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf835835b494592c58fe798cbd65be7f2098c2c7c2832d08bae5e48326fb2c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:40:20 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 06 Oct 2022 22:40:29 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:40:29 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 06 Oct 2022 22:40:29 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:40:30 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:40:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:40:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 06 Oct 2022 22:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:40:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce3f09ef3045575d0c8013e9b79575368b4854f9f960ca8ebf623845bc7c4bc`  
		Last Modified: Thu, 06 Oct 2022 22:43:38 GMT  
		Size: 56.5 MB (56503668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722ce550ab9d131d604789b351c758fbcb49c943245aca7e308df39b5699692a`  
		Last Modified: Thu, 06 Oct 2022 22:43:30 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66220e5ba00d4c40fa7c1f459663fa010dd302ffb46b3470cc651e35f9223d19`  
		Last Modified: Thu, 06 Oct 2022 22:43:30 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c327b9a7fb58412fa6ce33a8a8a5fb8d558c4d63454fd1b354a8e08977057b9`  
		Last Modified: Thu, 06 Oct 2022 22:43:30 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:6efc621cc68615b71d807e910eacc377f6f50422de79085d03add16253dcf5a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:bca158ede8b68ae864b71935c518028b82a9c8802bad623cefe9df0a068ebd89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.9 MB (168874810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1c226db87e0a435f23472b152ab184acbc42350f89803efab5952494c5809e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:05 GMT
ADD file:00d8a84de32d523b936621886a10683664f38d8ec0846a60511fcf3a99d0e0c4 in / 
# Tue, 06 Dec 2022 01:21:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:15:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:15:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 17:00:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 06 Dec 2022 17:00:55 GMT
ENV GOSU_VER=1.12
# Tue, 06 Dec 2022 17:00:58 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Fri, 16 Dec 2022 00:23:15 GMT
ENV INFLUXDB_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:21 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 16 Dec 2022 00:23:21 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Fri, 16 Dec 2022 00:23:24 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 16 Dec 2022 00:23:25 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 16 Dec 2022 00:23:25 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 16 Dec 2022 00:23:25 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 16 Dec 2022 00:23:25 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Fri, 16 Dec 2022 00:23:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 00:23:25 GMT
CMD ["influxd"]
# Fri, 16 Dec 2022 00:23:26 GMT
EXPOSE 8086
# Fri, 16 Dec 2022 00:23:26 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 16 Dec 2022 00:23:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 16 Dec 2022 00:23:26 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 16 Dec 2022 00:23:26 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0`  
		Last Modified: Tue, 06 Dec 2022 01:25:30 GMT  
		Size: 50.4 MB (50448865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae29f309a72482bf13fbb1a8f4889ab9107fcad0c9fda76586aa55445e93ded`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 7.9 MB (7859378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fca74d99b6532401bfe63d36e1bafb1ac839564d48aa4e6e0a6aa2706a4d12`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 10.0 MB (10001409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f72f7239d05382f875123b7701a9b8f046e57991ac382e3600cae19898be9ab`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b452aa99faf6a110eb189f03d75e819e130542d88549ff9683b32a72f9c1be1`  
		Last Modified: Tue, 06 Dec 2022 17:04:22 GMT  
		Size: 961.0 KB (960955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635166a7c0c120985669f335069fe29d36f8fcee4428f7fdd8ff5cdc86817957`  
		Last Modified: Fri, 16 Dec 2022 00:25:36 GMT  
		Size: 93.5 MB (93490547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8604ca7ede783db92247ea054bd3835357d16d60e0a89d07b13868ad8e8df786`  
		Last Modified: Fri, 16 Dec 2022 00:25:26 GMT  
		Size: 6.1 MB (6106184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9add9c5ef692a0519d4f8fc593c479aed010901de975280b780c2de72b885325`  
		Last Modified: Fri, 16 Dec 2022 00:25:25 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f57534d09bf184069894643dcd7e9bb6c6f9b037b97603a6157d9e160ea421`  
		Last Modified: Fri, 16 Dec 2022 00:25:25 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ca38a3cde39ecd033ca9a1fc04b7109142cd3433ddeeb2f9b317ba34d96e4f`  
		Last Modified: Fri, 16 Dec 2022 00:25:25 GMT  
		Size: 5.1 KB (5130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:dce33083b376d70d522d4c9bcacb161126e941fe2843653468c96f4cd30a5259
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.6 MB (163594927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb3e360f1d07719caa8d11b70c563218f3d1565b18c6d594ca8439d19e446a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:07:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 17:34:26 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 21 Dec 2022 17:34:26 GMT
ENV GOSU_VER=1.12
# Wed, 21 Dec 2022 17:34:30 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 21 Dec 2022 17:35:09 GMT
ENV INFLUXDB_VERSION=2.6.0
# Wed, 21 Dec 2022 17:35:19 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 21 Dec 2022 17:35:20 GMT
ENV INFLUX_CLI_VERSION=2.6.0
# Wed, 21 Dec 2022 17:35:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 21 Dec 2022 17:35:23 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 21 Dec 2022 17:35:23 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 21 Dec 2022 17:35:23 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 21 Dec 2022 17:35:23 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 21 Dec 2022 17:35:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Dec 2022 17:35:24 GMT
CMD ["influxd"]
# Wed, 21 Dec 2022 17:35:24 GMT
EXPOSE 8086
# Wed, 21 Dec 2022 17:35:24 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 21 Dec 2022 17:35:24 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 21 Dec 2022 17:35:24 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 21 Dec 2022 17:35:24 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2a650584f22c4b0b1ceb1f2afaa0462e3ae41ecb07c7cb82d338e99fc3a9e5`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 7.7 MB (7727254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4859d8b8d8b84e5f11d435628f9c17fbbf42bab8f1e960e9142d545c44a21c`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 10.0 MB (10003411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736da873ef8a7fcc9dbfebb96b5dc7a5b87635d6ba768c0e82074b4f88382c76`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d21b0febed14257c2a26f14a554e1f6dd6c25e80c9cce7fe4b2e82b6168ef9`  
		Last Modified: Wed, 21 Dec 2022 17:36:04 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb8383a95195d27a08b756f8ef636b60f6b7a7ad42818e2bcef38c87c07382e`  
		Last Modified: Wed, 21 Dec 2022 17:36:45 GMT  
		Size: 90.1 MB (90094082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3ad3e99fadc31f36ea5013275c8a61db4b4b420f6876d45943ca324bf62329`  
		Last Modified: Wed, 21 Dec 2022 17:36:39 GMT  
		Size: 5.6 MB (5632535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80b883f9de0c8dcf9f162683c641295a44259e95c389fc1207a6c1ada340022`  
		Last Modified: Wed, 21 Dec 2022 17:36:38 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dffd1dd6f12ff7bccff7fdf11daa70b8682c42bb88625a0bdfd7ca8f9e887c4`  
		Last Modified: Wed, 21 Dec 2022 17:36:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65317a6e67aa8f8ad0b46fd831052cab8ef6d5cf99b30254d5fae9b1c3de7483`  
		Last Modified: Wed, 21 Dec 2022 17:36:38 GMT  
		Size: 5.1 KB (5129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:107920d3821003e1c1bdbed734785a929b05ba6e2e202dccd44e954bca53b020
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:536141cb2fc369d3a3a239047bce1a8e3ce62742f3224c7c6275cbbebd69ec25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94499931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ceec4da767278293d67a5a1f4364babd005f6a8d176ea3f12e75c5f305bf5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 16:59:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 06 Dec 2022 17:00:04 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Tue, 06 Dec 2022 17:00:17 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 06 Dec 2022 17:00:17 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 06 Dec 2022 17:00:17 GMT
EXPOSE 8091
# Tue, 06 Dec 2022 17:00:17 GMT
VOLUME [/var/lib/influxdb]
# Tue, 06 Dec 2022 17:00:17 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 06 Dec 2022 17:00:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 17:00:17 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d38c4f1653f44b974d6db545ca56dffde5e7e6f73647fa98ad4556b8b84547`  
		Last Modified: Tue, 06 Dec 2022 17:02:37 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bffb67fb84c28ccc643c0f0d4cca77a82c41907cb197d7e0b39f94cbe52301`  
		Last Modified: Tue, 06 Dec 2022 17:03:16 GMT  
		Size: 23.4 MB (23412788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae5240e9f29e22b23228ba9d3b5bcc5dbaf38983b4b0eda57af1b1e61cf065f`  
		Last Modified: Tue, 06 Dec 2022 17:03:13 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd844b9be54263daf80ee9fabbd72b5b44aec54a2e7f5fbed25ecf25778b3c9`  
		Last Modified: Tue, 06 Dec 2022 17:03:13 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:e54c4cb5759595c14e3d8e9e84cf6d500951658b9cd1e5297c978e8516c73c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b0e146b30f81e6588cda723946c2e8b6feca9e6932e57a59585bf5ae43890db4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27602995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2afcdc6818b36dab0a9b82d98969c463aca2b85fd9602d1344baf017917c3c9e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 22:40:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 22:40:20 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 06 Oct 2022 22:40:39 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:40:40 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 06 Oct 2022 22:40:40 GMT
EXPOSE 8091
# Thu, 06 Oct 2022 22:40:40 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:40:40 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:40:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:40:40 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39caa57d4803ac41d99e33b97d3a30ededc88eb971422b972f621bf32733cc`  
		Last Modified: Thu, 06 Oct 2022 22:43:12 GMT  
		Size: 1.5 MB (1481282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2888fe258e30ad3d0dfc4c02cb57422a39f38c6535f624bf01a9e1a9fc3215f`  
		Last Modified: Thu, 06 Oct 2022 22:43:54 GMT  
		Size: 23.3 MB (23293473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd62607efcaec46b698b09a7ab3df2c11a01512bdadef6915d63b6ff5d9cdb9`  
		Last Modified: Thu, 06 Oct 2022 22:43:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cea404d4e11d2846f9a5d3ec2b3d200462d5d41e8ac23915813eda3bb3a1fd`  
		Last Modified: Thu, 06 Oct 2022 22:43:52 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
