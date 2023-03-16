## `influxdb:latest`

```console
$ docker pull influxdb@sha256:dfa86201228943d0ac8c3e675fc8e85843a872a9edeedb0b3fddf52e64414188
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:d9ea508f639968720934cc9dd727e83cd5515f87c7a35fec044728a455a9578b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.8 MB (98837218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a023b77ee0d8d5dbfca34a91f77e165247c3017017b782924ce74aa7dcfde836`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 00:56:52 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 00:56:53 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Thu, 16 Mar 2023 00:56:53 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 16 Mar 2023 00:56:53 GMT
ENV GOSU_VER=1.12
# Thu, 16 Mar 2023 00:56:56 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Thu, 16 Mar 2023 00:57:46 GMT
ENV INFLUXDB_VERSION=2.6.1
# Thu, 16 Mar 2023 00:57:50 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 16 Mar 2023 00:57:50 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Thu, 16 Mar 2023 00:57:52 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Mar 2023 00:57:53 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Mar 2023 00:57:53 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Mar 2023 00:57:53 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Mar 2023 00:57:53 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:57:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:57:53 GMT
CMD ["influxd"]
# Thu, 16 Mar 2023 00:57:53 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Mar 2023 00:57:53 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Mar 2023 00:57:53 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a794c78d7ad502e285244fde2dd7768065af2038670e7f34208e22d1c857e2`  
		Last Modified: Thu, 16 Mar 2023 01:02:10 GMT  
		Size: 6.3 MB (6327743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd90bd5b5e60e8373c43b82a755b742e62d469c7df42aef9ab6ad0ac943ef6b`  
		Last Modified: Thu, 16 Mar 2023 01:02:09 GMT  
		Size: 7.0 MB (7049181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549c3bac6c035d00d970ff0a7c39398de5b5355e5264970174a609dfcb350c1`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d52f68e8e59a067e13373eed04aa01fa28f3e99320d3ccfb46232c85efe7432`  
		Last Modified: Thu, 16 Mar 2023 01:02:08 GMT  
		Size: 982.0 KB (982043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48976d943c24ad838f918383f3fa1d1cbb1b40eb19d039b778c23ea46752a865`  
		Last Modified: Thu, 16 Mar 2023 01:03:12 GMT  
		Size: 46.8 MB (46844106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3539972aef6eac29878ccd083697a376eb1aec8d5e229b5c8a6dcab6036edea`  
		Last Modified: Thu, 16 Mar 2023 01:03:07 GMT  
		Size: 6.2 MB (6211626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb00e5e812eae43c162c6884051314289a906fcf9e53e5c6e8578ad0f5c1c00`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec172591e2a97b25dd5c54f835a03191efb469ea9b38708ac8c0d7c7dc16f764`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca79f302ed0dd277dff382083d00f0d5d62349e4defa511a5a54753e2358b2f5`  
		Last Modified: Thu, 16 Mar 2023 01:03:06 GMT  
		Size: 6.5 KB (6462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:750f7ade153ce2c99e6a718d63a82e6ef50c9b80edf08de87406a128725d0ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94794365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d965327ac4600487dce1bd0b2306373fc5b4ec9127b5274a7a4ca06c614dc065`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 23:41:07 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:41:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Wed, 15 Mar 2023 23:41:09 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 15 Mar 2023 23:41:09 GMT
ENV GOSU_VER=1.12
# Wed, 15 Mar 2023 23:41:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 15 Mar 2023 23:42:03 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:06 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 15 Mar 2023 23:42:07 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 15 Mar 2023 23:42:09 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 15 Mar 2023 23:42:09 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 15 Mar 2023 23:42:10 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 15 Mar 2023 23:42:10 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 15 Mar 2023 23:42:10 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 15 Mar 2023 23:42:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Mar 2023 23:42:10 GMT
CMD ["influxd"]
# Wed, 15 Mar 2023 23:42:10 GMT
EXPOSE 8086
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 15 Mar 2023 23:42:10 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 15 Mar 2023 23:42:10 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd6db03d5e7efd9c898c05fa431254e6753c9d39caf9a942d187e791ef698e`  
		Last Modified: Wed, 15 Mar 2023 23:42:58 GMT  
		Size: 6.3 MB (6308600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e77e647b06d59d840fce37c059b20aa366a51af80637fd63e1e5512a9e5e6`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 6.6 MB (6643045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316c8eeb27a0e8e1b5c0adabd0c1c7a915c9dfda919151dea2c1f0fbd9b5b8d`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 4.1 KB (4124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed509fbb0848d068923c7c2fb0326172783db14b7e706111aa8d36fef0724e1`  
		Last Modified: Wed, 15 Mar 2023 23:42:57 GMT  
		Size: 916.9 KB (916930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd9f815af9fa7713836edcaf8c0edfede3b00c2f262af85dee43e3bf5706a89`  
		Last Modified: Wed, 15 Mar 2023 23:43:53 GMT  
		Size: 45.1 MB (45145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e98fd076597f7d2ddfa0871be33a56e936d19752c20858efc5f76b0fe57e03`  
		Last Modified: Wed, 15 Mar 2023 23:43:50 GMT  
		Size: 5.7 MB (5706001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e1b9223729f0d3aebccfacb5a0b15c96af102a78398ac8b0df5cfa5329e7ed`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc31e1ada9713c6aa0ae771c2ff4a99aeaa09bcd46114941d005d37a165d5c8d`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f654e5c408f27396570fc3ebb1bfee8bd77d4e2f82a808aa4ce8cd861ff0af`  
		Last Modified: Wed, 15 Mar 2023 23:43:49 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
