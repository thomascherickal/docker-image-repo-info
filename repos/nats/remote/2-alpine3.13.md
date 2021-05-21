## `nats:2-alpine3.13`

```console
$ docker pull nats@sha256:6cf3cec87b97bc4869de88dda543bd1c400ccb9521c7aef36d33a99d515c0ce1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:05f0c41f3164ca644d2bb64afe5b19e6a1850b9cf533746cf91bd9aba605f6e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7343161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bcc5fe6b13327458c8febb3c390c500da37308da3903843de364de6a2ce554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 21 May 2021 01:20:29 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:20:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='12f06d3ac1af3872c8b77722e19faa508b979806641a6dc2707f641de270aa49' ;; 		armhf) natsArch='arm6'; sha256='a61769ab4f4176c882a69209bbff54e0e7e8bd6e986ba8841d5a061a4f8cc72f' ;; 		armv7) natsArch='arm7'; sha256='307b3a42492a0a0172df5d00dea3355064daf5cf38653a1835fab39ca0393415' ;; 		x86_64) natsArch='amd64'; sha256='e4f57f263c7411f6028e9cd6080c6fd35090de4168c21c3e8b7a5ee5a632d142' ;; 		x86) natsArch='386'; sha256='fd3025f88aca3e89d1015d5d3aedfd9390146b168703e2777616261bcc752e2c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 21 May 2021 01:20:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 21 May 2021 01:20:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 21 May 2021 01:20:32 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 May 2021 01:20:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ca912af8a523a4d5305fc703d6103e03f3994bccd440e31ede887688be714`  
		Last Modified: Fri, 21 May 2021 01:21:23 GMT  
		Size: 4.5 MB (4530220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108976c3e63e0003f5e4d5ed04bf985f6ac7f46826a9f2099ceb572d9e88cb0`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f907db8c0f6fef0f88ecb1319563866ac55ba7dc88a4d4b94a624ccb9896efe6`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:1c73109d6f0f4df4a01946b56cb9ee820e00ccab3a53a313fa455132eb429c5a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6817138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610510cf73d587ce2492ee376849f1ad1c1aa9c4302164b35201671f17e814f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:51:13 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:51:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:51:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:51:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:51:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:51:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:51:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f71d1e179b53574a4255bcfcd71fe370c624cd262a2ab7aaffd8e5d31720a`  
		Last Modified: Thu, 13 May 2021 17:55:46 GMT  
		Size: 4.2 MB (4194035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e8d47bbf0baab0970aae54c06f1e44815789587f8278d70e26399b9c5b6a52`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36205a7a8707754144c7268ec085628e59b88815290a05666849b317dc5cf11b`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:b3c5544c5b1d2029e036dc2d81c5ef9a9eac93c249716e18f44edef627978f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6614265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f522cda51f5777e741129fc6a3a6e6c829fd2ae89a356be63fa4d268fd59419d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:59:46 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:59:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:59:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:59:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:59:54 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:59:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:59:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7360a77507600c48adcac31f54a9378253c081d72935f0eae5e523bfd31b34`  
		Last Modified: Thu, 13 May 2021 18:07:02 GMT  
		Size: 4.2 MB (4189145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f603eb8e24e2c3c865dca1242b14eb6277a939d61d513679c8efc3d80a7a5373`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5013eb5a0ee908a4d4462e87197f966195cd787b7d3afe9392b7d36a3a2de10`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5d118edac8396ee73f73a2db080f4d870c52a48d1b7dfe932a8e3ec399e10ce5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6878882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7d4fedb21f182edb7ca233e3ca03ce7ce1ffc9da57a002a1c6fc3d470b9ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:39:53 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:39:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:39:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:40:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:40:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a5de4d48d58b6e52e98523137e1c70f8edaa9edaba04eef99d76177962a7f`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 4.2 MB (4165884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8bc18d6dca6719f9820cf0786282a7083a2b6ba41f6004e3a6b4e9aef5db72`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f454ed6fd75994bba5f04bf38710b744a0804d5bec911593148cd24993d73d86`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
