<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `influxdb`

-	[`influxdb:1.10-data`](#influxdb110-data)
-	[`influxdb:1.10-data-alpine`](#influxdb110-data-alpine)
-	[`influxdb:1.10-meta`](#influxdb110-meta)
-	[`influxdb:1.10-meta-alpine`](#influxdb110-meta-alpine)
-	[`influxdb:1.10.5-data`](#influxdb1105-data)
-	[`influxdb:1.10.5-data-alpine`](#influxdb1105-data-alpine)
-	[`influxdb:1.10.5-meta`](#influxdb1105-meta)
-	[`influxdb:1.10.5-meta-alpine`](#influxdb1105-meta-alpine)
-	[`influxdb:1.11-data`](#influxdb111-data)
-	[`influxdb:1.11-data-alpine`](#influxdb111-data-alpine)
-	[`influxdb:1.11-meta`](#influxdb111-meta)
-	[`influxdb:1.11-meta-alpine`](#influxdb111-meta-alpine)
-	[`influxdb:1.11.3-data`](#influxdb1113-data)
-	[`influxdb:1.11.3-data-alpine`](#influxdb1113-data-alpine)
-	[`influxdb:1.11.3-meta`](#influxdb1113-meta)
-	[`influxdb:1.11.3-meta-alpine`](#influxdb1113-meta-alpine)
-	[`influxdb:1.8`](#influxdb18)
-	[`influxdb:1.8-alpine`](#influxdb18-alpine)
-	[`influxdb:1.8.10`](#influxdb1810)
-	[`influxdb:1.8.10-alpine`](#influxdb1810-alpine)
-	[`influxdb:1.9-data`](#influxdb19-data)
-	[`influxdb:1.9-data-alpine`](#influxdb19-data-alpine)
-	[`influxdb:1.9-meta`](#influxdb19-meta)
-	[`influxdb:1.9-meta-alpine`](#influxdb19-meta-alpine)
-	[`influxdb:1.9.13-data`](#influxdb1913-data)
-	[`influxdb:1.9.13-data-alpine`](#influxdb1913-data-alpine)
-	[`influxdb:1.9.13-meta`](#influxdb1913-meta)
-	[`influxdb:1.9.13-meta-alpine`](#influxdb1913-meta-alpine)
-	[`influxdb:2.7`](#influxdb27)
-	[`influxdb:2.7-alpine`](#influxdb27-alpine)
-	[`influxdb:2.7.3`](#influxdb273)
-	[`influxdb:2.7.3-alpine`](#influxdb273-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:latest`](#influxdblatest)

## `influxdb:1.10-data`

```console
$ docker pull influxdb@sha256:ab0352e05edff1b0a9f6dceae0e4afc7330ba3ef6ede8f8cb14f1f55d2c7fc6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:9768c03e6954b0064fa72fbe319582f4ce8d43a22b01ba44d3e5040a227792d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111002134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b32111aaee22d987cd45b616203c1986b38f48338adb82a01c9c955abede9a3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:18 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Wed, 01 Nov 2023 02:35:22 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb*
# Wed, 01 Nov 2023 02:35:22 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 01 Nov 2023 02:35:22 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:35:22 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:22 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 01 Nov 2023 02:35:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:22 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469105de3319d3732d5d45b2577dd8bbb5a67a20c5f158e7a8d97e07b9c4063b`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17da4adebb0cb8fa52dd8c1f67cf8f7846879f8f3ca57fbefa7d46c827bc9e5`  
		Last Modified: Wed, 01 Nov 2023 02:37:31 GMT  
		Size: 40.2 MB (40176280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717e2111ef3c2433c7e030637868f66e4fd3e2ba65971294264f7c01cee508dc`  
		Last Modified: Wed, 01 Nov 2023 02:37:24 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7d74da89f14f6bcdee8321b0204e63a0be2922f9813f392b97e184d4da0aab`  
		Last Modified: Wed, 01 Nov 2023 02:37:24 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e274ce919e29df4a4953cfec481590de0b4ca7f89b41d87d6a1c374d75cb8ad1`  
		Last Modified: Wed, 01 Nov 2023 02:37:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-data-alpine`

```console
$ docker pull influxdb@sha256:85a08428cf33f91f70fc6a8da73e7f44742eb9bd623afd69086e2021bd57189e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:1692477b2285f24e7370f1644e5a3a418ba999e4b53469dfd7b13461564ca76e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44986189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c1e4702753f208df8e50294e772da0900b4f3c0f9c8fe4b0561c0f21cc29df9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:29:21 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:29:23 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 18 Oct 2023 00:22:23 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Wed, 18 Oct 2023 00:22:32 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 18 Oct 2023 00:22:33 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 18 Oct 2023 00:22:33 GMT
EXPOSE 8086
# Wed, 18 Oct 2023 00:22:33 GMT
VOLUME [/var/lib/influxdb]
# Wed, 18 Oct 2023 00:22:33 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 18 Oct 2023 00:22:33 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 18 Oct 2023 00:22:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Oct 2023 00:22:33 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b161763ec9e11116a97547438c5541153248aba5eddc76475885813812367da`  
		Last Modified: Tue, 17 Oct 2023 01:31:50 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d3938b55c32749418ec88153e08d27efa36f373c1b5b150ee9bb2d1e44c03`  
		Last Modified: Tue, 17 Oct 2023 01:31:49 GMT  
		Size: 1.5 MB (1472471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46796a2d86815c48009bd6afb4af527f9cd29d865c9c1b2e330065ab36803d69`  
		Last Modified: Wed, 18 Oct 2023 00:24:48 GMT  
		Size: 40.1 MB (40133034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc46034c19230b028299b721d7da78662bc4dd1c85c5e58b2ccbb2e9d8cc20e1`  
		Last Modified: Wed, 18 Oct 2023 00:24:42 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857ad96b70a5ce0b7c355b9f207088c2295361d360fd4adaa084eaf6950edd7`  
		Last Modified: Wed, 18 Oct 2023 00:24:42 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa160b98328868f93302e1e980a009e0cf64f934ef1de0b6108958e0e0c2efc5`  
		Last Modified: Wed, 18 Oct 2023 00:24:42 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta`

```console
$ docker pull influxdb@sha256:7f91356fcc4e76e6eac149dd75cb23a34ee82213a27dcbeb95e754cc80d6624a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:68e3c93ebc52837cdb8115dae15eef6e63cd8b3dce5ed139b96aa102bef6f0f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91201611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8106f1bfbeff72b7b64d2181f2bf2a0daeca000b80ace7034b0e2909c8ffec8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:18 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Wed, 01 Nov 2023 02:35:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb*
# Wed, 01 Nov 2023 02:35:31 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 01 Nov 2023 02:35:31 GMT
EXPOSE 8091
# Wed, 01 Nov 2023 02:35:31 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:31 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:31 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469105de3319d3732d5d45b2577dd8bbb5a67a20c5f158e7a8d97e07b9c4063b`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111a81bdb9b1ac7ef4986dc9b1bccac381591d729698367dc1a0878aeb3cb7af`  
		Last Modified: Wed, 01 Nov 2023 02:37:46 GMT  
		Size: 20.4 MB (20376966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9ddf7a793404ca6ae177f1763cfeb9251bf1c8162f7431fa7ca081adf93501`  
		Last Modified: Wed, 01 Nov 2023 02:37:42 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c28adbf2a1bf10f5cc9088f9b019ba01bcffd7e6901288b419f09d6cd5bca9`  
		Last Modified: Wed, 01 Nov 2023 02:37:42 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10-meta-alpine`

```console
$ docker pull influxdb@sha256:1461ecf4d8efc2517856ef896bf22f7524420de2f368e413843be5ccf2a2a660
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:895cc2e01d8aa1a3d36845e2ae0669d0c9ca7b1552be27e03dad16d422cc3889
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25195410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5108316637d2b092b532a36ceb69ff1bb4209916acb571c89af32ca0bdfa0b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:29:21 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:29:23 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 18 Oct 2023 00:22:23 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Wed, 18 Oct 2023 00:22:49 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 18 Oct 2023 00:22:49 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 18 Oct 2023 00:22:49 GMT
EXPOSE 8091
# Wed, 18 Oct 2023 00:22:49 GMT
VOLUME [/var/lib/influxdb]
# Wed, 18 Oct 2023 00:22:49 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 18 Oct 2023 00:22:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Oct 2023 00:22:49 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b161763ec9e11116a97547438c5541153248aba5eddc76475885813812367da`  
		Last Modified: Tue, 17 Oct 2023 01:31:50 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d3938b55c32749418ec88153e08d27efa36f373c1b5b150ee9bb2d1e44c03`  
		Last Modified: Tue, 17 Oct 2023 01:31:49 GMT  
		Size: 1.5 MB (1472471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d32614100effb115de2d98c6009103ed2d5f1e058ce932631036a6ec71e93c`  
		Last Modified: Wed, 18 Oct 2023 00:25:16 GMT  
		Size: 20.3 MB (20343457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa4b14105224639e8a75e3f3b6069d7e687b869e041001482709772490f1aaf`  
		Last Modified: Wed, 18 Oct 2023 00:25:12 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273f61c1ab423446bf797b1688e2fe9e74a2daa1719f88e2a441d3d7a46f2db0`  
		Last Modified: Wed, 18 Oct 2023 00:25:12 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.5-data`

```console
$ docker pull influxdb@sha256:ab0352e05edff1b0a9f6dceae0e4afc7330ba3ef6ede8f8cb14f1f55d2c7fc6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.5-data` - linux; amd64

```console
$ docker pull influxdb@sha256:9768c03e6954b0064fa72fbe319582f4ce8d43a22b01ba44d3e5040a227792d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111002134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b32111aaee22d987cd45b616203c1986b38f48338adb82a01c9c955abede9a3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:18 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Wed, 01 Nov 2023 02:35:22 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb*
# Wed, 01 Nov 2023 02:35:22 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 01 Nov 2023 02:35:22 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:35:22 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:22 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 01 Nov 2023 02:35:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:22 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469105de3319d3732d5d45b2577dd8bbb5a67a20c5f158e7a8d97e07b9c4063b`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17da4adebb0cb8fa52dd8c1f67cf8f7846879f8f3ca57fbefa7d46c827bc9e5`  
		Last Modified: Wed, 01 Nov 2023 02:37:31 GMT  
		Size: 40.2 MB (40176280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717e2111ef3c2433c7e030637868f66e4fd3e2ba65971294264f7c01cee508dc`  
		Last Modified: Wed, 01 Nov 2023 02:37:24 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7d74da89f14f6bcdee8321b0204e63a0be2922f9813f392b97e184d4da0aab`  
		Last Modified: Wed, 01 Nov 2023 02:37:24 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e274ce919e29df4a4953cfec481590de0b4ca7f89b41d87d6a1c374d75cb8ad1`  
		Last Modified: Wed, 01 Nov 2023 02:37:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.5-data-alpine`

```console
$ docker pull influxdb@sha256:85a08428cf33f91f70fc6a8da73e7f44742eb9bd623afd69086e2021bd57189e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.5-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:1692477b2285f24e7370f1644e5a3a418ba999e4b53469dfd7b13461564ca76e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44986189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c1e4702753f208df8e50294e772da0900b4f3c0f9c8fe4b0561c0f21cc29df9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:29:21 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:29:23 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 18 Oct 2023 00:22:23 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Wed, 18 Oct 2023 00:22:32 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 18 Oct 2023 00:22:33 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 18 Oct 2023 00:22:33 GMT
EXPOSE 8086
# Wed, 18 Oct 2023 00:22:33 GMT
VOLUME [/var/lib/influxdb]
# Wed, 18 Oct 2023 00:22:33 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 18 Oct 2023 00:22:33 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 18 Oct 2023 00:22:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Oct 2023 00:22:33 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b161763ec9e11116a97547438c5541153248aba5eddc76475885813812367da`  
		Last Modified: Tue, 17 Oct 2023 01:31:50 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d3938b55c32749418ec88153e08d27efa36f373c1b5b150ee9bb2d1e44c03`  
		Last Modified: Tue, 17 Oct 2023 01:31:49 GMT  
		Size: 1.5 MB (1472471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46796a2d86815c48009bd6afb4af527f9cd29d865c9c1b2e330065ab36803d69`  
		Last Modified: Wed, 18 Oct 2023 00:24:48 GMT  
		Size: 40.1 MB (40133034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc46034c19230b028299b721d7da78662bc4dd1c85c5e58b2ccbb2e9d8cc20e1`  
		Last Modified: Wed, 18 Oct 2023 00:24:42 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c857ad96b70a5ce0b7c355b9f207088c2295361d360fd4adaa084eaf6950edd7`  
		Last Modified: Wed, 18 Oct 2023 00:24:42 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa160b98328868f93302e1e980a009e0cf64f934ef1de0b6108958e0e0c2efc5`  
		Last Modified: Wed, 18 Oct 2023 00:24:42 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.5-meta`

```console
$ docker pull influxdb@sha256:7f91356fcc4e76e6eac149dd75cb23a34ee82213a27dcbeb95e754cc80d6624a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.5-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:68e3c93ebc52837cdb8115dae15eef6e63cd8b3dce5ed139b96aa102bef6f0f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91201611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8106f1bfbeff72b7b64d2181f2bf2a0daeca000b80ace7034b0e2909c8ffec8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:18 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Wed, 01 Nov 2023 02:35:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb*
# Wed, 01 Nov 2023 02:35:31 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 01 Nov 2023 02:35:31 GMT
EXPOSE 8091
# Wed, 01 Nov 2023 02:35:31 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:31 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:31 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469105de3319d3732d5d45b2577dd8bbb5a67a20c5f158e7a8d97e07b9c4063b`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111a81bdb9b1ac7ef4986dc9b1bccac381591d729698367dc1a0878aeb3cb7af`  
		Last Modified: Wed, 01 Nov 2023 02:37:46 GMT  
		Size: 20.4 MB (20376966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9ddf7a793404ca6ae177f1763cfeb9251bf1c8162f7431fa7ca081adf93501`  
		Last Modified: Wed, 01 Nov 2023 02:37:42 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c28adbf2a1bf10f5cc9088f9b019ba01bcffd7e6901288b419f09d6cd5bca9`  
		Last Modified: Wed, 01 Nov 2023 02:37:42 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.10.5-meta-alpine`

```console
$ docker pull influxdb@sha256:1461ecf4d8efc2517856ef896bf22f7524420de2f368e413843be5ccf2a2a660
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.5-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:895cc2e01d8aa1a3d36845e2ae0669d0c9ca7b1552be27e03dad16d422cc3889
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25195410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5108316637d2b092b532a36ceb69ff1bb4209916acb571c89af32ca0bdfa0b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:29:21 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:29:23 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 18 Oct 2023 00:22:23 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Wed, 18 Oct 2023 00:22:49 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 18 Oct 2023 00:22:49 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 18 Oct 2023 00:22:49 GMT
EXPOSE 8091
# Wed, 18 Oct 2023 00:22:49 GMT
VOLUME [/var/lib/influxdb]
# Wed, 18 Oct 2023 00:22:49 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 18 Oct 2023 00:22:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Oct 2023 00:22:49 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b161763ec9e11116a97547438c5541153248aba5eddc76475885813812367da`  
		Last Modified: Tue, 17 Oct 2023 01:31:50 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d3938b55c32749418ec88153e08d27efa36f373c1b5b150ee9bb2d1e44c03`  
		Last Modified: Tue, 17 Oct 2023 01:31:49 GMT  
		Size: 1.5 MB (1472471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d32614100effb115de2d98c6009103ed2d5f1e058ce932631036a6ec71e93c`  
		Last Modified: Wed, 18 Oct 2023 00:25:16 GMT  
		Size: 20.3 MB (20343457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa4b14105224639e8a75e3f3b6069d7e687b869e041001482709772490f1aaf`  
		Last Modified: Wed, 18 Oct 2023 00:25:12 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273f61c1ab423446bf797b1688e2fe9e74a2daa1719f88e2a441d3d7a46f2db0`  
		Last Modified: Wed, 18 Oct 2023 00:25:12 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-data`

```console
$ docker pull influxdb@sha256:af8377b323ee74736982960b27d80214c9bce1bc8db36aa7319f0ec289313088
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:02c9970f1a1e456215f124e97d204d1eb8e7ebb01a4d61ced0351a1638cb4e1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.8 MB (113809290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4738c5bd6f0add12d8f89d014369e1b5b6d35a33f8bc5bb891c9ab5ad076a4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:35:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:37 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Wed, 01 Nov 2023 02:35:41 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb*
# Wed, 01 Nov 2023 02:35:41 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 01 Nov 2023 02:35:41 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:35:41 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:41 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:41 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 01 Nov 2023 02:35:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b15edd27da99dfcc4a562fa21353856b433f3d088be84034b0d200e70adc63`  
		Last Modified: Wed, 01 Nov 2023 02:37:55 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e60eff18a916a66e0e81c141b72cdb59898ef7f710c3823641857da3eb016d`  
		Last Modified: Wed, 01 Nov 2023 02:38:01 GMT  
		Size: 40.2 MB (40174531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af825ccfbe379294f660b4ac6f4adae299c5175b85ed9d52e4757fc0f583f8ec`  
		Last Modified: Wed, 01 Nov 2023 02:37:55 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0218e4766a75cd240d0415b939d7b336a951381f0c7bffbcec9c5672a8275d`  
		Last Modified: Wed, 01 Nov 2023 02:37:54 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a723e9fe0bab63d1244255db1fa4c6f47681d24841e09d3278153771085e97`  
		Last Modified: Wed, 01 Nov 2023 02:37:55 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-data-alpine`

```console
$ docker pull influxdb@sha256:dd29ecf0082bf579438a79ca407cb00af0ccea1314b3a201167390b84106c48d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ea80cb2d0884ee4b48b30af9d76e6ce0558a700f0d53a4b22aa85a27b1c37d96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44943078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4eb53fe3ea56cd4a6e578cd107b997e52162a7cf2281bdc6a4aa4f4e0f51631`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:30:37 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:30:38 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 17 Oct 2023 01:30:38 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Tue, 17 Oct 2023 01:30:46 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 17 Oct 2023 01:30:46 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 17 Oct 2023 01:30:46 GMT
EXPOSE 8086
# Tue, 17 Oct 2023 01:30:46 GMT
VOLUME [/var/lib/influxdb]
# Tue, 17 Oct 2023 01:30:47 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 17 Oct 2023 01:30:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 17 Oct 2023 01:30:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Oct 2023 01:30:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5352bf3aec614dde8ac36d38f28f5021eff4c2ff0226eb22dfa667f2b2add1`  
		Last Modified: Tue, 17 Oct 2023 01:33:20 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0165a81397bc8c25031ed159801827c4fc37f5dba045ffd5bd32eeb6590ba`  
		Last Modified: Tue, 17 Oct 2023 01:33:18 GMT  
		Size: 1.4 MB (1407328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ff88a3565b599c0999572689b7ada926cd541f29a53748f076a1a4e428cf5c`  
		Last Modified: Tue, 17 Oct 2023 01:33:24 GMT  
		Size: 40.1 MB (40131704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd1384bec94ee9e6e672aa3fc7f67ed54cb4b8e0c9c9dd26ac83a0f753f5bd`  
		Last Modified: Tue, 17 Oct 2023 01:33:18 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaaaaea04c9cdf8e607c822cb85d5395086d8816921a964cb68acd8241726b9`  
		Last Modified: Tue, 17 Oct 2023 01:33:18 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31395564ab00aa4757a9a8d575593323885e42a4292aaca5a7aea4901459878b`  
		Last Modified: Tue, 17 Oct 2023 01:33:18 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-meta`

```console
$ docker pull influxdb@sha256:23ed1c7dc3a1e7ec91e7cdcf331b1e971382e20ca90326e51ee05aaf03aed764
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:5e1de343c2d3b7df14c07b212c9f121991fa526473dda9e61a9d9b8fc4680b77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (93960917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e682867e1e05d4ec47778ad813cb5908d8e70a313d7439c69b8f276e14ca576`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:35:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:37 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Wed, 01 Nov 2023 02:35:49 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb*
# Wed, 01 Nov 2023 02:35:50 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 01 Nov 2023 02:35:50 GMT
EXPOSE 8091
# Wed, 01 Nov 2023 02:35:50 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:50 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:50 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b15edd27da99dfcc4a562fa21353856b433f3d088be84034b0d200e70adc63`  
		Last Modified: Wed, 01 Nov 2023 02:37:55 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7063c8c1622de4ab01288e46ab10496452403319fdb371e739f73021e097fd6`  
		Last Modified: Wed, 01 Nov 2023 02:38:14 GMT  
		Size: 20.3 MB (20327364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3008bc9d51b12c0f9defa58b998fce1e4384cae7403d4d8e880c03e868ef5221`  
		Last Modified: Wed, 01 Nov 2023 02:38:10 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea95f18650ed3a1953cdc6a38b99484c60f73650806946b859560a67c137ae15`  
		Last Modified: Wed, 01 Nov 2023 02:38:10 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11-meta-alpine`

```console
$ docker pull influxdb@sha256:21192c610d5ed75d31095eadae94494891ee2268f40eb90abf350bcbb8fd88ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:1d112501c3c846cf26b990267cd073e313f761cc68bde5c1039745981e8137a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25099495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e63e124b0a32c5b678f94b576f72bcd1922f74973af5e08fe99a74452ef1f8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:30:37 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:30:38 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 17 Oct 2023 01:30:38 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Tue, 17 Oct 2023 01:31:02 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 17 Oct 2023 01:31:02 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 17 Oct 2023 01:31:02 GMT
EXPOSE 8091
# Tue, 17 Oct 2023 01:31:03 GMT
VOLUME [/var/lib/influxdb]
# Tue, 17 Oct 2023 01:31:03 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 17 Oct 2023 01:31:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Oct 2023 01:31:03 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5352bf3aec614dde8ac36d38f28f5021eff4c2ff0226eb22dfa667f2b2add1`  
		Last Modified: Tue, 17 Oct 2023 01:33:20 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0165a81397bc8c25031ed159801827c4fc37f5dba045ffd5bd32eeb6590ba`  
		Last Modified: Tue, 17 Oct 2023 01:33:18 GMT  
		Size: 1.4 MB (1407328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b75e8ab43c763fb6aa84d8c1e00f3936b2de4cb4a22224e85c96803274c0b19`  
		Last Modified: Tue, 17 Oct 2023 01:33:51 GMT  
		Size: 20.3 MB (20289325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b3beaea8b1c51930ec5853c23da81e6c3c8765ba085b28255213b3bedc71dd`  
		Last Modified: Tue, 17 Oct 2023 01:33:47 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e662f1436b64a817e96ca5ed1c6bae41a4b56321158903bc2ce93b432df76cde`  
		Last Modified: Tue, 17 Oct 2023 01:33:47 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.3-data`

```console
$ docker pull influxdb@sha256:af8377b323ee74736982960b27d80214c9bce1bc8db36aa7319f0ec289313088
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.3-data` - linux; amd64

```console
$ docker pull influxdb@sha256:02c9970f1a1e456215f124e97d204d1eb8e7ebb01a4d61ced0351a1638cb4e1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.8 MB (113809290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4738c5bd6f0add12d8f89d014369e1b5b6d35a33f8bc5bb891c9ab5ad076a4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:35:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:37 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Wed, 01 Nov 2023 02:35:41 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb*
# Wed, 01 Nov 2023 02:35:41 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 01 Nov 2023 02:35:41 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:35:41 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:41 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:41 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 01 Nov 2023 02:35:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b15edd27da99dfcc4a562fa21353856b433f3d088be84034b0d200e70adc63`  
		Last Modified: Wed, 01 Nov 2023 02:37:55 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e60eff18a916a66e0e81c141b72cdb59898ef7f710c3823641857da3eb016d`  
		Last Modified: Wed, 01 Nov 2023 02:38:01 GMT  
		Size: 40.2 MB (40174531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af825ccfbe379294f660b4ac6f4adae299c5175b85ed9d52e4757fc0f583f8ec`  
		Last Modified: Wed, 01 Nov 2023 02:37:55 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0218e4766a75cd240d0415b939d7b336a951381f0c7bffbcec9c5672a8275d`  
		Last Modified: Wed, 01 Nov 2023 02:37:54 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a723e9fe0bab63d1244255db1fa4c6f47681d24841e09d3278153771085e97`  
		Last Modified: Wed, 01 Nov 2023 02:37:55 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.3-data-alpine`

```console
$ docker pull influxdb@sha256:dd29ecf0082bf579438a79ca407cb00af0ccea1314b3a201167390b84106c48d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.3-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ea80cb2d0884ee4b48b30af9d76e6ce0558a700f0d53a4b22aa85a27b1c37d96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44943078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4eb53fe3ea56cd4a6e578cd107b997e52162a7cf2281bdc6a4aa4f4e0f51631`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:30:37 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:30:38 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 17 Oct 2023 01:30:38 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Tue, 17 Oct 2023 01:30:46 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 17 Oct 2023 01:30:46 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 17 Oct 2023 01:30:46 GMT
EXPOSE 8086
# Tue, 17 Oct 2023 01:30:46 GMT
VOLUME [/var/lib/influxdb]
# Tue, 17 Oct 2023 01:30:47 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 17 Oct 2023 01:30:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 17 Oct 2023 01:30:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Oct 2023 01:30:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5352bf3aec614dde8ac36d38f28f5021eff4c2ff0226eb22dfa667f2b2add1`  
		Last Modified: Tue, 17 Oct 2023 01:33:20 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0165a81397bc8c25031ed159801827c4fc37f5dba045ffd5bd32eeb6590ba`  
		Last Modified: Tue, 17 Oct 2023 01:33:18 GMT  
		Size: 1.4 MB (1407328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ff88a3565b599c0999572689b7ada926cd541f29a53748f076a1a4e428cf5c`  
		Last Modified: Tue, 17 Oct 2023 01:33:24 GMT  
		Size: 40.1 MB (40131704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd1384bec94ee9e6e672aa3fc7f67ed54cb4b8e0c9c9dd26ac83a0f753f5bd`  
		Last Modified: Tue, 17 Oct 2023 01:33:18 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaaaaea04c9cdf8e607c822cb85d5395086d8816921a964cb68acd8241726b9`  
		Last Modified: Tue, 17 Oct 2023 01:33:18 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31395564ab00aa4757a9a8d575593323885e42a4292aaca5a7aea4901459878b`  
		Last Modified: Tue, 17 Oct 2023 01:33:18 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.3-meta`

```console
$ docker pull influxdb@sha256:23ed1c7dc3a1e7ec91e7cdcf331b1e971382e20ca90326e51ee05aaf03aed764
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.3-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:5e1de343c2d3b7df14c07b212c9f121991fa526473dda9e61a9d9b8fc4680b77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (93960917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e682867e1e05d4ec47778ad813cb5908d8e70a313d7439c69b8f276e14ca576`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:35:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:37 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Wed, 01 Nov 2023 02:35:49 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb*
# Wed, 01 Nov 2023 02:35:50 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 01 Nov 2023 02:35:50 GMT
EXPOSE 8091
# Wed, 01 Nov 2023 02:35:50 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:50 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:50 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b15edd27da99dfcc4a562fa21353856b433f3d088be84034b0d200e70adc63`  
		Last Modified: Wed, 01 Nov 2023 02:37:55 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7063c8c1622de4ab01288e46ab10496452403319fdb371e739f73021e097fd6`  
		Last Modified: Wed, 01 Nov 2023 02:38:14 GMT  
		Size: 20.3 MB (20327364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3008bc9d51b12c0f9defa58b998fce1e4384cae7403d4d8e880c03e868ef5221`  
		Last Modified: Wed, 01 Nov 2023 02:38:10 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea95f18650ed3a1953cdc6a38b99484c60f73650806946b859560a67c137ae15`  
		Last Modified: Wed, 01 Nov 2023 02:38:10 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.11.3-meta-alpine`

```console
$ docker pull influxdb@sha256:21192c610d5ed75d31095eadae94494891ee2268f40eb90abf350bcbb8fd88ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.3-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:1d112501c3c846cf26b990267cd073e313f761cc68bde5c1039745981e8137a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25099495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e63e124b0a32c5b678f94b576f72bcd1922f74973af5e08fe99a74452ef1f8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:30:37 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:30:38 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 17 Oct 2023 01:30:38 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Tue, 17 Oct 2023 01:31:02 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 17 Oct 2023 01:31:02 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 17 Oct 2023 01:31:02 GMT
EXPOSE 8091
# Tue, 17 Oct 2023 01:31:03 GMT
VOLUME [/var/lib/influxdb]
# Tue, 17 Oct 2023 01:31:03 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 17 Oct 2023 01:31:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Oct 2023 01:31:03 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5352bf3aec614dde8ac36d38f28f5021eff4c2ff0226eb22dfa667f2b2add1`  
		Last Modified: Tue, 17 Oct 2023 01:33:20 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0165a81397bc8c25031ed159801827c4fc37f5dba045ffd5bd32eeb6590ba`  
		Last Modified: Tue, 17 Oct 2023 01:33:18 GMT  
		Size: 1.4 MB (1407328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b75e8ab43c763fb6aa84d8c1e00f3936b2de4cb4a22224e85c96803274c0b19`  
		Last Modified: Tue, 17 Oct 2023 01:33:51 GMT  
		Size: 20.3 MB (20289325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b3beaea8b1c51930ec5853c23da81e6c3c8765ba085b28255213b3bedc71dd`  
		Last Modified: Tue, 17 Oct 2023 01:33:47 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e662f1436b64a817e96ca5ed1c6bae41a4b56321158903bc2ce93b432df76cde`  
		Last Modified: Tue, 17 Oct 2023 01:33:47 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:da78dac8ee0dce55682dee13fc207de2cf086b618bc0ddaa945861860e46efa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:2bdb3a557864a3f7bc7be971ff1e355e0c8b87bf9c3586aadecd3c34c9c56bc5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125711558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f93b04c553e324af1781ca74a09b5fa1711f0ee4eef8098abbaea52b16c68`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:34:51 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 01 Nov 2023 02:34:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 01 Nov 2023 02:34:55 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 01 Nov 2023 02:34:55 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:34:55 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:34:55 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:34:56 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 01 Nov 2023 02:34:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:34:56 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469105de3319d3732d5d45b2577dd8bbb5a67a20c5f158e7a8d97e07b9c4063b`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdad387b329047304e8812566c42f4433f653a63ffa47242f9b5985c4427f1c3`  
		Last Modified: Wed, 01 Nov 2023 02:36:50 GMT  
		Size: 54.9 MB (54885762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b6af5df828ff786198caa94e15c1478eec62864bd5ff9e4e068d7ab8d93899`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20272ddaf2bf8aa01b23207c163be482dacd6b66798f4c99bfcafebad73d64be`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70894489304866ca8a1bed136fba77ec5195c57225c6c5b95adbbf563d453dae`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:c6a492d1da4168bbbdb0f57115ff22d6676b9981308a2736934926c6f477efa3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116712100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e134d5a1a37c5472bd78347a3a7cb2ab82e00ef38183b89b307dac5cd77abd60`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 09:28:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 12 Oct 2023 09:28:56 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 12 Oct 2023 09:29:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 12 Oct 2023 09:29:06 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 12 Oct 2023 09:29:06 GMT
EXPOSE 8086
# Thu, 12 Oct 2023 09:29:06 GMT
VOLUME [/var/lib/influxdb]
# Thu, 12 Oct 2023 09:29:06 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 12 Oct 2023 09:29:06 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 12 Oct 2023 09:29:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 09:29:07 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe33e05af9470f2356c8047560fded363dda4990bb2d70e9194f0dca496bb82`  
		Last Modified: Thu, 12 Oct 2023 03:57:11 GMT  
		Size: 14.9 MB (14879720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855c4fd3897115bfd9a2c87eae6e75d92fd5740a2487d4d1d94f3f926579f0d6`  
		Last Modified: Thu, 12 Oct 2023 09:29:13 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2324472b77a049e43be5308a51cb7079c54b03495c1c6b592b81b1159a2658cf`  
		Last Modified: Thu, 12 Oct 2023 09:29:20 GMT  
		Size: 51.6 MB (51613155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e31cf85d5e438988d0dee6c90500c8df2933395d625b23d878bf68a15a07af7`  
		Last Modified: Thu, 12 Oct 2023 09:29:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97e78981f2a685c2f840f7cfb5768d1b3859f2f439e93b9f1539ccb2272511b`  
		Last Modified: Thu, 12 Oct 2023 09:29:13 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1244d97456b616cede3afdc7ea0462f35265220b30fb6fc023c05ac74925329c`  
		Last Modified: Thu, 12 Oct 2023 09:29:13 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a3b326260795ca977e78223dc1abb5338d771f194bf2c2a69527e75a41401318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120691221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067cb5df06564b9d54ae8eebd7ad4951219abc4e9e8ca0f0faf1007fe8e483e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:48 GMT
ADD file:f5677286e85ce6a345c7f5937e1ec576c37228e49c0fafe33574614c81cb7f76 in / 
# Wed, 01 Nov 2023 00:39:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:06:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:01:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 03:01:47 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 01 Nov 2023 03:01:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 01 Nov 2023 03:01:52 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 01 Nov 2023 03:01:52 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 03:01:52 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 03:01:52 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 01 Nov 2023 03:01:52 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 01 Nov 2023 03:01:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 03:01:52 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d42ebdfc37acca5c3acbe173ac11133e691b402003a525c2b8431baf6935291e`  
		Last Modified: Wed, 01 Nov 2023 00:43:25 GMT  
		Size: 53.7 MB (53707757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bcc814ee5bafa2842bc45ecc3974bc4f2b66d05b05a8da5ac0c9fb91be947`  
		Last Modified: Wed, 01 Nov 2023 02:14:42 GMT  
		Size: 15.7 MB (15749872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847519f5e3f897501eb1a418c2317f94ac107ad7b62d8f28a72dbcb1582ffa70`  
		Last Modified: Wed, 01 Nov 2023 03:02:28 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235d6390a6e7d18674a529ced6e9f82db576f4a4eb580bb73390aace3ef43247`  
		Last Modified: Wed, 01 Nov 2023 03:02:33 GMT  
		Size: 51.2 MB (51230061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c7f4b19a5d5d29365641d0f8f3497d587a8301a036862379fca8f5edab4c5e`  
		Last Modified: Wed, 01 Nov 2023 03:02:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629472df44451d64a3cbddb9637e6ccf6d185602376a71e734459c734d679bed`  
		Last Modified: Wed, 01 Nov 2023 03:02:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55d1eca6fcf30f49bf28d94d19c655cd80f5ebbfc576bdac813de909fd71063`  
		Last Modified: Wed, 01 Nov 2023 03:02:28 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:28aa5d804d36089d624bddf37c16383f32b30888efe85922b1708667ab333626
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:75a44429c9b676cfd7ab26a41dcbee99625b430329b1b887db0892bb957901e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59499783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0885b5ae3f605f567b68faff2a5b313c727edc34aa72d452c74e1dac9431d92c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:29:21 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:29:23 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 17 Oct 2023 01:29:23 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 17 Oct 2023 01:29:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 17 Oct 2023 01:29:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 17 Oct 2023 01:29:30 GMT
EXPOSE 8086
# Tue, 17 Oct 2023 01:29:30 GMT
VOLUME [/var/lib/influxdb]
# Tue, 17 Oct 2023 01:29:30 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 17 Oct 2023 01:29:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 17 Oct 2023 01:29:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Oct 2023 01:29:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b161763ec9e11116a97547438c5541153248aba5eddc76475885813812367da`  
		Last Modified: Tue, 17 Oct 2023 01:31:50 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d3938b55c32749418ec88153e08d27efa36f373c1b5b150ee9bb2d1e44c03`  
		Last Modified: Tue, 17 Oct 2023 01:31:49 GMT  
		Size: 1.5 MB (1472471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7b44c92245f1274b5a6cf82c994751409a4e30c97857bf05c38589646aa752`  
		Last Modified: Tue, 17 Oct 2023 01:31:55 GMT  
		Size: 54.6 MB (54646685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1389282976594e9351f4df9741199697eecd901277efcb68579eb5c4e9e60dea`  
		Last Modified: Tue, 17 Oct 2023 01:31:48 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff4fc132f81a16403c1340d80a78aee9e0509bb194e314e2a1caeef795490eb`  
		Last Modified: Tue, 17 Oct 2023 01:31:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e118ae4fcd7a1c8378c5ff219f07c8c8b188f0b53e9b141c62bee9d68aadee`  
		Last Modified: Tue, 17 Oct 2023 01:31:48 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10`

```console
$ docker pull influxdb@sha256:da78dac8ee0dce55682dee13fc207de2cf086b618bc0ddaa945861860e46efa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:2bdb3a557864a3f7bc7be971ff1e355e0c8b87bf9c3586aadecd3c34c9c56bc5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125711558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f93b04c553e324af1781ca74a09b5fa1711f0ee4eef8098abbaea52b16c68`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:34:51 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 01 Nov 2023 02:34:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 01 Nov 2023 02:34:55 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 01 Nov 2023 02:34:55 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:34:55 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:34:55 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:34:56 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 01 Nov 2023 02:34:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:34:56 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469105de3319d3732d5d45b2577dd8bbb5a67a20c5f158e7a8d97e07b9c4063b`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdad387b329047304e8812566c42f4433f653a63ffa47242f9b5985c4427f1c3`  
		Last Modified: Wed, 01 Nov 2023 02:36:50 GMT  
		Size: 54.9 MB (54885762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b6af5df828ff786198caa94e15c1478eec62864bd5ff9e4e068d7ab8d93899`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20272ddaf2bf8aa01b23207c163be482dacd6b66798f4c99bfcafebad73d64be`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70894489304866ca8a1bed136fba77ec5195c57225c6c5b95adbbf563d453dae`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:c6a492d1da4168bbbdb0f57115ff22d6676b9981308a2736934926c6f477efa3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116712100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e134d5a1a37c5472bd78347a3a7cb2ab82e00ef38183b89b307dac5cd77abd60`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 09:28:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 12 Oct 2023 09:28:56 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 12 Oct 2023 09:29:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 12 Oct 2023 09:29:06 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 12 Oct 2023 09:29:06 GMT
EXPOSE 8086
# Thu, 12 Oct 2023 09:29:06 GMT
VOLUME [/var/lib/influxdb]
# Thu, 12 Oct 2023 09:29:06 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 12 Oct 2023 09:29:06 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 12 Oct 2023 09:29:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 09:29:07 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe33e05af9470f2356c8047560fded363dda4990bb2d70e9194f0dca496bb82`  
		Last Modified: Thu, 12 Oct 2023 03:57:11 GMT  
		Size: 14.9 MB (14879720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855c4fd3897115bfd9a2c87eae6e75d92fd5740a2487d4d1d94f3f926579f0d6`  
		Last Modified: Thu, 12 Oct 2023 09:29:13 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2324472b77a049e43be5308a51cb7079c54b03495c1c6b592b81b1159a2658cf`  
		Last Modified: Thu, 12 Oct 2023 09:29:20 GMT  
		Size: 51.6 MB (51613155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e31cf85d5e438988d0dee6c90500c8df2933395d625b23d878bf68a15a07af7`  
		Last Modified: Thu, 12 Oct 2023 09:29:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97e78981f2a685c2f840f7cfb5768d1b3859f2f439e93b9f1539ccb2272511b`  
		Last Modified: Thu, 12 Oct 2023 09:29:13 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1244d97456b616cede3afdc7ea0462f35265220b30fb6fc023c05ac74925329c`  
		Last Modified: Thu, 12 Oct 2023 09:29:13 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a3b326260795ca977e78223dc1abb5338d771f194bf2c2a69527e75a41401318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120691221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067cb5df06564b9d54ae8eebd7ad4951219abc4e9e8ca0f0faf1007fe8e483e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:48 GMT
ADD file:f5677286e85ce6a345c7f5937e1ec576c37228e49c0fafe33574614c81cb7f76 in / 
# Wed, 01 Nov 2023 00:39:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:06:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:01:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 03:01:47 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 01 Nov 2023 03:01:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 01 Nov 2023 03:01:52 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 01 Nov 2023 03:01:52 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 03:01:52 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 03:01:52 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 01 Nov 2023 03:01:52 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 01 Nov 2023 03:01:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 03:01:52 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d42ebdfc37acca5c3acbe173ac11133e691b402003a525c2b8431baf6935291e`  
		Last Modified: Wed, 01 Nov 2023 00:43:25 GMT  
		Size: 53.7 MB (53707757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bcc814ee5bafa2842bc45ecc3974bc4f2b66d05b05a8da5ac0c9fb91be947`  
		Last Modified: Wed, 01 Nov 2023 02:14:42 GMT  
		Size: 15.7 MB (15749872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847519f5e3f897501eb1a418c2317f94ac107ad7b62d8f28a72dbcb1582ffa70`  
		Last Modified: Wed, 01 Nov 2023 03:02:28 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235d6390a6e7d18674a529ced6e9f82db576f4a4eb580bb73390aace3ef43247`  
		Last Modified: Wed, 01 Nov 2023 03:02:33 GMT  
		Size: 51.2 MB (51230061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c7f4b19a5d5d29365641d0f8f3497d587a8301a036862379fca8f5edab4c5e`  
		Last Modified: Wed, 01 Nov 2023 03:02:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629472df44451d64a3cbddb9637e6ccf6d185602376a71e734459c734d679bed`  
		Last Modified: Wed, 01 Nov 2023 03:02:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55d1eca6fcf30f49bf28d94d19c655cd80f5ebbfc576bdac813de909fd71063`  
		Last Modified: Wed, 01 Nov 2023 03:02:28 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-alpine`

```console
$ docker pull influxdb@sha256:28aa5d804d36089d624bddf37c16383f32b30888efe85922b1708667ab333626
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:75a44429c9b676cfd7ab26a41dcbee99625b430329b1b887db0892bb957901e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59499783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0885b5ae3f605f567b68faff2a5b313c727edc34aa72d452c74e1dac9431d92c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:29:21 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:29:23 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 17 Oct 2023 01:29:23 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 17 Oct 2023 01:29:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     chmod +x /usr/src/influxdb-*/influx              /usr/src/influxdb-*/influx_inspect              /usr/src/influxdb-*/influx_stress              /usr/src/influxdb-*/influxd &&    mv /usr/src/influxdb-*/influx        /usr/src/influxdb-*/influx_inspect        /usr/src/influxdb-*/influx_stress         /usr/src/influxdb-*/influxd        /usr/bin/ &&    gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 17 Oct 2023 01:29:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 17 Oct 2023 01:29:30 GMT
EXPOSE 8086
# Tue, 17 Oct 2023 01:29:30 GMT
VOLUME [/var/lib/influxdb]
# Tue, 17 Oct 2023 01:29:30 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 17 Oct 2023 01:29:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 17 Oct 2023 01:29:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Oct 2023 01:29:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b161763ec9e11116a97547438c5541153248aba5eddc76475885813812367da`  
		Last Modified: Tue, 17 Oct 2023 01:31:50 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d3938b55c32749418ec88153e08d27efa36f373c1b5b150ee9bb2d1e44c03`  
		Last Modified: Tue, 17 Oct 2023 01:31:49 GMT  
		Size: 1.5 MB (1472471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7b44c92245f1274b5a6cf82c994751409a4e30c97857bf05c38589646aa752`  
		Last Modified: Tue, 17 Oct 2023 01:31:55 GMT  
		Size: 54.6 MB (54646685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1389282976594e9351f4df9741199697eecd901277efcb68579eb5c4e9e60dea`  
		Last Modified: Tue, 17 Oct 2023 01:31:48 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff4fc132f81a16403c1340d80a78aee9e0509bb194e314e2a1caeef795490eb`  
		Last Modified: Tue, 17 Oct 2023 01:31:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e118ae4fcd7a1c8378c5ff219f07c8c8b188f0b53e9b141c62bee9d68aadee`  
		Last Modified: Tue, 17 Oct 2023 01:31:48 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data`

```console
$ docker pull influxdb@sha256:7fcee3e49789437bbd92685d71753acc6199144264c06cf0c9358fa361f5caf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:fd2f221cdbe795af62fa07d8873eb92a492d29904469e3668edc34b5a5623488
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104114945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:647e089ddc6ab1885b1f343e99fb95dbcf7bb949dc44ec9f3ef7165a1da36cc0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:01 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Wed, 01 Nov 2023 02:35:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 01 Nov 2023 02:35:05 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 01 Nov 2023 02:35:05 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:35:05 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:05 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:05 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 01 Nov 2023 02:35:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:05 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469105de3319d3732d5d45b2577dd8bbb5a67a20c5f158e7a8d97e07b9c4063b`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d539382bffdc98d227f856678c1ff532ebeba47a9486a46f3956a7256e74f058`  
		Last Modified: Wed, 01 Nov 2023 02:37:05 GMT  
		Size: 33.3 MB (33289092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f22a5ef2bb99aa35c7a25318aad87ada4eda2476a94187c90976517c7252b`  
		Last Modified: Wed, 01 Nov 2023 02:36:59 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c587c47c3988d512589e5e046bacbcc2bb07a0b22c256e07b32dc7b917fdf153`  
		Last Modified: Wed, 01 Nov 2023 02:36:59 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb69329aa567c8a5e59df7f21751803ee050fb54b1ec6fb9ef5b5f9e8da8c09`  
		Last Modified: Wed, 01 Nov 2023 02:36:59 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:3255fa311d73664ad4c6f386cb68704baf271e36fa9b9acd75903475ec3df11c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:271f51b2a29798f656f5094bfa99d9f5190192952ece2e6220ae85bbe7d4d885
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38101831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef6dc0cf6790e6427bb4484e9b48e4b6ec7c7083d11d123e2d6705793fa4be6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:29:21 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:29:23 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 18 Oct 2023 00:21:52 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Wed, 18 Oct 2023 00:21:57 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 18 Oct 2023 00:21:57 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 18 Oct 2023 00:21:57 GMT
EXPOSE 8086
# Wed, 18 Oct 2023 00:21:57 GMT
VOLUME [/var/lib/influxdb]
# Wed, 18 Oct 2023 00:21:57 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 18 Oct 2023 00:21:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 18 Oct 2023 00:21:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Oct 2023 00:21:58 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b161763ec9e11116a97547438c5541153248aba5eddc76475885813812367da`  
		Last Modified: Tue, 17 Oct 2023 01:31:50 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d3938b55c32749418ec88153e08d27efa36f373c1b5b150ee9bb2d1e44c03`  
		Last Modified: Tue, 17 Oct 2023 01:31:49 GMT  
		Size: 1.5 MB (1472471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19733dee640ef65939bb0f4eb679d9a3824b115a74f158a387c94e66796df71d`  
		Last Modified: Wed, 18 Oct 2023 00:23:54 GMT  
		Size: 33.2 MB (33248677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41596727af6002e44f580e57e9ce9363aa43317bb9845d78157fa25a5151aca1`  
		Last Modified: Wed, 18 Oct 2023 00:23:49 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e87af7d3cec7c4d99e4c41e43daee82bf4fbcfab8a109f1e14235475ba24593`  
		Last Modified: Wed, 18 Oct 2023 00:23:49 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b7eb53ce4443a1b6f438fd48c0c0d92ac9956ca98118bb167e803ff6007674`  
		Last Modified: Wed, 18 Oct 2023 00:23:49 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:b79951fc5044bbd5a1ac6721f5f00a0adbd397fdf287e2dc9e9a55d24499ce92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:d8490916f66a58ebd1dab485461baa5c7c28dc0cbe87dfb91f848e9ab10a8f8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83594442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27a61ae7ebd7a0c002e2724d0584a32024d03a50ea977f3c6093c70affede2a4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:01 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Wed, 01 Nov 2023 02:35:12 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 01 Nov 2023 02:35:12 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 01 Nov 2023 02:35:12 GMT
EXPOSE 8091
# Wed, 01 Nov 2023 02:35:12 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:13 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:13 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469105de3319d3732d5d45b2577dd8bbb5a67a20c5f158e7a8d97e07b9c4063b`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e419816648a4c896df65016c711faf0e6c7eeee6998ef4943cde6c6040a06b`  
		Last Modified: Wed, 01 Nov 2023 02:37:16 GMT  
		Size: 12.8 MB (12769796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695f6e901a2caac2d2d5c47dbdc1d15dc1c7745dd05d2908b24cccd633dd1b98`  
		Last Modified: Wed, 01 Nov 2023 02:37:14 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32476c85b0e39a626dd5113e7539df98f69cc5283a232b17f23ed0b8798742c7`  
		Last Modified: Wed, 01 Nov 2023 02:37:14 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:d011eb9d31771aa655dc175009baf2067cb7d6b54a25f35f4c623007a84f83d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:390a320590b6f04854506526ce7b05525d9bfb6c2bf64f959948f36d9946ddbc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17586148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e0728481f74e448417005c44dab4d279656c1143c31479696a6b02b134b0b48`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:29:21 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:29:23 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 18 Oct 2023 00:21:52 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Wed, 18 Oct 2023 00:22:11 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 18 Oct 2023 00:22:12 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 18 Oct 2023 00:22:12 GMT
EXPOSE 8091
# Wed, 18 Oct 2023 00:22:12 GMT
VOLUME [/var/lib/influxdb]
# Wed, 18 Oct 2023 00:22:12 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 18 Oct 2023 00:22:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Oct 2023 00:22:12 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b161763ec9e11116a97547438c5541153248aba5eddc76475885813812367da`  
		Last Modified: Tue, 17 Oct 2023 01:31:50 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d3938b55c32749418ec88153e08d27efa36f373c1b5b150ee9bb2d1e44c03`  
		Last Modified: Tue, 17 Oct 2023 01:31:49 GMT  
		Size: 1.5 MB (1472471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49de28ed382fb4f08367907c0244b7020fbfbaa351bdd5d52aba54a54ee6d71c`  
		Last Modified: Wed, 18 Oct 2023 00:24:18 GMT  
		Size: 12.7 MB (12734196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee6b7737009168910c0beffc25ebc9d5e68c1c53e032a19dcaf88e493020391`  
		Last Modified: Wed, 18 Oct 2023 00:24:16 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c694141440b42bc6f1848f6119c5df52a9b243573707318f592c491e9a25448`  
		Last Modified: Wed, 18 Oct 2023 00:24:16 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.13-data`

```console
$ docker pull influxdb@sha256:7fcee3e49789437bbd92685d71753acc6199144264c06cf0c9358fa361f5caf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.13-data` - linux; amd64

```console
$ docker pull influxdb@sha256:fd2f221cdbe795af62fa07d8873eb92a492d29904469e3668edc34b5a5623488
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104114945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:647e089ddc6ab1885b1f343e99fb95dbcf7bb949dc44ec9f3ef7165a1da36cc0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:01 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Wed, 01 Nov 2023 02:35:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 01 Nov 2023 02:35:05 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 01 Nov 2023 02:35:05 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:35:05 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:05 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:05 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 01 Nov 2023 02:35:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:05 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469105de3319d3732d5d45b2577dd8bbb5a67a20c5f158e7a8d97e07b9c4063b`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d539382bffdc98d227f856678c1ff532ebeba47a9486a46f3956a7256e74f058`  
		Last Modified: Wed, 01 Nov 2023 02:37:05 GMT  
		Size: 33.3 MB (33289092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79f22a5ef2bb99aa35c7a25318aad87ada4eda2476a94187c90976517c7252b`  
		Last Modified: Wed, 01 Nov 2023 02:36:59 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c587c47c3988d512589e5e046bacbcc2bb07a0b22c256e07b32dc7b917fdf153`  
		Last Modified: Wed, 01 Nov 2023 02:36:59 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb69329aa567c8a5e59df7f21751803ee050fb54b1ec6fb9ef5b5f9e8da8c09`  
		Last Modified: Wed, 01 Nov 2023 02:36:59 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.13-data-alpine`

```console
$ docker pull influxdb@sha256:3255fa311d73664ad4c6f386cb68704baf271e36fa9b9acd75903475ec3df11c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.13-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:271f51b2a29798f656f5094bfa99d9f5190192952ece2e6220ae85bbe7d4d885
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38101831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef6dc0cf6790e6427bb4484e9b48e4b6ec7c7083d11d123e2d6705793fa4be6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:29:21 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:29:23 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 18 Oct 2023 00:21:52 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Wed, 18 Oct 2023 00:21:57 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 18 Oct 2023 00:21:57 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 18 Oct 2023 00:21:57 GMT
EXPOSE 8086
# Wed, 18 Oct 2023 00:21:57 GMT
VOLUME [/var/lib/influxdb]
# Wed, 18 Oct 2023 00:21:57 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 18 Oct 2023 00:21:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 18 Oct 2023 00:21:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Oct 2023 00:21:58 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b161763ec9e11116a97547438c5541153248aba5eddc76475885813812367da`  
		Last Modified: Tue, 17 Oct 2023 01:31:50 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d3938b55c32749418ec88153e08d27efa36f373c1b5b150ee9bb2d1e44c03`  
		Last Modified: Tue, 17 Oct 2023 01:31:49 GMT  
		Size: 1.5 MB (1472471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19733dee640ef65939bb0f4eb679d9a3824b115a74f158a387c94e66796df71d`  
		Last Modified: Wed, 18 Oct 2023 00:23:54 GMT  
		Size: 33.2 MB (33248677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41596727af6002e44f580e57e9ce9363aa43317bb9845d78157fa25a5151aca1`  
		Last Modified: Wed, 18 Oct 2023 00:23:49 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e87af7d3cec7c4d99e4c41e43daee82bf4fbcfab8a109f1e14235475ba24593`  
		Last Modified: Wed, 18 Oct 2023 00:23:49 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b7eb53ce4443a1b6f438fd48c0c0d92ac9956ca98118bb167e803ff6007674`  
		Last Modified: Wed, 18 Oct 2023 00:23:49 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.13-meta`

```console
$ docker pull influxdb@sha256:b79951fc5044bbd5a1ac6721f5f00a0adbd397fdf287e2dc9e9a55d24499ce92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.13-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:d8490916f66a58ebd1dab485461baa5c7c28dc0cbe87dfb91f848e9ab10a8f8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83594442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27a61ae7ebd7a0c002e2724d0584a32024d03a50ea977f3c6093c70affede2a4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Nov 2023 02:35:01 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Wed, 01 Nov 2023 02:35:12 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 01 Nov 2023 02:35:12 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 01 Nov 2023 02:35:12 GMT
EXPOSE 8091
# Wed, 01 Nov 2023 02:35:12 GMT
VOLUME [/var/lib/influxdb]
# Wed, 01 Nov 2023 02:35:13 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:35:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:35:13 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469105de3319d3732d5d45b2577dd8bbb5a67a20c5f158e7a8d97e07b9c4063b`  
		Last Modified: Wed, 01 Nov 2023 02:36:43 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e419816648a4c896df65016c711faf0e6c7eeee6998ef4943cde6c6040a06b`  
		Last Modified: Wed, 01 Nov 2023 02:37:16 GMT  
		Size: 12.8 MB (12769796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695f6e901a2caac2d2d5c47dbdc1d15dc1c7745dd05d2908b24cccd633dd1b98`  
		Last Modified: Wed, 01 Nov 2023 02:37:14 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32476c85b0e39a626dd5113e7539df98f69cc5283a232b17f23ed0b8798742c7`  
		Last Modified: Wed, 01 Nov 2023 02:37:14 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.13-meta-alpine`

```console
$ docker pull influxdb@sha256:d011eb9d31771aa655dc175009baf2067cb7d6b54a25f35f4c623007a84f83d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.13-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:390a320590b6f04854506526ce7b05525d9bfb6c2bf64f959948f36d9946ddbc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17586148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e0728481f74e448417005c44dab4d279656c1143c31479696a6b02b134b0b48`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:29:21 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:29:23 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 18 Oct 2023 00:21:52 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Wed, 18 Oct 2023 00:22:11 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/etc/influxdb/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/usr/bin/* &&     cp -a /usr/src/influxdb-*/usr/bin/. /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 18 Oct 2023 00:22:12 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 18 Oct 2023 00:22:12 GMT
EXPOSE 8091
# Wed, 18 Oct 2023 00:22:12 GMT
VOLUME [/var/lib/influxdb]
# Wed, 18 Oct 2023 00:22:12 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 18 Oct 2023 00:22:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Oct 2023 00:22:12 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b161763ec9e11116a97547438c5541153248aba5eddc76475885813812367da`  
		Last Modified: Tue, 17 Oct 2023 01:31:50 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d3938b55c32749418ec88153e08d27efa36f373c1b5b150ee9bb2d1e44c03`  
		Last Modified: Tue, 17 Oct 2023 01:31:49 GMT  
		Size: 1.5 MB (1472471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49de28ed382fb4f08367907c0244b7020fbfbaa351bdd5d52aba54a54ee6d71c`  
		Last Modified: Wed, 18 Oct 2023 00:24:18 GMT  
		Size: 12.7 MB (12734196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee6b7737009168910c0beffc25ebc9d5e68c1c53e032a19dcaf88e493020391`  
		Last Modified: Wed, 18 Oct 2023 00:24:16 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c694141440b42bc6f1848f6119c5df52a9b243573707318f592c491e9a25448`  
		Last Modified: Wed, 18 Oct 2023 00:24:16 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7`

```console
$ docker pull influxdb@sha256:5973b7698a7a8fddf60eca9c44077b062abb133aecfb193ec279ba2eeff253cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7` - linux; amd64

```console
$ docker pull influxdb@sha256:f02325b07c1105549c1e3099343f8cf8724497995b4795c5a1e0ddf5bd76fccf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.2 MB (162170896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165ce29e04361e963410915a225e528ec623101f733ba6196c7148947c9f4ecf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:49 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
# Wed, 01 Nov 2023 00:20:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:02 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:36:04 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 01 Nov 2023 02:36:05 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 01 Nov 2023 02:36:05 GMT
ENV GOSU_VER=1.12
# Wed, 01 Nov 2023 02:36:07 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 01 Nov 2023 02:36:07 GMT
ENV INFLUXDB_VERSION=2.7.3
# Wed, 01 Nov 2023 02:36:12 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 01 Nov 2023 02:36:12 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 01 Nov 2023 02:36:14 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 01 Nov 2023 02:36:15 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 01 Nov 2023 02:36:15 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 01 Nov 2023 02:36:15 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 01 Nov 2023 02:36:15 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:36:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:36:15 GMT
CMD ["influxd"]
# Wed, 01 Nov 2023 02:36:15 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:36:15 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 01 Nov 2023 02:36:16 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 01 Nov 2023 02:36:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 01 Nov 2023 02:36:16 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbcf0a0fd4f60b8f415999c5c7c9d499b5e065fc620ececfb9a9c50d925559b`  
		Last Modified: Wed, 01 Nov 2023 02:38:29 GMT  
		Size: 9.8 MB (9787149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc30a15212abb09190c168b0bfc858f7682098ef77f765b1b19158189864dfe3`  
		Last Modified: Wed, 01 Nov 2023 02:38:26 GMT  
		Size: 6.4 MB (6434099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159c705faba476f2d587c2b39871193bed7bbacd328eee135c265a65f3dc83f9`  
		Last Modified: Wed, 01 Nov 2023 02:38:25 GMT  
		Size: 3.3 KB (3281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d00aeef48a00456bd46e972f3c131543fd90b1d48c6fb6ff6934725e515d87`  
		Last Modified: Wed, 01 Nov 2023 02:38:25 GMT  
		Size: 986.0 KB (985995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c836d6efdfbcc4e1b254e82930240d4d4a638a95888229331e5322b9e778470`  
		Last Modified: Wed, 01 Nov 2023 02:38:33 GMT  
		Size: 92.7 MB (92675041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:979326e5d1b2d6f77813a9660d6d7f9d944a4787ed617053396d81a447bafc54`  
		Last Modified: Wed, 01 Nov 2023 02:38:26 GMT  
		Size: 23.1 MB (23128348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5797dc5b6cab1afb3734b6a1696fc3623e38f371fbace58f775402723df55c`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10179fcb509a5aeaf267fb8c50ce26d13a4da438fbfa3171be4b60ec97e92f09`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eff5c0be8ad19f7a47f14b95ce6e892461edf952e3932a02684e53e9c3f234d`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9a9d2ad170926a8880b35ade12fc7d226e688dda525331bd0a6f4117d807aaad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156471359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4209d6dee09892d6c679bc2479aaa59b63ff870a32188a3dd612ddd804967d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:41 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 01 Nov 2023 00:39:41 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 03:02:01 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:02:02 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 01 Nov 2023 03:02:03 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 01 Nov 2023 03:02:03 GMT
ENV GOSU_VER=1.12
# Wed, 01 Nov 2023 03:02:05 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 01 Nov 2023 03:02:05 GMT
ENV INFLUXDB_VERSION=2.7.3
# Wed, 01 Nov 2023 03:02:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 01 Nov 2023 03:02:13 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 01 Nov 2023 03:02:15 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 01 Nov 2023 03:02:15 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 01 Nov 2023 03:02:15 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 01 Nov 2023 03:02:15 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 01 Nov 2023 03:02:15 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Wed, 01 Nov 2023 03:02:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 03:02:15 GMT
CMD ["influxd"]
# Wed, 01 Nov 2023 03:02:16 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 01 Nov 2023 03:02:16 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262116acfec49dc20776eccd49619b880cec1fd47986b2f8309782cf13481e5d`  
		Last Modified: Wed, 01 Nov 2023 03:02:48 GMT  
		Size: 9.6 MB (9584486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d34c8bbe1ae9229eeb59ba5f8b19d8a31f7c63b8591315702334252f91b36`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 6.0 MB (5953766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e6bb63ae8bd4bca01c0bee81dec19e9bf0a7277d486d01551cd837ef2d4448`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 3.3 KB (3280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e1f23b16702da739edd9c930032d32ad1377ebc0f9ae7310ecf969942ed819`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 921.5 KB (921473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf396801ae61bebd6da034895d279d77471f5fba07e6ac918fd449def2ee46d`  
		Last Modified: Wed, 01 Nov 2023 03:02:50 GMT  
		Size: 89.2 MB (89159505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52a03c7703182a6c2dd7d8ae6c1c224bc82eebb3e930c0741c71f693d042733`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 21.7 MB (21662585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f072621e375faeb99e7f90b93f1bc33f921b5d92f0172580fba05b9e898ba5c2`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55de467c42ebc43636d37579756439b6fb6b7b6ef5f0c1d7021ee61c153898d7`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1efdf6846864ed36faf9ec3e47d4c9bf8a885651259e99a517f373e01b071c`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7-alpine`

```console
$ docker pull influxdb@sha256:b446da96ecd34ce116138f04d4384b4aac9ad9b6e82784fe72d426c7bc926bce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:c3c7cb54aaad254a5a917406e9bfa699d93e9d2206ed3942237e40784a588043
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88172341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5f754bb6c4eec50c8d1eb3dd579842aec6abab4f7e383b6768b873bb38bd61`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:30:37 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:31:11 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Tue, 17 Oct 2023 01:31:12 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 17 Oct 2023 01:31:13 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 19 Oct 2023 01:22:24 GMT
ENV INFLUXDB_VERSION=2.7.3
# Thu, 19 Oct 2023 01:22:28 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 19 Oct 2023 01:22:28 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 19 Oct 2023 01:22:30 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 19 Oct 2023 01:22:31 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 19 Oct 2023 01:22:31 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 19 Oct 2023 01:22:31 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 19 Oct 2023 01:22:31 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:22:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:22:31 GMT
CMD ["influxd"]
# Thu, 19 Oct 2023 01:22:32 GMT
EXPOSE 8086
# Thu, 19 Oct 2023 01:22:32 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 19 Oct 2023 01:22:32 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 19 Oct 2023 01:22:32 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 19 Oct 2023 01:22:32 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5352bf3aec614dde8ac36d38f28f5021eff4c2ff0226eb22dfa667f2b2add1`  
		Last Modified: Tue, 17 Oct 2023 01:33:20 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1571fe6e896787a9ed8a94a131ff6ea2380ac23074890f6eca0b0508ce78e4b3`  
		Last Modified: Tue, 17 Oct 2023 01:34:04 GMT  
		Size: 8.9 MB (8868212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39440e9faa9e55df70138260c3e8deba8040a52aa612269873118811755dac7c`  
		Last Modified: Tue, 17 Oct 2023 01:34:04 GMT  
		Size: 6.4 MB (6434122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713e365c08429ef4ca6fb360291a58e51a44a15f206de8851ddf86ab4c827d31`  
		Last Modified: Tue, 17 Oct 2023 01:34:03 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8801ab8f467b96c4f7b6c66b16fae8b1aa9db845c57b837ebf732ce77a7703`  
		Last Modified: Thu, 19 Oct 2023 01:23:56 GMT  
		Size: 46.3 MB (46330997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bbdab792656ecff534f8965a07f4605251ce55a66f92b18bced995cf352d83`  
		Last Modified: Thu, 19 Oct 2023 01:23:53 GMT  
		Size: 23.1 MB (23128345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed968514479db2a4e2763ab5893ca22009a90af55d20adeb7290f4349074667b`  
		Last Modified: Thu, 19 Oct 2023 01:23:50 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325dfb530e833cfb403ffa145eacb614e4ebac2a35de6abae006fcad01cd69b9`  
		Last Modified: Thu, 19 Oct 2023 01:23:50 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ef697a08bf4153a1f0585bd986d4b18038caed68d90237aebb1ff1e81ec25b`  
		Last Modified: Thu, 19 Oct 2023 01:23:50 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f9f7ecc114d6ef9dc076a59f69e979246bf46c6d607e26001e48ff2dc81f644c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84495706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc91cc0737069fb5fc50d6e58eecde0a60907cab49c819fd3a6d7025caa5b3f1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 00:43:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 00:43:53 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Tue, 17 Oct 2023 00:43:54 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 17 Oct 2023 00:43:55 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 19 Oct 2023 02:00:12 GMT
ENV INFLUXDB_VERSION=2.7.3
# Thu, 19 Oct 2023 02:00:15 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 19 Oct 2023 02:00:15 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 19 Oct 2023 02:00:17 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 19 Oct 2023 02:00:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 19 Oct 2023 02:00:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 19 Oct 2023 02:00:18 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 19 Oct 2023 02:00:18 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 19 Oct 2023 02:00:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 02:00:18 GMT
CMD ["influxd"]
# Thu, 19 Oct 2023 02:00:18 GMT
EXPOSE 8086
# Thu, 19 Oct 2023 02:00:18 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 19 Oct 2023 02:00:18 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 19 Oct 2023 02:00:18 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 19 Oct 2023 02:00:18 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e248ba14d9e254569a72ce1316c31cb26327474bc388ccd8fbd2fa78078db3aa`  
		Last Modified: Tue, 17 Oct 2023 00:44:22 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc059a59f82bcb99dccb07e78bca560aa59ed7395b4e1aca88e17625928caac3`  
		Last Modified: Tue, 17 Oct 2023 00:44:22 GMT  
		Size: 9.0 MB (8962246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6a92e4aeeabe0db41582e915d546ba0cdf83b3fa3b763d525457048749a9c8`  
		Last Modified: Tue, 17 Oct 2023 00:44:21 GMT  
		Size: 6.0 MB (5953765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e150933dfc1e072cfad77c042576074dad28047c0f9048064040a3bd04052307`  
		Last Modified: Tue, 17 Oct 2023 00:44:20 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc110e4198212cd2dbbba504dd9f88303cf9c8c97dde3d242a6f1ff7aa2c09d`  
		Last Modified: Thu, 19 Oct 2023 02:01:02 GMT  
		Size: 44.6 MB (44576567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40514d17fee131f5e8da357b64fe4da3d9d1bbf602132654b9f93576c52009dd`  
		Last Modified: Thu, 19 Oct 2023 02:00:59 GMT  
		Size: 21.7 MB (21662599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e864dc907306758f7e0256ea09a5f92ee6f2107adc28fdef2032ebab8316e`  
		Last Modified: Thu, 19 Oct 2023 02:00:57 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9d5e1a18d87ebbfe33ab40364e51b83468cd212e6b1f2cffddc87979dc13c`  
		Last Modified: Thu, 19 Oct 2023 02:00:57 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c33af00b9d093c0579d28427b2e1d869b0b36422922605b4288978a2377db2`  
		Last Modified: Thu, 19 Oct 2023 02:00:57 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.3`

```console
$ docker pull influxdb@sha256:5973b7698a7a8fddf60eca9c44077b062abb133aecfb193ec279ba2eeff253cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.3` - linux; amd64

```console
$ docker pull influxdb@sha256:f02325b07c1105549c1e3099343f8cf8724497995b4795c5a1e0ddf5bd76fccf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.2 MB (162170896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165ce29e04361e963410915a225e528ec623101f733ba6196c7148947c9f4ecf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:49 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
# Wed, 01 Nov 2023 00:20:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:02 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:36:04 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 01 Nov 2023 02:36:05 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 01 Nov 2023 02:36:05 GMT
ENV GOSU_VER=1.12
# Wed, 01 Nov 2023 02:36:07 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 01 Nov 2023 02:36:07 GMT
ENV INFLUXDB_VERSION=2.7.3
# Wed, 01 Nov 2023 02:36:12 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 01 Nov 2023 02:36:12 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 01 Nov 2023 02:36:14 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 01 Nov 2023 02:36:15 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 01 Nov 2023 02:36:15 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 01 Nov 2023 02:36:15 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 01 Nov 2023 02:36:15 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:36:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:36:15 GMT
CMD ["influxd"]
# Wed, 01 Nov 2023 02:36:15 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:36:15 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 01 Nov 2023 02:36:16 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 01 Nov 2023 02:36:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 01 Nov 2023 02:36:16 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbcf0a0fd4f60b8f415999c5c7c9d499b5e065fc620ececfb9a9c50d925559b`  
		Last Modified: Wed, 01 Nov 2023 02:38:29 GMT  
		Size: 9.8 MB (9787149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc30a15212abb09190c168b0bfc858f7682098ef77f765b1b19158189864dfe3`  
		Last Modified: Wed, 01 Nov 2023 02:38:26 GMT  
		Size: 6.4 MB (6434099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159c705faba476f2d587c2b39871193bed7bbacd328eee135c265a65f3dc83f9`  
		Last Modified: Wed, 01 Nov 2023 02:38:25 GMT  
		Size: 3.3 KB (3281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d00aeef48a00456bd46e972f3c131543fd90b1d48c6fb6ff6934725e515d87`  
		Last Modified: Wed, 01 Nov 2023 02:38:25 GMT  
		Size: 986.0 KB (985995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c836d6efdfbcc4e1b254e82930240d4d4a638a95888229331e5322b9e778470`  
		Last Modified: Wed, 01 Nov 2023 02:38:33 GMT  
		Size: 92.7 MB (92675041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:979326e5d1b2d6f77813a9660d6d7f9d944a4787ed617053396d81a447bafc54`  
		Last Modified: Wed, 01 Nov 2023 02:38:26 GMT  
		Size: 23.1 MB (23128348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5797dc5b6cab1afb3734b6a1696fc3623e38f371fbace58f775402723df55c`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10179fcb509a5aeaf267fb8c50ce26d13a4da438fbfa3171be4b60ec97e92f09`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eff5c0be8ad19f7a47f14b95ce6e892461edf952e3932a02684e53e9c3f234d`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.3` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9a9d2ad170926a8880b35ade12fc7d226e688dda525331bd0a6f4117d807aaad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156471359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4209d6dee09892d6c679bc2479aaa59b63ff870a32188a3dd612ddd804967d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:41 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 01 Nov 2023 00:39:41 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 03:02:01 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:02:02 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 01 Nov 2023 03:02:03 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 01 Nov 2023 03:02:03 GMT
ENV GOSU_VER=1.12
# Wed, 01 Nov 2023 03:02:05 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 01 Nov 2023 03:02:05 GMT
ENV INFLUXDB_VERSION=2.7.3
# Wed, 01 Nov 2023 03:02:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 01 Nov 2023 03:02:13 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 01 Nov 2023 03:02:15 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 01 Nov 2023 03:02:15 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 01 Nov 2023 03:02:15 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 01 Nov 2023 03:02:15 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 01 Nov 2023 03:02:15 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Wed, 01 Nov 2023 03:02:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 03:02:15 GMT
CMD ["influxd"]
# Wed, 01 Nov 2023 03:02:16 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 01 Nov 2023 03:02:16 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262116acfec49dc20776eccd49619b880cec1fd47986b2f8309782cf13481e5d`  
		Last Modified: Wed, 01 Nov 2023 03:02:48 GMT  
		Size: 9.6 MB (9584486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d34c8bbe1ae9229eeb59ba5f8b19d8a31f7c63b8591315702334252f91b36`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 6.0 MB (5953766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e6bb63ae8bd4bca01c0bee81dec19e9bf0a7277d486d01551cd837ef2d4448`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 3.3 KB (3280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e1f23b16702da739edd9c930032d32ad1377ebc0f9ae7310ecf969942ed819`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 921.5 KB (921473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf396801ae61bebd6da034895d279d77471f5fba07e6ac918fd449def2ee46d`  
		Last Modified: Wed, 01 Nov 2023 03:02:50 GMT  
		Size: 89.2 MB (89159505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52a03c7703182a6c2dd7d8ae6c1c224bc82eebb3e930c0741c71f693d042733`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 21.7 MB (21662585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f072621e375faeb99e7f90b93f1bc33f921b5d92f0172580fba05b9e898ba5c2`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55de467c42ebc43636d37579756439b6fb6b7b6ef5f0c1d7021ee61c153898d7`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1efdf6846864ed36faf9ec3e47d4c9bf8a885651259e99a517f373e01b071c`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.3-alpine`

```console
$ docker pull influxdb@sha256:b446da96ecd34ce116138f04d4384b4aac9ad9b6e82784fe72d426c7bc926bce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.3-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:c3c7cb54aaad254a5a917406e9bfa699d93e9d2206ed3942237e40784a588043
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88172341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5f754bb6c4eec50c8d1eb3dd579842aec6abab4f7e383b6768b873bb38bd61`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:30:37 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:31:11 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Tue, 17 Oct 2023 01:31:12 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 17 Oct 2023 01:31:13 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 19 Oct 2023 01:22:24 GMT
ENV INFLUXDB_VERSION=2.7.3
# Thu, 19 Oct 2023 01:22:28 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 19 Oct 2023 01:22:28 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 19 Oct 2023 01:22:30 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 19 Oct 2023 01:22:31 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 19 Oct 2023 01:22:31 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 19 Oct 2023 01:22:31 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 19 Oct 2023 01:22:31 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:22:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:22:31 GMT
CMD ["influxd"]
# Thu, 19 Oct 2023 01:22:32 GMT
EXPOSE 8086
# Thu, 19 Oct 2023 01:22:32 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 19 Oct 2023 01:22:32 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 19 Oct 2023 01:22:32 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 19 Oct 2023 01:22:32 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5352bf3aec614dde8ac36d38f28f5021eff4c2ff0226eb22dfa667f2b2add1`  
		Last Modified: Tue, 17 Oct 2023 01:33:20 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1571fe6e896787a9ed8a94a131ff6ea2380ac23074890f6eca0b0508ce78e4b3`  
		Last Modified: Tue, 17 Oct 2023 01:34:04 GMT  
		Size: 8.9 MB (8868212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39440e9faa9e55df70138260c3e8deba8040a52aa612269873118811755dac7c`  
		Last Modified: Tue, 17 Oct 2023 01:34:04 GMT  
		Size: 6.4 MB (6434122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713e365c08429ef4ca6fb360291a58e51a44a15f206de8851ddf86ab4c827d31`  
		Last Modified: Tue, 17 Oct 2023 01:34:03 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8801ab8f467b96c4f7b6c66b16fae8b1aa9db845c57b837ebf732ce77a7703`  
		Last Modified: Thu, 19 Oct 2023 01:23:56 GMT  
		Size: 46.3 MB (46330997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bbdab792656ecff534f8965a07f4605251ce55a66f92b18bced995cf352d83`  
		Last Modified: Thu, 19 Oct 2023 01:23:53 GMT  
		Size: 23.1 MB (23128345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed968514479db2a4e2763ab5893ca22009a90af55d20adeb7290f4349074667b`  
		Last Modified: Thu, 19 Oct 2023 01:23:50 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325dfb530e833cfb403ffa145eacb614e4ebac2a35de6abae006fcad01cd69b9`  
		Last Modified: Thu, 19 Oct 2023 01:23:50 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ef697a08bf4153a1f0585bd986d4b18038caed68d90237aebb1ff1e81ec25b`  
		Last Modified: Thu, 19 Oct 2023 01:23:50 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.3-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f9f7ecc114d6ef9dc076a59f69e979246bf46c6d607e26001e48ff2dc81f644c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84495706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc91cc0737069fb5fc50d6e58eecde0a60907cab49c819fd3a6d7025caa5b3f1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 00:43:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 00:43:53 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Tue, 17 Oct 2023 00:43:54 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 17 Oct 2023 00:43:55 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 19 Oct 2023 02:00:12 GMT
ENV INFLUXDB_VERSION=2.7.3
# Thu, 19 Oct 2023 02:00:15 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 19 Oct 2023 02:00:15 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 19 Oct 2023 02:00:17 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 19 Oct 2023 02:00:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 19 Oct 2023 02:00:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 19 Oct 2023 02:00:18 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 19 Oct 2023 02:00:18 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 19 Oct 2023 02:00:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 02:00:18 GMT
CMD ["influxd"]
# Thu, 19 Oct 2023 02:00:18 GMT
EXPOSE 8086
# Thu, 19 Oct 2023 02:00:18 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 19 Oct 2023 02:00:18 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 19 Oct 2023 02:00:18 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 19 Oct 2023 02:00:18 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e248ba14d9e254569a72ce1316c31cb26327474bc388ccd8fbd2fa78078db3aa`  
		Last Modified: Tue, 17 Oct 2023 00:44:22 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc059a59f82bcb99dccb07e78bca560aa59ed7395b4e1aca88e17625928caac3`  
		Last Modified: Tue, 17 Oct 2023 00:44:22 GMT  
		Size: 9.0 MB (8962246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6a92e4aeeabe0db41582e915d546ba0cdf83b3fa3b763d525457048749a9c8`  
		Last Modified: Tue, 17 Oct 2023 00:44:21 GMT  
		Size: 6.0 MB (5953765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e150933dfc1e072cfad77c042576074dad28047c0f9048064040a3bd04052307`  
		Last Modified: Tue, 17 Oct 2023 00:44:20 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc110e4198212cd2dbbba504dd9f88303cf9c8c97dde3d242a6f1ff7aa2c09d`  
		Last Modified: Thu, 19 Oct 2023 02:01:02 GMT  
		Size: 44.6 MB (44576567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40514d17fee131f5e8da357b64fe4da3d9d1bbf602132654b9f93576c52009dd`  
		Last Modified: Thu, 19 Oct 2023 02:00:59 GMT  
		Size: 21.7 MB (21662599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e864dc907306758f7e0256ea09a5f92ee6f2107adc28fdef2032ebab8316e`  
		Last Modified: Thu, 19 Oct 2023 02:00:57 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9d5e1a18d87ebbfe33ab40364e51b83468cd212e6b1f2cffddc87979dc13c`  
		Last Modified: Thu, 19 Oct 2023 02:00:57 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c33af00b9d093c0579d28427b2e1d869b0b36422922605b4288978a2377db2`  
		Last Modified: Thu, 19 Oct 2023 02:00:57 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:b446da96ecd34ce116138f04d4384b4aac9ad9b6e82784fe72d426c7bc926bce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:c3c7cb54aaad254a5a917406e9bfa699d93e9d2206ed3942237e40784a588043
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88172341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5f754bb6c4eec50c8d1eb3dd579842aec6abab4f7e383b6768b873bb38bd61`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:30:37 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:31:11 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Tue, 17 Oct 2023 01:31:12 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 17 Oct 2023 01:31:13 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 19 Oct 2023 01:22:24 GMT
ENV INFLUXDB_VERSION=2.7.3
# Thu, 19 Oct 2023 01:22:28 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 19 Oct 2023 01:22:28 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 19 Oct 2023 01:22:30 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 19 Oct 2023 01:22:31 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 19 Oct 2023 01:22:31 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 19 Oct 2023 01:22:31 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 19 Oct 2023 01:22:31 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:22:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:22:31 GMT
CMD ["influxd"]
# Thu, 19 Oct 2023 01:22:32 GMT
EXPOSE 8086
# Thu, 19 Oct 2023 01:22:32 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 19 Oct 2023 01:22:32 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 19 Oct 2023 01:22:32 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 19 Oct 2023 01:22:32 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5352bf3aec614dde8ac36d38f28f5021eff4c2ff0226eb22dfa667f2b2add1`  
		Last Modified: Tue, 17 Oct 2023 01:33:20 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1571fe6e896787a9ed8a94a131ff6ea2380ac23074890f6eca0b0508ce78e4b3`  
		Last Modified: Tue, 17 Oct 2023 01:34:04 GMT  
		Size: 8.9 MB (8868212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39440e9faa9e55df70138260c3e8deba8040a52aa612269873118811755dac7c`  
		Last Modified: Tue, 17 Oct 2023 01:34:04 GMT  
		Size: 6.4 MB (6434122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713e365c08429ef4ca6fb360291a58e51a44a15f206de8851ddf86ab4c827d31`  
		Last Modified: Tue, 17 Oct 2023 01:34:03 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8801ab8f467b96c4f7b6c66b16fae8b1aa9db845c57b837ebf732ce77a7703`  
		Last Modified: Thu, 19 Oct 2023 01:23:56 GMT  
		Size: 46.3 MB (46330997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bbdab792656ecff534f8965a07f4605251ce55a66f92b18bced995cf352d83`  
		Last Modified: Thu, 19 Oct 2023 01:23:53 GMT  
		Size: 23.1 MB (23128345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed968514479db2a4e2763ab5893ca22009a90af55d20adeb7290f4349074667b`  
		Last Modified: Thu, 19 Oct 2023 01:23:50 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325dfb530e833cfb403ffa145eacb614e4ebac2a35de6abae006fcad01cd69b9`  
		Last Modified: Thu, 19 Oct 2023 01:23:50 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ef697a08bf4153a1f0585bd986d4b18038caed68d90237aebb1ff1e81ec25b`  
		Last Modified: Thu, 19 Oct 2023 01:23:50 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f9f7ecc114d6ef9dc076a59f69e979246bf46c6d607e26001e48ff2dc81f644c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84495706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc91cc0737069fb5fc50d6e58eecde0a60907cab49c819fd3a6d7025caa5b3f1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 00:43:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 00:43:53 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Tue, 17 Oct 2023 00:43:54 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 17 Oct 2023 00:43:55 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 19 Oct 2023 02:00:12 GMT
ENV INFLUXDB_VERSION=2.7.3
# Thu, 19 Oct 2023 02:00:15 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 19 Oct 2023 02:00:15 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 19 Oct 2023 02:00:17 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 19 Oct 2023 02:00:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 19 Oct 2023 02:00:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 19 Oct 2023 02:00:18 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 19 Oct 2023 02:00:18 GMT
COPY file:0c651d5752d62a8235f9939458cdfe0447d6491e071a852d95bf87ff7179f6a0 in /entrypoint.sh 
# Thu, 19 Oct 2023 02:00:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 02:00:18 GMT
CMD ["influxd"]
# Thu, 19 Oct 2023 02:00:18 GMT
EXPOSE 8086
# Thu, 19 Oct 2023 02:00:18 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 19 Oct 2023 02:00:18 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 19 Oct 2023 02:00:18 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 19 Oct 2023 02:00:18 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e248ba14d9e254569a72ce1316c31cb26327474bc388ccd8fbd2fa78078db3aa`  
		Last Modified: Tue, 17 Oct 2023 00:44:22 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc059a59f82bcb99dccb07e78bca560aa59ed7395b4e1aca88e17625928caac3`  
		Last Modified: Tue, 17 Oct 2023 00:44:22 GMT  
		Size: 9.0 MB (8962246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6a92e4aeeabe0db41582e915d546ba0cdf83b3fa3b763d525457048749a9c8`  
		Last Modified: Tue, 17 Oct 2023 00:44:21 GMT  
		Size: 6.0 MB (5953765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e150933dfc1e072cfad77c042576074dad28047c0f9048064040a3bd04052307`  
		Last Modified: Tue, 17 Oct 2023 00:44:20 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc110e4198212cd2dbbba504dd9f88303cf9c8c97dde3d242a6f1ff7aa2c09d`  
		Last Modified: Thu, 19 Oct 2023 02:01:02 GMT  
		Size: 44.6 MB (44576567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40514d17fee131f5e8da357b64fe4da3d9d1bbf602132654b9f93576c52009dd`  
		Last Modified: Thu, 19 Oct 2023 02:00:59 GMT  
		Size: 21.7 MB (21662599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e864dc907306758f7e0256ea09a5f92ee6f2107adc28fdef2032ebab8316e`  
		Last Modified: Thu, 19 Oct 2023 02:00:57 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9d5e1a18d87ebbfe33ab40364e51b83468cd212e6b1f2cffddc87979dc13c`  
		Last Modified: Thu, 19 Oct 2023 02:00:57 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c33af00b9d093c0579d28427b2e1d869b0b36422922605b4288978a2377db2`  
		Last Modified: Thu, 19 Oct 2023 02:00:57 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:5973b7698a7a8fddf60eca9c44077b062abb133aecfb193ec279ba2eeff253cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:f02325b07c1105549c1e3099343f8cf8724497995b4795c5a1e0ddf5bd76fccf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.2 MB (162170896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165ce29e04361e963410915a225e528ec623101f733ba6196c7148947c9f4ecf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:49 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
# Wed, 01 Nov 2023 00:20:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:02 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:36:04 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 01 Nov 2023 02:36:05 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 01 Nov 2023 02:36:05 GMT
ENV GOSU_VER=1.12
# Wed, 01 Nov 2023 02:36:07 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 01 Nov 2023 02:36:07 GMT
ENV INFLUXDB_VERSION=2.7.3
# Wed, 01 Nov 2023 02:36:12 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 01 Nov 2023 02:36:12 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 01 Nov 2023 02:36:14 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 01 Nov 2023 02:36:15 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 01 Nov 2023 02:36:15 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 01 Nov 2023 02:36:15 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 01 Nov 2023 02:36:15 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:36:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:36:15 GMT
CMD ["influxd"]
# Wed, 01 Nov 2023 02:36:15 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:36:15 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 01 Nov 2023 02:36:16 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 01 Nov 2023 02:36:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 01 Nov 2023 02:36:16 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbcf0a0fd4f60b8f415999c5c7c9d499b5e065fc620ececfb9a9c50d925559b`  
		Last Modified: Wed, 01 Nov 2023 02:38:29 GMT  
		Size: 9.8 MB (9787149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc30a15212abb09190c168b0bfc858f7682098ef77f765b1b19158189864dfe3`  
		Last Modified: Wed, 01 Nov 2023 02:38:26 GMT  
		Size: 6.4 MB (6434099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159c705faba476f2d587c2b39871193bed7bbacd328eee135c265a65f3dc83f9`  
		Last Modified: Wed, 01 Nov 2023 02:38:25 GMT  
		Size: 3.3 KB (3281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d00aeef48a00456bd46e972f3c131543fd90b1d48c6fb6ff6934725e515d87`  
		Last Modified: Wed, 01 Nov 2023 02:38:25 GMT  
		Size: 986.0 KB (985995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c836d6efdfbcc4e1b254e82930240d4d4a638a95888229331e5322b9e778470`  
		Last Modified: Wed, 01 Nov 2023 02:38:33 GMT  
		Size: 92.7 MB (92675041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:979326e5d1b2d6f77813a9660d6d7f9d944a4787ed617053396d81a447bafc54`  
		Last Modified: Wed, 01 Nov 2023 02:38:26 GMT  
		Size: 23.1 MB (23128348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5797dc5b6cab1afb3734b6a1696fc3623e38f371fbace58f775402723df55c`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10179fcb509a5aeaf267fb8c50ce26d13a4da438fbfa3171be4b60ec97e92f09`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eff5c0be8ad19f7a47f14b95ce6e892461edf952e3932a02684e53e9c3f234d`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9a9d2ad170926a8880b35ade12fc7d226e688dda525331bd0a6f4117d807aaad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156471359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4209d6dee09892d6c679bc2479aaa59b63ff870a32188a3dd612ddd804967d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:41 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 01 Nov 2023 00:39:41 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 03:02:01 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:02:02 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 01 Nov 2023 03:02:03 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 01 Nov 2023 03:02:03 GMT
ENV GOSU_VER=1.12
# Wed, 01 Nov 2023 03:02:05 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 01 Nov 2023 03:02:05 GMT
ENV INFLUXDB_VERSION=2.7.3
# Wed, 01 Nov 2023 03:02:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 01 Nov 2023 03:02:13 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 01 Nov 2023 03:02:15 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 01 Nov 2023 03:02:15 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 01 Nov 2023 03:02:15 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 01 Nov 2023 03:02:15 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 01 Nov 2023 03:02:15 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Wed, 01 Nov 2023 03:02:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 03:02:15 GMT
CMD ["influxd"]
# Wed, 01 Nov 2023 03:02:16 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 01 Nov 2023 03:02:16 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262116acfec49dc20776eccd49619b880cec1fd47986b2f8309782cf13481e5d`  
		Last Modified: Wed, 01 Nov 2023 03:02:48 GMT  
		Size: 9.6 MB (9584486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d34c8bbe1ae9229eeb59ba5f8b19d8a31f7c63b8591315702334252f91b36`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 6.0 MB (5953766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e6bb63ae8bd4bca01c0bee81dec19e9bf0a7277d486d01551cd837ef2d4448`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 3.3 KB (3280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e1f23b16702da739edd9c930032d32ad1377ebc0f9ae7310ecf969942ed819`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 921.5 KB (921473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf396801ae61bebd6da034895d279d77471f5fba07e6ac918fd449def2ee46d`  
		Last Modified: Wed, 01 Nov 2023 03:02:50 GMT  
		Size: 89.2 MB (89159505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52a03c7703182a6c2dd7d8ae6c1c224bc82eebb3e930c0741c71f693d042733`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 21.7 MB (21662585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f072621e375faeb99e7f90b93f1bc33f921b5d92f0172580fba05b9e898ba5c2`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55de467c42ebc43636d37579756439b6fb6b7b6ef5f0c1d7021ee61c153898d7`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1efdf6846864ed36faf9ec3e47d4c9bf8a885651259e99a517f373e01b071c`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
