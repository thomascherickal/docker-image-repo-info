## `influxdb:latest`

```console
$ docker pull influxdb@sha256:7d6dcce155a3a09d2c29e0d03c8f26514081b730938aab560df3d40044a9a9f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:eb77f0b6b3aa3bd48b85a13901d15ab14f45886139726e62749a26361bb9fad6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178699726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f26c7e4d38bc7c7152149e875c156ea37b264cad7ab9c8dcd870f3b36c56fa4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:52:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:53:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 24 Jun 2021 01:34:12 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 24 Jun 2021 01:34:12 GMT
ENV GOSU_VER=1.12
# Thu, 24 Jun 2021 01:34:16 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Thu, 24 Jun 2021 01:34:16 GMT
ENV INFLUXDB_VERSION=2.0.7
# Thu, 24 Jun 2021 01:34:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Thu, 24 Jun 2021 01:34:24 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 24 Jun 2021 01:34:24 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 24 Jun 2021 01:34:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 24 Jun 2021 01:34:25 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Thu, 24 Jun 2021 01:34:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:25 GMT
CMD ["influxd"]
# Thu, 24 Jun 2021 01:34:25 GMT
EXPOSE 8086
# Thu, 24 Jun 2021 01:34:25 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 24 Jun 2021 01:34:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 24 Jun 2021 01:34:26 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110e58716600c199fc95f633b30735c33a25b5adcfb16d1d7edbcb78a3f1b62`  
		Last Modified: Wed, 23 Jun 2021 01:01:46 GMT  
		Size: 7.8 MB (7832997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c0fa203acbade733bff627daa75b84c97f9d0553bcdf967a3f1d37471277`  
		Last Modified: Wed, 23 Jun 2021 01:01:47 GMT  
		Size: 10.0 MB (9997255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe08b7c7bd34fd2cc223ec3dfd86c583df78662452299ef0b9a600029277aa4`  
		Last Modified: Thu, 24 Jun 2021 01:37:16 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a752c953de6a8c86fd67cb69bc183cdded89c24ed14841e10e7940e368e70e`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 961.0 KB (960991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fee0b4534651e45a7733ad0a8f540ba6fbd8244fe01d2ef2f40de41592d00b`  
		Last Modified: Thu, 24 Jun 2021 01:37:24 GMT  
		Size: 109.5 MB (109466206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d853369c0c65d10005eb5b355804eee81fadd95f33c395921e83bb9dbe45ea`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fd4c49d9b93bd5c6e45ae0d18613bedcdaabaf2d18c8aa29a601ba1f8beefb`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f535b15085d744218e83e7393e9e3b586063a472fa97ed6af28157042b1dcb1`  
		Last Modified: Thu, 24 Jun 2021 01:37:15 GMT  
		Size: 4.3 KB (4316 bytes)  
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
