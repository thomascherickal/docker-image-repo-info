## `influxdb:latest`

```console
$ docker pull influxdb@sha256:a34519b04044084c0e23192a464799577e6713ddbd957824b14d5a86b671788d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:0a4a3f27c53a8963ba1d5e944e33cc4226942df15c41bc1b0d95655e43750bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182884723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d73c2625c70a1fa038f94f56dbe38725259ded80a853869ac5552980a875948`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:44:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:44:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 07:07:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 13 Oct 2021 07:07:17 GMT
ENV GOSU_VER=1.12
# Wed, 13 Oct 2021 07:07:21 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 10 Nov 2021 00:20:22 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 10 Nov 2021 00:20:32 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 10 Nov 2021 00:20:32 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 10 Nov 2021 00:20:35 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 10 Nov 2021 00:20:36 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 10 Nov 2021 00:20:36 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 10 Nov 2021 00:20:36 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 10 Nov 2021 00:20:37 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Wed, 10 Nov 2021 00:20:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Nov 2021 00:20:37 GMT
CMD ["influxd"]
# Wed, 10 Nov 2021 00:20:37 GMT
EXPOSE 8086
# Wed, 10 Nov 2021 00:20:37 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 10 Nov 2021 00:20:38 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 10 Nov 2021 00:20:38 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 10 Nov 2021 00:20:38 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cef1aa2170c001b320769bf8b018ed82d2c94a673e3010ea1ffe152e107419`  
		Last Modified: Tue, 12 Oct 2021 15:54:16 GMT  
		Size: 7.8 MB (7833862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a51f13be8e69cfc526b671d0bbf621b985b0932acd1523050e2995777b5926`  
		Last Modified: Tue, 12 Oct 2021 15:54:17 GMT  
		Size: 10.0 MB (9997204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f021d1bd1c1c4ade3c6735b14217da448a0652423cc873ea756cd9ff8be885`  
		Last Modified: Wed, 13 Oct 2021 07:10:56 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf4e96afd5f402dd4d28be0dbec47de5eb545cf12acc2bcc50a5de9a6ae4f3b`  
		Last Modified: Wed, 13 Oct 2021 07:10:53 GMT  
		Size: 961.0 KB (960997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea3525456d27d9e69f3f8be22a430daafe3ad52c92e2129e63245c44d18a4d0`  
		Last Modified: Wed, 10 Nov 2021 00:22:07 GMT  
		Size: 108.3 MB (108324821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db20b0028f015ac48eb0cf65daa17d5a172b16e146ecef780686c5899380ce3`  
		Last Modified: Wed, 10 Nov 2021 00:21:59 GMT  
		Size: 5.3 MB (5324481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18eff06d4dacfca68004495e56ef068c52d0019ce0e0ecda8ac905ed82a67831`  
		Last Modified: Wed, 10 Nov 2021 00:21:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60506ad273aca7ac342f92ebd651d41e34803959355ae77b00f5898373a84f6`  
		Last Modified: Wed, 10 Nov 2021 00:21:58 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684cd31a7f229ab0a7c2521acc3172cc797b2a4b8b2af3b16066a1ecb21236e4`  
		Last Modified: Wed, 10 Nov 2021 00:21:59 GMT  
		Size: 4.3 KB (4325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c4f1637011d9aa0523f9ebd5890018f1e425acb65b8b43e85c59be8efafd4702
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183386249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ff72e7682d1fca9dc68c41b265e5100456409ce4cd5f2881b18d0aca772dbad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:59:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:59:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 09:51:21 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 16 Oct 2021 09:51:22 GMT
ENV GOSU_VER=1.12
# Sat, 16 Oct 2021 09:51:26 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 10 Nov 2021 00:39:54 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 10 Nov 2021 00:40:06 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 10 Nov 2021 00:40:06 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 10 Nov 2021 00:40:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 10 Nov 2021 00:40:12 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 10 Nov 2021 00:40:12 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 10 Nov 2021 00:40:14 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 10 Nov 2021 00:40:15 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Wed, 10 Nov 2021 00:40:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Nov 2021 00:40:16 GMT
CMD ["influxd"]
# Wed, 10 Nov 2021 00:40:17 GMT
EXPOSE 8086
# Wed, 10 Nov 2021 00:40:18 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 10 Nov 2021 00:40:19 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 10 Nov 2021 00:40:20 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 10 Nov 2021 00:40:21 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7324ea4098419bc5fa2ac5a138522230bf12cef3996d1740dd00f9d4737d004`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 7.7 MB (7695063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e213c33a07316d84d829be685bd3b02e1e2bc135f7748c932050e6ed6a3a0d3`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 9.8 MB (9767289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9ddab23aef29b7845339636b8bdfc07fb3962d4faae05bdcd6c63537409d9e`  
		Last Modified: Sat, 16 Oct 2021 09:52:59 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ec40b1bb8f9487939e97b4f5d1e9aaf97b63c2a0dad7c6c4e913156ddf60c9`  
		Last Modified: Sat, 16 Oct 2021 09:52:57 GMT  
		Size: 896.4 KB (896360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21612e5bd4d177dfc9a948ce5fa9a85d371256482abf0239541292cd086c729f`  
		Last Modified: Wed, 10 Nov 2021 00:41:39 GMT  
		Size: 110.9 MB (110891631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b410920a725d90aac7e05b4498eebde21be3718218e67e3c774884408b287b9e`  
		Last Modified: Wed, 10 Nov 2021 00:41:31 GMT  
		Size: 4.9 MB (4906725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161c4d8eec87606c7b67194b4f51cb6e2bcdc8fca0c5819e7b7601b3f077f8cd`  
		Last Modified: Wed, 10 Nov 2021 00:41:29 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f40a4045524de3ff1b560dd07242f5ab4932568e5c45e861527d4af77bd0c48`  
		Last Modified: Wed, 10 Nov 2021 00:41:29 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a391d9c7ca413fa7d4eeef02791c4781e6738de022e558016837a08ddceca459`  
		Last Modified: Wed, 10 Nov 2021 00:41:29 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
