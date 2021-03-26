## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:9d1c10a7c73c7bf354e12a1c24620e4020a5f81d3cb06ff73316305558ebf83f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff85e83ddea77c39183aed2eae77d09809eeecbfd51aa8e8ab2cc3ca136a0db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012e69812f1330d74532543e68955276fbb8390f06a1c627873fbfd88ec23f3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:12:03 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 08:12:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 08:12:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 08:12:06 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 08:12:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:12:07 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f43604faee33fd935c231c8add7a2f9f6d33712dc31de6ae1e1fde55fbbcb83`  
		Last Modified: Fri, 26 Mar 2021 08:12:37 GMT  
		Size: 6.0 MB (5962455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173cba00661220a72d7a394a5993bdc17325ab50875040ecc6eb5bc6dc8e65c9`  
		Last Modified: Fri, 26 Mar 2021 08:12:36 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:19373a83f61771319d0aacfab1086d496a2dd1535970f8a20652d56cf2b7578e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935ff18ff1bfcc7d421f422b0d98ef2b111e05c4e09b1e57aef68d71b18156b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:57:34 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 05:57:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 05:57:42 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 05:57:43 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 05:57:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:57:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dde547b7fced1153630086dee787892a218966ea430c2964f55f72bcbbf83a`  
		Last Modified: Fri, 26 Mar 2021 05:58:16 GMT  
		Size: 5.5 MB (5533929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df980303a7fb93b8683964b371b30ef03ef35e26de48621d858290228f8b3346`  
		Last Modified: Fri, 26 Mar 2021 05:58:14 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:f167b7ef1b6e893d3e176ad7fd41597e8a4da3720d0694b407e19e24b68cd5f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e033b7fa5e49122eff8379884102467952cb9d40190588eee42fd608ecbfe3d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:51:55 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 01:52:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 01:52:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 01:52:11 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 01:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 01:52:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ca624cfb490a8a9fb48110381475a59604ddfd4920f6496398a887f8a37b73`  
		Last Modified: Fri, 26 Mar 2021 01:52:52 GMT  
		Size: 5.5 MB (5527163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3957a11b701f02a3361d365cd9b9c63fcafa89f362a40471a527bb31bbbe1de6`  
		Last Modified: Fri, 26 Mar 2021 01:52:50 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:1740e224df015e33133a9db91519ebc8601bf64861cde979a2ed6c556b649395
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8164487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205e781a3be342b949194bab8b6fde3763da1876fe7fac88af8efa1a07b3f204`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:46:28 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 01:46:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 01:46:33 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 01:46:34 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:46:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:46:35 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e334db32136252e9605e0a6ef0426e8c0c50e757bb238a24330339d3dedbe84`  
		Last Modified: Sat, 06 Mar 2021 01:51:34 GMT  
		Size: 5.5 MB (5452492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e903d8d08305b07378aef2e8c19af9f0d6b899ce053c33e5b6022c07b155e2`  
		Last Modified: Sat, 06 Mar 2021 01:51:32 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
