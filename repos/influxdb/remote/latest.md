## `influxdb:latest`

```console
$ docker pull influxdb@sha256:02d64a7a0219c4d2f898c17bb296f2e2af93263bc7c8ad52e0387700d362df7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:83ac305bee315e207ab8f8f26ee32c0d187d5450635a1e656bf7e132a735f84a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161550409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bc5178d3c0c8b8f63136cd3934cdfa042fb46c879aeb242502354bbb09b03cd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:51:39 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 01:51:40 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 19 Dec 2023 01:51:41 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 19 Dec 2023 01:51:41 GMT
ENV GOSU_VER=1.16
# Tue, 19 Dec 2023 01:51:43 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 19 Dec 2023 01:51:44 GMT
ENV INFLUXDB_VERSION=2.7.4
# Tue, 19 Dec 2023 01:51:48 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 19 Dec 2023 01:51:49 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 19 Dec 2023 01:51:51 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 19 Dec 2023 01:51:52 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 19 Dec 2023 01:51:52 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 19 Dec 2023 01:51:52 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 19 Dec 2023 01:51:52 GMT
COPY file:b5520696339eadb7386055c1dc9487351aa145a79b0cf206d8b1a79699c4a7f1 in /entrypoint.sh 
# Tue, 19 Dec 2023 01:51:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Dec 2023 01:51:52 GMT
CMD ["influxd"]
# Tue, 19 Dec 2023 01:51:52 GMT
EXPOSE 8086
# Tue, 19 Dec 2023 01:51:53 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 19 Dec 2023 01:51:53 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 19 Dec 2023 01:51:53 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 19 Dec 2023 01:51:53 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a67906d7dd432103b1c780bdbd13d9854069a64837d52b35c1a79be909c434`  
		Last Modified: Tue, 19 Dec 2023 01:52:35 GMT  
		Size: 9.8 MB (9784167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1ea001fd75e454d218e376727e04b64120d9f6637e29a008283b9a05e9abe6`  
		Last Modified: Tue, 19 Dec 2023 01:52:32 GMT  
		Size: 5.8 MB (5820930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325b8c3f9e1a6f5b8bf051ae41832f890e4b5cb509ec02adaed17cceaeadd894`  
		Last Modified: Tue, 19 Dec 2023 01:52:31 GMT  
		Size: 3.3 KB (3286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc333a124f91c1f052346fefad42c58d67029e7718007339eb0a339de90fc04`  
		Last Modified: Tue, 19 Dec 2023 01:52:32 GMT  
		Size: 1.0 MB (1006424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be14e5496008b67fe836d1820f9700cac4d0eda12e0e0a4a31a7b66eafe72fc`  
		Last Modified: Tue, 19 Dec 2023 01:52:39 GMT  
		Size: 92.7 MB (92674473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8da0fdfa83ae5d71b4efd5c40117d71e5d7b7be3279171dd6c227d5b2324e6`  
		Last Modified: Tue, 19 Dec 2023 01:52:32 GMT  
		Size: 23.1 MB (23128345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4909fd9fdca3fbafe1bb2853d3a7a59422b1ae92b36869fe1b5936b42e10b2c`  
		Last Modified: Tue, 19 Dec 2023 01:52:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9509ef8906240332891b90cf4b788cfd5f708f3adac0eb69d2b36ac93476bfcc`  
		Last Modified: Tue, 19 Dec 2023 01:52:30 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1abd7ca0728b7df5e4c0769b186b09d7edec32a92bf908e5c270f03c1df7af8`  
		Last Modified: Tue, 19 Dec 2023 01:52:29 GMT  
		Size: 6.3 KB (6286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b36a01dd51a24fb80cf30b4b22f4a6eb71b62342708222d2f1ca212baa95eb27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (155974341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27d9b13011007948e72cbd314cd10cea9e8cfe61ac1e0c5ad6d7aeafa0c241e5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:11 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 19 Dec 2023 01:41:11 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:34:14 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:34:16 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Tue, 19 Dec 2023 07:34:16 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Tue, 19 Dec 2023 07:34:16 GMT
ENV GOSU_VER=1.16
# Tue, 19 Dec 2023 07:34:19 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 19 Dec 2023 07:34:19 GMT
ENV INFLUXDB_VERSION=2.7.4
# Tue, 19 Dec 2023 07:34:22 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Tue, 19 Dec 2023 07:34:24 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Tue, 19 Dec 2023 07:34:26 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Tue, 19 Dec 2023 07:34:26 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 19 Dec 2023 07:34:26 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 19 Dec 2023 07:34:26 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 19 Dec 2023 07:34:27 GMT
COPY file:b5520696339eadb7386055c1dc9487351aa145a79b0cf206d8b1a79699c4a7f1 in /entrypoint.sh 
# Tue, 19 Dec 2023 07:34:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Dec 2023 07:34:27 GMT
CMD ["influxd"]
# Tue, 19 Dec 2023 07:34:27 GMT
EXPOSE 8086
# Tue, 19 Dec 2023 07:34:27 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 19 Dec 2023 07:34:27 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 19 Dec 2023 07:34:27 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 19 Dec 2023 07:34:27 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2564449ef650cbc8bfab8a892f7ded6422f10bd6bc66908b0153ca82fe7b5820`  
		Last Modified: Tue, 19 Dec 2023 07:34:45 GMT  
		Size: 9.6 MB (9581183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e99c97e2b822c1f88a75a194fb4dd14910f3acff9adb09679948fc5062fa6`  
		Last Modified: Tue, 19 Dec 2023 07:34:43 GMT  
		Size: 5.5 MB (5463803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cd8b077ebf07d964105ce3d55f5321e05d32fa1b44a2ca3882ea55e7da7bb5`  
		Last Modified: Tue, 19 Dec 2023 07:34:42 GMT  
		Size: 3.3 KB (3282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae792bd3e5ab80e8d51bafbfbc9f7626bb8ae474570409e5575837a4e52fe4e`  
		Last Modified: Tue, 19 Dec 2023 07:34:42 GMT  
		Size: 936.1 KB (936109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b67c4b041bb4c971df09e8dbfc1524ca43ca49408a91fcb70a912891370078`  
		Last Modified: Tue, 19 Dec 2023 07:34:47 GMT  
		Size: 89.2 MB (89163305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e9dd0616bb377914dbd81f68ee4e60c96aaadd04d751785176816ad96a841d`  
		Last Modified: Tue, 19 Dec 2023 07:34:42 GMT  
		Size: 21.7 MB (21662565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff7694a6727dd7cfc25ec1e9bf98a733eba6c549dfa0d1faf3dab66f15e4065`  
		Last Modified: Tue, 19 Dec 2023 07:34:40 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d0595fb6a836a2b7a181565f4567fc1323b07040323bb04b75baa83a66845a`  
		Last Modified: Tue, 19 Dec 2023 07:34:40 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d2d7f7906195fd440248ebfbce4bae214239d3b876592067e2c5df3b3fca7d`  
		Last Modified: Tue, 19 Dec 2023 07:34:40 GMT  
		Size: 6.3 KB (6286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
