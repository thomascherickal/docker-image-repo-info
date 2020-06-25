## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:eff8ac1f5a7e6729103dfcc46da04d450d64b0145b214ab4b6c7b6158b6a63fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5e26f04be49fde97b89ffbe97802d111bb613022d4157384f8dff1f965353233
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0081104aa8b1b99cca0a885d70e36b87da9f8b46e2680f818f427c3aff3db082`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:50:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:50:30 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:50:31 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea42d87d9aceed297b04cbb66a98d0502d1a4e4d7fbf4a24da0eb5e117aa0b34`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 5.8 MB (5810721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398ee71ef2c48adc42b0180ed8f9f18ec21b79821006b92b9c101969c91ca0cd`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:edc847c0db6be8390fb0d380f79011c2b9a250c2fd8127dc42c7fb46ccfa2162
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc8a653819ac1d586c5211f81be29e3376947f8eb669460a290893d6daa4ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 18:58:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 18:58:58 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 18:58:58 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 18:58:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 18:58:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286fedac0aa1b93bebceb6fbb3de07a7c57160e1fd714403afea49b08e2887ce`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 5.8 MB (5806653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f45eb729be07e4f3dffb7b479060f228cab76029542a382f3d9d661cde0a0c5`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
