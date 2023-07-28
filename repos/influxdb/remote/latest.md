## `influxdb:latest`

```console
$ docker pull influxdb@sha256:d7ebb72e456bb865aeb56a036c0568e5101d63192f862fd1aa4e9c2fe6147d03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:1838836254a474d10f8400e15c562ca5f832c1073270a7cf79fd7454d9ebc014
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114639473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b36d12738189d8020349ee0843af1bb7dc878bb79a45bdfb8abbb8c789fd6ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:53:00 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:53:01 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Jul 2023 03:53:02 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Fri, 28 Jul 2023 03:53:02 GMT
ENV GOSU_VER=1.12
# Fri, 28 Jul 2023 03:53:05 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Fri, 28 Jul 2023 03:53:05 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Jul 2023 03:53:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Jul 2023 03:53:08 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Jul 2023 03:53:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Jul 2023 03:53:11 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Jul 2023 03:53:11 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Jul 2023 03:53:11 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Jul 2023 03:53:11 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:53:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:53:12 GMT
CMD ["influxd"]
# Fri, 28 Jul 2023 03:53:12 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Jul 2023 03:53:12 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Jul 2023 03:53:12 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c856600570b3e8899338e040b207edb1edf918e2f432d172e7c2d7c7711cf54`  
		Last Modified: Fri, 28 Jul 2023 03:55:28 GMT  
		Size: 6.3 MB (6327879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcecbec27943f040bac0f4c870b267decadf6cf5ef35377709951978b5ad07e`  
		Last Modified: Fri, 28 Jul 2023 03:55:26 GMT  
		Size: 6.4 MB (6434101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f2e28ccd0d15763d6e5cc9aa775a980c328a5c4169da74ac67e5be373618ce`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d716e4775561a7cbcd4ff11201c60ffcfcf71f9d9449f17b1dd7edb9561240`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 986.0 KB (986004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbcd38ba0cde636731c1e6fb50c227e90d58b771250494e0d51e7d112dabfca6`  
		Last Modified: Fri, 28 Jul 2023 03:55:28 GMT  
		Size: 46.3 MB (46334285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d59db4f14987c78976a827eefb8fff5b9e041b2f8a949158a34cb59324340bd`  
		Last Modified: Fri, 28 Jul 2023 03:55:25 GMT  
		Size: 23.1 MB (23128349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f7ca5eb043f964a733d65e3663217a8dd57e05c38db1dc144e832907d3a393`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45e929d4c8d8366919fa009f30a42250c0ad7296c2e2618236863d7c4058ee5`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249e42eb63e85ab22dfd19ff8e32bd8f851e947eb87a90896cdf87419b81a703`  
		Last Modified: Fri, 28 Jul 2023 03:55:23 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a7ce35b71b89218687209d08387415c6fd46fcab2cf2e88d3565bb743b15f0d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.4 MB (109356501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaf3349d3cdff14ca2ddda721d19071ec4ca1b24c46320cc922c3f37647ee62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:39:00 GMT
RUN export DEBIAN_FRONTEND=noninteractive &&     apt-get update -y &&     apt-get install -y --no-install-recommends       ca-certificates       curl       gnupg &&     apt-get clean &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:39:01 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fLo /usr/local/bin/dasel "https://github.com/TomWright/dasel/releases/download/v2.1.2/dasel_linux_${arch}" &&     case ${arch} in       amd64) echo 'e4b43d8c7d76904e2401dc81de0900d9cb69b006794ff3901ec5d50e96baa8ef  /usr/local/bin/dasel' ;;       arm64) echo '92b83f30949679197403ff7a7e0f9ef3e458c1c55031d9c1bc112364e487d57d  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Fri, 28 Jul 2023 03:39:02 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --create-home --home-dir=/home/influxdb --shell=/bin/bash influxdb
# Fri, 28 Jul 2023 03:39:02 GMT
ENV GOSU_VER=1.12
# Fri, 28 Jul 2023 03:39:04 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     curl -fLo /usr/local/bin/gosu     "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}"          -fLo /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-${arch}.asc" &&     gpg --batch --verify /usr/local/bin/gosu.asc                          /usr/local/bin/gosu &&     rm -rf /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Fri, 28 Jul 2023 03:39:04 GMT
ENV INFLUXDB_VERSION=2.7.1
# Fri, 28 Jul 2023 03:39:08 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Fri, 28 Jul 2023 03:39:08 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Fri, 28 Jul 2023 03:39:11 GMT
RUN case "$(dpkg --print-architecture)" in       *amd64) arch=amd64 ;;       *arm64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Fri, 28 Jul 2023 03:39:11 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 28 Jul 2023 03:39:11 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 28 Jul 2023 03:39:11 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 28 Jul 2023 03:39:11 GMT
COPY file:3ef80d0bcfdeda3282c98ad7a6b84218cd7593d6a3bbf027c3083db3b7acad32 in /entrypoint.sh 
# Fri, 28 Jul 2023 03:39:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 03:39:12 GMT
CMD ["influxd"]
# Fri, 28 Jul 2023 03:39:12 GMT
EXPOSE 8086
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 28 Jul 2023 03:39:12 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 28 Jul 2023 03:39:12 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac205f561e969edd084e6d4d75c4df5abee0eb6c7118268b7aa992fa9f77ea55`  
		Last Modified: Fri, 28 Jul 2023 03:39:43 GMT  
		Size: 6.3 MB (6308722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b5dc0299ed71c049212b9e0bcffec4e1e356fdb96f1271d2c942761106a512`  
		Last Modified: Fri, 28 Jul 2023 03:39:41 GMT  
		Size: 6.0 MB (5953767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0add7db58fdd1110f5835913a59f75f54a51838dcc82e57abe402a4008f1bbfb`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 4.1 KB (4119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ecad330e1544d9821b3b317eac5f9c6e1a3c3d4ea2c13a6c4168566a590bdf`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 921.5 KB (921481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef78635da685d858c3c6e47eafaa8b38f930d66a6268ed4ac2b0cdfca4f6370f`  
		Last Modified: Fri, 28 Jul 2023 03:39:42 GMT  
		Size: 44.4 MB (44435850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e517c72b8b39e3045970fe57e8b1c2156856199598109fd8bbe70cd5fa09b71`  
		Last Modified: Fri, 28 Jul 2023 03:39:40 GMT  
		Size: 21.7 MB (21662584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb59ddc55e6888e46120c967f51de5dcb7e3aaf990180cce7ca6aa8473c7091a`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7a6621084b5af4a1eb1151d31c94d38d395376114f8659027af2a24dede674`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc1473a02bf03ce6f291ffa11958d92504b2a0be69b89e96bb15a107fb8dd07`  
		Last Modified: Fri, 28 Jul 2023 03:39:38 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
