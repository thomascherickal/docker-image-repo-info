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
-	[`influxdb:2.3`](#influxdb23)
-	[`influxdb:2.3-alpine`](#influxdb23-alpine)
-	[`influxdb:2.3.0`](#influxdb230)
-	[`influxdb:2.3.0-alpine`](#influxdb230-alpine)
-	[`influxdb:2.4`](#influxdb24)
-	[`influxdb:2.4-alpine`](#influxdb24-alpine)
-	[`influxdb:2.4.0`](#influxdb240)
-	[`influxdb:2.4.0-alpine`](#influxdb240-alpine)
-	[`influxdb:2.5`](#influxdb25)
-	[`influxdb:2.5-alpine`](#influxdb25-alpine)
-	[`influxdb:2.5.1`](#influxdb251)
-	[`influxdb:2.5.1-alpine`](#influxdb251-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.10-data`

```console
$ docker pull influxdb@sha256:bc872e5625df09f82deaa136598b0e37c35e585dc929f25a99834736967c2b16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:a25c4833d481ac01ddf22cd23c055d4912bbedc9db13e267edbe6eeac4da17e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101778875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ba217229d611e12859361bdbd4d3754654eb8e05ae8d6b1dc4cc5ba4bff6a36`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:38:26 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Wed, 16 Nov 2022 03:38:29 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:38:29 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 16 Nov 2022 03:38:29 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:38:30 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:38:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:38:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 16 Nov 2022 03:38:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:38:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7da312b5df063a0b9103f9ba6c3866d916b877be64d7e852b765666b2993f5d`  
		Last Modified: Wed, 16 Nov 2022 03:42:02 GMT  
		Size: 30.7 MB (30693312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c703224cd9f7fff787704da9f65e8f5e64cea07d863da12b62d7d4393a8c1a`  
		Last Modified: Wed, 16 Nov 2022 03:41:57 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a12e64ac314770c10a22f419bf8e1c393c283feed10a2538495dded4a53e57`  
		Last Modified: Wed, 16 Nov 2022 03:41:57 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97e5b5853d4989ee1ac1c885ce69b00a6ea40905a154a29048360e686b83da9`  
		Last Modified: Wed, 16 Nov 2022 03:41:57 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:d2a2e460d093712eb44ff7d5eb146170b45e0b1bd36017777653c6f56455b04a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:b244ea89030ac046d23c602fb248e414cc980c1f685a3d1e71731a1d2f7a95d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.0 MB (82991552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8421c5fceeaf68d543c0eeadd8fb37a5dc1cc9b8274c44adee54c29608bb14a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:38:26 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Wed, 16 Nov 2022 03:38:37 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:38:38 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 16 Nov 2022 03:38:38 GMT
EXPOSE 8091
# Wed, 16 Nov 2022 03:38:38 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:38:38 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:38:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:38:38 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714e248afd352d0861b7d4384114cff6e05cabebc6690a712c660fb346bff0e6`  
		Last Modified: Wed, 16 Nov 2022 03:42:14 GMT  
		Size: 11.9 MB (11907196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6395ae4c99c9e2a5d74712096ece3f2947b0151c2c046ccd0089ae0cf4fb7e`  
		Last Modified: Wed, 16 Nov 2022 03:42:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f3b40dc1f758b0a046a19cbf0cee89f5e96d4d090542fdefc8efa65de82a35`  
		Last Modified: Wed, 16 Nov 2022 03:42:12 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:bc872e5625df09f82deaa136598b0e37c35e585dc929f25a99834736967c2b16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.0-data` - linux; amd64

```console
$ docker pull influxdb@sha256:a25c4833d481ac01ddf22cd23c055d4912bbedc9db13e267edbe6eeac4da17e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101778875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ba217229d611e12859361bdbd4d3754654eb8e05ae8d6b1dc4cc5ba4bff6a36`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:38:26 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Wed, 16 Nov 2022 03:38:29 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:38:29 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 16 Nov 2022 03:38:29 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:38:30 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:38:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:38:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 16 Nov 2022 03:38:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:38:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7da312b5df063a0b9103f9ba6c3866d916b877be64d7e852b765666b2993f5d`  
		Last Modified: Wed, 16 Nov 2022 03:42:02 GMT  
		Size: 30.7 MB (30693312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c703224cd9f7fff787704da9f65e8f5e64cea07d863da12b62d7d4393a8c1a`  
		Last Modified: Wed, 16 Nov 2022 03:41:57 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a12e64ac314770c10a22f419bf8e1c393c283feed10a2538495dded4a53e57`  
		Last Modified: Wed, 16 Nov 2022 03:41:57 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97e5b5853d4989ee1ac1c885ce69b00a6ea40905a154a29048360e686b83da9`  
		Last Modified: Wed, 16 Nov 2022 03:41:57 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:d2a2e460d093712eb44ff7d5eb146170b45e0b1bd36017777653c6f56455b04a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.0-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:b244ea89030ac046d23c602fb248e414cc980c1f685a3d1e71731a1d2f7a95d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.0 MB (82991552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8421c5fceeaf68d543c0eeadd8fb37a5dc1cc9b8274c44adee54c29608bb14a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:38:26 GMT
ENV INFLUXDB_VERSION=1.10.0-c1.10.0
# Wed, 16 Nov 2022 03:38:37 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:38:38 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 16 Nov 2022 03:38:38 GMT
EXPOSE 8091
# Wed, 16 Nov 2022 03:38:38 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:38:38 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:38:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:38:38 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714e248afd352d0861b7d4384114cff6e05cabebc6690a712c660fb346bff0e6`  
		Last Modified: Wed, 16 Nov 2022 03:42:14 GMT  
		Size: 11.9 MB (11907196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6395ae4c99c9e2a5d74712096ece3f2947b0151c2c046ccd0089ae0cf4fb7e`  
		Last Modified: Wed, 16 Nov 2022 03:42:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f3b40dc1f758b0a046a19cbf0cee89f5e96d4d090542fdefc8efa65de82a35`  
		Last Modified: Wed, 16 Nov 2022 03:42:12 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:80e27a7af363c70597993003831703cf914105331dfa3f0268d4b2c42970e361
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:fdb4ef5837bb5762dfc231135b077efef47b7952efebe09362f9d9c97ce8b80d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125971220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064158037146b77396457276c2ee520b18d8651b8024db3074c99a8e2608f55e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:37:35 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 16 Nov 2022 03:37:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 16 Nov 2022 03:37:41 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 16 Nov 2022 03:37:41 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:37:41 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:37:41 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:37:41 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 16 Nov 2022 03:37:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:37:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c31834a2f75e74be484f3f42b00064f9b0e6eb4adf101faed2c2bd0c4a3ba02`  
		Last Modified: Wed, 16 Nov 2022 03:40:45 GMT  
		Size: 54.9 MB (54885716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2b3307f4e33d16c2844142a7820da2d2dbf8ae0cd9978d71a91c75e563ab29`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90b3746a2a14c0fac7120989f19e980ef7e22ca9825e71283c2b6529269ef8f`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec26e29524b43c1f4e12eacd58980d06123b4a72d3ea5ad66796c30f97fe35f`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:f43d85acbe7083c7626314cd53416396d06a29fcd2c2ef90e29fe474888ef90d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (116975412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f4ac1a41d6a1daf3374d8108ca714ef1f2c8ed39b456f430791a9bcbe156ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 20:01:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 20:01:57 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 15 Nov 2022 20:02:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 15 Nov 2022 20:02:02 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 15 Nov 2022 20:02:02 GMT
EXPOSE 8086
# Tue, 15 Nov 2022 20:02:02 GMT
VOLUME [/var/lib/influxdb]
# Tue, 15 Nov 2022 20:02:02 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 15 Nov 2022 20:02:02 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 15 Nov 2022 20:02:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 20:02:03 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d3899047f7c882bea0751eec4f1fd0724cf724d35e74d5b7fd88af7a12b21e`  
		Last Modified: Tue, 15 Nov 2022 20:02:17 GMT  
		Size: 2.9 KB (2867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04c3f6e008cfac2d38a4403d44375691bc9e440ed79ce092a61e9598df34802`  
		Last Modified: Tue, 15 Nov 2022 20:02:25 GMT  
		Size: 51.6 MB (51613115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:979013be481d988cbca5b372ae8b9199c0fd45f59a0a64acc3bea4bff25d50ac`  
		Last Modified: Tue, 15 Nov 2022 20:02:17 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0486c78717eaf58687e0f77fff94aedf2d8623e84392b15d05550ddecda544`  
		Last Modified: Tue, 15 Nov 2022 20:02:17 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c7aafa4a83172c0868728c7d479b50856a5162461797592a30637e2315f657`  
		Last Modified: Tue, 15 Nov 2022 20:02:17 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:604a6d1945b365f7cdb2c4ce693ca0cbfbc9a92b6439e5442e6237b2b45d8d61
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (120960098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42239e0f695cdc6f9e151d81ed049e35b98ab54bf0e88864c23ce54eafd45fd5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:43:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 22:43:08 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 15 Nov 2022 22:43:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 15 Nov 2022 22:43:11 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 15 Nov 2022 22:43:12 GMT
EXPOSE 8086
# Tue, 15 Nov 2022 22:43:12 GMT
VOLUME [/var/lib/influxdb]
# Tue, 15 Nov 2022 22:43:12 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 15 Nov 2022 22:43:12 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 15 Nov 2022 22:43:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:43:12 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a46b7076227d429761713a8eebfe83391136c8ae33e1b12d28761158f9aabdf`  
		Last Modified: Tue, 15 Nov 2022 22:44:54 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1788f8199066710c971cfc7a021e0aea702c039bb3c205c29082bc154f8c1ed8`  
		Last Modified: Tue, 15 Nov 2022 22:44:59 GMT  
		Size: 51.2 MB (51230052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85137112acfa062ab1ff8ad295cb14ee62fab91e8054d6fe8077d1fc75aeaf4`  
		Last Modified: Tue, 15 Nov 2022 22:44:54 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d7b7be7877701f78b9b5f9beeb83dd68ab15d2f26360ffb3aaa426ac9562fc`  
		Last Modified: Tue, 15 Nov 2022 22:44:54 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119797dd151b1eac5241bba5e902507e565cf013318bc9f239060ffdb6007e6d`  
		Last Modified: Tue, 15 Nov 2022 22:44:54 GMT  
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
$ docker pull influxdb@sha256:02fc8a445a027909472c1e6c8160c8dce42a1cd1b2def387df343bb139b2d205
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:b49c21b9b250a8666ee8fc42360a2ffbce1966197ccb7026d67e20f864cc335e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127790650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f83fb437508b57df2a7ab0d0b3f77490382d6142a4c0f7506b66d587e3281aff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:37:46 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 16 Nov 2022 03:37:53 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:37:53 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 16 Nov 2022 03:37:53 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:37:54 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:37:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:37:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 16 Nov 2022 03:37:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:37:54 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb18277636b07158c3da12d135bc54bec1ec06b16a565cb69ad7c50afa3c016`  
		Last Modified: Wed, 16 Nov 2022 03:41:02 GMT  
		Size: 56.7 MB (56705087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83138449ad58e4bb50abcead99e29058051b490a79f74c5be0fff1635ee10de7`  
		Last Modified: Wed, 16 Nov 2022 03:40:55 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bb00425aa8c285a1f52d835e16efb158e7b7fe59a31f736515dc3b134f5796`  
		Last Modified: Wed, 16 Nov 2022 03:40:55 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987bc8cd1a9dfc6e265d1da41619150448665b9ecf60ec13c23663997c4f5802`  
		Last Modified: Wed, 16 Nov 2022 03:40:55 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:86a9d3f7be75bd7c2950a5a2566c40a0c67e972449c19e06d0f665a1dcd0bf18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:63bf5d77f46263bf1b4556fea1e18c83d1de9f90b8cc38f63a9896107656a199
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94497125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea5556aa02f76556fe0d09b6653e860506d511be3248e932a568196616a2cc8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:37:46 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 16 Nov 2022 03:38:02 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:38:02 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 16 Nov 2022 03:38:02 GMT
EXPOSE 8091
# Wed, 16 Nov 2022 03:38:02 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:38:03 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:38:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:38:03 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede8efbb1c1aa522033dd60d8f1c5ba0bb1e345784eaafe964147ac151f83b34`  
		Last Modified: Wed, 16 Nov 2022 03:41:18 GMT  
		Size: 23.4 MB (23412767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533a5a045a893342d58b1fb54b1d496d13066a0f2f6354a780b5f727795ff9e`  
		Last Modified: Wed, 16 Nov 2022 03:41:15 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901296ce31db8a7ef6bb26b11e6d399f7b9e4f50c5283a2339c444e5895f89e6`  
		Last Modified: Wed, 16 Nov 2022 03:41:15 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:80e27a7af363c70597993003831703cf914105331dfa3f0268d4b2c42970e361
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:fdb4ef5837bb5762dfc231135b077efef47b7952efebe09362f9d9c97ce8b80d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125971220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064158037146b77396457276c2ee520b18d8651b8024db3074c99a8e2608f55e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:37:35 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 16 Nov 2022 03:37:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 16 Nov 2022 03:37:41 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 16 Nov 2022 03:37:41 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:37:41 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:37:41 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:37:41 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 16 Nov 2022 03:37:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:37:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c31834a2f75e74be484f3f42b00064f9b0e6eb4adf101faed2c2bd0c4a3ba02`  
		Last Modified: Wed, 16 Nov 2022 03:40:45 GMT  
		Size: 54.9 MB (54885716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2b3307f4e33d16c2844142a7820da2d2dbf8ae0cd9978d71a91c75e563ab29`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90b3746a2a14c0fac7120989f19e980ef7e22ca9825e71283c2b6529269ef8f`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec26e29524b43c1f4e12eacd58980d06123b4a72d3ea5ad66796c30f97fe35f`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:f43d85acbe7083c7626314cd53416396d06a29fcd2c2ef90e29fe474888ef90d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (116975412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f4ac1a41d6a1daf3374d8108ca714ef1f2c8ed39b456f430791a9bcbe156ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 20:01:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 20:01:57 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 15 Nov 2022 20:02:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 15 Nov 2022 20:02:02 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 15 Nov 2022 20:02:02 GMT
EXPOSE 8086
# Tue, 15 Nov 2022 20:02:02 GMT
VOLUME [/var/lib/influxdb]
# Tue, 15 Nov 2022 20:02:02 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 15 Nov 2022 20:02:02 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 15 Nov 2022 20:02:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 20:02:03 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d3899047f7c882bea0751eec4f1fd0724cf724d35e74d5b7fd88af7a12b21e`  
		Last Modified: Tue, 15 Nov 2022 20:02:17 GMT  
		Size: 2.9 KB (2867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04c3f6e008cfac2d38a4403d44375691bc9e440ed79ce092a61e9598df34802`  
		Last Modified: Tue, 15 Nov 2022 20:02:25 GMT  
		Size: 51.6 MB (51613115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:979013be481d988cbca5b372ae8b9199c0fd45f59a0a64acc3bea4bff25d50ac`  
		Last Modified: Tue, 15 Nov 2022 20:02:17 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0486c78717eaf58687e0f77fff94aedf2d8623e84392b15d05550ddecda544`  
		Last Modified: Tue, 15 Nov 2022 20:02:17 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c7aafa4a83172c0868728c7d479b50856a5162461797592a30637e2315f657`  
		Last Modified: Tue, 15 Nov 2022 20:02:17 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:604a6d1945b365f7cdb2c4ce693ca0cbfbc9a92b6439e5442e6237b2b45d8d61
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (120960098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42239e0f695cdc6f9e151d81ed049e35b98ab54bf0e88864c23ce54eafd45fd5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:43:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 22:43:08 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 15 Nov 2022 22:43:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 15 Nov 2022 22:43:11 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 15 Nov 2022 22:43:12 GMT
EXPOSE 8086
# Tue, 15 Nov 2022 22:43:12 GMT
VOLUME [/var/lib/influxdb]
# Tue, 15 Nov 2022 22:43:12 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 15 Nov 2022 22:43:12 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 15 Nov 2022 22:43:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:43:12 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a46b7076227d429761713a8eebfe83391136c8ae33e1b12d28761158f9aabdf`  
		Last Modified: Tue, 15 Nov 2022 22:44:54 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1788f8199066710c971cfc7a021e0aea702c039bb3c205c29082bc154f8c1ed8`  
		Last Modified: Tue, 15 Nov 2022 22:44:59 GMT  
		Size: 51.2 MB (51230052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85137112acfa062ab1ff8ad295cb14ee62fab91e8054d6fe8077d1fc75aeaf4`  
		Last Modified: Tue, 15 Nov 2022 22:44:54 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d7b7be7877701f78b9b5f9beeb83dd68ab15d2f26360ffb3aaa426ac9562fc`  
		Last Modified: Tue, 15 Nov 2022 22:44:54 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119797dd151b1eac5241bba5e902507e565cf013318bc9f239060ffdb6007e6d`  
		Last Modified: Tue, 15 Nov 2022 22:44:54 GMT  
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
$ docker pull influxdb@sha256:02fc8a445a027909472c1e6c8160c8dce42a1cd1b2def387df343bb139b2d205
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:b49c21b9b250a8666ee8fc42360a2ffbce1966197ccb7026d67e20f864cc335e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127790650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f83fb437508b57df2a7ab0d0b3f77490382d6142a4c0f7506b66d587e3281aff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:37:46 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 16 Nov 2022 03:37:53 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:37:53 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 16 Nov 2022 03:37:53 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:37:54 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:37:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:37:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 16 Nov 2022 03:37:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:37:54 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb18277636b07158c3da12d135bc54bec1ec06b16a565cb69ad7c50afa3c016`  
		Last Modified: Wed, 16 Nov 2022 03:41:02 GMT  
		Size: 56.7 MB (56705087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83138449ad58e4bb50abcead99e29058051b490a79f74c5be0fff1635ee10de7`  
		Last Modified: Wed, 16 Nov 2022 03:40:55 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bb00425aa8c285a1f52d835e16efb158e7b7fe59a31f736515dc3b134f5796`  
		Last Modified: Wed, 16 Nov 2022 03:40:55 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987bc8cd1a9dfc6e265d1da41619150448665b9ecf60ec13c23663997c4f5802`  
		Last Modified: Wed, 16 Nov 2022 03:40:55 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:86a9d3f7be75bd7c2950a5a2566c40a0c67e972449c19e06d0f665a1dcd0bf18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:63bf5d77f46263bf1b4556fea1e18c83d1de9f90b8cc38f63a9896107656a199
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94497125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea5556aa02f76556fe0d09b6653e860506d511be3248e932a568196616a2cc8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:37:46 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 16 Nov 2022 03:38:02 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:38:02 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 16 Nov 2022 03:38:02 GMT
EXPOSE 8091
# Wed, 16 Nov 2022 03:38:02 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:38:03 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:38:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:38:03 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede8efbb1c1aa522033dd60d8f1c5ba0bb1e345784eaafe964147ac151f83b34`  
		Last Modified: Wed, 16 Nov 2022 03:41:18 GMT  
		Size: 23.4 MB (23412767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533a5a045a893342d58b1fb54b1d496d13066a0f2f6354a780b5f727795ff9e`  
		Last Modified: Wed, 16 Nov 2022 03:41:15 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901296ce31db8a7ef6bb26b11e6d399f7b9e4f50c5283a2339c444e5895f89e6`  
		Last Modified: Wed, 16 Nov 2022 03:41:15 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:c2149b2e5898cc2a3c127b776594bd4a6b3805aa07c061b6851bd47b763edf2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:1311a7bf54543e305808edb76c7d612bdb51b7ab4f5644cbc12d05a717290eb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100706471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c8701e029980b3a6d12059cf8f20ae15d60d271566992060621026fedc33df4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:38:07 GMT
ENV INFLUXDB_VERSION=1.9.8-c1.9.8
# Wed, 16 Nov 2022 03:38:13 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:38:13 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 16 Nov 2022 03:38:13 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:38:13 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:38:13 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:38:13 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 16 Nov 2022 03:38:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:38:13 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08b9cc9f0d0bf6279ae66dbb655d085565a40f033fdbec963174d84312c201d`  
		Last Modified: Wed, 16 Nov 2022 03:41:36 GMT  
		Size: 29.6 MB (29620910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2067724f4f792f261be634917a7749db82e5b11ddafff4b3cfb56444064724`  
		Last Modified: Wed, 16 Nov 2022 03:41:31 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2621f8633d7c79cec9b93236baf2472ceda8ebfbc62c07d0abdaad468ab39234`  
		Last Modified: Wed, 16 Nov 2022 03:41:31 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439376b4a97c62e2b7f06b3bad1963e68b5d1b542a7692ebcc63cfa4fb819938`  
		Last Modified: Wed, 16 Nov 2022 03:41:30 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:c906779c133c17191a7fd25b79e186adea461344a8599e72e7389a58265ea480
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:144e05504daf7822b3d321b255da2a299678119ba61496b64b5d6b8acec6d73a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33892268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0db6c89c144c3d3e48a1dae2124de0ff025bf941bca90942d30d3b73b312867`
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
# Thu, 06 Oct 2022 22:40:44 GMT
ENV INFLUXDB_VERSION=1.9.8-c1.9.8
# Thu, 06 Oct 2022 22:40:51 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:40:51 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 06 Oct 2022 22:40:51 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:40:51 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:40:51 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:40:51 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 06 Oct 2022 22:40:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:40:52 GMT
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
	-	`sha256:bf337aa6876df971a95bcefe7863c941df440e23edbba78d5b844adc3484f959`  
		Last Modified: Thu, 06 Oct 2022 22:44:12 GMT  
		Size: 29.6 MB (29581543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608fc838e03119e34209c37aba266a8e6ea9a5e26cf594a50456fb6f6eef7266`  
		Last Modified: Thu, 06 Oct 2022 22:44:07 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807c89d83ef932e7ff68d277a8640ded2a3c042a0e3c0a902acf81ab09a27c48`  
		Last Modified: Thu, 06 Oct 2022 22:44:07 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a367fe28788aa1e2d857ab8c9973bc3d8fcaa8701f6f44eb7cae9143c6898d`  
		Last Modified: Thu, 06 Oct 2022 22:44:07 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:3cebf4c20bdf4e11b71b92e62e1bcdafe469e021ed5cc82f0fd7f7551ebd242e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ddfc5b6c01ef0b43e9ed3a5e20d1d709bb2394c08b8d0ae6c2bb227b49cc0f67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82484462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3c864dbe647acc7ebd8088be2d34ce634ac1bef51b9ef9407b7357012f8b534`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:38:07 GMT
ENV INFLUXDB_VERSION=1.9.8-c1.9.8
# Wed, 16 Nov 2022 03:38:21 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:38:21 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 16 Nov 2022 03:38:21 GMT
EXPOSE 8091
# Wed, 16 Nov 2022 03:38:21 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:38:21 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:38:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:38:21 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37eae804cd91f6c734408b2c3640b2e1c63189f903c068221d1587b9af930526`  
		Last Modified: Wed, 16 Nov 2022 03:41:47 GMT  
		Size: 11.4 MB (11400106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0d1a653cc355c586ed0fa77e0e86ae2ad2324b06725089cb81cb0b88ca83e4`  
		Last Modified: Wed, 16 Nov 2022 03:41:45 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71af18623830e2a50b5263792d51530a7d9ca325f034a22f3a54d6708d96a70`  
		Last Modified: Wed, 16 Nov 2022 03:41:45 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:827f677ac56421c6b06b51a5ec6898e97443103f4e55bf1a774367add6565df7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:af6d01cf6b7af7cf50e449eda694a8e12c5aba98c7403ad5c01902083decf145
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15670709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5434775788926cc4a978991eb508c5efd79dea7e3a8958b95df2a5b6907d74`
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
# Thu, 06 Oct 2022 22:40:44 GMT
ENV INFLUXDB_VERSION=1.9.8-c1.9.8
# Thu, 06 Oct 2022 22:41:00 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:41:00 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 06 Oct 2022 22:41:00 GMT
EXPOSE 8091
# Thu, 06 Oct 2022 22:41:01 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:41:01 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:41:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:41:01 GMT
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
	-	`sha256:8095753f12e066a0f18c6b1746f9bd09b6f5c9f51cbcb4454b4aa21aadacf1f2`  
		Last Modified: Thu, 06 Oct 2022 22:44:25 GMT  
		Size: 11.4 MB (11361192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d9340d3f7a38930960ec6452a608bd8fd8784ddec743172a38763501720f3e`  
		Last Modified: Thu, 06 Oct 2022 22:44:23 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad0cc9662945e5b928a143911c4284cb9660009f69f50290d4c6e76fbd39405`  
		Last Modified: Thu, 06 Oct 2022 22:44:23 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.8-data`

```console
$ docker pull influxdb@sha256:c2149b2e5898cc2a3c127b776594bd4a6b3805aa07c061b6851bd47b763edf2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:1311a7bf54543e305808edb76c7d612bdb51b7ab4f5644cbc12d05a717290eb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100706471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c8701e029980b3a6d12059cf8f20ae15d60d271566992060621026fedc33df4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:38:07 GMT
ENV INFLUXDB_VERSION=1.9.8-c1.9.8
# Wed, 16 Nov 2022 03:38:13 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:38:13 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 16 Nov 2022 03:38:13 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:38:13 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:38:13 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:38:13 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 16 Nov 2022 03:38:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:38:13 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08b9cc9f0d0bf6279ae66dbb655d085565a40f033fdbec963174d84312c201d`  
		Last Modified: Wed, 16 Nov 2022 03:41:36 GMT  
		Size: 29.6 MB (29620910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2067724f4f792f261be634917a7749db82e5b11ddafff4b3cfb56444064724`  
		Last Modified: Wed, 16 Nov 2022 03:41:31 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2621f8633d7c79cec9b93236baf2472ceda8ebfbc62c07d0abdaad468ab39234`  
		Last Modified: Wed, 16 Nov 2022 03:41:31 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439376b4a97c62e2b7f06b3bad1963e68b5d1b542a7692ebcc63cfa4fb819938`  
		Last Modified: Wed, 16 Nov 2022 03:41:30 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.8-data-alpine`

```console
$ docker pull influxdb@sha256:c906779c133c17191a7fd25b79e186adea461344a8599e72e7389a58265ea480
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:144e05504daf7822b3d321b255da2a299678119ba61496b64b5d6b8acec6d73a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33892268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0db6c89c144c3d3e48a1dae2124de0ff025bf941bca90942d30d3b73b312867`
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
# Thu, 06 Oct 2022 22:40:44 GMT
ENV INFLUXDB_VERSION=1.9.8-c1.9.8
# Thu, 06 Oct 2022 22:40:51 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:40:51 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 06 Oct 2022 22:40:51 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:40:51 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:40:51 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:40:51 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 06 Oct 2022 22:40:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:40:52 GMT
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
	-	`sha256:bf337aa6876df971a95bcefe7863c941df440e23edbba78d5b844adc3484f959`  
		Last Modified: Thu, 06 Oct 2022 22:44:12 GMT  
		Size: 29.6 MB (29581543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608fc838e03119e34209c37aba266a8e6ea9a5e26cf594a50456fb6f6eef7266`  
		Last Modified: Thu, 06 Oct 2022 22:44:07 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807c89d83ef932e7ff68d277a8640ded2a3c042a0e3c0a902acf81ab09a27c48`  
		Last Modified: Thu, 06 Oct 2022 22:44:07 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a367fe28788aa1e2d857ab8c9973bc3d8fcaa8701f6f44eb7cae9143c6898d`  
		Last Modified: Thu, 06 Oct 2022 22:44:07 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.8-meta`

```console
$ docker pull influxdb@sha256:3cebf4c20bdf4e11b71b92e62e1bcdafe469e021ed5cc82f0fd7f7551ebd242e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ddfc5b6c01ef0b43e9ed3a5e20d1d709bb2394c08b8d0ae6c2bb227b49cc0f67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82484462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3c864dbe647acc7ebd8088be2d34ce634ac1bef51b9ef9407b7357012f8b534`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:38:07 GMT
ENV INFLUXDB_VERSION=1.9.8-c1.9.8
# Wed, 16 Nov 2022 03:38:21 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:38:21 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 16 Nov 2022 03:38:21 GMT
EXPOSE 8091
# Wed, 16 Nov 2022 03:38:21 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:38:21 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:38:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:38:21 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37eae804cd91f6c734408b2c3640b2e1c63189f903c068221d1587b9af930526`  
		Last Modified: Wed, 16 Nov 2022 03:41:47 GMT  
		Size: 11.4 MB (11400106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0d1a653cc355c586ed0fa77e0e86ae2ad2324b06725089cb81cb0b88ca83e4`  
		Last Modified: Wed, 16 Nov 2022 03:41:45 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71af18623830e2a50b5263792d51530a7d9ca325f034a22f3a54d6708d96a70`  
		Last Modified: Wed, 16 Nov 2022 03:41:45 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.8-meta-alpine`

```console
$ docker pull influxdb@sha256:827f677ac56421c6b06b51a5ec6898e97443103f4e55bf1a774367add6565df7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:af6d01cf6b7af7cf50e449eda694a8e12c5aba98c7403ad5c01902083decf145
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15670709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5434775788926cc4a978991eb508c5efd79dea7e3a8958b95df2a5b6907d74`
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
# Thu, 06 Oct 2022 22:40:44 GMT
ENV INFLUXDB_VERSION=1.9.8-c1.9.8
# Thu, 06 Oct 2022 22:41:00 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 22:41:00 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 06 Oct 2022 22:41:00 GMT
EXPOSE 8091
# Thu, 06 Oct 2022 22:41:01 GMT
VOLUME [/var/lib/influxdb]
# Thu, 06 Oct 2022 22:41:01 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:41:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:41:01 GMT
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
	-	`sha256:8095753f12e066a0f18c6b1746f9bd09b6f5c9f51cbcb4454b4aa21aadacf1f2`  
		Last Modified: Thu, 06 Oct 2022 22:44:25 GMT  
		Size: 11.4 MB (11361192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d9340d3f7a38930960ec6452a608bd8fd8784ddec743172a38763501720f3e`  
		Last Modified: Thu, 06 Oct 2022 22:44:23 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad0cc9662945e5b928a143911c4284cb9660009f69f50290d4c6e76fbd39405`  
		Last Modified: Thu, 06 Oct 2022 22:44:23 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.3`

```console
$ docker pull influxdb@sha256:1fc1628431b1aacf6c34d7dbbf52a032a49cc5536176d00b53c862042aa31533
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.3` - linux; amd64

```console
$ docker pull influxdb@sha256:00f934ab103fbb503ebd981af2185e1da7c02e96a6a173481dd39489e6e8c444
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255123096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86beffc756e50e85989a0a2118281c1eeb60f9e9dbe75a96cf75d6c5fc52dc39`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:25:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:38:43 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Nov 2022 03:38:43 GMT
ENV GOSU_VER=1.12
# Wed, 16 Nov 2022 03:38:47 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 16 Nov 2022 03:38:48 GMT
ENV INFLUXDB_VERSION=2.3.0
# Wed, 16 Nov 2022 03:38:56 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 16 Nov 2022 03:38:56 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 16 Nov 2022 03:38:59 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 16 Nov 2022 03:39:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Nov 2022 03:39:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Nov 2022 03:39:00 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Nov 2022 03:39:00 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 16 Nov 2022 03:39:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:39:00 GMT
CMD ["influxd"]
# Wed, 16 Nov 2022 03:39:00 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:39:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Nov 2022 03:39:01 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Nov 2022 03:39:01 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 16 Nov 2022 03:39:01 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a122751b35336c158fc53a3bb03c6b11b414387589e5455e99baecdd803c6318`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 7.9 MB (7858972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a277c3efe7c0d28e443180df5a70570f6baed1f16a4ceeb88e9dd299df62dc6`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 10.0 MB (10001396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1142272673814766ad5baafaa0df451f964fe5ead8a55486c0f88af0b1182`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2b3f636f80ac907b1c6acada387a6d8d0582773aa7c240822e85028c650220`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6ceb667e9e348b22531916425693bdb4c080eacb89f4242c2be96ba54ae74`  
		Last Modified: Wed, 16 Nov 2022 03:42:37 GMT  
		Size: 180.5 MB (180478628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46aa930953f3ab315f69fbf16b7c70a7245d721be3e8983352c09eb4e0c6aeab`  
		Last Modified: Wed, 16 Nov 2022 03:42:25 GMT  
		Size: 5.4 MB (5366844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190dc59bac37828bb8144bd225ff98d707eb26c7d90630a6c5651d6bc6e50e41`  
		Last Modified: Wed, 16 Nov 2022 03:42:24 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108b2514b932e1a212105877d36f3831fb2c37078d038134f359f1dea67f5de5`  
		Last Modified: Wed, 16 Nov 2022 03:42:24 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62504d8ff3ba1ed08cedde6f4ddf2cd92fdff32f4481fa206ccf9dd5620e7460`  
		Last Modified: Wed, 16 Nov 2022 03:42:24 GMT  
		Size: 5.1 KB (5131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.3` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:da8c28616dc16e48ac59c52111edaa33a9818cd286d0a73ee076dfd1fc8b8dd8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.6 MB (253612770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:663d98990a7336cf38b91d7679824f66c9f93e0a60ef40a27172f476f4fafce2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:37:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:37:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:43:15 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 15 Nov 2022 22:43:15 GMT
ENV GOSU_VER=1.12
# Tue, 15 Nov 2022 22:43:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 15 Nov 2022 22:43:23 GMT
ENV INFLUXDB_VERSION=2.3.0
# Tue, 15 Nov 2022 22:43:34 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 15 Nov 2022 22:43:35 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Tue, 15 Nov 2022 22:43:39 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 15 Nov 2022 22:43:40 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 15 Nov 2022 22:43:40 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 15 Nov 2022 22:43:40 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 15 Nov 2022 22:43:40 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Tue, 15 Nov 2022 22:43:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:43:40 GMT
CMD ["influxd"]
# Tue, 15 Nov 2022 22:43:40 GMT
EXPOSE 8086
# Tue, 15 Nov 2022 22:43:40 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 15 Nov 2022 22:43:40 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 15 Nov 2022 22:43:40 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 15 Nov 2022 22:43:40 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35873fa6ec375a28180771e63a96f2039703f6658efa32da2e83a64f6919bf1e`  
		Last Modified: Tue, 15 Nov 2022 05:43:54 GMT  
		Size: 7.7 MB (7726432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07615c620859a5288e844fd58e708c735c884a4b600e9ea4bd3f26ca5744f723`  
		Last Modified: Tue, 15 Nov 2022 05:43:55 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56083cb8575ae4dd09c622cbf882282b81072805ba5cbd10cacfd31f55807c6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cedcc4b339b2253be7ad805bfbf7286a12d211b2582ccd8518975394ed70f6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c59819c85af7042ea0bfed9c8af3050706c0077db302ea92d6f31a70b40fbb7`  
		Last Modified: Tue, 15 Nov 2022 22:45:19 GMT  
		Size: 180.8 MB (180792463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fd4f889638bb821b070fe938e60e482142832617cfc6e95dbc101db934d1e9`  
		Last Modified: Tue, 15 Nov 2022 22:45:09 GMT  
		Size: 5.0 MB (4952681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16562308e633613df172f44c2eb08cd7b7e7a6049a5af81ad448e47b58e94412`  
		Last Modified: Tue, 15 Nov 2022 22:45:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1bf8be503e469d8e91ddc831545d89cbe070bf6b9c1ecd1c7ac4a1ff306b29`  
		Last Modified: Tue, 15 Nov 2022 22:45:08 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf603e67d95b03a223f5b8a0cac3ab46e8705bc51592c9ccf286eea0baf4ea5`  
		Last Modified: Tue, 15 Nov 2022 22:45:08 GMT  
		Size: 5.1 KB (5130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.3-alpine`

```console
$ docker pull influxdb@sha256:d7f5dd5f70e2f07391da189c7a3419fd4bba75086cb51eb894c125c866531c34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.3-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:abc16f418524ec4598372458fcc6ab5e711c4abade713645d67634b44ea1122a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.5 MB (198529319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03dea0505e2bf966f9dee4945ed4bd1e07e8d9eaf76a9f2931d46c7a2ad5436`
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
# Thu, 06 Oct 2022 22:41:52 GMT
ENV INFLUXDB_VERSION=2.3.0
# Thu, 06 Oct 2022 22:41:59 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 06 Oct 2022 22:41:59 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 06 Oct 2022 22:42:02 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 06 Oct 2022 22:42:03 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 06 Oct 2022 22:42:03 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 06 Oct 2022 22:42:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 06 Oct 2022 22:42:03 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:42:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:42:03 GMT
CMD ["influxd"]
# Thu, 06 Oct 2022 22:42:03 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:42:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 06 Oct 2022 22:42:04 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 06 Oct 2022 22:42:04 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 06 Oct 2022 22:42:04 GMT
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
	-	`sha256:735ca3c9c55ece0fe60b814f5687ae0be43581dbe1385a3ef6a05c71cc15c1ad`  
		Last Modified: Thu, 06 Oct 2022 22:45:34 GMT  
		Size: 180.5 MB (180478628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d0999ec3c2a8ab832576fafcb6a001e0d58571758c2a899fb778dbff478829`  
		Last Modified: Thu, 06 Oct 2022 22:45:22 GMT  
		Size: 5.4 MB (5366868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdade7e062b4896fa081bd00da1ea0643c5d309ed5836632719f899997573f20`  
		Last Modified: Thu, 06 Oct 2022 22:45:21 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ef27b8fdf84bf3a174772a5a966dfe77f68f96abbe8f1e49a72bd0c2ebc66a`  
		Last Modified: Thu, 06 Oct 2022 22:45:21 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1393ea92ccda79b2af6882b858326cac797b4cf7521a611969665e6683a26ca`  
		Last Modified: Thu, 06 Oct 2022 22:45:21 GMT  
		Size: 5.0 KB (5019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:08d2690d37d78f5c82c2cc2b371f98a85a7bd761f9b46f64b5bcc947d4c651bf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.1 MB (198149758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0730654e9fb5470fbeccdc6d99b7b32f6525fbb31ec27caa62937cdb69080e7`
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
# Thu, 10 Nov 2022 21:47:22 GMT
ENV INFLUXDB_VERSION=2.3.0
# Thu, 10 Nov 2022 21:47:32 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 10 Nov 2022 21:47:34 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 10 Nov 2022 21:47:38 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 10 Nov 2022 21:47:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 10 Nov 2022 21:47:38 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 10 Nov 2022 21:47:39 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 10 Nov 2022 21:47:39 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 10 Nov 2022 21:47:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 10 Nov 2022 21:47:39 GMT
CMD ["influxd"]
# Thu, 10 Nov 2022 21:47:39 GMT
EXPOSE 8086
# Thu, 10 Nov 2022 21:47:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 10 Nov 2022 21:47:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 10 Nov 2022 21:47:39 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 10 Nov 2022 21:47:39 GMT
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
	-	`sha256:98e184716bee119b6c06bd5e8b9ff3baf80352446439608c46e6d7f07fc9a612`  
		Last Modified: Thu, 10 Nov 2022 21:48:52 GMT  
		Size: 180.8 MB (180792458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870cb3efb889f7dc13b713ff3ba4cf8d54f7d4225eb9ce6228f3bdd4910dce4c`  
		Last Modified: Thu, 10 Nov 2022 21:48:43 GMT  
		Size: 5.0 MB (4952681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbfaffa0ce99042c18e406e600f26cc3488bafca6ec7b59ec4f57f5be28614d`  
		Last Modified: Thu, 10 Nov 2022 21:48:42 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642a32668da8150e300883304a84fa725614c615afa38f4400c38f19b446b1e5`  
		Last Modified: Thu, 10 Nov 2022 21:48:42 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04332880f45b19eef70613049b212f2c6fdd34ed3375270262d4544bb2d0cd`  
		Last Modified: Thu, 10 Nov 2022 21:48:42 GMT  
		Size: 5.0 KB (5018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.3.0`

```console
$ docker pull influxdb@sha256:1fc1628431b1aacf6c34d7dbbf52a032a49cc5536176d00b53c862042aa31533
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.3.0` - linux; amd64

```console
$ docker pull influxdb@sha256:00f934ab103fbb503ebd981af2185e1da7c02e96a6a173481dd39489e6e8c444
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255123096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86beffc756e50e85989a0a2118281c1eeb60f9e9dbe75a96cf75d6c5fc52dc39`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:25:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:38:43 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Nov 2022 03:38:43 GMT
ENV GOSU_VER=1.12
# Wed, 16 Nov 2022 03:38:47 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 16 Nov 2022 03:38:48 GMT
ENV INFLUXDB_VERSION=2.3.0
# Wed, 16 Nov 2022 03:38:56 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 16 Nov 2022 03:38:56 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 16 Nov 2022 03:38:59 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 16 Nov 2022 03:39:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Nov 2022 03:39:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Nov 2022 03:39:00 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Nov 2022 03:39:00 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 16 Nov 2022 03:39:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:39:00 GMT
CMD ["influxd"]
# Wed, 16 Nov 2022 03:39:00 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:39:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Nov 2022 03:39:01 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Nov 2022 03:39:01 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 16 Nov 2022 03:39:01 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a122751b35336c158fc53a3bb03c6b11b414387589e5455e99baecdd803c6318`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 7.9 MB (7858972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a277c3efe7c0d28e443180df5a70570f6baed1f16a4ceeb88e9dd299df62dc6`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 10.0 MB (10001396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1142272673814766ad5baafaa0df451f964fe5ead8a55486c0f88af0b1182`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2b3f636f80ac907b1c6acada387a6d8d0582773aa7c240822e85028c650220`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6ceb667e9e348b22531916425693bdb4c080eacb89f4242c2be96ba54ae74`  
		Last Modified: Wed, 16 Nov 2022 03:42:37 GMT  
		Size: 180.5 MB (180478628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46aa930953f3ab315f69fbf16b7c70a7245d721be3e8983352c09eb4e0c6aeab`  
		Last Modified: Wed, 16 Nov 2022 03:42:25 GMT  
		Size: 5.4 MB (5366844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190dc59bac37828bb8144bd225ff98d707eb26c7d90630a6c5651d6bc6e50e41`  
		Last Modified: Wed, 16 Nov 2022 03:42:24 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108b2514b932e1a212105877d36f3831fb2c37078d038134f359f1dea67f5de5`  
		Last Modified: Wed, 16 Nov 2022 03:42:24 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62504d8ff3ba1ed08cedde6f4ddf2cd92fdff32f4481fa206ccf9dd5620e7460`  
		Last Modified: Wed, 16 Nov 2022 03:42:24 GMT  
		Size: 5.1 KB (5131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.3.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:da8c28616dc16e48ac59c52111edaa33a9818cd286d0a73ee076dfd1fc8b8dd8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.6 MB (253612770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:663d98990a7336cf38b91d7679824f66c9f93e0a60ef40a27172f476f4fafce2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:37:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:37:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:43:15 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 15 Nov 2022 22:43:15 GMT
ENV GOSU_VER=1.12
# Tue, 15 Nov 2022 22:43:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 15 Nov 2022 22:43:23 GMT
ENV INFLUXDB_VERSION=2.3.0
# Tue, 15 Nov 2022 22:43:34 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 15 Nov 2022 22:43:35 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Tue, 15 Nov 2022 22:43:39 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 15 Nov 2022 22:43:40 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 15 Nov 2022 22:43:40 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 15 Nov 2022 22:43:40 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 15 Nov 2022 22:43:40 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Tue, 15 Nov 2022 22:43:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:43:40 GMT
CMD ["influxd"]
# Tue, 15 Nov 2022 22:43:40 GMT
EXPOSE 8086
# Tue, 15 Nov 2022 22:43:40 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 15 Nov 2022 22:43:40 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 15 Nov 2022 22:43:40 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 15 Nov 2022 22:43:40 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35873fa6ec375a28180771e63a96f2039703f6658efa32da2e83a64f6919bf1e`  
		Last Modified: Tue, 15 Nov 2022 05:43:54 GMT  
		Size: 7.7 MB (7726432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07615c620859a5288e844fd58e708c735c884a4b600e9ea4bd3f26ca5744f723`  
		Last Modified: Tue, 15 Nov 2022 05:43:55 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56083cb8575ae4dd09c622cbf882282b81072805ba5cbd10cacfd31f55807c6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cedcc4b339b2253be7ad805bfbf7286a12d211b2582ccd8518975394ed70f6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c59819c85af7042ea0bfed9c8af3050706c0077db302ea92d6f31a70b40fbb7`  
		Last Modified: Tue, 15 Nov 2022 22:45:19 GMT  
		Size: 180.8 MB (180792463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fd4f889638bb821b070fe938e60e482142832617cfc6e95dbc101db934d1e9`  
		Last Modified: Tue, 15 Nov 2022 22:45:09 GMT  
		Size: 5.0 MB (4952681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16562308e633613df172f44c2eb08cd7b7e7a6049a5af81ad448e47b58e94412`  
		Last Modified: Tue, 15 Nov 2022 22:45:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1bf8be503e469d8e91ddc831545d89cbe070bf6b9c1ecd1c7ac4a1ff306b29`  
		Last Modified: Tue, 15 Nov 2022 22:45:08 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf603e67d95b03a223f5b8a0cac3ab46e8705bc51592c9ccf286eea0baf4ea5`  
		Last Modified: Tue, 15 Nov 2022 22:45:08 GMT  
		Size: 5.1 KB (5130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.3.0-alpine`

```console
$ docker pull influxdb@sha256:d7f5dd5f70e2f07391da189c7a3419fd4bba75086cb51eb894c125c866531c34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.3.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:abc16f418524ec4598372458fcc6ab5e711c4abade713645d67634b44ea1122a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.5 MB (198529319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03dea0505e2bf966f9dee4945ed4bd1e07e8d9eaf76a9f2931d46c7a2ad5436`
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
# Thu, 06 Oct 2022 22:41:52 GMT
ENV INFLUXDB_VERSION=2.3.0
# Thu, 06 Oct 2022 22:41:59 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 06 Oct 2022 22:41:59 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 06 Oct 2022 22:42:02 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 06 Oct 2022 22:42:03 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 06 Oct 2022 22:42:03 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 06 Oct 2022 22:42:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 06 Oct 2022 22:42:03 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 06 Oct 2022 22:42:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 22:42:03 GMT
CMD ["influxd"]
# Thu, 06 Oct 2022 22:42:03 GMT
EXPOSE 8086
# Thu, 06 Oct 2022 22:42:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 06 Oct 2022 22:42:04 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 06 Oct 2022 22:42:04 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 06 Oct 2022 22:42:04 GMT
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
	-	`sha256:735ca3c9c55ece0fe60b814f5687ae0be43581dbe1385a3ef6a05c71cc15c1ad`  
		Last Modified: Thu, 06 Oct 2022 22:45:34 GMT  
		Size: 180.5 MB (180478628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d0999ec3c2a8ab832576fafcb6a001e0d58571758c2a899fb778dbff478829`  
		Last Modified: Thu, 06 Oct 2022 22:45:22 GMT  
		Size: 5.4 MB (5366868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdade7e062b4896fa081bd00da1ea0643c5d309ed5836632719f899997573f20`  
		Last Modified: Thu, 06 Oct 2022 22:45:21 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ef27b8fdf84bf3a174772a5a966dfe77f68f96abbe8f1e49a72bd0c2ebc66a`  
		Last Modified: Thu, 06 Oct 2022 22:45:21 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1393ea92ccda79b2af6882b858326cac797b4cf7521a611969665e6683a26ca`  
		Last Modified: Thu, 06 Oct 2022 22:45:21 GMT  
		Size: 5.0 KB (5019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:08d2690d37d78f5c82c2cc2b371f98a85a7bd761f9b46f64b5bcc947d4c651bf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.1 MB (198149758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0730654e9fb5470fbeccdc6d99b7b32f6525fbb31ec27caa62937cdb69080e7`
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
# Thu, 10 Nov 2022 21:47:22 GMT
ENV INFLUXDB_VERSION=2.3.0
# Thu, 10 Nov 2022 21:47:32 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 10 Nov 2022 21:47:34 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 10 Nov 2022 21:47:38 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 10 Nov 2022 21:47:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 10 Nov 2022 21:47:38 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 10 Nov 2022 21:47:39 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 10 Nov 2022 21:47:39 GMT
COPY file:a6a402694185d5f58fa629116844ddbbc1c391c2cafad4c8077c27ee45de05a8 in /entrypoint.sh 
# Thu, 10 Nov 2022 21:47:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 10 Nov 2022 21:47:39 GMT
CMD ["influxd"]
# Thu, 10 Nov 2022 21:47:39 GMT
EXPOSE 8086
# Thu, 10 Nov 2022 21:47:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 10 Nov 2022 21:47:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 10 Nov 2022 21:47:39 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 10 Nov 2022 21:47:39 GMT
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
	-	`sha256:98e184716bee119b6c06bd5e8b9ff3baf80352446439608c46e6d7f07fc9a612`  
		Last Modified: Thu, 10 Nov 2022 21:48:52 GMT  
		Size: 180.8 MB (180792458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870cb3efb889f7dc13b713ff3ba4cf8d54f7d4225eb9ce6228f3bdd4910dce4c`  
		Last Modified: Thu, 10 Nov 2022 21:48:43 GMT  
		Size: 5.0 MB (4952681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbfaffa0ce99042c18e406e600f26cc3488bafca6ec7b59ec4f57f5be28614d`  
		Last Modified: Thu, 10 Nov 2022 21:48:42 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642a32668da8150e300883304a84fa725614c615afa38f4400c38f19b446b1e5`  
		Last Modified: Thu, 10 Nov 2022 21:48:42 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04332880f45b19eef70613049b212f2c6fdd34ed3375270262d4544bb2d0cd`  
		Last Modified: Thu, 10 Nov 2022 21:48:42 GMT  
		Size: 5.0 KB (5018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.4`

```console
$ docker pull influxdb@sha256:b2e781355663380d7495875f7316cc2deab546a440fe40010c4fd2bd709dfdca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.4` - linux; amd64

```console
$ docker pull influxdb@sha256:d90318bf60abc864fc6f47adb6d0399ceee96d71b4879368fb5c4df42d83549c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261150783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31fb15462c98119224e43b4255ac457fe634a767d07b03200a12d857ffef6d66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:25:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:38:43 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Nov 2022 03:38:43 GMT
ENV GOSU_VER=1.12
# Wed, 16 Nov 2022 03:38:47 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 16 Nov 2022 03:39:08 GMT
ENV INFLUXDB_VERSION=2.4.0
# Wed, 16 Nov 2022 03:39:16 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 16 Nov 2022 03:39:17 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Wed, 16 Nov 2022 03:39:21 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 16 Nov 2022 03:39:22 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Nov 2022 03:39:22 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Nov 2022 03:39:22 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Nov 2022 03:39:22 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 16 Nov 2022 03:39:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:39:22 GMT
CMD ["influxd"]
# Wed, 16 Nov 2022 03:39:22 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:39:22 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Nov 2022 03:39:22 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Nov 2022 03:39:23 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 16 Nov 2022 03:39:23 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a122751b35336c158fc53a3bb03c6b11b414387589e5455e99baecdd803c6318`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 7.9 MB (7858972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a277c3efe7c0d28e443180df5a70570f6baed1f16a4ceeb88e9dd299df62dc6`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 10.0 MB (10001396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1142272673814766ad5baafaa0df451f964fe5ead8a55486c0f88af0b1182`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2b3f636f80ac907b1c6acada387a6d8d0582773aa7c240822e85028c650220`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2176a2c0371442ac4a854e5413294f71914384dbede0d19aa14c94c59919bc14`  
		Last Modified: Wed, 16 Nov 2022 03:43:01 GMT  
		Size: 185.8 MB (185802086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1060de88079127709936d0440daa1247c443ac5f5c3fd1060abca59ead5c1a3d`  
		Last Modified: Wed, 16 Nov 2022 03:42:48 GMT  
		Size: 6.1 MB (6071075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07468dcd99cc1a5a8cfb8e98fe551268b1f4d9e4e70d583a0a9d5a155630f6a6`  
		Last Modified: Wed, 16 Nov 2022 03:42:47 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7485ca17fe850724b44f658d27a1c3afdecfc7014b4dccefacb77d42fc46c627`  
		Last Modified: Wed, 16 Nov 2022 03:42:47 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab331f4a39495689c7806c559c5b1a1dc05ba58132ee7f8509a581e16a9a400c`  
		Last Modified: Wed, 16 Nov 2022 03:42:47 GMT  
		Size: 5.1 KB (5131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.4` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:5d018ba4598e69cea2a73a889612b2b599e900a0bd00bb1009a6c0040d09388e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255913866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c60ef5b6ac1b1211ec86e4bfa4af85e913eba8738676933cb4d3a294d39309b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:37:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:37:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:43:15 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 15 Nov 2022 22:43:15 GMT
ENV GOSU_VER=1.12
# Tue, 15 Nov 2022 22:43:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 15 Nov 2022 22:43:44 GMT
ENV INFLUXDB_VERSION=2.4.0
# Tue, 15 Nov 2022 22:43:53 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 15 Nov 2022 22:43:55 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Tue, 15 Nov 2022 22:43:59 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 15 Nov 2022 22:44:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 15 Nov 2022 22:44:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 15 Nov 2022 22:44:00 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 15 Nov 2022 22:44:00 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Tue, 15 Nov 2022 22:44:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:44:00 GMT
CMD ["influxd"]
# Tue, 15 Nov 2022 22:44:00 GMT
EXPOSE 8086
# Tue, 15 Nov 2022 22:44:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 15 Nov 2022 22:44:00 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 15 Nov 2022 22:44:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 15 Nov 2022 22:44:01 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35873fa6ec375a28180771e63a96f2039703f6658efa32da2e83a64f6919bf1e`  
		Last Modified: Tue, 15 Nov 2022 05:43:54 GMT  
		Size: 7.7 MB (7726432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07615c620859a5288e844fd58e708c735c884a4b600e9ea4bd3f26ca5744f723`  
		Last Modified: Tue, 15 Nov 2022 05:43:55 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56083cb8575ae4dd09c622cbf882282b81072805ba5cbd10cacfd31f55807c6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cedcc4b339b2253be7ad805bfbf7286a12d211b2582ccd8518975394ed70f6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111d3581520e6beeee83909293642e6f4020ceaa3c0813dcc93f93b864da336c`  
		Last Modified: Tue, 15 Nov 2022 22:45:38 GMT  
		Size: 182.4 MB (182445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed247dfe12dc5822a94bc28d62321083023359d002fc5f9b5c4f7dd2b923d8`  
		Last Modified: Tue, 15 Nov 2022 22:45:29 GMT  
		Size: 5.6 MB (5600679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376f7900e94ef0fb0a35f0b4fa7a8f28676e91a9bb24726099463d61369ea0c8`  
		Last Modified: Tue, 15 Nov 2022 22:45:28 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ee6ce4d98818f3128db0d30badbce9d7bc1bd59537d09b8789ab067c8cb697`  
		Last Modified: Tue, 15 Nov 2022 22:45:28 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29bad7124968f5bdb571d970c5b3392767af928b8197b0003ffd5a3d0131348`  
		Last Modified: Tue, 15 Nov 2022 22:45:28 GMT  
		Size: 5.1 KB (5130 bytes)  
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
$ docker pull influxdb@sha256:b2e781355663380d7495875f7316cc2deab546a440fe40010c4fd2bd709dfdca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.4.0` - linux; amd64

```console
$ docker pull influxdb@sha256:d90318bf60abc864fc6f47adb6d0399ceee96d71b4879368fb5c4df42d83549c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261150783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31fb15462c98119224e43b4255ac457fe634a767d07b03200a12d857ffef6d66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:25:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:38:43 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Nov 2022 03:38:43 GMT
ENV GOSU_VER=1.12
# Wed, 16 Nov 2022 03:38:47 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 16 Nov 2022 03:39:08 GMT
ENV INFLUXDB_VERSION=2.4.0
# Wed, 16 Nov 2022 03:39:16 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 16 Nov 2022 03:39:17 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Wed, 16 Nov 2022 03:39:21 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 16 Nov 2022 03:39:22 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Nov 2022 03:39:22 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Nov 2022 03:39:22 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Nov 2022 03:39:22 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 16 Nov 2022 03:39:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:39:22 GMT
CMD ["influxd"]
# Wed, 16 Nov 2022 03:39:22 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:39:22 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Nov 2022 03:39:22 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Nov 2022 03:39:23 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 16 Nov 2022 03:39:23 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a122751b35336c158fc53a3bb03c6b11b414387589e5455e99baecdd803c6318`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 7.9 MB (7858972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a277c3efe7c0d28e443180df5a70570f6baed1f16a4ceeb88e9dd299df62dc6`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 10.0 MB (10001396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1142272673814766ad5baafaa0df451f964fe5ead8a55486c0f88af0b1182`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2b3f636f80ac907b1c6acada387a6d8d0582773aa7c240822e85028c650220`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2176a2c0371442ac4a854e5413294f71914384dbede0d19aa14c94c59919bc14`  
		Last Modified: Wed, 16 Nov 2022 03:43:01 GMT  
		Size: 185.8 MB (185802086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1060de88079127709936d0440daa1247c443ac5f5c3fd1060abca59ead5c1a3d`  
		Last Modified: Wed, 16 Nov 2022 03:42:48 GMT  
		Size: 6.1 MB (6071075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07468dcd99cc1a5a8cfb8e98fe551268b1f4d9e4e70d583a0a9d5a155630f6a6`  
		Last Modified: Wed, 16 Nov 2022 03:42:47 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7485ca17fe850724b44f658d27a1c3afdecfc7014b4dccefacb77d42fc46c627`  
		Last Modified: Wed, 16 Nov 2022 03:42:47 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab331f4a39495689c7806c559c5b1a1dc05ba58132ee7f8509a581e16a9a400c`  
		Last Modified: Wed, 16 Nov 2022 03:42:47 GMT  
		Size: 5.1 KB (5131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.4.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:5d018ba4598e69cea2a73a889612b2b599e900a0bd00bb1009a6c0040d09388e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255913866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c60ef5b6ac1b1211ec86e4bfa4af85e913eba8738676933cb4d3a294d39309b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:37:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:37:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:43:15 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 15 Nov 2022 22:43:15 GMT
ENV GOSU_VER=1.12
# Tue, 15 Nov 2022 22:43:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 15 Nov 2022 22:43:44 GMT
ENV INFLUXDB_VERSION=2.4.0
# Tue, 15 Nov 2022 22:43:53 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 15 Nov 2022 22:43:55 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Tue, 15 Nov 2022 22:43:59 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 15 Nov 2022 22:44:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 15 Nov 2022 22:44:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 15 Nov 2022 22:44:00 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 15 Nov 2022 22:44:00 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Tue, 15 Nov 2022 22:44:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:44:00 GMT
CMD ["influxd"]
# Tue, 15 Nov 2022 22:44:00 GMT
EXPOSE 8086
# Tue, 15 Nov 2022 22:44:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 15 Nov 2022 22:44:00 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 15 Nov 2022 22:44:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 15 Nov 2022 22:44:01 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35873fa6ec375a28180771e63a96f2039703f6658efa32da2e83a64f6919bf1e`  
		Last Modified: Tue, 15 Nov 2022 05:43:54 GMT  
		Size: 7.7 MB (7726432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07615c620859a5288e844fd58e708c735c884a4b600e9ea4bd3f26ca5744f723`  
		Last Modified: Tue, 15 Nov 2022 05:43:55 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56083cb8575ae4dd09c622cbf882282b81072805ba5cbd10cacfd31f55807c6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cedcc4b339b2253be7ad805bfbf7286a12d211b2582ccd8518975394ed70f6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111d3581520e6beeee83909293642e6f4020ceaa3c0813dcc93f93b864da336c`  
		Last Modified: Tue, 15 Nov 2022 22:45:38 GMT  
		Size: 182.4 MB (182445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed247dfe12dc5822a94bc28d62321083023359d002fc5f9b5c4f7dd2b923d8`  
		Last Modified: Tue, 15 Nov 2022 22:45:29 GMT  
		Size: 5.6 MB (5600679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376f7900e94ef0fb0a35f0b4fa7a8f28676e91a9bb24726099463d61369ea0c8`  
		Last Modified: Tue, 15 Nov 2022 22:45:28 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ee6ce4d98818f3128db0d30badbce9d7bc1bd59537d09b8789ab067c8cb697`  
		Last Modified: Tue, 15 Nov 2022 22:45:28 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29bad7124968f5bdb571d970c5b3392767af928b8197b0003ffd5a3d0131348`  
		Last Modified: Tue, 15 Nov 2022 22:45:28 GMT  
		Size: 5.1 KB (5130 bytes)  
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
$ docker pull influxdb@sha256:a25bc8310582069b76214f20df5a158d1d7e37e8be12b6ba05e4492876f8e083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5` - linux; amd64

```console
$ docker pull influxdb@sha256:d8f17fc8f7fdf70445eab97dca8f8e6a3a8d370521950de31d40cf74210b3de3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169817570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8edfd8e887ea20edd57a072fb3f82d1858ea69d02d4729d516611b708e0fca14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:25:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:38:43 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Nov 2022 03:38:43 GMT
ENV GOSU_VER=1.12
# Wed, 16 Nov 2022 03:38:47 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 16 Nov 2022 03:39:27 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 16 Nov 2022 03:39:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 16 Nov 2022 03:39:34 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 16 Nov 2022 03:39:37 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 16 Nov 2022 03:39:37 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Nov 2022 03:39:37 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Nov 2022 03:39:38 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Nov 2022 03:39:38 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 16 Nov 2022 03:39:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:39:38 GMT
CMD ["influxd"]
# Wed, 16 Nov 2022 03:39:38 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:39:38 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Nov 2022 03:39:38 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Nov 2022 03:39:38 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 16 Nov 2022 03:39:39 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a122751b35336c158fc53a3bb03c6b11b414387589e5455e99baecdd803c6318`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 7.9 MB (7858972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a277c3efe7c0d28e443180df5a70570f6baed1f16a4ceeb88e9dd299df62dc6`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 10.0 MB (10001396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1142272673814766ad5baafaa0df451f964fe5ead8a55486c0f88af0b1182`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2b3f636f80ac907b1c6acada387a6d8d0582773aa7c240822e85028c650220`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f914dc08485b5091c280062a8092f20fcde37815f19086600fcfd41f0feb892`  
		Last Modified: Wed, 16 Nov 2022 03:43:23 GMT  
		Size: 94.4 MB (94434171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadb747586e24b8af81f0d40f4fac94bdecc543fb992b3cdaf9f2a7186a36386`  
		Last Modified: Wed, 16 Nov 2022 03:43:13 GMT  
		Size: 6.1 MB (6105778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78b7ff7a1015a059b121301b150caa0500d5b36d0e9533094ce3f247c66c330`  
		Last Modified: Wed, 16 Nov 2022 03:43:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481246db4da4d13c0fcfadc9a75cf6ab565de517354176f01487aa9632789255`  
		Last Modified: Wed, 16 Nov 2022 03:43:11 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6158bbfd0260c1653f85a21b7a31d6f515fe9ae5ed1fb7c92668da524b4901`  
		Last Modified: Wed, 16 Nov 2022 03:43:11 GMT  
		Size: 5.1 KB (5129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:09d210b6496b8a86ffc468c7a1a260650a06b4b352fa6c9f61fc0249a4af07bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164547937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38e6f0940f7edc3b656a3cfbb514782bf614d69ee5ca6ec5fba895bd345141b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:37:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:37:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:43:15 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 15 Nov 2022 22:43:15 GMT
ENV GOSU_VER=1.12
# Tue, 15 Nov 2022 22:43:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 15 Nov 2022 22:44:06 GMT
ENV INFLUXDB_VERSION=2.5.1
# Tue, 15 Nov 2022 22:44:17 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 15 Nov 2022 22:44:18 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Tue, 15 Nov 2022 22:44:26 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 15 Nov 2022 22:44:27 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 15 Nov 2022 22:44:27 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 15 Nov 2022 22:44:27 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 15 Nov 2022 22:44:27 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Tue, 15 Nov 2022 22:44:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:44:27 GMT
CMD ["influxd"]
# Tue, 15 Nov 2022 22:44:27 GMT
EXPOSE 8086
# Tue, 15 Nov 2022 22:44:27 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 15 Nov 2022 22:44:27 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 15 Nov 2022 22:44:27 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 15 Nov 2022 22:44:27 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35873fa6ec375a28180771e63a96f2039703f6658efa32da2e83a64f6919bf1e`  
		Last Modified: Tue, 15 Nov 2022 05:43:54 GMT  
		Size: 7.7 MB (7726432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07615c620859a5288e844fd58e708c735c884a4b600e9ea4bd3f26ca5744f723`  
		Last Modified: Tue, 15 Nov 2022 05:43:55 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56083cb8575ae4dd09c622cbf882282b81072805ba5cbd10cacfd31f55807c6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cedcc4b339b2253be7ad805bfbf7286a12d211b2582ccd8518975394ed70f6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c721b94e77060569d1275db29f5a067f36151f592420324bee957cb5038c37`  
		Last Modified: Tue, 15 Nov 2022 22:45:54 GMT  
		Size: 91.0 MB (91048415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9ccbd6b14bc77ccde497162dceffd41be9ae214ec8133e8c51d68b14a0def0`  
		Last Modified: Tue, 15 Nov 2022 22:45:48 GMT  
		Size: 5.6 MB (5631894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945380806ffe05380b7504b3a5f533c9c2aee129954a280b3ecf717b05add7f3`  
		Last Modified: Tue, 15 Nov 2022 22:45:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab60a0d6ab37feed69241f2083d85d550c70ee05c7eba2fa6e80b48de664590`  
		Last Modified: Tue, 15 Nov 2022 22:45:47 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df37f9148102a85400a9c8e3cecc121f59012557d5b79242f14234304bd0567b`  
		Last Modified: Tue, 15 Nov 2022 22:45:47 GMT  
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
$ docker pull influxdb@sha256:a25bc8310582069b76214f20df5a158d1d7e37e8be12b6ba05e4492876f8e083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.5.1` - linux; amd64

```console
$ docker pull influxdb@sha256:d8f17fc8f7fdf70445eab97dca8f8e6a3a8d370521950de31d40cf74210b3de3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169817570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8edfd8e887ea20edd57a072fb3f82d1858ea69d02d4729d516611b708e0fca14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:25:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:38:43 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Nov 2022 03:38:43 GMT
ENV GOSU_VER=1.12
# Wed, 16 Nov 2022 03:38:47 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 16 Nov 2022 03:39:27 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 16 Nov 2022 03:39:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 16 Nov 2022 03:39:34 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 16 Nov 2022 03:39:37 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 16 Nov 2022 03:39:37 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Nov 2022 03:39:37 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Nov 2022 03:39:38 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Nov 2022 03:39:38 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 16 Nov 2022 03:39:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:39:38 GMT
CMD ["influxd"]
# Wed, 16 Nov 2022 03:39:38 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:39:38 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Nov 2022 03:39:38 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Nov 2022 03:39:38 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 16 Nov 2022 03:39:39 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a122751b35336c158fc53a3bb03c6b11b414387589e5455e99baecdd803c6318`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 7.9 MB (7858972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a277c3efe7c0d28e443180df5a70570f6baed1f16a4ceeb88e9dd299df62dc6`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 10.0 MB (10001396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1142272673814766ad5baafaa0df451f964fe5ead8a55486c0f88af0b1182`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2b3f636f80ac907b1c6acada387a6d8d0582773aa7c240822e85028c650220`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f914dc08485b5091c280062a8092f20fcde37815f19086600fcfd41f0feb892`  
		Last Modified: Wed, 16 Nov 2022 03:43:23 GMT  
		Size: 94.4 MB (94434171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadb747586e24b8af81f0d40f4fac94bdecc543fb992b3cdaf9f2a7186a36386`  
		Last Modified: Wed, 16 Nov 2022 03:43:13 GMT  
		Size: 6.1 MB (6105778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78b7ff7a1015a059b121301b150caa0500d5b36d0e9533094ce3f247c66c330`  
		Last Modified: Wed, 16 Nov 2022 03:43:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481246db4da4d13c0fcfadc9a75cf6ab565de517354176f01487aa9632789255`  
		Last Modified: Wed, 16 Nov 2022 03:43:11 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6158bbfd0260c1653f85a21b7a31d6f515fe9ae5ed1fb7c92668da524b4901`  
		Last Modified: Wed, 16 Nov 2022 03:43:11 GMT  
		Size: 5.1 KB (5129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.5.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:09d210b6496b8a86ffc468c7a1a260650a06b4b352fa6c9f61fc0249a4af07bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164547937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38e6f0940f7edc3b656a3cfbb514782bf614d69ee5ca6ec5fba895bd345141b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:37:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:37:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:43:15 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 15 Nov 2022 22:43:15 GMT
ENV GOSU_VER=1.12
# Tue, 15 Nov 2022 22:43:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 15 Nov 2022 22:44:06 GMT
ENV INFLUXDB_VERSION=2.5.1
# Tue, 15 Nov 2022 22:44:17 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 15 Nov 2022 22:44:18 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Tue, 15 Nov 2022 22:44:26 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 15 Nov 2022 22:44:27 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 15 Nov 2022 22:44:27 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 15 Nov 2022 22:44:27 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 15 Nov 2022 22:44:27 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Tue, 15 Nov 2022 22:44:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:44:27 GMT
CMD ["influxd"]
# Tue, 15 Nov 2022 22:44:27 GMT
EXPOSE 8086
# Tue, 15 Nov 2022 22:44:27 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 15 Nov 2022 22:44:27 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 15 Nov 2022 22:44:27 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 15 Nov 2022 22:44:27 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35873fa6ec375a28180771e63a96f2039703f6658efa32da2e83a64f6919bf1e`  
		Last Modified: Tue, 15 Nov 2022 05:43:54 GMT  
		Size: 7.7 MB (7726432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07615c620859a5288e844fd58e708c735c884a4b600e9ea4bd3f26ca5744f723`  
		Last Modified: Tue, 15 Nov 2022 05:43:55 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56083cb8575ae4dd09c622cbf882282b81072805ba5cbd10cacfd31f55807c6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cedcc4b339b2253be7ad805bfbf7286a12d211b2582ccd8518975394ed70f6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c721b94e77060569d1275db29f5a067f36151f592420324bee957cb5038c37`  
		Last Modified: Tue, 15 Nov 2022 22:45:54 GMT  
		Size: 91.0 MB (91048415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9ccbd6b14bc77ccde497162dceffd41be9ae214ec8133e8c51d68b14a0def0`  
		Last Modified: Tue, 15 Nov 2022 22:45:48 GMT  
		Size: 5.6 MB (5631894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945380806ffe05380b7504b3a5f533c9c2aee129954a280b3ecf717b05add7f3`  
		Last Modified: Tue, 15 Nov 2022 22:45:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab60a0d6ab37feed69241f2083d85d550c70ee05c7eba2fa6e80b48de664590`  
		Last Modified: Tue, 15 Nov 2022 22:45:47 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df37f9148102a85400a9c8e3cecc121f59012557d5b79242f14234304bd0567b`  
		Last Modified: Tue, 15 Nov 2022 22:45:47 GMT  
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

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:0cde017d9bc2e77fbb3cdc258cfdaebc2059e8aca8edac61c2f4a290a3a3bc6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

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

### `influxdb:alpine` - linux; arm64 variant v8

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

## `influxdb:data`

```console
$ docker pull influxdb@sha256:02fc8a445a027909472c1e6c8160c8dce42a1cd1b2def387df343bb139b2d205
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:b49c21b9b250a8666ee8fc42360a2ffbce1966197ccb7026d67e20f864cc335e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127790650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f83fb437508b57df2a7ab0d0b3f77490382d6142a4c0f7506b66d587e3281aff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:37:46 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 16 Nov 2022 03:37:53 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:37:53 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 16 Nov 2022 03:37:53 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:37:54 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:37:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:37:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 16 Nov 2022 03:37:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:37:54 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb18277636b07158c3da12d135bc54bec1ec06b16a565cb69ad7c50afa3c016`  
		Last Modified: Wed, 16 Nov 2022 03:41:02 GMT  
		Size: 56.7 MB (56705087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83138449ad58e4bb50abcead99e29058051b490a79f74c5be0fff1635ee10de7`  
		Last Modified: Wed, 16 Nov 2022 03:40:55 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bb00425aa8c285a1f52d835e16efb158e7b7fe59a31f736515dc3b134f5796`  
		Last Modified: Wed, 16 Nov 2022 03:40:55 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987bc8cd1a9dfc6e265d1da41619150448665b9ecf60ec13c23663997c4f5802`  
		Last Modified: Wed, 16 Nov 2022 03:40:55 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:a25bc8310582069b76214f20df5a158d1d7e37e8be12b6ba05e4492876f8e083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:d8f17fc8f7fdf70445eab97dca8f8e6a3a8d370521950de31d40cf74210b3de3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169817570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8edfd8e887ea20edd57a072fb3f82d1858ea69d02d4729d516611b708e0fca14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:25:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:38:43 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Nov 2022 03:38:43 GMT
ENV GOSU_VER=1.12
# Wed, 16 Nov 2022 03:38:47 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 16 Nov 2022 03:39:27 GMT
ENV INFLUXDB_VERSION=2.5.1
# Wed, 16 Nov 2022 03:39:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 16 Nov 2022 03:39:34 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Wed, 16 Nov 2022 03:39:37 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 16 Nov 2022 03:39:37 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Nov 2022 03:39:37 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Nov 2022 03:39:38 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Nov 2022 03:39:38 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Wed, 16 Nov 2022 03:39:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:39:38 GMT
CMD ["influxd"]
# Wed, 16 Nov 2022 03:39:38 GMT
EXPOSE 8086
# Wed, 16 Nov 2022 03:39:38 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Nov 2022 03:39:38 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Nov 2022 03:39:38 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 16 Nov 2022 03:39:39 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a122751b35336c158fc53a3bb03c6b11b414387589e5455e99baecdd803c6318`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 7.9 MB (7858972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a277c3efe7c0d28e443180df5a70570f6baed1f16a4ceeb88e9dd299df62dc6`  
		Last Modified: Tue, 15 Nov 2022 10:32:48 GMT  
		Size: 10.0 MB (10001396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1142272673814766ad5baafaa0df451f964fe5ead8a55486c0f88af0b1182`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2b3f636f80ac907b1c6acada387a6d8d0582773aa7c240822e85028c650220`  
		Last Modified: Wed, 16 Nov 2022 03:42:26 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f914dc08485b5091c280062a8092f20fcde37815f19086600fcfd41f0feb892`  
		Last Modified: Wed, 16 Nov 2022 03:43:23 GMT  
		Size: 94.4 MB (94434171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadb747586e24b8af81f0d40f4fac94bdecc543fb992b3cdaf9f2a7186a36386`  
		Last Modified: Wed, 16 Nov 2022 03:43:13 GMT  
		Size: 6.1 MB (6105778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78b7ff7a1015a059b121301b150caa0500d5b36d0e9533094ce3f247c66c330`  
		Last Modified: Wed, 16 Nov 2022 03:43:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481246db4da4d13c0fcfadc9a75cf6ab565de517354176f01487aa9632789255`  
		Last Modified: Wed, 16 Nov 2022 03:43:11 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6158bbfd0260c1653f85a21b7a31d6f515fe9ae5ed1fb7c92668da524b4901`  
		Last Modified: Wed, 16 Nov 2022 03:43:11 GMT  
		Size: 5.1 KB (5129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:09d210b6496b8a86ffc468c7a1a260650a06b4b352fa6c9f61fc0249a4af07bb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164547937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38e6f0940f7edc3b656a3cfbb514782bf614d69ee5ca6ec5fba895bd345141b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:37:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:37:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:43:15 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 15 Nov 2022 22:43:15 GMT
ENV GOSU_VER=1.12
# Tue, 15 Nov 2022 22:43:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 15 Nov 2022 22:44:06 GMT
ENV INFLUXDB_VERSION=2.5.1
# Tue, 15 Nov 2022 22:44:17 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 15 Nov 2022 22:44:18 GMT
ENV INFLUX_CLI_VERSION=2.5.0
# Tue, 15 Nov 2022 22:44:26 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 15 Nov 2022 22:44:27 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 15 Nov 2022 22:44:27 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 15 Nov 2022 22:44:27 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 15 Nov 2022 22:44:27 GMT
COPY file:dbf3d010c7392537ae2b4c9b0d90a1ba01accd63948136585d5decc93bb52afc in /entrypoint.sh 
# Tue, 15 Nov 2022 22:44:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:44:27 GMT
CMD ["influxd"]
# Tue, 15 Nov 2022 22:44:27 GMT
EXPOSE 8086
# Tue, 15 Nov 2022 22:44:27 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 15 Nov 2022 22:44:27 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 15 Nov 2022 22:44:27 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 15 Nov 2022 22:44:27 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35873fa6ec375a28180771e63a96f2039703f6658efa32da2e83a64f6919bf1e`  
		Last Modified: Tue, 15 Nov 2022 05:43:54 GMT  
		Size: 7.7 MB (7726432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07615c620859a5288e844fd58e708c735c884a4b600e9ea4bd3f26ca5744f723`  
		Last Modified: Tue, 15 Nov 2022 05:43:55 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56083cb8575ae4dd09c622cbf882282b81072805ba5cbd10cacfd31f55807c6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cedcc4b339b2253be7ad805bfbf7286a12d211b2582ccd8518975394ed70f6`  
		Last Modified: Tue, 15 Nov 2022 22:45:10 GMT  
		Size: 896.4 KB (896355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c721b94e77060569d1275db29f5a067f36151f592420324bee957cb5038c37`  
		Last Modified: Tue, 15 Nov 2022 22:45:54 GMT  
		Size: 91.0 MB (91048415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9ccbd6b14bc77ccde497162dceffd41be9ae214ec8133e8c51d68b14a0def0`  
		Last Modified: Tue, 15 Nov 2022 22:45:48 GMT  
		Size: 5.6 MB (5631894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945380806ffe05380b7504b3a5f533c9c2aee129954a280b3ecf717b05add7f3`  
		Last Modified: Tue, 15 Nov 2022 22:45:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab60a0d6ab37feed69241f2083d85d550c70ee05c7eba2fa6e80b48de664590`  
		Last Modified: Tue, 15 Nov 2022 22:45:47 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df37f9148102a85400a9c8e3cecc121f59012557d5b79242f14234304bd0567b`  
		Last Modified: Tue, 15 Nov 2022 22:45:47 GMT  
		Size: 5.1 KB (5131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:86a9d3f7be75bd7c2950a5a2566c40a0c67e972449c19e06d0f665a1dcd0bf18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:63bf5d77f46263bf1b4556fea1e18c83d1de9f90b8cc38f63a9896107656a199
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94497125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea5556aa02f76556fe0d09b6653e860506d511be3248e932a568196616a2cc8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 03:37:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 03:37:46 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 16 Nov 2022 03:38:02 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 16 Nov 2022 03:38:02 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 16 Nov 2022 03:38:02 GMT
EXPOSE 8091
# Wed, 16 Nov 2022 03:38:02 GMT
VOLUME [/var/lib/influxdb]
# Wed, 16 Nov 2022 03:38:03 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 16 Nov 2022 03:38:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 03:38:03 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4db93e59de8bbf2496b71cb41920eb9d1d565e46be51046279f7f290957bcb`  
		Last Modified: Wed, 16 Nov 2022 03:40:38 GMT  
		Size: 2.9 KB (2887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede8efbb1c1aa522033dd60d8f1c5ba0bb1e345784eaafe964147ac151f83b34`  
		Last Modified: Wed, 16 Nov 2022 03:41:18 GMT  
		Size: 23.4 MB (23412767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533a5a045a893342d58b1fb54b1d496d13066a0f2f6354a780b5f727795ff9e`  
		Last Modified: Wed, 16 Nov 2022 03:41:15 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901296ce31db8a7ef6bb26b11e6d399f7b9e4f50c5283a2339c444e5895f89e6`  
		Last Modified: Wed, 16 Nov 2022 03:41:15 GMT  
		Size: 374.0 B  
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
