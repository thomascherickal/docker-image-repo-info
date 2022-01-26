## `nats:alpine3.15`

```console
$ docker pull nats@sha256:dfe1a05929337ec7ed34a219272b33e2b6e4714026bda4d3f65ec76268c1d31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:26978eb91b6f1aa3e255e1ed6c93cd09b25fd6ba284e8a9cd74bae36a3662ea3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf084274d588debf1c2d46247d20cb4f80d354aacb7604005572da5725c2a3fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:19:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:19:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:19:59 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:20:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fb380648df7ec4ba92f1d4d6ffdf641d6819466cce6509f667d94dad9f4c69`  
		Last Modified: Wed, 26 Jan 2022 01:20:55 GMT  
		Size: 4.8 MB (4752823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af65214d163d00ee68245e5e22e1265fec2c0c7f8e0ff23a89f90f9e4689a0`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c8e4a874ee3840ec1c17b0f4143368c54e8fd6a755ffd09e1cdb8290815db`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:b6a9f4ca613ad4869cb2048285f4bc14df63f5fda1926e40372cdb6958971766
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7050090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c9f21447079232e09b46ce60dc7bfc566b5cae47fe9d4100b4eabc6de14936b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:49:39 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:49:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:49:44 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:49:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:49:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2920b3e5877b294e547d8a1c4e3bd607d6d83ad295477663360ca72b6e5405`  
		Last Modified: Wed, 26 Jan 2022 00:51:54 GMT  
		Size: 4.4 MB (4417672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fda4f318c0b4553cdc860867481a33a7dc2d3f2000375a6d2ee053a7f0bd6c`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8d7862ab8d965976774963f71fd952ad4c0d3a294fbd0034121f156e12327d`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:219dd303cee8ae337143fe43e817e9ce1450302f257c28549de920aba7dcf73a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6845712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84db81365408c4dd9fc830a014f69e97973210f093c604deedf93de41f67a0b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:57:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:58:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:58:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:58:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:58:01 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:58:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6564f7bd948d1e195bd1386ecec2e370d1b2519e03c2063cc8789eb90c7ac1`  
		Last Modified: Wed, 26 Jan 2022 01:00:12 GMT  
		Size: 4.4 MB (4409947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30ca090f2ff1db96c07f94e0c463753271d0ef0e5b04768f02b4e5f737ec337`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74fc96dcbe074fbbffd72d2f6aecde13fbb3d4f5dbd99f56f69399990f575f`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:daa50ac3732d7450e429c84a408abcc2940731eff3a98eac7d02fe8436fffe56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7114110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422afb577fe2f6b912aa5793d6553b65bb59ae601e1fb3907b86db1dd09bc725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:55:21 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:55:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:55:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:55:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:55:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:55:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445060b32655cb4edfe06eac59815dabef07ff7dc77d6a7463d35b9b088aa395`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 4.4 MB (4397704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b12cd52fb778db44d89c0599ce5808fa58b7f70290c54a57a59c61eed5b92`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1dc49cd213767a62d094faba237957b6f75ab6f11a040305af507228108cc7`  
		Last Modified: Wed, 26 Jan 2022 01:56:27 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
