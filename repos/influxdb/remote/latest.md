## `influxdb:latest`

```console
$ docker pull influxdb@sha256:f991db159c58376cadbff1f5d54f59da8f040e29f334ccc2661ab66453fbd469
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:d8630b3f410f847abb2be757f19516fb7838692bde91688bd7b03ec346f2f3f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114862116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d48c9f096b931faaa88dc23e815697b02fca67cdce67bb75c87d7867d31fb494`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 09:11:24 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:11:26 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Thu, 23 Mar 2023 09:11:26 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 23 Mar 2023 09:11:26 GMT
ENV GOSU_VER=1.12
# Thu, 23 Mar 2023 09:11:29 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 05 Apr 2023 21:20:14 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 05 Apr 2023 21:20:20 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 05 Apr 2023 21:20:20 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 05 Apr 2023 21:20:23 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 05 Apr 2023 21:20:24 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 05 Apr 2023 21:20:24 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 05 Apr 2023 21:20:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 05 Apr 2023 21:20:24 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 05 Apr 2023 21:20:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Apr 2023 21:20:24 GMT
CMD ["influxd"]
# Wed, 05 Apr 2023 21:20:24 GMT
EXPOSE 8086
# Wed, 05 Apr 2023 21:20:24 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 05 Apr 2023 21:20:25 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 05 Apr 2023 21:20:25 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 05 Apr 2023 21:20:25 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d55eeb8b14defb8ac4850a09e8ad01f5c4cf5c1e3bc96a4d6ddcb5dd99b2967`  
		Last Modified: Thu, 23 Mar 2023 09:14:07 GMT  
		Size: 6.3 MB (6327646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25ee49adb76883236157ca880b95c0b39a86ffc4928c6cb5d600138d2327b8b`  
		Last Modified: Thu, 23 Mar 2023 09:14:06 GMT  
		Size: 7.0 MB (7049180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444ced87a2669810a478f0be91960e726ec68f41768a5278616dee7e45cdce25`  
		Last Modified: Thu, 23 Mar 2023 09:14:05 GMT  
		Size: 4.1 KB (4108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dd140e260ecbccf7980d8969186acc4a361852da08029550e9b500459cdb27`  
		Last Modified: Thu, 23 Mar 2023 09:14:05 GMT  
		Size: 982.0 KB (982038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b13f8c0f03e488ac345e4c54b392ada7bea33791c8569e7f5304bdf5b88273`  
		Last Modified: Wed, 05 Apr 2023 21:21:15 GMT  
		Size: 46.3 MB (46334691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbbb0b954da21f0ff030c13e4951d252a8801fc7c088b6cc4a5a09c39f37227`  
		Last Modified: Wed, 05 Apr 2023 21:21:12 GMT  
		Size: 22.7 MB (22746049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c1fc7c31d917dc7ffbbfa812cd5b1d2a83a18ecc91fccc6568c6bf4e226e44`  
		Last Modified: Wed, 05 Apr 2023 21:21:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eff0a31ac58f609012736c101726ce68168330589a80b4cbb7dc2db8c4dc207`  
		Last Modified: Wed, 05 Apr 2023 21:21:10 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff71809269295a86462bb7be5f16a94e51520381abe9790af4e1464c1d73306e`  
		Last Modified: Wed, 05 Apr 2023 21:21:10 GMT  
		Size: 6.5 KB (6463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c6406c96db6fa542c09423db7e6152e32733caaa991cebfe2e3aa62c3e92d19c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109728836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4976cf34febb0ff48161da94e8cf38a62ab904e55127318cf2046a45f380833b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 09:10:14 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:10:15 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/yq "https://github.com/mikefarah/yq/releases/download/v4.30.8/yq_linux_${arch}" &&     case ${arch} in       amd64) echo '6c911103e0dcc54e2ba07e767d2d62bcfc77452b39ebaee45b1c46f062f4fd26 /usr/local/bin/yq' ;;       arm64) echo '95092e8b5332890c46689679b5e4360d96873c025ad8bafd961688f28ea434c7 /usr/local/bin/yq' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/yq &&     yq --version
# Thu, 23 Mar 2023 09:10:16 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Thu, 23 Mar 2023 09:10:16 GMT
ENV GOSU_VER=1.12
# Thu, 23 Mar 2023 09:10:18 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 05 Apr 2023 21:40:22 GMT
ENV INFLUXDB_VERSION=2.7.0
# Wed, 05 Apr 2023 21:40:27 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 05 Apr 2023 21:40:27 GMT
ENV INFLUX_CLI_VERSION=2.7.1
# Wed, 05 Apr 2023 21:40:30 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 05 Apr 2023 21:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 05 Apr 2023 21:40:31 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 05 Apr 2023 21:40:31 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 05 Apr 2023 21:40:31 GMT
COPY file:595a669a2c2c2f47df93700fcd3e412750aae40abb979bb4af48a89af97a8b72 in /entrypoint.sh 
# Wed, 05 Apr 2023 21:40:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Apr 2023 21:40:31 GMT
CMD ["influxd"]
# Wed, 05 Apr 2023 21:40:31 GMT
EXPOSE 8086
# Wed, 05 Apr 2023 21:40:31 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 05 Apr 2023 21:40:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 05 Apr 2023 21:40:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 05 Apr 2023 21:40:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40871433b7864a6c0d657efda2cc53b8cf76c232272114d18e5c2396c63ac2b6`  
		Last Modified: Thu, 23 Mar 2023 09:11:26 GMT  
		Size: 6.3 MB (6308577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d3802a08020fc6ebf59c0ccf78c1e9f6f60beb4140a800717ca5f23067a10a`  
		Last Modified: Thu, 23 Mar 2023 09:11:25 GMT  
		Size: 6.6 MB (6643026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd72245adc39892c036094c00d370bbeb5f97382ca50ea59f0f9fb34d40b576`  
		Last Modified: Thu, 23 Mar 2023 09:11:24 GMT  
		Size: 4.1 KB (4120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745a7db30e3c11be3091abb0811f7b9428c1af6f2506a38017c133262db389f4`  
		Last Modified: Thu, 23 Mar 2023 09:11:24 GMT  
		Size: 916.9 KB (916930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c667bc50792e66907430393f8acb0123f48894c5ed84e8747da72191dca630`  
		Last Modified: Wed, 05 Apr 2023 21:40:59 GMT  
		Size: 44.4 MB (44435726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddf9f5ed8c708714549d5d2aa74ca887aca00944ef70042b68392b65daf4e88`  
		Last Modified: Wed, 05 Apr 2023 21:40:57 GMT  
		Size: 21.4 MB (21350759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c49b72735919470893e424b8616b53597d18f870c5b7677b0535ec51ee24f`  
		Last Modified: Wed, 05 Apr 2023 21:40:55 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e544db534725d5eeab9a2a8ffc497abee06f26eb98ffbc3d5cdd42921566c856`  
		Last Modified: Wed, 05 Apr 2023 21:40:55 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5d545a85cb4bd35b4212dca560c8729138de93377979029e8bca5f22e0cd3`  
		Last Modified: Wed, 05 Apr 2023 21:40:55 GMT  
		Size: 6.5 KB (6464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
