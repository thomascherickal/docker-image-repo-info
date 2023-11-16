## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:8344faf145ca0d2b938574b77847bcbdfd13df4774147cb9cedbb9f5910f9eba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ba08c9a5aed86654ce80f9e27fcb5e9a1b470f031bca320e7a7852ac6d8345f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.6 MB (87558514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e6885ff789a2b352d3025a6f80b199f107f56a65bb83bc64dd511b2f79ad381`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 01:30:37 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 01:31:11 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Thu, 16 Nov 2023 01:34:39 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 16 Nov 2023 01:34:39 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Nov 2023 01:34:39 GMT
ENV INFLUXDB_VERSION=2.7.4
# Thu, 16 Nov 2023 01:34:43 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 16 Nov 2023 01:34:43 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 16 Nov 2023 01:34:45 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Nov 2023 01:34:46 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Nov 2023 01:34:46 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Nov 2023 01:34:46 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Nov 2023 01:34:46 GMT
COPY file:6341d1dd8e0763e797b79985007acd07a4686ed831d55018f6e390823bad9d07 in /entrypoint.sh 
# Thu, 16 Nov 2023 01:34:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Nov 2023 01:34:46 GMT
CMD ["influxd"]
# Thu, 16 Nov 2023 01:34:46 GMT
EXPOSE 8086
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Nov 2023 01:34:47 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Nov 2023 01:34:47 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5352bf3aec614dde8ac36d38f28f5021eff4c2ff0226eb22dfa667f2b2add1`  
		Last Modified: Tue, 17 Oct 2023 01:33:20 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1571fe6e896787a9ed8a94a131ff6ea2380ac23074890f6eca0b0508ce78e4b3`  
		Last Modified: Tue, 17 Oct 2023 01:34:04 GMT  
		Size: 8.9 MB (8868212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcc69539951a864422f2d214e44ee6fc6d9c57c0a4edaefde6efc460ff2d90f`  
		Last Modified: Thu, 16 Nov 2023 01:35:47 GMT  
		Size: 5.8 MB (5820946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8bf8a03db3cd399c817901c93c81f234d4088e8ee6666a44c151359c18e67`  
		Last Modified: Thu, 16 Nov 2023 01:35:46 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f16af9f58f64f3fdd9b70d190a136a6b4a5d1192e277314a5d985beee82ce`  
		Last Modified: Thu, 16 Nov 2023 01:35:50 GMT  
		Size: 46.3 MB (46330663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dece05f716fd0148569f71292f440015201cb062bfc7680182e1ce7fc48373`  
		Last Modified: Thu, 16 Nov 2023 01:35:47 GMT  
		Size: 23.1 MB (23128356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4edff2dff21ee3c7321ec441eefc00e97710ee5ce673bd7e9a0bb586e451395`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5be165bc94e79bc9ed0eb2a05cbb0d303f08b60e263bf48b3280e4ca44443ae`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598b9a7d76be7074485ba1aa2c15542be5f810d6cec44b0484f7ebaca3c803a8`  
		Last Modified: Thu, 16 Nov 2023 01:35:44 GMT  
		Size: 6.3 KB (6281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a42cd43a35de01ffcda2ddc8660e6f29f1f22c5928e8d288765cd8ebaf065b37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.0 MB (84006245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af78fd2382c4ce48b45f435206d8b7d093ff91de8e1ea63c11c06929e9a9b00`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Tue, 17 Oct 2023 00:43:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 17 Oct 2023 00:43:53 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata &&     update-ca-certificates
# Thu, 16 Nov 2023 01:47:26 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     curl -fL "https://github.com/TomWright/dasel/releases/download/v2.4.1/dasel_linux_${arch}.gz" | gzip -d > /usr/local/bin/dasel &&     case ${arch} in       amd64) echo '8e9fb0aa24e35774fab792005f05f9df141c22ec0a7436c7329a932582a10200  /usr/local/bin/dasel' ;;       arm64) echo '535f0f4c6362aa4b773664f7cfdb52d86f2723eac52a1aca6dfc6a69e2341c17  /usr/local/bin/dasel' ;;     esac | sha256sum -c - &&     chmod +x /usr/local/bin/dasel &&     dasel --version
# Thu, 16 Nov 2023 01:47:27 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Nov 2023 01:47:27 GMT
ENV INFLUXDB_VERSION=2.7.4
# Thu, 16 Nov 2023 01:47:30 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz" &&     cp "influxdb2-${INFLUXDB_VERSION}/usr/bin/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}_linux_${arch}.tar.gz.asc"            "influxdb2-${INFLUXDB_VERSION}" &&     influxd version
# Thu, 16 Nov 2023 01:47:30 GMT
ENV INFLUX_CLI_VERSION=2.7.3
# Thu, 16 Nov 2023 01:47:32 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp influx /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 16 Nov 2023 01:47:33 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Nov 2023 01:47:33 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Nov 2023 01:47:33 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Nov 2023 01:47:33 GMT
COPY file:6341d1dd8e0763e797b79985007acd07a4686ed831d55018f6e390823bad9d07 in /entrypoint.sh 
# Thu, 16 Nov 2023 01:47:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Nov 2023 01:47:33 GMT
CMD ["influxd"]
# Thu, 16 Nov 2023 01:47:33 GMT
EXPOSE 8086
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Nov 2023 01:47:33 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Nov 2023 01:47:34 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e248ba14d9e254569a72ce1316c31cb26327474bc388ccd8fbd2fa78078db3aa`  
		Last Modified: Tue, 17 Oct 2023 00:44:22 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc059a59f82bcb99dccb07e78bca560aa59ed7395b4e1aca88e17625928caac3`  
		Last Modified: Tue, 17 Oct 2023 00:44:22 GMT  
		Size: 9.0 MB (8962246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f430534be970bcb57121ee1018f70360775d0bcf788ebdfa18a2b01c395e00a3`  
		Last Modified: Thu, 16 Nov 2023 01:48:08 GMT  
		Size: 5.5 MB (5463814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f302449250fc8480c8e59e4d8a9ff2cbb6abd3b805653cedc341b214bf20f0d2`  
		Last Modified: Thu, 16 Nov 2023 01:48:07 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156308fdb6aae0ed74aaea1ad996cb6711847dd546ba9a0fbb5d5fae588a788`  
		Last Modified: Thu, 16 Nov 2023 01:48:09 GMT  
		Size: 44.6 MB (44577399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b761820425e0d7dcd3a64ed40d5ecad5e65ea25f3ff316c5b5b22b70f4c064ed`  
		Last Modified: Thu, 16 Nov 2023 01:48:07 GMT  
		Size: 21.7 MB (21662586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c0e72f2f4415fe3b12828eea02e2d97fae456d91d1eddc77605207468f68ba`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fe7982d92d0b7304a9b203c4ae4d3c0740510e88bad5bdfc374cc099035858`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a66d9f557b60a3b1f2a1b5de2d9614dacbd3e5ae74579600877aafa1f42aad9`  
		Last Modified: Thu, 16 Nov 2023 01:48:05 GMT  
		Size: 6.3 KB (6282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
