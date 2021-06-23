## `influxdb:latest`

```console
$ docker pull influxdb@sha256:e80fe1f239c78881571d487d4356f3ae379dbedf44f2cf8dcb2444e2c3229222
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:b50f219df32da917355b0db781150e6d0b89f149805663440a9e04c796ac13c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178697196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd6a4507399651c8d686cd4a63db7ef4312feb26e62846dc2398df2358bfbd63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:10:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 12 May 2021 20:10:17 GMT
ENV GOSU_VER=1.12
# Wed, 12 May 2021 20:10:20 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 05 Jun 2021 00:31:22 GMT
ENV INFLUXDB_VERSION=2.0.7
# Sat, 05 Jun 2021 00:31:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 05 Jun 2021 00:31:35 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 05 Jun 2021 00:31:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 05 Jun 2021 00:31:35 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 05 Jun 2021 00:31:35 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Sat, 05 Jun 2021 00:31:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Jun 2021 00:31:36 GMT
CMD ["influxd"]
# Sat, 05 Jun 2021 00:31:36 GMT
EXPOSE 8086
# Sat, 05 Jun 2021 00:31:36 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 05 Jun 2021 00:31:36 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 05 Jun 2021 00:31:37 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b26e21cfb07a9a6fd606a130ce8206843d702e4f616d53df1321437a01a0ac0`  
		Last Modified: Wed, 12 May 2021 20:13:23 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77b907603e396f34b2bbb8229e1a740deabeb6537f737d78db0f2452f2504e8`  
		Last Modified: Wed, 12 May 2021 20:13:20 GMT  
		Size: 961.0 KB (960988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9591ed1fb6b3d71a7c4957993349963b5bf90e1a59c9104548b9c7afc65b1a08`  
		Last Modified: Sat, 05 Jun 2021 00:32:49 GMT  
		Size: 109.5 MB (109466216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba458e8eb79c92d9d076a9758c228a52d495388a8520755dbd5869f878de262c`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac66788c54e9775c3aef47ef263022a66b957839916cb13f5750434938853cfa`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608813173efe22b91f20d22d9f0056154ffdf93c54dbb83c2656215808797c30`  
		Last Modified: Sat, 05 Jun 2021 00:32:39 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:d9825b3d372ad663f34bf92a3ebc1b9022906062b06986a0f203c5ab8670fec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180628536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcdad0ed3f5fbd15e87467aad894389fa02f9ecb82c2710bc7bd62d50db96409`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:34:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 23 Jun 2021 18:34:17 GMT
ENV GOSU_VER=1.12
# Wed, 23 Jun 2021 18:34:20 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 23 Jun 2021 18:34:20 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 23 Jun 2021 18:34:28 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 23 Jun 2021 18:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 23 Jun 2021 18:34:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 23 Jun 2021 18:34:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 23 Jun 2021 18:34:30 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 23 Jun 2021 18:34:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:34:30 GMT
CMD ["influxd"]
# Wed, 23 Jun 2021 18:34:30 GMT
EXPOSE 8086
# Wed, 23 Jun 2021 18:34:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b86f0fed5df426869e08ab884f79326e9a310498fb9c49929e08f9ef9002b`  
		Last Modified: Wed, 23 Jun 2021 18:35:51 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f865c284b0e6b32bd1f1dd14ec1e334cbadc7d6292712190efa42f4718b8dd`  
		Last Modified: Wed, 23 Jun 2021 18:35:48 GMT  
		Size: 896.4 KB (896380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea300fef38e2d57c2657aaad371813835137c72d9f2c258e56af5006e4e5797`  
		Last Modified: Wed, 23 Jun 2021 18:36:00 GMT  
		Size: 112.8 MB (112824510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0fc3d9ce52b5368331dd5726abd82bd12ed7c3e8a23a33cdc89f2fbf64ab73`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f091d2bde4f35ffdd2cb09c6e1bdce03228e14e72564adc636b11ddf9829ce`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b9b006308f765debe388af66277c827d88a43a1cc4a90dee951af142b3d1d0`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
