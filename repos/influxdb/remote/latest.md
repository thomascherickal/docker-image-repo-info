## `influxdb:latest`

```console
$ docker pull influxdb@sha256:f2543c9cc70fd75298a52647d828047ff5fbcd28f19be8a70bf9fb1429b5b6f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:7fd69f4a2c16efc0d5c2863ce2d74d9479dfc458ade2132379b94c28a04913c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182885029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfb4d421b2f653f5e58125af722b2677eb5c4f0fc2a125ef654b8ebd91550f34`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:45:40 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 18 Nov 2021 09:45:40 GMT
ENV GOSU_VER=1.12
# Thu, 18 Nov 2021 09:45:44 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Thu, 18 Nov 2021 09:46:04 GMT
ENV INFLUXDB_VERSION=2.1.1
# Thu, 18 Nov 2021 09:46:12 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 18 Nov 2021 09:46:13 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Thu, 18 Nov 2021 09:46:17 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 18 Nov 2021 09:46:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 18 Nov 2021 09:46:19 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 18 Nov 2021 09:46:19 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 18 Nov 2021 09:46:19 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:46:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:46:20 GMT
CMD ["influxd"]
# Thu, 18 Nov 2021 09:46:20 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 18 Nov 2021 09:46:21 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a603b07c93043ffbd790761bf1cf232dd2763ec10c3ef84ce381390713c99`  
		Last Modified: Thu, 18 Nov 2021 09:50:12 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80de06b69dbd583c55db5aebf57682c087c624d343e0410552603f35686a40`  
		Last Modified: Thu, 18 Nov 2021 09:50:10 GMT  
		Size: 961.0 KB (960988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf4fe7d34889b9b417a1448e1fee0a421bef2c9533916a1f513e8fdfd7baf99`  
		Last Modified: Thu, 18 Nov 2021 09:50:44 GMT  
		Size: 108.3 MB (108324825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8efd2d9a5def9f50aa609b47f8a39012190fb713c9ea285b497c24d014155`  
		Last Modified: Thu, 18 Nov 2021 09:50:36 GMT  
		Size: 5.3 MB (5324484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0d1b444bc9f9096339ec15ce0e4456f4823121b9214b2710b46c82e9147c8d`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f05877070f022483807a8ff887e1619260f8008f79b31053d9d3761acc7174`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c522e98cfb3d02a730692d7aef75148fd190b0192ed98300bed425c66842a9fd`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 4.3 KB (4321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b50ab5a02481210516a7b440d910051c76f1b3fea61255bf554657f7368bb60d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183386413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905455e4cd353ee4e93fd7658b084034e0ad5661373b055973befbc41ae696c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:39:03 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 17 Nov 2021 21:39:04 GMT
ENV GOSU_VER=1.12
# Wed, 17 Nov 2021 21:39:08 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 17 Nov 2021 21:39:43 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 17 Nov 2021 21:40:02 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 17 Nov 2021 21:40:02 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 17 Nov 2021 21:40:07 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 17 Nov 2021 21:40:07 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 17 Nov 2021 21:40:08 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 17 Nov 2021 21:40:10 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 17 Nov 2021 21:40:11 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Wed, 17 Nov 2021 21:40:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:40:12 GMT
CMD ["influxd"]
# Wed, 17 Nov 2021 21:40:13 GMT
EXPOSE 8086
# Wed, 17 Nov 2021 21:40:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 17 Nov 2021 21:40:15 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 17 Nov 2021 21:40:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 17 Nov 2021 21:40:17 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90efb0d865d89e679077061bdca34c60306bacab5579d93a951cd8c31441ec`  
		Last Modified: Wed, 17 Nov 2021 21:41:46 GMT  
		Size: 1.7 KB (1659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f283e1015297042ffd1e94f9753b4ef6b9ce33339509b31d96c13eb7dcd03f82`  
		Last Modified: Wed, 17 Nov 2021 21:41:44 GMT  
		Size: 896.4 KB (896361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d89c50dbb1d05a49120a4b621b6b382d2b29d6304c7f10b0eee084dab7d8dac`  
		Last Modified: Wed, 17 Nov 2021 21:42:16 GMT  
		Size: 110.9 MB (110891616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e6709d1f966cd8da3d817ff591df547559a47204cff841140f0c4f205c829f`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 4.9 MB (4906724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31859363882c3135133fce1a0f41006d7cb4c7ee4a669ea650ba2c541af3b7d5`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec1462a4ae6c9e136f82cbc586a32ea5c2b7089fa2ae02d94cdb2380b2369f`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e7de37831dc0c6521d41919d1fff71b50a3dfe399e29199fcb1e812dad17cb`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
