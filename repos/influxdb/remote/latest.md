## `influxdb:latest`

```console
$ docker pull influxdb@sha256:fab9340bffa2f23c7e96d765b8403aefdec07d948151d44336976f402e01a211
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:11b8f3ad1e8a41a028b2de4b9a0466a57df7a25386bfd347d220ccca1a75b4dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114621478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ca18052b424265e2afadad6d256121ef833fc3a7ca8e77a14832a2aa1d8218`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 12:40:19 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:40:20 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 03 May 2023 12:40:20 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 03 May 2023 12:40:21 GMT
ENV GOSU_VER=1.12
# Wed, 03 May 2023 12:40:23 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 03 May 2023 12:40:23 GMT
ENV INFLUXDB_VERSION=2.7.1
# Wed, 03 May 2023 12:40:27 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 03 May 2023 12:40:27 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 03 May 2023 12:40:29 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 03 May 2023 12:40:30 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 03 May 2023 12:40:30 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 03 May 2023 12:40:30 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 03 May 2023 12:40:30 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Wed, 03 May 2023 12:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 12:40:30 GMT
CMD ["influxd"]
# Wed, 03 May 2023 12:40:30 GMT
EXPOSE 8086
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 03 May 2023 12:40:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 03 May 2023 12:40:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0794cf0495a3caa74a71b6504803db62386b162e0862936e7094165af35a7ca2`  
		Last Modified: Wed, 03 May 2023 12:42:34 GMT  
		Size: 6.3 MB (6327884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4f7028e33b7b5de9c755a27c3e9ea1cf7d9913cb6c9b5cfcac31cd9a447a8`  
		Last Modified: Wed, 03 May 2023 12:42:33 GMT  
		Size: 6.4 MB (6434104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf91486cf86efc213e9b76cad5e74d49d01dc78896657c3d004b559198f73be`  
		Last Modified: Wed, 03 May 2023 12:42:31 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91daaa2fee4ceb2f269b802c20828e0ac42083951c9fcc9ed0e3c4dc42153f6`  
		Last Modified: Wed, 03 May 2023 12:42:32 GMT  
		Size: 982.0 KB (982049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fdcd2c51969abd5037cc3d56c63e90bc690dde62815fd99efb0efb695b0e52`  
		Last Modified: Wed, 03 May 2023 12:42:35 GMT  
		Size: 46.3 MB (46334322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46a6f45402719e52e80ca1165e7f375999ec943f1e31d5c15ac0f5cc0ef1569`  
		Last Modified: Wed, 03 May 2023 12:42:32 GMT  
		Size: 23.1 MB (23128344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c1d04df637a1edfea8b7f4a66691694104d136429b8fde52098203255c22a1`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a0962e3a5b231760a56a750fbb7f02fa94037b65c765177e10391997d8edf0`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bcae2cf40e36863a533dc1b6c6b622312e7460093175b16b1622fb656f721c`  
		Last Modified: Wed, 03 May 2023 12:42:30 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:fc5b1620f2feb33fb628b98cf8be819b20b9388a4a0876fe8616f46297577dd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109341848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c07a0fdb5b8d38ca2dfc1bd9fcd0ebd2b8732afcff491b0c7175eb2b8cddfc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 10:28:31 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 10:28:32 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 23 May 2023 10:28:33 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 23 May 2023 10:28:33 GMT
ENV GOSU_VER=1.12
# Tue, 23 May 2023 10:28:35 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 23 May 2023 10:28:35 GMT
ENV INFLUXDB_VERSION=2.7.1
# Tue, 23 May 2023 10:28:40 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 23 May 2023 10:28:40 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 23 May 2023 10:28:42 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 23 May 2023 10:28:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 23 May 2023 10:28:43 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 23 May 2023 10:28:43 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 23 May 2023 10:28:43 GMT
COPY file:b2f82a21cacf15bfd33d086d13395b3fe609087beb55e405789439a8db276c76 in /entrypoint.sh 
# Tue, 23 May 2023 10:28:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 10:28:43 GMT
CMD ["influxd"]
# Tue, 23 May 2023 10:28:44 GMT
EXPOSE 8086
# Tue, 23 May 2023 10:28:44 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 23 May 2023 10:28:44 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 23 May 2023 10:28:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 23 May 2023 10:28:44 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b4d959f2a9e6dcc2b76d362fb3b4ce079e2a2ae97d087dc48b592ea417673d`  
		Last Modified: Tue, 23 May 2023 10:29:14 GMT  
		Size: 6.3 MB (6308721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80c3ff93d7127588716c356d3a1fbee44c7910aed9625985d243262a739486`  
		Last Modified: Tue, 23 May 2023 10:29:12 GMT  
		Size: 6.0 MB (5953759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c42b946f32ece6dc24bd81c3cb18d01a5e00925d2b98a24bc66136754654ae`  
		Last Modified: Tue, 23 May 2023 10:29:11 GMT  
		Size: 4.1 KB (4121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115ee03ed541a9e07eb4f08ab1f8938f528cf06c36b6cbe3c4a12f36a1242036`  
		Last Modified: Tue, 23 May 2023 10:29:11 GMT  
		Size: 916.9 KB (916936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e32c1c91c4e7a2d414267d7cf78594949fa1c65ac1fea536914acab85c31371`  
		Last Modified: Tue, 23 May 2023 10:29:13 GMT  
		Size: 44.4 MB (44435842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b1582531b40c1ff0c2720a6a9f7e679c904245d6d4ab89001a99ced4a5956e`  
		Last Modified: Tue, 23 May 2023 10:29:11 GMT  
		Size: 21.7 MB (21662580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398c9eb2b6b7c104a3340a8d44153126934d5733dde6d6902910b28a53f67c52`  
		Last Modified: Tue, 23 May 2023 10:29:09 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb5fc2f382c7d2d699bb3ee83e946931f18ac38f28c60e58bf4036887059f48`  
		Last Modified: Tue, 23 May 2023 10:29:09 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f306a50992ccab8341525a69be57c1d4afe200910b4f9490a045c95252a483`  
		Last Modified: Tue, 23 May 2023 10:29:09 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
