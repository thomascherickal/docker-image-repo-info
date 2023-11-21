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
-	[`influxdb:2.7.4`](#influxdb274)
-	[`influxdb:2.7.4-alpine`](#influxdb274-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:latest`](#influxdblatest)

## `influxdb:1.10-data`

```console
$ docker pull influxdb@sha256:184e1fad2bdd645d45d9c05727c63dc6ac97ce1322ad0bc95b4b54f97f7fcae1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:312d10de5556119f876f5b531922ac9d4528cef36dae9f617b79be88ed7ce086
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111001989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f4a1e723a3dd1d22cc185e40da0bd92bf5723a406dae2e3e5a87dc9597f49e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:24:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:24:50 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Tue, 21 Nov 2023 13:24:55 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb*
# Tue, 21 Nov 2023 13:24:56 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 13:24:56 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 13:24:56 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:24:56 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:24:56 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 13:24:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:24:56 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b56497929001edaa7b3b8ccd4526b31c1b1f8b37b2fc3749d2a27fbbb54f8`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b52b315868f38e6c136deb5891ae553733a86dd49861e3be2549534591edce2`  
		Last Modified: Tue, 21 Nov 2023 13:27:05 GMT  
		Size: 40.2 MB (40176250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6dcab4dbd39dae7297e165fe3a734b423db68e89a6986e1a084ea344815bc4`  
		Last Modified: Tue, 21 Nov 2023 13:26:58 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f625dd632edabee8bdab6befe809a916f0fbcbb918f67a6b077a64eac747abeb`  
		Last Modified: Tue, 21 Nov 2023 13:26:58 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7b8fb8b2845bd1488ce92718841444b337f8b535e228de8f19086ba72378b1`  
		Last Modified: Tue, 21 Nov 2023 13:26:58 GMT  
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
$ docker pull influxdb@sha256:355d7e0d9ae14e3aa41173dfe6c4eb78074e848e103a1d266889c14f765b6401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:11d82e26b255fc235a4a16f86d3cfcc727cebbd6be8bb78151cc237bf281adcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91201456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0493d1e159ef0789b7d7ca266f3dc4e289bf970c0152991f8368c905a90ea34`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:24:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:24:50 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Tue, 21 Nov 2023 13:25:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb*
# Tue, 21 Nov 2023 13:25:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 21 Nov 2023 13:25:04 GMT
EXPOSE 8091
# Tue, 21 Nov 2023 13:25:04 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:25:04 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:25:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:25:05 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b56497929001edaa7b3b8ccd4526b31c1b1f8b37b2fc3749d2a27fbbb54f8`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c47f1e2903c15c0e186238f819c6a1b7a16b892b9c14718f188d47575015c83`  
		Last Modified: Tue, 21 Nov 2023 13:27:17 GMT  
		Size: 20.4 MB (20376921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7528c7a79cfe70da62c4b7a882d7b7cb847a02789725169880fd55e533bae8c3`  
		Last Modified: Tue, 21 Nov 2023 13:27:14 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340039b60eb149ae94a58b346652030ac828e27de81d1f8d618dbf433bbec95b`  
		Last Modified: Tue, 21 Nov 2023 13:27:14 GMT  
		Size: 375.0 B  
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
$ docker pull influxdb@sha256:184e1fad2bdd645d45d9c05727c63dc6ac97ce1322ad0bc95b4b54f97f7fcae1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.5-data` - linux; amd64

```console
$ docker pull influxdb@sha256:312d10de5556119f876f5b531922ac9d4528cef36dae9f617b79be88ed7ce086
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111001989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f4a1e723a3dd1d22cc185e40da0bd92bf5723a406dae2e3e5a87dc9597f49e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:24:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:24:50 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Tue, 21 Nov 2023 13:24:55 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb*
# Tue, 21 Nov 2023 13:24:56 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 13:24:56 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 13:24:56 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:24:56 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:24:56 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 13:24:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:24:56 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b56497929001edaa7b3b8ccd4526b31c1b1f8b37b2fc3749d2a27fbbb54f8`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b52b315868f38e6c136deb5891ae553733a86dd49861e3be2549534591edce2`  
		Last Modified: Tue, 21 Nov 2023 13:27:05 GMT  
		Size: 40.2 MB (40176250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6dcab4dbd39dae7297e165fe3a734b423db68e89a6986e1a084ea344815bc4`  
		Last Modified: Tue, 21 Nov 2023 13:26:58 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f625dd632edabee8bdab6befe809a916f0fbcbb918f67a6b077a64eac747abeb`  
		Last Modified: Tue, 21 Nov 2023 13:26:58 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7b8fb8b2845bd1488ce92718841444b337f8b535e228de8f19086ba72378b1`  
		Last Modified: Tue, 21 Nov 2023 13:26:58 GMT  
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
$ docker pull influxdb@sha256:355d7e0d9ae14e3aa41173dfe6c4eb78074e848e103a1d266889c14f765b6401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.10.5-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:11d82e26b255fc235a4a16f86d3cfcc727cebbd6be8bb78151cc237bf281adcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91201456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0493d1e159ef0789b7d7ca266f3dc4e289bf970c0152991f8368c905a90ea34`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:24:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:24:50 GMT
ENV INFLUXDB_VERSION=1.10.5-c1.10.5
# Tue, 21 Nov 2023 13:25:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb*
# Tue, 21 Nov 2023 13:25:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 21 Nov 2023 13:25:04 GMT
EXPOSE 8091
# Tue, 21 Nov 2023 13:25:04 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:25:04 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:25:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:25:05 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b56497929001edaa7b3b8ccd4526b31c1b1f8b37b2fc3749d2a27fbbb54f8`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c47f1e2903c15c0e186238f819c6a1b7a16b892b9c14718f188d47575015c83`  
		Last Modified: Tue, 21 Nov 2023 13:27:17 GMT  
		Size: 20.4 MB (20376921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7528c7a79cfe70da62c4b7a882d7b7cb847a02789725169880fd55e533bae8c3`  
		Last Modified: Tue, 21 Nov 2023 13:27:14 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340039b60eb149ae94a58b346652030ac828e27de81d1f8d618dbf433bbec95b`  
		Last Modified: Tue, 21 Nov 2023 13:27:14 GMT  
		Size: 375.0 B  
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
$ docker pull influxdb@sha256:9ed35295c8f2804caaf0ff8d6ec16220f6a822491092ccf6242b00da4d516034
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:38ca74e74f24098007b58fb5372ed2e9ee4b34586045ea48cdc7cb6e8a4dc918
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.8 MB (113809472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99471449acf9cdce18d77d82ef512620771271485cd8d7456ae96374f30701d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:25:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:25:12 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Tue, 21 Nov 2023 13:25:15 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb*
# Tue, 21 Nov 2023 13:25:16 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 13:25:16 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 13:25:16 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:25:16 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:25:16 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 13:25:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:25:16 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e1a8ca91d35598fbae8dee7f1c211f0f93cec529f6804a60e9301c53a604d0`  
		Last Modified: Tue, 21 Nov 2023 10:01:22 GMT  
		Size: 24.0 MB (24049172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92ded14df63cfaaaa84ec9bab96fe32ef57c633934a4cb00c6aa68b9023e2b6`  
		Last Modified: Tue, 21 Nov 2023 13:27:27 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24994d50b5874c66f06db93133e6e81eb864ee4e57c9c59b6d184dd1c741833`  
		Last Modified: Tue, 21 Nov 2023 13:27:33 GMT  
		Size: 40.2 MB (40174482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0917ab01b983465dc8161bea84eb81dd173f3fd62034f74ce8e2e0087e7a2`  
		Last Modified: Tue, 21 Nov 2023 13:27:27 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f660b59ea99114a6273fb8e3f85a7a9ad8790b4998b0da86a200ea29545b853c`  
		Last Modified: Tue, 21 Nov 2023 13:27:27 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3b23a91addd53514f429f5355aeba299b2c55f490b7cc8d4d7a0d3aff40afd`  
		Last Modified: Tue, 21 Nov 2023 13:27:27 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:fc6f6d1d9ed509d71df549c1e43a85cc23f9ce6dd8def3334f9206fbbd0ed7e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:491aa919423097dfb5b03f6e098f8b5d92c0166a97d050ebf873ad4148af3353
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (93961130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d314c8ca1ed123b8a184812869c7606c8f2b5a988d457210a516f39406c034`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:25:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:25:12 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Tue, 21 Nov 2023 13:25:24 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb*
# Tue, 21 Nov 2023 13:25:24 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 21 Nov 2023 13:25:24 GMT
EXPOSE 8091
# Tue, 21 Nov 2023 13:25:24 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:25:24 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:25:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:25:24 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e1a8ca91d35598fbae8dee7f1c211f0f93cec529f6804a60e9301c53a604d0`  
		Last Modified: Tue, 21 Nov 2023 10:01:22 GMT  
		Size: 24.0 MB (24049172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92ded14df63cfaaaa84ec9bab96fe32ef57c633934a4cb00c6aa68b9023e2b6`  
		Last Modified: Tue, 21 Nov 2023 13:27:27 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f11dfac2fef9aeb2a320e5afa9c89ca8052e67b25c43c2f7ed0960d5b1af2a`  
		Last Modified: Tue, 21 Nov 2023 13:27:45 GMT  
		Size: 20.3 MB (20327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e3269339dec6c9bf564f0de779c24a53aeaa6b4f66e8c67c216c9dfb18a563`  
		Last Modified: Tue, 21 Nov 2023 13:27:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799d349be84ff8ea1547dc37154471754ebea44b204123fe143391109909ddce`  
		Last Modified: Tue, 21 Nov 2023 13:27:42 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:9ed35295c8f2804caaf0ff8d6ec16220f6a822491092ccf6242b00da4d516034
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.3-data` - linux; amd64

```console
$ docker pull influxdb@sha256:38ca74e74f24098007b58fb5372ed2e9ee4b34586045ea48cdc7cb6e8a4dc918
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.8 MB (113809472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99471449acf9cdce18d77d82ef512620771271485cd8d7456ae96374f30701d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:25:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:25:12 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Tue, 21 Nov 2023 13:25:15 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}-1_amd64.deb*
# Tue, 21 Nov 2023 13:25:16 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 13:25:16 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 13:25:16 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:25:16 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:25:16 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 13:25:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:25:16 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e1a8ca91d35598fbae8dee7f1c211f0f93cec529f6804a60e9301c53a604d0`  
		Last Modified: Tue, 21 Nov 2023 10:01:22 GMT  
		Size: 24.0 MB (24049172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92ded14df63cfaaaa84ec9bab96fe32ef57c633934a4cb00c6aa68b9023e2b6`  
		Last Modified: Tue, 21 Nov 2023 13:27:27 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24994d50b5874c66f06db93133e6e81eb864ee4e57c9c59b6d184dd1c741833`  
		Last Modified: Tue, 21 Nov 2023 13:27:33 GMT  
		Size: 40.2 MB (40174482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0917ab01b983465dc8161bea84eb81dd173f3fd62034f74ce8e2e0087e7a2`  
		Last Modified: Tue, 21 Nov 2023 13:27:27 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f660b59ea99114a6273fb8e3f85a7a9ad8790b4998b0da86a200ea29545b853c`  
		Last Modified: Tue, 21 Nov 2023 13:27:27 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3b23a91addd53514f429f5355aeba299b2c55f490b7cc8d4d7a0d3aff40afd`  
		Last Modified: Tue, 21 Nov 2023 13:27:27 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:fc6f6d1d9ed509d71df549c1e43a85cc23f9ce6dd8def3334f9206fbbd0ed7e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.11.3-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:491aa919423097dfb5b03f6e098f8b5d92c0166a97d050ebf873ad4148af3353
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (93961130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d314c8ca1ed123b8a184812869c7606c8f2b5a988d457210a516f39406c034`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:25:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:25:12 GMT
ENV INFLUXDB_VERSION=1.11.3-c1.11.3
# Tue, 21 Nov 2023 13:25:24 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}-1_amd64.deb*
# Tue, 21 Nov 2023 13:25:24 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 21 Nov 2023 13:25:24 GMT
EXPOSE 8091
# Tue, 21 Nov 2023 13:25:24 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:25:24 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:25:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:25:24 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e1a8ca91d35598fbae8dee7f1c211f0f93cec529f6804a60e9301c53a604d0`  
		Last Modified: Tue, 21 Nov 2023 10:01:22 GMT  
		Size: 24.0 MB (24049172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92ded14df63cfaaaa84ec9bab96fe32ef57c633934a4cb00c6aa68b9023e2b6`  
		Last Modified: Tue, 21 Nov 2023 13:27:27 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f11dfac2fef9aeb2a320e5afa9c89ca8052e67b25c43c2f7ed0960d5b1af2a`  
		Last Modified: Tue, 21 Nov 2023 13:27:45 GMT  
		Size: 20.3 MB (20327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e3269339dec6c9bf564f0de779c24a53aeaa6b4f66e8c67c216c9dfb18a563`  
		Last Modified: Tue, 21 Nov 2023 13:27:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799d349be84ff8ea1547dc37154471754ebea44b204123fe143391109909ddce`  
		Last Modified: Tue, 21 Nov 2023 13:27:42 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:fa0bd1644943ffe40549c0dc45c2a6217618b5cb53abf610aea38d60cf6bea1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:8dc017e964c0275548b7aa557254565b5924ffb60528ccc4936f263c85370201
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125711402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6679abb00ea8e08c41a2e2f04a93c81ec7acf2a578ee58dba840191fc016cee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:24:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:24:23 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 21 Nov 2023 13:24:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 21 Nov 2023 13:24:28 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 13:24:28 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 13:24:28 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:24:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:24:28 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 13:24:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:24:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b56497929001edaa7b3b8ccd4526b31c1b1f8b37b2fc3749d2a27fbbb54f8`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1043e72c9779ad4ab33fbbda035b07e44bd49c22b1d970e4c7f9da11d916a341`  
		Last Modified: Tue, 21 Nov 2023 13:26:23 GMT  
		Size: 54.9 MB (54885722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411efc9ff2930c3ec1193406a37df96bcc48b49c5a3a2ecc66320889f0d273f6`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045979ae36fffbf6636859d83faff7289a8c29823344dcded7a24807be5a466`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d8b4d7ea562415f6d5547101045321386fc5c2945df2da56c03173e8d220a4`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:8ba1ba50beca66b884165303909b85a2c5c415fe4159e235381281e15dbafe51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116711986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91fcd4a94f47f0edefabafcd6d0dee5a63a354860b7fe55b738cb40dd1d7ada`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:05:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:24:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 19:24:03 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 21 Nov 2023 19:24:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 21 Nov 2023 19:24:10 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 19:24:10 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 19:24:10 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 19:24:10 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 21 Nov 2023 19:24:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 19:24:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 19:24:10 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98461d76c0d7c5e4d320986d659d56aba23d807280d398632ef50acd8a6e028d`  
		Last Modified: Tue, 21 Nov 2023 14:15:07 GMT  
		Size: 14.9 MB (14879655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c61572961c1e618cc37e89887bb1a789dcd5b04da2e2af4e1aab31e28c995d`  
		Last Modified: Tue, 21 Nov 2023 19:24:17 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dcf7a00ad35a2d6f33563cd5a5eb7eed864cb1c4b302586c336452807206ac`  
		Last Modified: Tue, 21 Nov 2023 19:24:23 GMT  
		Size: 51.6 MB (51613147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0071fd422df6106f15f4c67acc39c4601928d95caf844ace3920d328671f2ad`  
		Last Modified: Tue, 21 Nov 2023 19:24:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290b8ee9d3d0941ffda3306dfa5858e9179ee493e847ebac79c7f5abe34713bf`  
		Last Modified: Tue, 21 Nov 2023 19:24:17 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f96a06b5d8eeafe6c4b90dec1a41dc064333f0fe9f241c3c3ee1e3bf81f70fd`  
		Last Modified: Tue, 21 Nov 2023 19:24:17 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a209f0677c86d1e7d8bf217c8c49349e44f8447a4a42d825724e4569af3b3f91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120691595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e5441f2ea17588daadb4f5e52a4b9e7fc514155d1d71e9aaaedb0c8736a02bf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:12:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 08:12:18 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 21 Nov 2023 08:12:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 21 Nov 2023 08:12:22 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 08:12:22 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 08:12:22 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 08:12:23 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 21 Nov 2023 08:12:23 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 08:12:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 08:12:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e860a4a6ca9e583881322c2e78baef1911e4d61bc607563e8ad9891e2d91f9`  
		Last Modified: Tue, 21 Nov 2023 08:07:01 GMT  
		Size: 15.8 MB (15750113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa3806cdb7669428cb75364396884c21d2e33668180efde9caf4a4adf2fe8da`  
		Last Modified: Tue, 21 Nov 2023 08:12:57 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264f8f135e2ec57a525ee13d9fe418786a1cd6bfdb057473daceda831f636fe2`  
		Last Modified: Tue, 21 Nov 2023 08:13:02 GMT  
		Size: 51.2 MB (51230081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05203f2334183ec6a948778045e77a9e40381429613e66d01db761efff43b29`  
		Last Modified: Tue, 21 Nov 2023 08:12:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cdb203931ad840be2b80589297032c968f53460ed839275ab26d35e5c1acfc`  
		Last Modified: Tue, 21 Nov 2023 08:12:57 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de133f0c8cebf0acaa4dae51a07ba40bcf3cd78248102741b0cea043b985270`  
		Last Modified: Tue, 21 Nov 2023 08:12:57 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:fa0bd1644943ffe40549c0dc45c2a6217618b5cb53abf610aea38d60cf6bea1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:8dc017e964c0275548b7aa557254565b5924ffb60528ccc4936f263c85370201
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125711402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6679abb00ea8e08c41a2e2f04a93c81ec7acf2a578ee58dba840191fc016cee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:24:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:24:23 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 21 Nov 2023 13:24:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 21 Nov 2023 13:24:28 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 13:24:28 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 13:24:28 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:24:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:24:28 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 13:24:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:24:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b56497929001edaa7b3b8ccd4526b31c1b1f8b37b2fc3749d2a27fbbb54f8`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1043e72c9779ad4ab33fbbda035b07e44bd49c22b1d970e4c7f9da11d916a341`  
		Last Modified: Tue, 21 Nov 2023 13:26:23 GMT  
		Size: 54.9 MB (54885722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411efc9ff2930c3ec1193406a37df96bcc48b49c5a3a2ecc66320889f0d273f6`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045979ae36fffbf6636859d83faff7289a8c29823344dcded7a24807be5a466`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d8b4d7ea562415f6d5547101045321386fc5c2945df2da56c03173e8d220a4`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:8ba1ba50beca66b884165303909b85a2c5c415fe4159e235381281e15dbafe51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116711986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91fcd4a94f47f0edefabafcd6d0dee5a63a354860b7fe55b738cb40dd1d7ada`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:05:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:24:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 19:24:03 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 21 Nov 2023 19:24:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 21 Nov 2023 19:24:10 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 19:24:10 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 19:24:10 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 19:24:10 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 21 Nov 2023 19:24:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 19:24:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 19:24:10 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98461d76c0d7c5e4d320986d659d56aba23d807280d398632ef50acd8a6e028d`  
		Last Modified: Tue, 21 Nov 2023 14:15:07 GMT  
		Size: 14.9 MB (14879655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c61572961c1e618cc37e89887bb1a789dcd5b04da2e2af4e1aab31e28c995d`  
		Last Modified: Tue, 21 Nov 2023 19:24:17 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dcf7a00ad35a2d6f33563cd5a5eb7eed864cb1c4b302586c336452807206ac`  
		Last Modified: Tue, 21 Nov 2023 19:24:23 GMT  
		Size: 51.6 MB (51613147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0071fd422df6106f15f4c67acc39c4601928d95caf844ace3920d328671f2ad`  
		Last Modified: Tue, 21 Nov 2023 19:24:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290b8ee9d3d0941ffda3306dfa5858e9179ee493e847ebac79c7f5abe34713bf`  
		Last Modified: Tue, 21 Nov 2023 19:24:17 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f96a06b5d8eeafe6c4b90dec1a41dc064333f0fe9f241c3c3ee1e3bf81f70fd`  
		Last Modified: Tue, 21 Nov 2023 19:24:17 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a209f0677c86d1e7d8bf217c8c49349e44f8447a4a42d825724e4569af3b3f91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120691595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e5441f2ea17588daadb4f5e52a4b9e7fc514155d1d71e9aaaedb0c8736a02bf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:12:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 08:12:18 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 21 Nov 2023 08:12:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 21 Nov 2023 08:12:22 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 08:12:22 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 08:12:22 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 08:12:23 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 21 Nov 2023 08:12:23 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 08:12:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 08:12:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e860a4a6ca9e583881322c2e78baef1911e4d61bc607563e8ad9891e2d91f9`  
		Last Modified: Tue, 21 Nov 2023 08:07:01 GMT  
		Size: 15.8 MB (15750113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa3806cdb7669428cb75364396884c21d2e33668180efde9caf4a4adf2fe8da`  
		Last Modified: Tue, 21 Nov 2023 08:12:57 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264f8f135e2ec57a525ee13d9fe418786a1cd6bfdb057473daceda831f636fe2`  
		Last Modified: Tue, 21 Nov 2023 08:13:02 GMT  
		Size: 51.2 MB (51230081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05203f2334183ec6a948778045e77a9e40381429613e66d01db761efff43b29`  
		Last Modified: Tue, 21 Nov 2023 08:12:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cdb203931ad840be2b80589297032c968f53460ed839275ab26d35e5c1acfc`  
		Last Modified: Tue, 21 Nov 2023 08:12:57 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de133f0c8cebf0acaa4dae51a07ba40bcf3cd78248102741b0cea043b985270`  
		Last Modified: Tue, 21 Nov 2023 08:12:57 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:9b39cab8290b301034f96e08da0a5dd48e74c65bb2e7e8aa845942c5e36aa9e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:db910c8e2ae0d6118501122413ee9712ff5fa01a4190f63e223b44ce82ad1abd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104114834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b8cf9dbd85524b09e33f9c9c2e4071a519a32e7ef61b9a18b961add60b5b226`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:24:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:24:33 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Tue, 21 Nov 2023 13:24:36 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 21 Nov 2023 13:24:37 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 13:24:37 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 13:24:37 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:24:37 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:24:37 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 13:24:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:24:37 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b56497929001edaa7b3b8ccd4526b31c1b1f8b37b2fc3749d2a27fbbb54f8`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4aab81b3c628eaf68afed1c0fedbf609478d07a8318f6f993299ff301f57382`  
		Last Modified: Tue, 21 Nov 2023 13:26:38 GMT  
		Size: 33.3 MB (33289097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767be1851407708cde76d7a932a2ece37f86d927fefd6ac771d8de7a500a1974`  
		Last Modified: Tue, 21 Nov 2023 13:26:33 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e06b7e9696ff8c222e0fa8fc9b19f9f4f9015f2aa3b62eb13d2d87bdf24026`  
		Last Modified: Tue, 21 Nov 2023 13:26:33 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33eb76aa93a6901b0afd5dfc57f5c89dae7ddb7e24b64402f74accda29b89f98`  
		Last Modified: Tue, 21 Nov 2023 13:26:33 GMT  
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
$ docker pull influxdb@sha256:57fdf2fa8f4a0c530bdaba4094446c47cfdac1eda5243103fe21e81f4b73bfc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:2928eb3b0d1789498887acc5aa2a3da7353d691cf704269bbc8dc5cdaa0012f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83594299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9ed5912604d6c7734d131d255ae2dfcd0042ae8736391ee2a15f651d31ab220`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:24:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:24:33 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Tue, 21 Nov 2023 13:24:45 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 21 Nov 2023 13:24:45 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 21 Nov 2023 13:24:45 GMT
EXPOSE 8091
# Tue, 21 Nov 2023 13:24:45 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:24:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:24:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:24:46 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b56497929001edaa7b3b8ccd4526b31c1b1f8b37b2fc3749d2a27fbbb54f8`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817dc9d15be53e0f0a2218617c284ad1870e15b18690076ca71bb3c792a12363`  
		Last Modified: Tue, 21 Nov 2023 13:26:49 GMT  
		Size: 12.8 MB (12769765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf93934ec654ea4d75a4a109aae61c0bcda0e88f547441e3be1fe58b433238dc`  
		Last Modified: Tue, 21 Nov 2023 13:26:47 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95611eba682d852f08c7bd94a07c53cf96b64dc0ec19d25e926569911e8ac8a1`  
		Last Modified: Tue, 21 Nov 2023 13:26:47 GMT  
		Size: 375.0 B  
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
$ docker pull influxdb@sha256:9b39cab8290b301034f96e08da0a5dd48e74c65bb2e7e8aa845942c5e36aa9e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.13-data` - linux; amd64

```console
$ docker pull influxdb@sha256:db910c8e2ae0d6118501122413ee9712ff5fa01a4190f63e223b44ce82ad1abd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104114834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b8cf9dbd85524b09e33f9c9c2e4071a519a32e7ef61b9a18b961add60b5b226`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:24:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:24:33 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Tue, 21 Nov 2023 13:24:36 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 21 Nov 2023 13:24:37 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 21 Nov 2023 13:24:37 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 13:24:37 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:24:37 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:24:37 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Nov 2023 13:24:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:24:37 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b56497929001edaa7b3b8ccd4526b31c1b1f8b37b2fc3749d2a27fbbb54f8`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4aab81b3c628eaf68afed1c0fedbf609478d07a8318f6f993299ff301f57382`  
		Last Modified: Tue, 21 Nov 2023 13:26:38 GMT  
		Size: 33.3 MB (33289097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767be1851407708cde76d7a932a2ece37f86d927fefd6ac771d8de7a500a1974`  
		Last Modified: Tue, 21 Nov 2023 13:26:33 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e06b7e9696ff8c222e0fa8fc9b19f9f4f9015f2aa3b62eb13d2d87bdf24026`  
		Last Modified: Tue, 21 Nov 2023 13:26:33 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33eb76aa93a6901b0afd5dfc57f5c89dae7ddb7e24b64402f74accda29b89f98`  
		Last Modified: Tue, 21 Nov 2023 13:26:33 GMT  
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
$ docker pull influxdb@sha256:57fdf2fa8f4a0c530bdaba4094446c47cfdac1eda5243103fe21e81f4b73bfc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.13-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:2928eb3b0d1789498887acc5aa2a3da7353d691cf704269bbc8dc5cdaa0012f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83594299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9ed5912604d6c7734d131d255ae2dfcd0042ae8736391ee2a15f651d31ab220`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:24:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 13:24:33 GMT
ENV INFLUXDB_VERSION=1.9.13-c1.9.13
# Tue, 21 Nov 2023 13:24:45 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 21 Nov 2023 13:24:45 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 21 Nov 2023 13:24:45 GMT
EXPOSE 8091
# Tue, 21 Nov 2023 13:24:45 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Nov 2023 13:24:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:24:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:24:46 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b56497929001edaa7b3b8ccd4526b31c1b1f8b37b2fc3749d2a27fbbb54f8`  
		Last Modified: Tue, 21 Nov 2023 13:26:16 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817dc9d15be53e0f0a2218617c284ad1870e15b18690076ca71bb3c792a12363`  
		Last Modified: Tue, 21 Nov 2023 13:26:49 GMT  
		Size: 12.8 MB (12769765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf93934ec654ea4d75a4a109aae61c0bcda0e88f547441e3be1fe58b433238dc`  
		Last Modified: Tue, 21 Nov 2023 13:26:47 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95611eba682d852f08c7bd94a07c53cf96b64dc0ec19d25e926569911e8ac8a1`  
		Last Modified: Tue, 21 Nov 2023 13:26:47 GMT  
		Size: 375.0 B  
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
$ docker pull influxdb@sha256:e0c66207e3f5cc16bc0730dc52a7fa81dbba6e366fe6ddf3daab0c3008af64c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7` - linux; amd64

```console
$ docker pull influxdb@sha256:f29b8f0b153b60f8de48c24c306aaa529d7d41b34a218de66f5be54fff381f1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161577286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7897b6955cd3f184c223a285b295fe5ae8ef0987a48f0a55e8187eb712a26e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 13:25:37 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:25:38 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 21 Nov 2023 13:25:39 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 21 Nov 2023 13:25:39 GMT
ENV GOSU_VER=1.16
# Tue, 21 Nov 2023 13:25:42 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 21 Nov 2023 13:25:42 GMT
ENV INFLUXDB_VERSION=2.7.4
# Tue, 21 Nov 2023 13:25:46 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 21 Nov 2023 13:25:46 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 21 Nov 2023 13:25:48 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 21 Nov 2023 13:25:49 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 21 Nov 2023 13:25:49 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 21 Nov 2023 13:25:49 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 21 Nov 2023 13:25:49 GMT
COPY file:b5520696339eadb7386055c1dc9487351aa145a79b0cf206d8b1a79699c4a7f1 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:25:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:25:49 GMT
CMD ["influxd"]
# Tue, 21 Nov 2023 13:25:49 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 13:25:49 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 21 Nov 2023 13:25:49 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 21 Nov 2023 13:25:49 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 21 Nov 2023 13:25:49 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e16ccbb43e210cb9b0da0a8b4971c0fa31d20a2056b04b5484971672f4ecae`  
		Last Modified: Tue, 21 Nov 2023 13:28:00 GMT  
		Size: 9.8 MB (9787108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a7bc1934b125acef1dad572f6f4b9b2b067b0e2401fe3101c6f9c84fd2d66`  
		Last Modified: Tue, 21 Nov 2023 13:27:57 GMT  
		Size: 5.8 MB (5820939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0cc3c0c6d9b72e7a3405cd4e2d34d728114b9ef2f0a56f171c59a55c62560c`  
		Last Modified: Tue, 21 Nov 2023 13:27:56 GMT  
		Size: 3.3 KB (3281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6061761101c04e03323a78d890270df54f990643cb9a0fe4333ba062f551bb9b`  
		Last Modified: Tue, 21 Nov 2023 13:27:57 GMT  
		Size: 1.0 MB (1006415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bd7f35f51975fa9760f3b0e622e785db6345d9d3cdcf3d25c0d16ccc635885`  
		Last Modified: Tue, 21 Nov 2023 13:28:04 GMT  
		Size: 92.7 MB (92674468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42be173071fe813e09b2d2158e616e057dd18dbe899346d3670654e88416afd1`  
		Last Modified: Tue, 21 Nov 2023 13:27:57 GMT  
		Size: 23.1 MB (23128346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883524767a4d5892b71184007462ac2378706bfa480c5e6de52f94801c6a1161`  
		Last Modified: Tue, 21 Nov 2023 13:27:54 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbf9c48eb4f1377d905b362d02efe85e89a620b11f1fc7136fbdc6206eb1a72`  
		Last Modified: Tue, 21 Nov 2023 13:27:54 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fee5c5d25312db4b409b99ebc4a11b460ec71a3503f6e40d0d3cd2c1d3d6222`  
		Last Modified: Tue, 21 Nov 2023 13:27:54 GMT  
		Size: 6.3 KB (6285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c4ecdce031166cf259e184f5d4cdea7d44c2aec27b8420e458f57f31089af977
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (155999608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27028005c79759ba5d348e4ae235461f63fcfb8c96bf5ad5a7a9772d7f7fdb5d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:12:32 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:12:33 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 21 Nov 2023 08:12:33 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 21 Nov 2023 08:12:33 GMT
ENV GOSU_VER=1.16
# Tue, 21 Nov 2023 08:12:36 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 21 Nov 2023 08:12:36 GMT
ENV INFLUXDB_VERSION=2.7.4
# Tue, 21 Nov 2023 08:12:40 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 21 Nov 2023 08:12:41 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 21 Nov 2023 08:12:43 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 21 Nov 2023 08:12:44 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 21 Nov 2023 08:12:44 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 21 Nov 2023 08:12:44 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 21 Nov 2023 08:12:44 GMT
COPY file:b5520696339eadb7386055c1dc9487351aa145a79b0cf206d8b1a79699c4a7f1 in /entrypoint.sh 
# Tue, 21 Nov 2023 08:12:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 08:12:44 GMT
CMD ["influxd"]
# Tue, 21 Nov 2023 08:12:44 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 08:12:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 21 Nov 2023 08:12:45 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 21 Nov 2023 08:12:45 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 21 Nov 2023 08:12:45 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f21dcbd9a86a0ef0a65a79975ce3e1ae090d7e20a5afcfbfc4e957bfccfef3`  
		Last Modified: Tue, 21 Nov 2023 08:13:15 GMT  
		Size: 9.6 MB (9584431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e12bc048239d052071a3cbdf062079b2cb0180d5716ba182c6b3d2a6dfec8a`  
		Last Modified: Tue, 21 Nov 2023 08:13:13 GMT  
		Size: 5.5 MB (5463797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604f72c66d9980711956c4e97a5e3a0331740e66209cdd848eeda95043aa6451`  
		Last Modified: Tue, 21 Nov 2023 08:13:12 GMT  
		Size: 3.3 KB (3279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28de35d37027aca235911a96ae3677e70df9d467bb195edb64f7a019cdb4a305`  
		Last Modified: Tue, 21 Nov 2023 08:13:13 GMT  
		Size: 936.1 KB (936110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d993395bbc46da711c512c8810005a2fddb2c46a658158ce0d8b0c203099b47`  
		Last Modified: Tue, 21 Nov 2023 08:13:17 GMT  
		Size: 89.2 MB (89163303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a148cd27f6958cb31dc0bc6d823c22fc5d6af19c1da775f87e67b5499a34db1`  
		Last Modified: Tue, 21 Nov 2023 08:13:12 GMT  
		Size: 21.7 MB (21662590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf608d5cbe30ca39e096fb8f5b5bbebb4f4e5a052fd9c2979d560e85a9c84546`  
		Last Modified: Tue, 21 Nov 2023 08:13:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3c788fa955fb8f765a8186d1ee4a82b4834a5f49f0b30d6558400eb79b1294`  
		Last Modified: Tue, 21 Nov 2023 08:13:10 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fff7c0e260aa2c2f71bb6437dcceb236b4429b6d65a0980032d83daebba1b4f`  
		Last Modified: Tue, 21 Nov 2023 08:13:11 GMT  
		Size: 6.3 KB (6285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7-alpine`

```console
$ docker pull influxdb@sha256:8344faf145ca0d2b938574b77847bcbdfd13df4774147cb9cedbb9f5910f9eba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ba08c9a5aed86654ce80f9e27fcb5e9a1b470f031bca320e7a7852ac6d8345f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.6 MB (87558514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e6885ff789a2b352d3025a6f80b199f107f56a65bb83bc64dd511b2f79ad381`
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
# Thu, 16 Nov 2023 01:34:39 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 16 Nov 2023 01:34:39 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Nov 2023 01:34:39 GMT
ENV INFLUXDB_VERSION=2.7.4
# Thu, 16 Nov 2023 01:34:43 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 16 Nov 2023 01:34:43 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 16 Nov 2023 01:34:45 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Nov 2023 01:34:46 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Nov 2023 01:34:46 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Nov 2023 01:34:46 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Nov 2023 01:34:46 GMT
COPY file:6341d1dd8e0763e797b79985007acd07a4686ed831d55018f6e390823bad9d07 in /entrypoint.sh 
# Thu, 16 Nov 2023 01:34:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Nov 2023 01:34:46 GMT
CMD ["influxd"]
# Thu, 16 Nov 2023 01:34:46 GMT
EXPOSE 8086
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Nov 2023 01:34:47 GMT
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
	-	`sha256:afcc69539951a864422f2d214e44ee6fc6d9c57c0a4edaefde6efc460ff2d90f`  
		Last Modified: Thu, 16 Nov 2023 01:35:47 GMT  
		Size: 5.8 MB (5820946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8bf8a03db3cd399c817901c93c81f234d4088e8ee6666a44c151359c18e67`  
		Last Modified: Thu, 16 Nov 2023 01:35:46 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f16af9f58f64f3fdd9b70d190a136a6b4a5d1192e277314a5d985beee82ce`  
		Last Modified: Thu, 16 Nov 2023 01:35:50 GMT  
		Size: 46.3 MB (46330663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dece05f716fd0148569f71292f440015201cb062bfc7680182e1ce7fc48373`  
		Last Modified: Thu, 16 Nov 2023 01:35:47 GMT  
		Size: 23.1 MB (23128356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4edff2dff21ee3c7321ec441eefc00e97710ee5ce673bd7e9a0bb586e451395`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5be165bc94e79bc9ed0eb2a05cbb0d303f08b60e263bf48b3280e4ca44443ae`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598b9a7d76be7074485ba1aa2c15542be5f810d6cec44b0484f7ebaca3c803a8`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 6.3 KB (6281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a42cd43a35de01ffcda2ddc8660e6f29f1f22c5928e8d288765cd8ebaf065b37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.0 MB (84006245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af78fd2382c4ce48b45f435206d8b7d093ff91de8e1ea63c11c06929e9a9b00`
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
# Thu, 16 Nov 2023 01:47:26 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 16 Nov 2023 01:47:27 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Nov 2023 01:47:27 GMT
ENV INFLUXDB_VERSION=2.7.4
# Thu, 16 Nov 2023 01:47:30 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 16 Nov 2023 01:47:30 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 16 Nov 2023 01:47:32 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Nov 2023 01:47:33 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Nov 2023 01:47:33 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Nov 2023 01:47:33 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Nov 2023 01:47:33 GMT
COPY file:6341d1dd8e0763e797b79985007acd07a4686ed831d55018f6e390823bad9d07 in /entrypoint.sh 
# Thu, 16 Nov 2023 01:47:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Nov 2023 01:47:33 GMT
CMD ["influxd"]
# Thu, 16 Nov 2023 01:47:33 GMT
EXPOSE 8086
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Nov 2023 01:47:34 GMT
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
	-	`sha256:f430534be970bcb57121ee1018f70360775d0bcf788ebdfa18a2b01c395e00a3`  
		Last Modified: Thu, 16 Nov 2023 01:48:08 GMT  
		Size: 5.5 MB (5463814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f302449250fc8480c8e59e4d8a9ff2cbb6abd3b805653cedc341b214bf20f0d2`  
		Last Modified: Thu, 16 Nov 2023 01:48:07 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156308fdb6aae0ed74aaea1ad996cb6711847dd546ba9a0fbb5d5fae588a788`  
		Last Modified: Thu, 16 Nov 2023 01:48:09 GMT  
		Size: 44.6 MB (44577399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b761820425e0d7dcd3a64ed40d5ecad5e65ea25f3ff316c5b5b22b70f4c064ed`  
		Last Modified: Thu, 16 Nov 2023 01:48:07 GMT  
		Size: 21.7 MB (21662586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c0e72f2f4415fe3b12828eea02e2d97fae456d91d1eddc77605207468f68ba`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fe7982d92d0b7304a9b203c4ae4d3c0740510e88bad5bdfc374cc099035858`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a66d9f557b60a3b1f2a1b5de2d9614dacbd3e5ae74579600877aafa1f42aad9`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 6.3 KB (6282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.4`

```console
$ docker pull influxdb@sha256:e0c66207e3f5cc16bc0730dc52a7fa81dbba6e366fe6ddf3daab0c3008af64c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.4` - linux; amd64

```console
$ docker pull influxdb@sha256:f29b8f0b153b60f8de48c24c306aaa529d7d41b34a218de66f5be54fff381f1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161577286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7897b6955cd3f184c223a285b295fe5ae8ef0987a48f0a55e8187eb712a26e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 13:25:37 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:25:38 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 21 Nov 2023 13:25:39 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 21 Nov 2023 13:25:39 GMT
ENV GOSU_VER=1.16
# Tue, 21 Nov 2023 13:25:42 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 21 Nov 2023 13:25:42 GMT
ENV INFLUXDB_VERSION=2.7.4
# Tue, 21 Nov 2023 13:25:46 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 21 Nov 2023 13:25:46 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 21 Nov 2023 13:25:48 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 21 Nov 2023 13:25:49 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 21 Nov 2023 13:25:49 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 21 Nov 2023 13:25:49 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 21 Nov 2023 13:25:49 GMT
COPY file:b5520696339eadb7386055c1dc9487351aa145a79b0cf206d8b1a79699c4a7f1 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:25:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:25:49 GMT
CMD ["influxd"]
# Tue, 21 Nov 2023 13:25:49 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 13:25:49 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 21 Nov 2023 13:25:49 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 21 Nov 2023 13:25:49 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 21 Nov 2023 13:25:49 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e16ccbb43e210cb9b0da0a8b4971c0fa31d20a2056b04b5484971672f4ecae`  
		Last Modified: Tue, 21 Nov 2023 13:28:00 GMT  
		Size: 9.8 MB (9787108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a7bc1934b125acef1dad572f6f4b9b2b067b0e2401fe3101c6f9c84fd2d66`  
		Last Modified: Tue, 21 Nov 2023 13:27:57 GMT  
		Size: 5.8 MB (5820939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0cc3c0c6d9b72e7a3405cd4e2d34d728114b9ef2f0a56f171c59a55c62560c`  
		Last Modified: Tue, 21 Nov 2023 13:27:56 GMT  
		Size: 3.3 KB (3281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6061761101c04e03323a78d890270df54f990643cb9a0fe4333ba062f551bb9b`  
		Last Modified: Tue, 21 Nov 2023 13:27:57 GMT  
		Size: 1.0 MB (1006415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bd7f35f51975fa9760f3b0e622e785db6345d9d3cdcf3d25c0d16ccc635885`  
		Last Modified: Tue, 21 Nov 2023 13:28:04 GMT  
		Size: 92.7 MB (92674468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42be173071fe813e09b2d2158e616e057dd18dbe899346d3670654e88416afd1`  
		Last Modified: Tue, 21 Nov 2023 13:27:57 GMT  
		Size: 23.1 MB (23128346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883524767a4d5892b71184007462ac2378706bfa480c5e6de52f94801c6a1161`  
		Last Modified: Tue, 21 Nov 2023 13:27:54 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbf9c48eb4f1377d905b362d02efe85e89a620b11f1fc7136fbdc6206eb1a72`  
		Last Modified: Tue, 21 Nov 2023 13:27:54 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fee5c5d25312db4b409b99ebc4a11b460ec71a3503f6e40d0d3cd2c1d3d6222`  
		Last Modified: Tue, 21 Nov 2023 13:27:54 GMT  
		Size: 6.3 KB (6285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.4` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c4ecdce031166cf259e184f5d4cdea7d44c2aec27b8420e458f57f31089af977
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (155999608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27028005c79759ba5d348e4ae235461f63fcfb8c96bf5ad5a7a9772d7f7fdb5d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:12:32 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:12:33 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 21 Nov 2023 08:12:33 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 21 Nov 2023 08:12:33 GMT
ENV GOSU_VER=1.16
# Tue, 21 Nov 2023 08:12:36 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 21 Nov 2023 08:12:36 GMT
ENV INFLUXDB_VERSION=2.7.4
# Tue, 21 Nov 2023 08:12:40 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 21 Nov 2023 08:12:41 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 21 Nov 2023 08:12:43 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 21 Nov 2023 08:12:44 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 21 Nov 2023 08:12:44 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 21 Nov 2023 08:12:44 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 21 Nov 2023 08:12:44 GMT
COPY file:b5520696339eadb7386055c1dc9487351aa145a79b0cf206d8b1a79699c4a7f1 in /entrypoint.sh 
# Tue, 21 Nov 2023 08:12:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 08:12:44 GMT
CMD ["influxd"]
# Tue, 21 Nov 2023 08:12:44 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 08:12:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 21 Nov 2023 08:12:45 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 21 Nov 2023 08:12:45 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 21 Nov 2023 08:12:45 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f21dcbd9a86a0ef0a65a79975ce3e1ae090d7e20a5afcfbfc4e957bfccfef3`  
		Last Modified: Tue, 21 Nov 2023 08:13:15 GMT  
		Size: 9.6 MB (9584431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e12bc048239d052071a3cbdf062079b2cb0180d5716ba182c6b3d2a6dfec8a`  
		Last Modified: Tue, 21 Nov 2023 08:13:13 GMT  
		Size: 5.5 MB (5463797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604f72c66d9980711956c4e97a5e3a0331740e66209cdd848eeda95043aa6451`  
		Last Modified: Tue, 21 Nov 2023 08:13:12 GMT  
		Size: 3.3 KB (3279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28de35d37027aca235911a96ae3677e70df9d467bb195edb64f7a019cdb4a305`  
		Last Modified: Tue, 21 Nov 2023 08:13:13 GMT  
		Size: 936.1 KB (936110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d993395bbc46da711c512c8810005a2fddb2c46a658158ce0d8b0c203099b47`  
		Last Modified: Tue, 21 Nov 2023 08:13:17 GMT  
		Size: 89.2 MB (89163303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a148cd27f6958cb31dc0bc6d823c22fc5d6af19c1da775f87e67b5499a34db1`  
		Last Modified: Tue, 21 Nov 2023 08:13:12 GMT  
		Size: 21.7 MB (21662590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf608d5cbe30ca39e096fb8f5b5bbebb4f4e5a052fd9c2979d560e85a9c84546`  
		Last Modified: Tue, 21 Nov 2023 08:13:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3c788fa955fb8f765a8186d1ee4a82b4834a5f49f0b30d6558400eb79b1294`  
		Last Modified: Tue, 21 Nov 2023 08:13:10 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fff7c0e260aa2c2f71bb6437dcceb236b4429b6d65a0980032d83daebba1b4f`  
		Last Modified: Tue, 21 Nov 2023 08:13:11 GMT  
		Size: 6.3 KB (6285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.7.4-alpine`

```console
$ docker pull influxdb@sha256:8344faf145ca0d2b938574b77847bcbdfd13df4774147cb9cedbb9f5910f9eba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.7.4-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ba08c9a5aed86654ce80f9e27fcb5e9a1b470f031bca320e7a7852ac6d8345f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.6 MB (87558514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e6885ff789a2b352d3025a6f80b199f107f56a65bb83bc64dd511b2f79ad381`
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
# Thu, 16 Nov 2023 01:34:39 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 16 Nov 2023 01:34:39 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Nov 2023 01:34:39 GMT
ENV INFLUXDB_VERSION=2.7.4
# Thu, 16 Nov 2023 01:34:43 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 16 Nov 2023 01:34:43 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 16 Nov 2023 01:34:45 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Nov 2023 01:34:46 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Nov 2023 01:34:46 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Nov 2023 01:34:46 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Nov 2023 01:34:46 GMT
COPY file:6341d1dd8e0763e797b79985007acd07a4686ed831d55018f6e390823bad9d07 in /entrypoint.sh 
# Thu, 16 Nov 2023 01:34:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Nov 2023 01:34:46 GMT
CMD ["influxd"]
# Thu, 16 Nov 2023 01:34:46 GMT
EXPOSE 8086
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Nov 2023 01:34:47 GMT
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
	-	`sha256:afcc69539951a864422f2d214e44ee6fc6d9c57c0a4edaefde6efc460ff2d90f`  
		Last Modified: Thu, 16 Nov 2023 01:35:47 GMT  
		Size: 5.8 MB (5820946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8bf8a03db3cd399c817901c93c81f234d4088e8ee6666a44c151359c18e67`  
		Last Modified: Thu, 16 Nov 2023 01:35:46 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f16af9f58f64f3fdd9b70d190a136a6b4a5d1192e277314a5d985beee82ce`  
		Last Modified: Thu, 16 Nov 2023 01:35:50 GMT  
		Size: 46.3 MB (46330663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dece05f716fd0148569f71292f440015201cb062bfc7680182e1ce7fc48373`  
		Last Modified: Thu, 16 Nov 2023 01:35:47 GMT  
		Size: 23.1 MB (23128356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4edff2dff21ee3c7321ec441eefc00e97710ee5ce673bd7e9a0bb586e451395`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5be165bc94e79bc9ed0eb2a05cbb0d303f08b60e263bf48b3280e4ca44443ae`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598b9a7d76be7074485ba1aa2c15542be5f810d6cec44b0484f7ebaca3c803a8`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 6.3 KB (6281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.7.4-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a42cd43a35de01ffcda2ddc8660e6f29f1f22c5928e8d288765cd8ebaf065b37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.0 MB (84006245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af78fd2382c4ce48b45f435206d8b7d093ff91de8e1ea63c11c06929e9a9b00`
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
# Thu, 16 Nov 2023 01:47:26 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 16 Nov 2023 01:47:27 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Nov 2023 01:47:27 GMT
ENV INFLUXDB_VERSION=2.7.4
# Thu, 16 Nov 2023 01:47:30 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 16 Nov 2023 01:47:30 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 16 Nov 2023 01:47:32 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Nov 2023 01:47:33 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Nov 2023 01:47:33 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Nov 2023 01:47:33 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Nov 2023 01:47:33 GMT
COPY file:6341d1dd8e0763e797b79985007acd07a4686ed831d55018f6e390823bad9d07 in /entrypoint.sh 
# Thu, 16 Nov 2023 01:47:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Nov 2023 01:47:33 GMT
CMD ["influxd"]
# Thu, 16 Nov 2023 01:47:33 GMT
EXPOSE 8086
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Nov 2023 01:47:34 GMT
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
	-	`sha256:f430534be970bcb57121ee1018f70360775d0bcf788ebdfa18a2b01c395e00a3`  
		Last Modified: Thu, 16 Nov 2023 01:48:08 GMT  
		Size: 5.5 MB (5463814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f302449250fc8480c8e59e4d8a9ff2cbb6abd3b805653cedc341b214bf20f0d2`  
		Last Modified: Thu, 16 Nov 2023 01:48:07 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156308fdb6aae0ed74aaea1ad996cb6711847dd546ba9a0fbb5d5fae588a788`  
		Last Modified: Thu, 16 Nov 2023 01:48:09 GMT  
		Size: 44.6 MB (44577399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b761820425e0d7dcd3a64ed40d5ecad5e65ea25f3ff316c5b5b22b70f4c064ed`  
		Last Modified: Thu, 16 Nov 2023 01:48:07 GMT  
		Size: 21.7 MB (21662586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c0e72f2f4415fe3b12828eea02e2d97fae456d91d1eddc77605207468f68ba`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fe7982d92d0b7304a9b203c4ae4d3c0740510e88bad5bdfc374cc099035858`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a66d9f557b60a3b1f2a1b5de2d9614dacbd3e5ae74579600877aafa1f42aad9`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 6.3 KB (6282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:8344faf145ca0d2b938574b77847bcbdfd13df4774147cb9cedbb9f5910f9eba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ba08c9a5aed86654ce80f9e27fcb5e9a1b470f031bca320e7a7852ac6d8345f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.6 MB (87558514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e6885ff789a2b352d3025a6f80b199f107f56a65bb83bc64dd511b2f79ad381`
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
# Thu, 16 Nov 2023 01:34:39 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 16 Nov 2023 01:34:39 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Nov 2023 01:34:39 GMT
ENV INFLUXDB_VERSION=2.7.4
# Thu, 16 Nov 2023 01:34:43 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 16 Nov 2023 01:34:43 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 16 Nov 2023 01:34:45 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Nov 2023 01:34:46 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Nov 2023 01:34:46 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Nov 2023 01:34:46 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Nov 2023 01:34:46 GMT
COPY file:6341d1dd8e0763e797b79985007acd07a4686ed831d55018f6e390823bad9d07 in /entrypoint.sh 
# Thu, 16 Nov 2023 01:34:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Nov 2023 01:34:46 GMT
CMD ["influxd"]
# Thu, 16 Nov 2023 01:34:46 GMT
EXPOSE 8086
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Nov 2023 01:34:47 GMT
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
	-	`sha256:afcc69539951a864422f2d214e44ee6fc6d9c57c0a4edaefde6efc460ff2d90f`  
		Last Modified: Thu, 16 Nov 2023 01:35:47 GMT  
		Size: 5.8 MB (5820946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8bf8a03db3cd399c817901c93c81f234d4088e8ee6666a44c151359c18e67`  
		Last Modified: Thu, 16 Nov 2023 01:35:46 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f16af9f58f64f3fdd9b70d190a136a6b4a5d1192e277314a5d985beee82ce`  
		Last Modified: Thu, 16 Nov 2023 01:35:50 GMT  
		Size: 46.3 MB (46330663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dece05f716fd0148569f71292f440015201cb062bfc7680182e1ce7fc48373`  
		Last Modified: Thu, 16 Nov 2023 01:35:47 GMT  
		Size: 23.1 MB (23128356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4edff2dff21ee3c7321ec441eefc00e97710ee5ce673bd7e9a0bb586e451395`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5be165bc94e79bc9ed0eb2a05cbb0d303f08b60e263bf48b3280e4ca44443ae`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598b9a7d76be7074485ba1aa2c15542be5f810d6cec44b0484f7ebaca3c803a8`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 6.3 KB (6281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a42cd43a35de01ffcda2ddc8660e6f29f1f22c5928e8d288765cd8ebaf065b37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.0 MB (84006245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af78fd2382c4ce48b45f435206d8b7d093ff91de8e1ea63c11c06929e9a9b00`
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
# Thu, 16 Nov 2023 01:47:26 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 16 Nov 2023 01:47:27 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Nov 2023 01:47:27 GMT
ENV INFLUXDB_VERSION=2.7.4
# Thu, 16 Nov 2023 01:47:30 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 16 Nov 2023 01:47:30 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 16 Nov 2023 01:47:32 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Nov 2023 01:47:33 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Nov 2023 01:47:33 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Nov 2023 01:47:33 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Nov 2023 01:47:33 GMT
COPY file:6341d1dd8e0763e797b79985007acd07a4686ed831d55018f6e390823bad9d07 in /entrypoint.sh 
# Thu, 16 Nov 2023 01:47:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Nov 2023 01:47:33 GMT
CMD ["influxd"]
# Thu, 16 Nov 2023 01:47:33 GMT
EXPOSE 8086
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Nov 2023 01:47:34 GMT
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
	-	`sha256:f430534be970bcb57121ee1018f70360775d0bcf788ebdfa18a2b01c395e00a3`  
		Last Modified: Thu, 16 Nov 2023 01:48:08 GMT  
		Size: 5.5 MB (5463814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f302449250fc8480c8e59e4d8a9ff2cbb6abd3b805653cedc341b214bf20f0d2`  
		Last Modified: Thu, 16 Nov 2023 01:48:07 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156308fdb6aae0ed74aaea1ad996cb6711847dd546ba9a0fbb5d5fae588a788`  
		Last Modified: Thu, 16 Nov 2023 01:48:09 GMT  
		Size: 44.6 MB (44577399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b761820425e0d7dcd3a64ed40d5ecad5e65ea25f3ff316c5b5b22b70f4c064ed`  
		Last Modified: Thu, 16 Nov 2023 01:48:07 GMT  
		Size: 21.7 MB (21662586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c0e72f2f4415fe3b12828eea02e2d97fae456d91d1eddc77605207468f68ba`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fe7982d92d0b7304a9b203c4ae4d3c0740510e88bad5bdfc374cc099035858`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a66d9f557b60a3b1f2a1b5de2d9614dacbd3e5ae74579600877aafa1f42aad9`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 6.3 KB (6282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:e0c66207e3f5cc16bc0730dc52a7fa81dbba6e366fe6ddf3daab0c3008af64c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:f29b8f0b153b60f8de48c24c306aaa529d7d41b34a218de66f5be54fff381f1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161577286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7897b6955cd3f184c223a285b295fe5ae8ef0987a48f0a55e8187eb712a26e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 13:25:37 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:25:38 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 21 Nov 2023 13:25:39 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 21 Nov 2023 13:25:39 GMT
ENV GOSU_VER=1.16
# Tue, 21 Nov 2023 13:25:42 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 21 Nov 2023 13:25:42 GMT
ENV INFLUXDB_VERSION=2.7.4
# Tue, 21 Nov 2023 13:25:46 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 21 Nov 2023 13:25:46 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 21 Nov 2023 13:25:48 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 21 Nov 2023 13:25:49 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 21 Nov 2023 13:25:49 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 21 Nov 2023 13:25:49 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 21 Nov 2023 13:25:49 GMT
COPY file:b5520696339eadb7386055c1dc9487351aa145a79b0cf206d8b1a79699c4a7f1 in /entrypoint.sh 
# Tue, 21 Nov 2023 13:25:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 13:25:49 GMT
CMD ["influxd"]
# Tue, 21 Nov 2023 13:25:49 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 13:25:49 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 21 Nov 2023 13:25:49 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 21 Nov 2023 13:25:49 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 21 Nov 2023 13:25:49 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e16ccbb43e210cb9b0da0a8b4971c0fa31d20a2056b04b5484971672f4ecae`  
		Last Modified: Tue, 21 Nov 2023 13:28:00 GMT  
		Size: 9.8 MB (9787108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a7bc1934b125acef1dad572f6f4b9b2b067b0e2401fe3101c6f9c84fd2d66`  
		Last Modified: Tue, 21 Nov 2023 13:27:57 GMT  
		Size: 5.8 MB (5820939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0cc3c0c6d9b72e7a3405cd4e2d34d728114b9ef2f0a56f171c59a55c62560c`  
		Last Modified: Tue, 21 Nov 2023 13:27:56 GMT  
		Size: 3.3 KB (3281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6061761101c04e03323a78d890270df54f990643cb9a0fe4333ba062f551bb9b`  
		Last Modified: Tue, 21 Nov 2023 13:27:57 GMT  
		Size: 1.0 MB (1006415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bd7f35f51975fa9760f3b0e622e785db6345d9d3cdcf3d25c0d16ccc635885`  
		Last Modified: Tue, 21 Nov 2023 13:28:04 GMT  
		Size: 92.7 MB (92674468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42be173071fe813e09b2d2158e616e057dd18dbe899346d3670654e88416afd1`  
		Last Modified: Tue, 21 Nov 2023 13:27:57 GMT  
		Size: 23.1 MB (23128346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883524767a4d5892b71184007462ac2378706bfa480c5e6de52f94801c6a1161`  
		Last Modified: Tue, 21 Nov 2023 13:27:54 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbf9c48eb4f1377d905b362d02efe85e89a620b11f1fc7136fbdc6206eb1a72`  
		Last Modified: Tue, 21 Nov 2023 13:27:54 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fee5c5d25312db4b409b99ebc4a11b460ec71a3503f6e40d0d3cd2c1d3d6222`  
		Last Modified: Tue, 21 Nov 2023 13:27:54 GMT  
		Size: 6.3 KB (6285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c4ecdce031166cf259e184f5d4cdea7d44c2aec27b8420e458f57f31089af977
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (155999608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27028005c79759ba5d348e4ae235461f63fcfb8c96bf5ad5a7a9772d7f7fdb5d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:12:32 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:12:33 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 21 Nov 2023 08:12:33 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 21 Nov 2023 08:12:33 GMT
ENV GOSU_VER=1.16
# Tue, 21 Nov 2023 08:12:36 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 21 Nov 2023 08:12:36 GMT
ENV INFLUXDB_VERSION=2.7.4
# Tue, 21 Nov 2023 08:12:40 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 21 Nov 2023 08:12:41 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 21 Nov 2023 08:12:43 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 21 Nov 2023 08:12:44 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 21 Nov 2023 08:12:44 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 21 Nov 2023 08:12:44 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 21 Nov 2023 08:12:44 GMT
COPY file:b5520696339eadb7386055c1dc9487351aa145a79b0cf206d8b1a79699c4a7f1 in /entrypoint.sh 
# Tue, 21 Nov 2023 08:12:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 08:12:44 GMT
CMD ["influxd"]
# Tue, 21 Nov 2023 08:12:44 GMT
EXPOSE 8086
# Tue, 21 Nov 2023 08:12:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 21 Nov 2023 08:12:45 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 21 Nov 2023 08:12:45 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 21 Nov 2023 08:12:45 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f21dcbd9a86a0ef0a65a79975ce3e1ae090d7e20a5afcfbfc4e957bfccfef3`  
		Last Modified: Tue, 21 Nov 2023 08:13:15 GMT  
		Size: 9.6 MB (9584431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e12bc048239d052071a3cbdf062079b2cb0180d5716ba182c6b3d2a6dfec8a`  
		Last Modified: Tue, 21 Nov 2023 08:13:13 GMT  
		Size: 5.5 MB (5463797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604f72c66d9980711956c4e97a5e3a0331740e66209cdd848eeda95043aa6451`  
		Last Modified: Tue, 21 Nov 2023 08:13:12 GMT  
		Size: 3.3 KB (3279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28de35d37027aca235911a96ae3677e70df9d467bb195edb64f7a019cdb4a305`  
		Last Modified: Tue, 21 Nov 2023 08:13:13 GMT  
		Size: 936.1 KB (936110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d993395bbc46da711c512c8810005a2fddb2c46a658158ce0d8b0c203099b47`  
		Last Modified: Tue, 21 Nov 2023 08:13:17 GMT  
		Size: 89.2 MB (89163303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a148cd27f6958cb31dc0bc6d823c22fc5d6af19c1da775f87e67b5499a34db1`  
		Last Modified: Tue, 21 Nov 2023 08:13:12 GMT  
		Size: 21.7 MB (21662590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf608d5cbe30ca39e096fb8f5b5bbebb4f4e5a052fd9c2979d560e85a9c84546`  
		Last Modified: Tue, 21 Nov 2023 08:13:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3c788fa955fb8f765a8186d1ee4a82b4834a5f49f0b30d6558400eb79b1294`  
		Last Modified: Tue, 21 Nov 2023 08:13:10 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fff7c0e260aa2c2f71bb6437dcceb236b4429b6d65a0980032d83daebba1b4f`  
		Last Modified: Tue, 21 Nov 2023 08:13:11 GMT  
		Size: 6.3 KB (6285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
