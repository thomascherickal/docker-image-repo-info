## `nats-streaming:alpine3.13`

```console
$ docker pull nats-streaming@sha256:17ee27f3d8f547400a952dcb9ddc3fade80fb324a17fd7e674fdf893cb8a21f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f6662c1e1e718f3d9fcb6bdb60e804f2713ab87d3d79e87867aad686c1bf26f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8772720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040b7462b8eea20a68c23764a3d2155ba5c5c77fee37f82ac9bd0a08fd88004a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 00:25:25 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 00:25:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 00:25:28 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 00:25:29 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:25:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 00:25:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1fe86c18b7461fe173b47d88cd5c5dacf60a7445982cc8df67073d31ce5d59`  
		Last Modified: Tue, 02 Mar 2021 00:26:12 GMT  
		Size: 6.0 MB (5960641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2eda78ff92213f3dfa2cf8f7843e06a7cd05c95b0b51247ca95152fd3ef6c8`  
		Last Modified: Tue, 02 Mar 2021 00:26:11 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7c20fa0d0dbabb6bae2cd97d317f128827a248bc562d6d9c4834c790bf4a7021
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8154253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe07a490b2b30897bbc5fa50238530420e06b6f3e56a1bd8cbe98ac24212b3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 00:26:32 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 00:26:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 00:26:37 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 00:26:38 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 00:26:39 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13c49183b721e7bfb4ccc166dd54d945cc1db5205af3d2ac4d23532e68688d4`  
		Last Modified: Tue, 02 Mar 2021 00:27:19 GMT  
		Size: 5.5 MB (5531793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d856ec09a697525b968975b09d200f2f6f7816f402c6883ff0ec86b6e925fa`  
		Last Modified: Tue, 02 Mar 2021 00:27:13 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:782e4290f2c50dd5e8a0714f8cfa35d8575577910ff3252c757d3a64e6bd4d47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88cdb45d1d7d80ee678f8f1ca18f6c67822632552ea1ceb8a6a91ecc72503f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 00:59:37 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 00:59:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 00:59:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 00:59:43 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 00:59:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 00:59:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b550ac0781e9d06a2d5602aa128b8085d9808f31821df0db0fdb3378e4beb64`  
		Last Modified: Sat, 06 Mar 2021 01:00:55 GMT  
		Size: 5.5 MB (5527196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9fcc13222a0356f1399ed180350034d92d18fa5262cd34421cb52915ca14df`  
		Last Modified: Sat, 06 Mar 2021 01:00:53 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:10777a97b0533815b574cb3e18f05a66ac7b41009f455c2ebcb1539d007307f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8162049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d442b80f45600e050156b1173265cf35372b99dffd0fb8bfdad973fd77b339`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 01:13:01 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 01:13:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 01:13:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 01:13:06 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 01:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 01:13:08 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c50e699e530e5249c2caf763d7dc8d6e6b7cc9c789aa8ed85de12bee5223a2`  
		Last Modified: Tue, 02 Mar 2021 01:15:04 GMT  
		Size: 5.5 MB (5450055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ae0645459f8848b2db6912d3c7cb864e3ed29d733b3476e1f4416849d3f383`  
		Last Modified: Tue, 02 Mar 2021 01:15:01 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
