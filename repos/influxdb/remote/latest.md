## `influxdb:latest`

```console
$ docker pull influxdb@sha256:5973b7698a7a8fddf60eca9c44077b062abb133aecfb193ec279ba2eeff253cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:f02325b07c1105549c1e3099343f8cf8724497995b4795c5a1e0ddf5bd76fccf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.2 MB (162170896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165ce29e04361e963410915a225e528ec623101f733ba6196c7148947c9f4ecf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:49 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
# Wed, 01 Nov 2023 00:20:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:02 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:36:04 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 01 Nov 2023 02:36:05 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 01 Nov 2023 02:36:05 GMT
ENV GOSU_VER=1.12
# Wed, 01 Nov 2023 02:36:07 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 01 Nov 2023 02:36:07 GMT
ENV INFLUXDB_VERSION=2.7.3
# Wed, 01 Nov 2023 02:36:12 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 01 Nov 2023 02:36:12 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 01 Nov 2023 02:36:14 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 01 Nov 2023 02:36:15 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 01 Nov 2023 02:36:15 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 01 Nov 2023 02:36:15 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 01 Nov 2023 02:36:15 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Wed, 01 Nov 2023 02:36:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 02:36:15 GMT
CMD ["influxd"]
# Wed, 01 Nov 2023 02:36:15 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 02:36:15 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 01 Nov 2023 02:36:16 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 01 Nov 2023 02:36:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 01 Nov 2023 02:36:16 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbcf0a0fd4f60b8f415999c5c7c9d499b5e065fc620ececfb9a9c50d925559b`  
		Last Modified: Wed, 01 Nov 2023 02:38:29 GMT  
		Size: 9.8 MB (9787149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc30a15212abb09190c168b0bfc858f7682098ef77f765b1b19158189864dfe3`  
		Last Modified: Wed, 01 Nov 2023 02:38:26 GMT  
		Size: 6.4 MB (6434099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159c705faba476f2d587c2b39871193bed7bbacd328eee135c265a65f3dc83f9`  
		Last Modified: Wed, 01 Nov 2023 02:38:25 GMT  
		Size: 3.3 KB (3281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d00aeef48a00456bd46e972f3c131543fd90b1d48c6fb6ff6934725e515d87`  
		Last Modified: Wed, 01 Nov 2023 02:38:25 GMT  
		Size: 986.0 KB (985995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c836d6efdfbcc4e1b254e82930240d4d4a638a95888229331e5322b9e778470`  
		Last Modified: Wed, 01 Nov 2023 02:38:33 GMT  
		Size: 92.7 MB (92675041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:979326e5d1b2d6f77813a9660d6d7f9d944a4787ed617053396d81a447bafc54`  
		Last Modified: Wed, 01 Nov 2023 02:38:26 GMT  
		Size: 23.1 MB (23128348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5797dc5b6cab1afb3734b6a1696fc3623e38f371fbace58f775402723df55c`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10179fcb509a5aeaf267fb8c50ce26d13a4da438fbfa3171be4b60ec97e92f09`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eff5c0be8ad19f7a47f14b95ce6e892461edf952e3932a02684e53e9c3f234d`  
		Last Modified: Wed, 01 Nov 2023 02:38:23 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:9a9d2ad170926a8880b35ade12fc7d226e688dda525331bd0a6f4117d807aaad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156471359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4209d6dee09892d6c679bc2479aaa59b63ff870a32188a3dd612ddd804967d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:41 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 01 Nov 2023 00:39:41 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 03:02:01 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:02:02 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Wed, 01 Nov 2023 03:02:03 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Wed, 01 Nov 2023 03:02:03 GMT
ENV GOSU_VER=1.12
# Wed, 01 Nov 2023 03:02:05 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 01 Nov 2023 03:02:05 GMT
ENV INFLUXDB_VERSION=2.7.3
# Wed, 01 Nov 2023 03:02:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 01 Nov 2023 03:02:13 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Wed, 01 Nov 2023 03:02:15 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 01 Nov 2023 03:02:15 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 01 Nov 2023 03:02:15 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 01 Nov 2023 03:02:15 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 01 Nov 2023 03:02:15 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Wed, 01 Nov 2023 03:02:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 03:02:15 GMT
CMD ["influxd"]
# Wed, 01 Nov 2023 03:02:16 GMT
EXPOSE 8086
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 01 Nov 2023 03:02:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 01 Nov 2023 03:02:16 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262116acfec49dc20776eccd49619b880cec1fd47986b2f8309782cf13481e5d`  
		Last Modified: Wed, 01 Nov 2023 03:02:48 GMT  
		Size: 9.6 MB (9584486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d34c8bbe1ae9229eeb59ba5f8b19d8a31f7c63b8591315702334252f91b36`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 6.0 MB (5953766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e6bb63ae8bd4bca01c0bee81dec19e9bf0a7277d486d01551cd837ef2d4448`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 3.3 KB (3280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e1f23b16702da739edd9c930032d32ad1377ebc0f9ae7310ecf969942ed819`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 921.5 KB (921473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf396801ae61bebd6da034895d279d77471f5fba07e6ac918fd449def2ee46d`  
		Last Modified: Wed, 01 Nov 2023 03:02:50 GMT  
		Size: 89.2 MB (89159505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52a03c7703182a6c2dd7d8ae6c1c224bc82eebb3e930c0741c71f693d042733`  
		Last Modified: Wed, 01 Nov 2023 03:02:45 GMT  
		Size: 21.7 MB (21662585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f072621e375faeb99e7f90b93f1bc33f921b5d92f0172580fba05b9e898ba5c2`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55de467c42ebc43636d37579756439b6fb6b7b6ef5f0c1d7021ee61c153898d7`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1efdf6846864ed36faf9ec3e47d4c9bf8a885651259e99a517f373e01b071c`  
		Last Modified: Wed, 01 Nov 2023 03:02:43 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
