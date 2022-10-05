## `influxdb:latest`

```console
$ docker pull influxdb@sha256:ca943fe9d445aafc3e767a4a9e2c066f6c7abf562c75793b2e43f34a614ba4bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:3f24f79110e6f15f3cf46b70861b88f22a9063e36e505ce6940122da5e9ef85d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261138289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4beafc45eab51a6f2f21fc0c8609edec4f551edef0086a67096dc4d92e8b5ffe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 22:57:58 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 05 Oct 2022 22:57:58 GMT
ENV GOSU_VER=1.12
# Wed, 05 Oct 2022 22:58:01 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 05 Oct 2022 22:58:38 GMT
ENV INFLUXDB_VERSION=2.4.0
# Wed, 05 Oct 2022 22:58:45 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 05 Oct 2022 22:58:45 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Wed, 05 Oct 2022 22:58:49 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 05 Oct 2022 22:58:50 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 05 Oct 2022 22:58:50 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 05 Oct 2022 22:58:50 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 05 Oct 2022 22:58:50 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 05 Oct 2022 22:58:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 22:58:50 GMT
CMD ["influxd"]
# Wed, 05 Oct 2022 22:58:50 GMT
EXPOSE 8086
# Wed, 05 Oct 2022 22:58:50 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 05 Oct 2022 22:58:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 05 Oct 2022 22:58:51 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 05 Oct 2022 22:58:51 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052939bebd2aaf4445f0253bd9d7dfecad1616c16f16bbe5e67f21abe684c52a`  
		Last Modified: Wed, 05 Oct 2022 23:01:35 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21609a5a5a7297f0a4c26a0c8c5e0948ce744bd4ee7a01dac18955bdce73a6ef`  
		Last Modified: Wed, 05 Oct 2022 23:01:35 GMT  
		Size: 961.0 KB (960955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220dce776f1773db0f6103bcc2b22674fbdf73f3e247ef7282fb0c1375abcdd5`  
		Last Modified: Wed, 05 Oct 2022 23:02:30 GMT  
		Size: 185.8 MB (185802077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280ab4f4051a1633d0c818a64d6f0488501a45fd0a41d9d9b046db27a489440b`  
		Last Modified: Wed, 05 Oct 2022 23:02:18 GMT  
		Size: 6.1 MB (6071075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb09a2adf00cf3112a483cc1456749f358ce4a6738cfc0305866a440a3958e7`  
		Last Modified: Wed, 05 Oct 2022 23:02:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374968ae152709cb0c5b02d6895e5c118240eb6263f4772629f3d2c3f9ed731b`  
		Last Modified: Wed, 05 Oct 2022 23:02:17 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3db19ce805e81726d539935183be0758fe1f732fac44822ae6629d366e50d`  
		Last Modified: Wed, 05 Oct 2022 23:02:17 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:2d8e959e3d780ff1fa2881ac5c1ab41e165559de9a22afeb2bd6ca5a7e9acba5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255669493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a135265d8df6ac8017a3c343d561ee5e86adeaabddb8c6b5c157c7649b8e24`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:24:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:24:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 20:58:07 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 05 Oct 2022 20:58:08 GMT
ENV GOSU_VER=1.12
# Wed, 05 Oct 2022 20:58:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 05 Oct 2022 20:59:34 GMT
ENV INFLUXDB_VERSION=2.4.0
# Wed, 05 Oct 2022 20:59:43 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 05 Oct 2022 20:59:43 GMT
ENV INFLUX_CLI_VERSION=2.4.0
# Wed, 05 Oct 2022 20:59:47 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 05 Oct 2022 20:59:48 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 05 Oct 2022 20:59:48 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 05 Oct 2022 20:59:50 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 05 Oct 2022 20:59:51 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 05 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 20:59:52 GMT
CMD ["influxd"]
# Wed, 05 Oct 2022 20:59:53 GMT
EXPOSE 8086
# Wed, 05 Oct 2022 20:59:54 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 05 Oct 2022 20:59:55 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 05 Oct 2022 20:59:56 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 05 Oct 2022 20:59:57 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ae492f07ea828401b80eb34c8c630b72cb66cac155b003e81ab2921dc57f3d`  
		Last Modified: Wed, 05 Oct 2022 00:38:37 GMT  
		Size: 7.7 MB (7722031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c91e11c5a0db8322590ddbb61600624fdd82d3d6174d1de01c30be3e7ca535`  
		Last Modified: Wed, 05 Oct 2022 00:38:37 GMT  
		Size: 9.8 MB (9769003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3f86ba99cb6f7aa838b8b9d0c8aa2c75e63661ad283271f2747865bfc22ee4`  
		Last Modified: Wed, 05 Oct 2022 21:01:03 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003eb57573f5de13e555520181770c0cb9e21888eba93c783c220a2ddb85238`  
		Last Modified: Wed, 05 Oct 2022 21:01:03 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58da9769a7796dec848467f73dc66e715c8b627ad82dc306623d689e5e76ce0e`  
		Last Modified: Wed, 05 Oct 2022 21:02:06 GMT  
		Size: 182.4 MB (182445460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c1c4715d791da6b7234886b2c257b50ad82a521f6fe87782d139a93566c2f9`  
		Last Modified: Wed, 05 Oct 2022 21:01:52 GMT  
		Size: 5.6 MB (5600656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42fef127012439ecff5200afd74130edfa1c75d7ffaed41e09b086f10bc246d8`  
		Last Modified: Wed, 05 Oct 2022 21:01:51 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f05bdc200edb765aef94fd5df982cd0c8781b9ace6f52ffd8106489b07b02c2`  
		Last Modified: Wed, 05 Oct 2022 21:01:52 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a2c20123359c4152c0d6a010123c8cf5818b61a4765015b44cb15a4f81604b`  
		Last Modified: Wed, 05 Oct 2022 21:01:51 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
