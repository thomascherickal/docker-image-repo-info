## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:44a366dd7724453547c612a9fef7a00f9dcfbfafa30e6a1fe164f640d492051c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:87b888ae6fd20ba37c52e820792d062565455fd22f1e06c92db70799f0f8f6b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68813553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f293d68a70a77a309865be452fc9105c40052a028062346b3c73286a5e49e25c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 21:59:54 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Wed, 29 Mar 2023 21:59:54 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 29 Mar 2023 22:00:23 GMT
ENV INFLUXDB_VERSION=2.6.1
# Wed, 29 Mar 2023 22:00:27 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Wed, 29 Mar 2023 22:00:27 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Wed, 29 Mar 2023 22:00:29 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Wed, 29 Mar 2023 22:00:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 29 Mar 2023 22:00:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 29 Mar 2023 22:00:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 29 Mar 2023 22:00:29 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Wed, 29 Mar 2023 22:00:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:00:29 GMT
CMD ["influxd"]
# Wed, 29 Mar 2023 22:00:30 GMT
EXPOSE 8086
# Wed, 29 Mar 2023 22:00:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 29 Mar 2023 22:00:30 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 29 Mar 2023 22:00:30 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 29 Mar 2023 22:00:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1afb36336fe98dd703c1041000d89b9bae5d279480c46f77620057018d3e2b2`  
		Last Modified: Wed, 29 Mar 2023 22:02:42 GMT  
		Size: 12.4 MB (12374741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b2ee057b405e8d7b36616d40cb252eca7fb22085cad6642982f54ab0ca2baa`  
		Last Modified: Wed, 29 Mar 2023 22:02:40 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4e244e44c220124d50f4b21f2c127272a1eb13cb3dd1490e1f3e62e888ac51`  
		Last Modified: Wed, 29 Mar 2023 22:03:15 GMT  
		Size: 46.8 MB (46844109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b977b87996ce033faf2c8183c2a398750b2b340a4ca825945b9f618f5e62d206`  
		Last Modified: Wed, 29 Mar 2023 22:03:11 GMT  
		Size: 6.2 MB (6211617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e2093bd79c7edc07287626340a770f377039d0c28f65782d0aed46ed62ef7c`  
		Last Modified: Wed, 29 Mar 2023 22:03:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1dec79611f531d445ddb24ef322318ba9d758c57d9e10396d752658c52f747`  
		Last Modified: Wed, 29 Mar 2023 22:03:10 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3f9ce0715ec46219cae98741924a2e9ef4fbd5cd670d313dbec0c417400d39`  
		Last Modified: Wed, 29 Mar 2023 22:03:10 GMT  
		Size: 6.4 KB (6440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ee4ee039c462fa847783f32633966c0fe6947248eca56b7c35b742e865596472
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66150114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:193c86b0009ec4e7f7f54f88d5213d7dfb37b7f2e260c23c93636bdbffb0c7da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 04:17:15 GMT
RUN apk add --no-cache       bash       ca-certificates       curl       gnupg       run-parts       su-exec       tzdata       yq &&     update-ca-certificates
# Thu, 30 Mar 2023 04:17:16 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 30 Mar 2023 04:17:42 GMT
ENV INFLUXDB_VERSION=2.6.1
# Thu, 30 Mar 2023 04:17:46 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&    curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2_linux_${arch}/influxd" /usr/local/bin/influxd &&     rm -rf "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz"            "influxdb2-${INFLUXDB_VERSION}-linux-${arch}.tar.gz.asc"            "influxdb2_linux_${arch}" &&     influxd version
# Thu, 30 Mar 2023 04:17:46 GMT
ENV INFLUX_CLI_VERSION=2.6.1
# Thu, 30 Mar 2023 04:17:48 GMT
RUN case "$(apk --print-arch)" in       x86_64)  arch=amd64 ;;       aarch64) arch=arm64 ;;       *) echo 'Unsupported architecture' && exit 1 ;;     esac &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys       9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     curl -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"          -fLO "https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     gpg --batch --verify "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc"                          "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     tar xzf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz" &&     cp "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}/influx" /usr/local/bin/influx &&     rm -rf "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz"            "influxdb2-client-${INFLUX_CLI_VERSION}-linux-${arch}.tar.gz.asc" &&     influx version
# Thu, 30 Mar 2023 04:17:48 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 30 Mar 2023 04:17:48 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 30 Mar 2023 04:17:48 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 30 Mar 2023 04:17:48 GMT
COPY file:708cccb15c29f10eb0c29e47f1c676d76b8ea9be434cce106ef95a7ba844bb2c in /entrypoint.sh 
# Thu, 30 Mar 2023 04:17:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 04:17:49 GMT
CMD ["influxd"]
# Thu, 30 Mar 2023 04:17:49 GMT
EXPOSE 8086
# Thu, 30 Mar 2023 04:17:49 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 30 Mar 2023 04:17:49 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 30 Mar 2023 04:17:49 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 30 Mar 2023 04:17:49 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed363db396bd455184362560a01cd691a111fe2dea827312e4f70ec9d621fee`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b6f835aacf2662a2b94c43a8ea49fa6bb22e7462d8ac83f92e9fcb65b3adf4`  
		Last Modified: Thu, 30 Mar 2023 04:18:06 GMT  
		Size: 12.0 MB (12027921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16b3409528a44a440ba66163e99ee9e4c43bc43aa2a65788460f2007c77cc47`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8069e6f5b40dc3a481f27e6b9cd9683635ad4706e6cf40e8bb7f91f1ec0c0c6`  
		Last Modified: Thu, 30 Mar 2023 04:18:33 GMT  
		Size: 45.1 MB (45145855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e33d27d7ae6e2689df7f613565e3f228fb3f31e857c12ab7ce5d99043ec28e`  
		Last Modified: Thu, 30 Mar 2023 04:18:30 GMT  
		Size: 5.7 MB (5705962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59d6829fb6ef1e27307189d7b43692e46ece823a98e909ce715dbf75925c80f`  
		Last Modified: Thu, 30 Mar 2023 04:18:29 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8520cd6bff44fdf9b485bea4d6ddde01727bd01eff2c77cdaafd5055ede6a4f0`  
		Last Modified: Thu, 30 Mar 2023 04:18:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1025a916b3c0633180eceb173ac7b89a1e6e618ffc81884bccb7be67ed2e1715`  
		Last Modified: Thu, 30 Mar 2023 04:18:29 GMT  
		Size: 6.4 KB (6441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
