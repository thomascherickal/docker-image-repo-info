<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.24`](#nats-streaming024)
-	[`nats-streaming:0.24-alpine`](#nats-streaming024-alpine)
-	[`nats-streaming:0.24-alpine3.15`](#nats-streaming024-alpine315)
-	[`nats-streaming:0.24-linux`](#nats-streaming024-linux)
-	[`nats-streaming:0.24-nanoserver`](#nats-streaming024-nanoserver)
-	[`nats-streaming:0.24-nanoserver-1809`](#nats-streaming024-nanoserver-1809)
-	[`nats-streaming:0.24-scratch`](#nats-streaming024-scratch)
-	[`nats-streaming:0.24-windowsservercore`](#nats-streaming024-windowsservercore)
-	[`nats-streaming:0.24-windowsservercore-1809`](#nats-streaming024-windowsservercore-1809)
-	[`nats-streaming:0.24.3`](#nats-streaming0243)
-	[`nats-streaming:0.24.3-alpine`](#nats-streaming0243-alpine)
-	[`nats-streaming:0.24.3-alpine3.15`](#nats-streaming0243-alpine315)
-	[`nats-streaming:0.24.3-linux`](#nats-streaming0243-linux)
-	[`nats-streaming:0.24.3-nanoserver`](#nats-streaming0243-nanoserver)
-	[`nats-streaming:0.24.3-nanoserver-1809`](#nats-streaming0243-nanoserver-1809)
-	[`nats-streaming:0.24.3-scratch`](#nats-streaming0243-scratch)
-	[`nats-streaming:0.24.3-windowsservercore`](#nats-streaming0243-windowsservercore)
-	[`nats-streaming:0.24.3-windowsservercore-1809`](#nats-streaming0243-windowsservercore-1809)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.15`](#nats-streamingalpine315)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)

## `nats-streaming:0.24`

```console
$ docker pull nats-streaming@sha256:9f8cedbf2e74e6679e9ab44848904ad048f1f9202d1dd72e203002605ba4a331
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:0.24` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eea355922fa3e329228180c171fe18939205a5828944f3c0ec23c0816eef7982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7081263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0f18c883ff929dfaae3de15de5562de5be34b4a941aa05c6d52112b8e4c84`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:21:18 GMT
COPY file:6fcfe62a6cc0951979b80258fb3d207e13828d9234e227e1398cab40548702d7 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:21:18 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:21:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:64b920df5d588d78c6c317a08480a016eb7b6433705c1a3811a22e4e422e61d0`  
		Last Modified: Wed, 09 Mar 2022 23:22:00 GMT  
		Size: 7.1 MB (7081263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:36364386127a72bc130f59fb33c4119222fc6c671e33aea460f694025b82cd46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6597197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a965dc95f8a3e6631c5ca714f0aafd2acc1508a1f6d3298300876536949f11b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:49:55 GMT
COPY file:d62d923585419f7f9d263c0018d56cc159b1092bf7bae749223f339a514a81d9 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:49:56 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:49:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0b00cb53513f9c5bd72363c73ee281128c2cedd1d7653aa7278a2a6536c86a14`  
		Last Modified: Wed, 09 Mar 2022 23:51:50 GMT  
		Size: 6.6 MB (6597197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c786255507edae1bf8167b3adbe962fa9c4ba18fd683462921df662c86e5f36f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6589565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb16b4f9d4a38de66adad0c74fd19049b37e96277e0cd459805b74bdf9474ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:29:51 GMT
COPY file:a5f2524f76b038dc99564d67f8cf6396171fe569b86b60aa9892eca88643b977 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:29:52 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:29:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:29:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:271fefa5e75537e471ab2e96d1b28b6614b2103db059b37f0e60bcc9b8ab40d8`  
		Last Modified: Wed, 09 Mar 2022 23:31:44 GMT  
		Size: 6.6 MB (6589565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb6e16886863d8c84bc6427c4a45c43bca8f97adcddd602756dddc70fa826a6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6510632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd1fc4d49faf17ca5b2a9d116b2758a93de1af0ea5b526e23128bd6bbd00b5f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:41:07 GMT
COPY file:f47e5ea058ace7f6cdb8bca186dec2b15d364fff4ff67303ae8d2cfe38435050 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:41:07 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:41:08 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:41:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9e32cf3eae8c97676148171d71a3cc25149de87eecd89a137222b3b382cdf8f2`  
		Last Modified: Wed, 09 Mar 2022 23:42:13 GMT  
		Size: 6.5 MB (6510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:bf5f4238170d36fdc3b99a4ab8acea5c5755564d3d97131d48d0730dee33bbdc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110249474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68219116c19a9ac4e2603cd23ba4233e15f3ab67ba4a4e9169a2c000801679cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:21:44 GMT
RUN cmd /S /C #(nop) COPY file:2bdfa73d50ba6f64f600945ecab061708a66086f5dd80ec5e00ad93c8bf3b8b6 in C:\nats-streaming-server.exe 
# Wed, 09 Mar 2022 23:21:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:47 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128e56b52a1dd66549cb7830a9bc9f9352ab11829fe936a4bd03858ac830160`  
		Last Modified: Wed, 09 Mar 2022 23:22:35 GMT  
		Size: 7.2 MB (7190251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c581f41ddfe2959d4092845a36fa343eaddd42a160cd818cbca5c31671bff`  
		Last Modified: Wed, 09 Mar 2022 23:22:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba79d16ae428589a386d36328db720a9ac0eb1abd0014da9992cb03cf4df1e`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c567d244b9f979dfa1c24fe471a72b7dc849619f91830d175ca5454f357a2eb`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-alpine`

```console
$ docker pull nats-streaming@sha256:46f6bc8a055bbcd1b58ffaafc158248686f5851a822f184b5201fd1a38795716
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d12746a51c48aba10e7525afe1d2d1e612c23c12e567bac1a553e0acb30e2557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10169886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c721de8113076f98fcb23b6d322f71d6cc6961d8a9d46d3679595678a23d09b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:10:02 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:10:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:10:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:10:04 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:10:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:10:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1b12db41de2569beb9dcd6e97d377d7cba39c4b53203728e8b6639f55e3c72`  
		Last Modified: Tue, 29 Mar 2022 12:10:31 GMT  
		Size: 7.4 MB (7354954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cb35217e54e379f5c8b6c74c11b655397a50428aad62e14a41028fbd0c8f9f`  
		Last Modified: Tue, 29 Mar 2022 12:10:30 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a996504162f4e1defefdf39b9c815aebedc4b6f2d2368653eaff75b86ac1b32a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9492290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4835a9d80927dd9ffba7d9af4330eba813d53c9e63f04157183b2e05d3bba213`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:11:46 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 08:11:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 08:11:51 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 08:11:52 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 08:11:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:11:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988a41d26b8437b47dc078307d79dfa59992c450ff7d3d77b3aed78aac1e9f23`  
		Last Modified: Tue, 29 Mar 2022 08:13:30 GMT  
		Size: 6.9 MB (6869927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cbde1f81c36c2e615065eefa7eeee2461e95df69f9b125ca0346ab588cdb59`  
		Last Modified: Tue, 29 Mar 2022 08:13:27 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:fbe91d8ff12c500ed54662cf8f8c58c24dc31bbe9e39c6da8a85073b01cbcbcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9286866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b926d3d9d831788c13a302b4722dcea8e9f661c41cd57ff54e435acdb94c11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 02:45:23 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 30 Mar 2022 02:45:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 30 Mar 2022 02:45:28 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 30 Mar 2022 02:45:28 GMT
EXPOSE 4222 8222
# Wed, 30 Mar 2022 02:45:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 02:45:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0161c199af9c847e577fd8dd8ca4fe0e491151ddbc5f639a00e503390f25a`  
		Last Modified: Wed, 30 Mar 2022 02:47:12 GMT  
		Size: 6.9 MB (6862142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4686eb18883d40d09804b1dd68b0562efa06de2e4360a100b0d45c8c20352a`  
		Last Modified: Wed, 30 Mar 2022 02:47:07 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4d5d2d2ac8b13c2832901d028154d57915b444280c14d4245b91d4dc7d40153f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c44957ce449564ad5e2f054dc1d3977b918d450e5ce2fe316b9161ae123a69da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:20:52 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:20:56 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:20:58 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691a8d335004266b96b913aebd2472d7fa602c3dbf4470ed5e37e44442df6c9c`  
		Last Modified: Tue, 29 Mar 2022 12:21:45 GMT  
		Size: 6.8 MB (6783079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12fa80c013fd2dd33c06703fc0d1f756eed95dd0d4487fb239b94ce014ba65f`  
		Last Modified: Tue, 29 Mar 2022 12:21:43 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-alpine3.15`

```console
$ docker pull nats-streaming@sha256:46f6bc8a055bbcd1b58ffaafc158248686f5851a822f184b5201fd1a38795716
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d12746a51c48aba10e7525afe1d2d1e612c23c12e567bac1a553e0acb30e2557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10169886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c721de8113076f98fcb23b6d322f71d6cc6961d8a9d46d3679595678a23d09b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:10:02 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:10:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:10:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:10:04 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:10:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:10:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1b12db41de2569beb9dcd6e97d377d7cba39c4b53203728e8b6639f55e3c72`  
		Last Modified: Tue, 29 Mar 2022 12:10:31 GMT  
		Size: 7.4 MB (7354954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cb35217e54e379f5c8b6c74c11b655397a50428aad62e14a41028fbd0c8f9f`  
		Last Modified: Tue, 29 Mar 2022 12:10:30 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a996504162f4e1defefdf39b9c815aebedc4b6f2d2368653eaff75b86ac1b32a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9492290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4835a9d80927dd9ffba7d9af4330eba813d53c9e63f04157183b2e05d3bba213`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:11:46 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 08:11:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 08:11:51 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 08:11:52 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 08:11:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:11:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988a41d26b8437b47dc078307d79dfa59992c450ff7d3d77b3aed78aac1e9f23`  
		Last Modified: Tue, 29 Mar 2022 08:13:30 GMT  
		Size: 6.9 MB (6869927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cbde1f81c36c2e615065eefa7eeee2461e95df69f9b125ca0346ab588cdb59`  
		Last Modified: Tue, 29 Mar 2022 08:13:27 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:fbe91d8ff12c500ed54662cf8f8c58c24dc31bbe9e39c6da8a85073b01cbcbcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9286866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b926d3d9d831788c13a302b4722dcea8e9f661c41cd57ff54e435acdb94c11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 02:45:23 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 30 Mar 2022 02:45:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 30 Mar 2022 02:45:28 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 30 Mar 2022 02:45:28 GMT
EXPOSE 4222 8222
# Wed, 30 Mar 2022 02:45:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 02:45:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0161c199af9c847e577fd8dd8ca4fe0e491151ddbc5f639a00e503390f25a`  
		Last Modified: Wed, 30 Mar 2022 02:47:12 GMT  
		Size: 6.9 MB (6862142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4686eb18883d40d09804b1dd68b0562efa06de2e4360a100b0d45c8c20352a`  
		Last Modified: Wed, 30 Mar 2022 02:47:07 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4d5d2d2ac8b13c2832901d028154d57915b444280c14d4245b91d4dc7d40153f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c44957ce449564ad5e2f054dc1d3977b918d450e5ce2fe316b9161ae123a69da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:20:52 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:20:56 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:20:58 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691a8d335004266b96b913aebd2472d7fa602c3dbf4470ed5e37e44442df6c9c`  
		Last Modified: Tue, 29 Mar 2022 12:21:45 GMT  
		Size: 6.8 MB (6783079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12fa80c013fd2dd33c06703fc0d1f756eed95dd0d4487fb239b94ce014ba65f`  
		Last Modified: Tue, 29 Mar 2022 12:21:43 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-linux`

```console
$ docker pull nats-streaming@sha256:4f097bcee579937a2b55f7702298c9d0ccf44bc8fc2820b81ef02b1a9b146e37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eea355922fa3e329228180c171fe18939205a5828944f3c0ec23c0816eef7982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7081263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0f18c883ff929dfaae3de15de5562de5be34b4a941aa05c6d52112b8e4c84`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:21:18 GMT
COPY file:6fcfe62a6cc0951979b80258fb3d207e13828d9234e227e1398cab40548702d7 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:21:18 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:21:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:64b920df5d588d78c6c317a08480a016eb7b6433705c1a3811a22e4e422e61d0`  
		Last Modified: Wed, 09 Mar 2022 23:22:00 GMT  
		Size: 7.1 MB (7081263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:36364386127a72bc130f59fb33c4119222fc6c671e33aea460f694025b82cd46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6597197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a965dc95f8a3e6631c5ca714f0aafd2acc1508a1f6d3298300876536949f11b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:49:55 GMT
COPY file:d62d923585419f7f9d263c0018d56cc159b1092bf7bae749223f339a514a81d9 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:49:56 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:49:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0b00cb53513f9c5bd72363c73ee281128c2cedd1d7653aa7278a2a6536c86a14`  
		Last Modified: Wed, 09 Mar 2022 23:51:50 GMT  
		Size: 6.6 MB (6597197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c786255507edae1bf8167b3adbe962fa9c4ba18fd683462921df662c86e5f36f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6589565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb16b4f9d4a38de66adad0c74fd19049b37e96277e0cd459805b74bdf9474ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:29:51 GMT
COPY file:a5f2524f76b038dc99564d67f8cf6396171fe569b86b60aa9892eca88643b977 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:29:52 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:29:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:29:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:271fefa5e75537e471ab2e96d1b28b6614b2103db059b37f0e60bcc9b8ab40d8`  
		Last Modified: Wed, 09 Mar 2022 23:31:44 GMT  
		Size: 6.6 MB (6589565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb6e16886863d8c84bc6427c4a45c43bca8f97adcddd602756dddc70fa826a6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6510632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd1fc4d49faf17ca5b2a9d116b2758a93de1af0ea5b526e23128bd6bbd00b5f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:41:07 GMT
COPY file:f47e5ea058ace7f6cdb8bca186dec2b15d364fff4ff67303ae8d2cfe38435050 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:41:07 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:41:08 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:41:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9e32cf3eae8c97676148171d71a3cc25149de87eecd89a137222b3b382cdf8f2`  
		Last Modified: Wed, 09 Mar 2022 23:42:13 GMT  
		Size: 6.5 MB (6510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-nanoserver`

```console
$ docker pull nats-streaming@sha256:427167cf68f6cc7da882af2fe3a4b7c8089d370a60bdfb20d1c2f432095618d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:0.24-nanoserver` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:bf5f4238170d36fdc3b99a4ab8acea5c5755564d3d97131d48d0730dee33bbdc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110249474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68219116c19a9ac4e2603cd23ba4233e15f3ab67ba4a4e9169a2c000801679cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:21:44 GMT
RUN cmd /S /C #(nop) COPY file:2bdfa73d50ba6f64f600945ecab061708a66086f5dd80ec5e00ad93c8bf3b8b6 in C:\nats-streaming-server.exe 
# Wed, 09 Mar 2022 23:21:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:47 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128e56b52a1dd66549cb7830a9bc9f9352ab11829fe936a4bd03858ac830160`  
		Last Modified: Wed, 09 Mar 2022 23:22:35 GMT  
		Size: 7.2 MB (7190251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c581f41ddfe2959d4092845a36fa343eaddd42a160cd818cbca5c31671bff`  
		Last Modified: Wed, 09 Mar 2022 23:22:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba79d16ae428589a386d36328db720a9ac0eb1abd0014da9992cb03cf4df1e`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c567d244b9f979dfa1c24fe471a72b7dc849619f91830d175ca5454f357a2eb`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:427167cf68f6cc7da882af2fe3a4b7c8089d370a60bdfb20d1c2f432095618d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:0.24-nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:bf5f4238170d36fdc3b99a4ab8acea5c5755564d3d97131d48d0730dee33bbdc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110249474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68219116c19a9ac4e2603cd23ba4233e15f3ab67ba4a4e9169a2c000801679cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:21:44 GMT
RUN cmd /S /C #(nop) COPY file:2bdfa73d50ba6f64f600945ecab061708a66086f5dd80ec5e00ad93c8bf3b8b6 in C:\nats-streaming-server.exe 
# Wed, 09 Mar 2022 23:21:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:47 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128e56b52a1dd66549cb7830a9bc9f9352ab11829fe936a4bd03858ac830160`  
		Last Modified: Wed, 09 Mar 2022 23:22:35 GMT  
		Size: 7.2 MB (7190251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c581f41ddfe2959d4092845a36fa343eaddd42a160cd818cbca5c31671bff`  
		Last Modified: Wed, 09 Mar 2022 23:22:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba79d16ae428589a386d36328db720a9ac0eb1abd0014da9992cb03cf4df1e`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c567d244b9f979dfa1c24fe471a72b7dc849619f91830d175ca5454f357a2eb`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-scratch`

```console
$ docker pull nats-streaming@sha256:4f097bcee579937a2b55f7702298c9d0ccf44bc8fc2820b81ef02b1a9b146e37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eea355922fa3e329228180c171fe18939205a5828944f3c0ec23c0816eef7982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7081263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0f18c883ff929dfaae3de15de5562de5be34b4a941aa05c6d52112b8e4c84`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:21:18 GMT
COPY file:6fcfe62a6cc0951979b80258fb3d207e13828d9234e227e1398cab40548702d7 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:21:18 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:21:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:64b920df5d588d78c6c317a08480a016eb7b6433705c1a3811a22e4e422e61d0`  
		Last Modified: Wed, 09 Mar 2022 23:22:00 GMT  
		Size: 7.1 MB (7081263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:36364386127a72bc130f59fb33c4119222fc6c671e33aea460f694025b82cd46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6597197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a965dc95f8a3e6631c5ca714f0aafd2acc1508a1f6d3298300876536949f11b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:49:55 GMT
COPY file:d62d923585419f7f9d263c0018d56cc159b1092bf7bae749223f339a514a81d9 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:49:56 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:49:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0b00cb53513f9c5bd72363c73ee281128c2cedd1d7653aa7278a2a6536c86a14`  
		Last Modified: Wed, 09 Mar 2022 23:51:50 GMT  
		Size: 6.6 MB (6597197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c786255507edae1bf8167b3adbe962fa9c4ba18fd683462921df662c86e5f36f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6589565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb16b4f9d4a38de66adad0c74fd19049b37e96277e0cd459805b74bdf9474ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:29:51 GMT
COPY file:a5f2524f76b038dc99564d67f8cf6396171fe569b86b60aa9892eca88643b977 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:29:52 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:29:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:29:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:271fefa5e75537e471ab2e96d1b28b6614b2103db059b37f0e60bcc9b8ab40d8`  
		Last Modified: Wed, 09 Mar 2022 23:31:44 GMT  
		Size: 6.6 MB (6589565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb6e16886863d8c84bc6427c4a45c43bca8f97adcddd602756dddc70fa826a6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6510632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd1fc4d49faf17ca5b2a9d116b2758a93de1af0ea5b526e23128bd6bbd00b5f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:41:07 GMT
COPY file:f47e5ea058ace7f6cdb8bca186dec2b15d364fff4ff67303ae8d2cfe38435050 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:41:07 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:41:08 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:41:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9e32cf3eae8c97676148171d71a3cc25149de87eecd89a137222b3b382cdf8f2`  
		Last Modified: Wed, 09 Mar 2022 23:42:13 GMT  
		Size: 6.5 MB (6510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-windowsservercore`

```console
$ docker pull nats-streaming@sha256:112510afc4add9efb62621bbcbd4c03a62c4efa7bebfa2854d896a3b81b4822b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:0.24-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:38aa3744b326ea3530932f9ae38c5884a7cc4f4e5e71b77f330b5634d79fa79a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723329559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5125257a9aa0beaab36a017e9f82750b3aac24f4719374d6cc8e339fc187cdd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.3/nats-streaming-server-v0.24.3-windows-amd64.zip
# Wed, 09 Mar 2022 23:18:48 GMT
ENV NATS_STREAMING_SERVER_SHASUM=7473bfa7efd734ca6984907bc9586260031cca926883b468b4752557ecefaff0
# Wed, 09 Mar 2022 23:19:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:21:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:21:28 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1aac6ec834525c931dc81bbbb6d32996b82fd755a3bd625af11f40b8fc66bb`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d303e56675a80a6fa4eef8ef31d6f93742709f41058dcf6e36b8ba6d71a466f8`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8122e4b6aba607bd3d7b17a847d8ab75da7d7cb7a2bbb035e4a31cfc1b7ce6`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393372fa0a20ba2589a43d177f33a0360245be974d231efaa7ab980bc342b574`  
		Last Modified: Wed, 09 Mar 2022 23:22:13 GMT  
		Size: 349.0 KB (348988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3cf158dc37e43f4d84e520f088e32b2851abbf4a70af92161ab5e0d7e3ecbd`  
		Last Modified: Wed, 09 Mar 2022 23:22:20 GMT  
		Size: 7.5 MB (7516588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fff4072b17e75a66709617708b8b9263dabe4a12c4e0a594fb52e058977fa83`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de86f56dd22fbee61ed7161f763ba9de61d7cbf9623b85a879723ea5670f6e20`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04add3ff0ef25a1f32aab83f90a95cffab3d4b55afd3eb376a861b36094a0b0`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:112510afc4add9efb62621bbcbd4c03a62c4efa7bebfa2854d896a3b81b4822b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:0.24-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:38aa3744b326ea3530932f9ae38c5884a7cc4f4e5e71b77f330b5634d79fa79a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723329559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5125257a9aa0beaab36a017e9f82750b3aac24f4719374d6cc8e339fc187cdd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.3/nats-streaming-server-v0.24.3-windows-amd64.zip
# Wed, 09 Mar 2022 23:18:48 GMT
ENV NATS_STREAMING_SERVER_SHASUM=7473bfa7efd734ca6984907bc9586260031cca926883b468b4752557ecefaff0
# Wed, 09 Mar 2022 23:19:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:21:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:21:28 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1aac6ec834525c931dc81bbbb6d32996b82fd755a3bd625af11f40b8fc66bb`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d303e56675a80a6fa4eef8ef31d6f93742709f41058dcf6e36b8ba6d71a466f8`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8122e4b6aba607bd3d7b17a847d8ab75da7d7cb7a2bbb035e4a31cfc1b7ce6`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393372fa0a20ba2589a43d177f33a0360245be974d231efaa7ab980bc342b574`  
		Last Modified: Wed, 09 Mar 2022 23:22:13 GMT  
		Size: 349.0 KB (348988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3cf158dc37e43f4d84e520f088e32b2851abbf4a70af92161ab5e0d7e3ecbd`  
		Last Modified: Wed, 09 Mar 2022 23:22:20 GMT  
		Size: 7.5 MB (7516588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fff4072b17e75a66709617708b8b9263dabe4a12c4e0a594fb52e058977fa83`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de86f56dd22fbee61ed7161f763ba9de61d7cbf9623b85a879723ea5670f6e20`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04add3ff0ef25a1f32aab83f90a95cffab3d4b55afd3eb376a861b36094a0b0`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.3`

```console
$ docker pull nats-streaming@sha256:9f8cedbf2e74e6679e9ab44848904ad048f1f9202d1dd72e203002605ba4a331
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:0.24.3` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eea355922fa3e329228180c171fe18939205a5828944f3c0ec23c0816eef7982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7081263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0f18c883ff929dfaae3de15de5562de5be34b4a941aa05c6d52112b8e4c84`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:21:18 GMT
COPY file:6fcfe62a6cc0951979b80258fb3d207e13828d9234e227e1398cab40548702d7 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:21:18 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:21:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:64b920df5d588d78c6c317a08480a016eb7b6433705c1a3811a22e4e422e61d0`  
		Last Modified: Wed, 09 Mar 2022 23:22:00 GMT  
		Size: 7.1 MB (7081263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:36364386127a72bc130f59fb33c4119222fc6c671e33aea460f694025b82cd46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6597197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a965dc95f8a3e6631c5ca714f0aafd2acc1508a1f6d3298300876536949f11b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:49:55 GMT
COPY file:d62d923585419f7f9d263c0018d56cc159b1092bf7bae749223f339a514a81d9 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:49:56 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:49:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0b00cb53513f9c5bd72363c73ee281128c2cedd1d7653aa7278a2a6536c86a14`  
		Last Modified: Wed, 09 Mar 2022 23:51:50 GMT  
		Size: 6.6 MB (6597197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c786255507edae1bf8167b3adbe962fa9c4ba18fd683462921df662c86e5f36f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6589565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb16b4f9d4a38de66adad0c74fd19049b37e96277e0cd459805b74bdf9474ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:29:51 GMT
COPY file:a5f2524f76b038dc99564d67f8cf6396171fe569b86b60aa9892eca88643b977 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:29:52 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:29:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:29:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:271fefa5e75537e471ab2e96d1b28b6614b2103db059b37f0e60bcc9b8ab40d8`  
		Last Modified: Wed, 09 Mar 2022 23:31:44 GMT  
		Size: 6.6 MB (6589565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb6e16886863d8c84bc6427c4a45c43bca8f97adcddd602756dddc70fa826a6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6510632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd1fc4d49faf17ca5b2a9d116b2758a93de1af0ea5b526e23128bd6bbd00b5f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:41:07 GMT
COPY file:f47e5ea058ace7f6cdb8bca186dec2b15d364fff4ff67303ae8d2cfe38435050 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:41:07 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:41:08 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:41:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9e32cf3eae8c97676148171d71a3cc25149de87eecd89a137222b3b382cdf8f2`  
		Last Modified: Wed, 09 Mar 2022 23:42:13 GMT  
		Size: 6.5 MB (6510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:bf5f4238170d36fdc3b99a4ab8acea5c5755564d3d97131d48d0730dee33bbdc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110249474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68219116c19a9ac4e2603cd23ba4233e15f3ab67ba4a4e9169a2c000801679cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:21:44 GMT
RUN cmd /S /C #(nop) COPY file:2bdfa73d50ba6f64f600945ecab061708a66086f5dd80ec5e00ad93c8bf3b8b6 in C:\nats-streaming-server.exe 
# Wed, 09 Mar 2022 23:21:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:47 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128e56b52a1dd66549cb7830a9bc9f9352ab11829fe936a4bd03858ac830160`  
		Last Modified: Wed, 09 Mar 2022 23:22:35 GMT  
		Size: 7.2 MB (7190251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c581f41ddfe2959d4092845a36fa343eaddd42a160cd818cbca5c31671bff`  
		Last Modified: Wed, 09 Mar 2022 23:22:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba79d16ae428589a386d36328db720a9ac0eb1abd0014da9992cb03cf4df1e`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c567d244b9f979dfa1c24fe471a72b7dc849619f91830d175ca5454f357a2eb`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.3-alpine`

```console
$ docker pull nats-streaming@sha256:46f6bc8a055bbcd1b58ffaafc158248686f5851a822f184b5201fd1a38795716
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.3-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d12746a51c48aba10e7525afe1d2d1e612c23c12e567bac1a553e0acb30e2557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10169886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c721de8113076f98fcb23b6d322f71d6cc6961d8a9d46d3679595678a23d09b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:10:02 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:10:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:10:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:10:04 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:10:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:10:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1b12db41de2569beb9dcd6e97d377d7cba39c4b53203728e8b6639f55e3c72`  
		Last Modified: Tue, 29 Mar 2022 12:10:31 GMT  
		Size: 7.4 MB (7354954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cb35217e54e379f5c8b6c74c11b655397a50428aad62e14a41028fbd0c8f9f`  
		Last Modified: Tue, 29 Mar 2022 12:10:30 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a996504162f4e1defefdf39b9c815aebedc4b6f2d2368653eaff75b86ac1b32a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9492290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4835a9d80927dd9ffba7d9af4330eba813d53c9e63f04157183b2e05d3bba213`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:11:46 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 08:11:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 08:11:51 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 08:11:52 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 08:11:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:11:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988a41d26b8437b47dc078307d79dfa59992c450ff7d3d77b3aed78aac1e9f23`  
		Last Modified: Tue, 29 Mar 2022 08:13:30 GMT  
		Size: 6.9 MB (6869927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cbde1f81c36c2e615065eefa7eeee2461e95df69f9b125ca0346ab588cdb59`  
		Last Modified: Tue, 29 Mar 2022 08:13:27 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:fbe91d8ff12c500ed54662cf8f8c58c24dc31bbe9e39c6da8a85073b01cbcbcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9286866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b926d3d9d831788c13a302b4722dcea8e9f661c41cd57ff54e435acdb94c11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 02:45:23 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 30 Mar 2022 02:45:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 30 Mar 2022 02:45:28 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 30 Mar 2022 02:45:28 GMT
EXPOSE 4222 8222
# Wed, 30 Mar 2022 02:45:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 02:45:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0161c199af9c847e577fd8dd8ca4fe0e491151ddbc5f639a00e503390f25a`  
		Last Modified: Wed, 30 Mar 2022 02:47:12 GMT  
		Size: 6.9 MB (6862142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4686eb18883d40d09804b1dd68b0562efa06de2e4360a100b0d45c8c20352a`  
		Last Modified: Wed, 30 Mar 2022 02:47:07 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4d5d2d2ac8b13c2832901d028154d57915b444280c14d4245b91d4dc7d40153f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c44957ce449564ad5e2f054dc1d3977b918d450e5ce2fe316b9161ae123a69da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:20:52 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:20:56 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:20:58 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691a8d335004266b96b913aebd2472d7fa602c3dbf4470ed5e37e44442df6c9c`  
		Last Modified: Tue, 29 Mar 2022 12:21:45 GMT  
		Size: 6.8 MB (6783079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12fa80c013fd2dd33c06703fc0d1f756eed95dd0d4487fb239b94ce014ba65f`  
		Last Modified: Tue, 29 Mar 2022 12:21:43 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.3-alpine3.15`

```console
$ docker pull nats-streaming@sha256:46f6bc8a055bbcd1b58ffaafc158248686f5851a822f184b5201fd1a38795716
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.3-alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d12746a51c48aba10e7525afe1d2d1e612c23c12e567bac1a553e0acb30e2557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10169886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c721de8113076f98fcb23b6d322f71d6cc6961d8a9d46d3679595678a23d09b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:10:02 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:10:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:10:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:10:04 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:10:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:10:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1b12db41de2569beb9dcd6e97d377d7cba39c4b53203728e8b6639f55e3c72`  
		Last Modified: Tue, 29 Mar 2022 12:10:31 GMT  
		Size: 7.4 MB (7354954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cb35217e54e379f5c8b6c74c11b655397a50428aad62e14a41028fbd0c8f9f`  
		Last Modified: Tue, 29 Mar 2022 12:10:30 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a996504162f4e1defefdf39b9c815aebedc4b6f2d2368653eaff75b86ac1b32a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9492290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4835a9d80927dd9ffba7d9af4330eba813d53c9e63f04157183b2e05d3bba213`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:11:46 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 08:11:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 08:11:51 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 08:11:52 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 08:11:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:11:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988a41d26b8437b47dc078307d79dfa59992c450ff7d3d77b3aed78aac1e9f23`  
		Last Modified: Tue, 29 Mar 2022 08:13:30 GMT  
		Size: 6.9 MB (6869927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cbde1f81c36c2e615065eefa7eeee2461e95df69f9b125ca0346ab588cdb59`  
		Last Modified: Tue, 29 Mar 2022 08:13:27 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:fbe91d8ff12c500ed54662cf8f8c58c24dc31bbe9e39c6da8a85073b01cbcbcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9286866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b926d3d9d831788c13a302b4722dcea8e9f661c41cd57ff54e435acdb94c11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 02:45:23 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 30 Mar 2022 02:45:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 30 Mar 2022 02:45:28 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 30 Mar 2022 02:45:28 GMT
EXPOSE 4222 8222
# Wed, 30 Mar 2022 02:45:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 02:45:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0161c199af9c847e577fd8dd8ca4fe0e491151ddbc5f639a00e503390f25a`  
		Last Modified: Wed, 30 Mar 2022 02:47:12 GMT  
		Size: 6.9 MB (6862142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4686eb18883d40d09804b1dd68b0562efa06de2e4360a100b0d45c8c20352a`  
		Last Modified: Wed, 30 Mar 2022 02:47:07 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4d5d2d2ac8b13c2832901d028154d57915b444280c14d4245b91d4dc7d40153f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c44957ce449564ad5e2f054dc1d3977b918d450e5ce2fe316b9161ae123a69da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:20:52 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:20:56 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:20:58 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691a8d335004266b96b913aebd2472d7fa602c3dbf4470ed5e37e44442df6c9c`  
		Last Modified: Tue, 29 Mar 2022 12:21:45 GMT  
		Size: 6.8 MB (6783079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12fa80c013fd2dd33c06703fc0d1f756eed95dd0d4487fb239b94ce014ba65f`  
		Last Modified: Tue, 29 Mar 2022 12:21:43 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.3-linux`

```console
$ docker pull nats-streaming@sha256:4f097bcee579937a2b55f7702298c9d0ccf44bc8fc2820b81ef02b1a9b146e37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.3-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eea355922fa3e329228180c171fe18939205a5828944f3c0ec23c0816eef7982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7081263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0f18c883ff929dfaae3de15de5562de5be34b4a941aa05c6d52112b8e4c84`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:21:18 GMT
COPY file:6fcfe62a6cc0951979b80258fb3d207e13828d9234e227e1398cab40548702d7 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:21:18 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:21:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:64b920df5d588d78c6c317a08480a016eb7b6433705c1a3811a22e4e422e61d0`  
		Last Modified: Wed, 09 Mar 2022 23:22:00 GMT  
		Size: 7.1 MB (7081263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:36364386127a72bc130f59fb33c4119222fc6c671e33aea460f694025b82cd46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6597197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a965dc95f8a3e6631c5ca714f0aafd2acc1508a1f6d3298300876536949f11b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:49:55 GMT
COPY file:d62d923585419f7f9d263c0018d56cc159b1092bf7bae749223f339a514a81d9 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:49:56 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:49:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0b00cb53513f9c5bd72363c73ee281128c2cedd1d7653aa7278a2a6536c86a14`  
		Last Modified: Wed, 09 Mar 2022 23:51:50 GMT  
		Size: 6.6 MB (6597197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c786255507edae1bf8167b3adbe962fa9c4ba18fd683462921df662c86e5f36f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6589565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb16b4f9d4a38de66adad0c74fd19049b37e96277e0cd459805b74bdf9474ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:29:51 GMT
COPY file:a5f2524f76b038dc99564d67f8cf6396171fe569b86b60aa9892eca88643b977 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:29:52 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:29:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:29:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:271fefa5e75537e471ab2e96d1b28b6614b2103db059b37f0e60bcc9b8ab40d8`  
		Last Modified: Wed, 09 Mar 2022 23:31:44 GMT  
		Size: 6.6 MB (6589565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb6e16886863d8c84bc6427c4a45c43bca8f97adcddd602756dddc70fa826a6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6510632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd1fc4d49faf17ca5b2a9d116b2758a93de1af0ea5b526e23128bd6bbd00b5f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:41:07 GMT
COPY file:f47e5ea058ace7f6cdb8bca186dec2b15d364fff4ff67303ae8d2cfe38435050 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:41:07 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:41:08 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:41:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9e32cf3eae8c97676148171d71a3cc25149de87eecd89a137222b3b382cdf8f2`  
		Last Modified: Wed, 09 Mar 2022 23:42:13 GMT  
		Size: 6.5 MB (6510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.3-nanoserver`

```console
$ docker pull nats-streaming@sha256:427167cf68f6cc7da882af2fe3a4b7c8089d370a60bdfb20d1c2f432095618d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:0.24.3-nanoserver` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:bf5f4238170d36fdc3b99a4ab8acea5c5755564d3d97131d48d0730dee33bbdc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110249474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68219116c19a9ac4e2603cd23ba4233e15f3ab67ba4a4e9169a2c000801679cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:21:44 GMT
RUN cmd /S /C #(nop) COPY file:2bdfa73d50ba6f64f600945ecab061708a66086f5dd80ec5e00ad93c8bf3b8b6 in C:\nats-streaming-server.exe 
# Wed, 09 Mar 2022 23:21:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:47 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128e56b52a1dd66549cb7830a9bc9f9352ab11829fe936a4bd03858ac830160`  
		Last Modified: Wed, 09 Mar 2022 23:22:35 GMT  
		Size: 7.2 MB (7190251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c581f41ddfe2959d4092845a36fa343eaddd42a160cd818cbca5c31671bff`  
		Last Modified: Wed, 09 Mar 2022 23:22:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba79d16ae428589a386d36328db720a9ac0eb1abd0014da9992cb03cf4df1e`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c567d244b9f979dfa1c24fe471a72b7dc849619f91830d175ca5454f357a2eb`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.3-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:427167cf68f6cc7da882af2fe3a4b7c8089d370a60bdfb20d1c2f432095618d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:0.24.3-nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:bf5f4238170d36fdc3b99a4ab8acea5c5755564d3d97131d48d0730dee33bbdc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110249474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68219116c19a9ac4e2603cd23ba4233e15f3ab67ba4a4e9169a2c000801679cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:21:44 GMT
RUN cmd /S /C #(nop) COPY file:2bdfa73d50ba6f64f600945ecab061708a66086f5dd80ec5e00ad93c8bf3b8b6 in C:\nats-streaming-server.exe 
# Wed, 09 Mar 2022 23:21:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:47 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128e56b52a1dd66549cb7830a9bc9f9352ab11829fe936a4bd03858ac830160`  
		Last Modified: Wed, 09 Mar 2022 23:22:35 GMT  
		Size: 7.2 MB (7190251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c581f41ddfe2959d4092845a36fa343eaddd42a160cd818cbca5c31671bff`  
		Last Modified: Wed, 09 Mar 2022 23:22:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba79d16ae428589a386d36328db720a9ac0eb1abd0014da9992cb03cf4df1e`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c567d244b9f979dfa1c24fe471a72b7dc849619f91830d175ca5454f357a2eb`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.3-scratch`

```console
$ docker pull nats-streaming@sha256:4f097bcee579937a2b55f7702298c9d0ccf44bc8fc2820b81ef02b1a9b146e37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.3-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eea355922fa3e329228180c171fe18939205a5828944f3c0ec23c0816eef7982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7081263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0f18c883ff929dfaae3de15de5562de5be34b4a941aa05c6d52112b8e4c84`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:21:18 GMT
COPY file:6fcfe62a6cc0951979b80258fb3d207e13828d9234e227e1398cab40548702d7 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:21:18 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:21:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:64b920df5d588d78c6c317a08480a016eb7b6433705c1a3811a22e4e422e61d0`  
		Last Modified: Wed, 09 Mar 2022 23:22:00 GMT  
		Size: 7.1 MB (7081263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:36364386127a72bc130f59fb33c4119222fc6c671e33aea460f694025b82cd46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6597197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a965dc95f8a3e6631c5ca714f0aafd2acc1508a1f6d3298300876536949f11b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:49:55 GMT
COPY file:d62d923585419f7f9d263c0018d56cc159b1092bf7bae749223f339a514a81d9 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:49:56 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:49:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0b00cb53513f9c5bd72363c73ee281128c2cedd1d7653aa7278a2a6536c86a14`  
		Last Modified: Wed, 09 Mar 2022 23:51:50 GMT  
		Size: 6.6 MB (6597197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c786255507edae1bf8167b3adbe962fa9c4ba18fd683462921df662c86e5f36f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6589565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb16b4f9d4a38de66adad0c74fd19049b37e96277e0cd459805b74bdf9474ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:29:51 GMT
COPY file:a5f2524f76b038dc99564d67f8cf6396171fe569b86b60aa9892eca88643b977 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:29:52 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:29:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:29:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:271fefa5e75537e471ab2e96d1b28b6614b2103db059b37f0e60bcc9b8ab40d8`  
		Last Modified: Wed, 09 Mar 2022 23:31:44 GMT  
		Size: 6.6 MB (6589565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.3-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb6e16886863d8c84bc6427c4a45c43bca8f97adcddd602756dddc70fa826a6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6510632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd1fc4d49faf17ca5b2a9d116b2758a93de1af0ea5b526e23128bd6bbd00b5f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:41:07 GMT
COPY file:f47e5ea058ace7f6cdb8bca186dec2b15d364fff4ff67303ae8d2cfe38435050 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:41:07 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:41:08 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:41:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9e32cf3eae8c97676148171d71a3cc25149de87eecd89a137222b3b382cdf8f2`  
		Last Modified: Wed, 09 Mar 2022 23:42:13 GMT  
		Size: 6.5 MB (6510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.3-windowsservercore`

```console
$ docker pull nats-streaming@sha256:112510afc4add9efb62621bbcbd4c03a62c4efa7bebfa2854d896a3b81b4822b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:0.24.3-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:38aa3744b326ea3530932f9ae38c5884a7cc4f4e5e71b77f330b5634d79fa79a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723329559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5125257a9aa0beaab36a017e9f82750b3aac24f4719374d6cc8e339fc187cdd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.3/nats-streaming-server-v0.24.3-windows-amd64.zip
# Wed, 09 Mar 2022 23:18:48 GMT
ENV NATS_STREAMING_SERVER_SHASUM=7473bfa7efd734ca6984907bc9586260031cca926883b468b4752557ecefaff0
# Wed, 09 Mar 2022 23:19:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:21:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:21:28 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1aac6ec834525c931dc81bbbb6d32996b82fd755a3bd625af11f40b8fc66bb`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d303e56675a80a6fa4eef8ef31d6f93742709f41058dcf6e36b8ba6d71a466f8`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8122e4b6aba607bd3d7b17a847d8ab75da7d7cb7a2bbb035e4a31cfc1b7ce6`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393372fa0a20ba2589a43d177f33a0360245be974d231efaa7ab980bc342b574`  
		Last Modified: Wed, 09 Mar 2022 23:22:13 GMT  
		Size: 349.0 KB (348988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3cf158dc37e43f4d84e520f088e32b2851abbf4a70af92161ab5e0d7e3ecbd`  
		Last Modified: Wed, 09 Mar 2022 23:22:20 GMT  
		Size: 7.5 MB (7516588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fff4072b17e75a66709617708b8b9263dabe4a12c4e0a594fb52e058977fa83`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de86f56dd22fbee61ed7161f763ba9de61d7cbf9623b85a879723ea5670f6e20`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04add3ff0ef25a1f32aab83f90a95cffab3d4b55afd3eb376a861b36094a0b0`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.3-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:112510afc4add9efb62621bbcbd4c03a62c4efa7bebfa2854d896a3b81b4822b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:0.24.3-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:38aa3744b326ea3530932f9ae38c5884a7cc4f4e5e71b77f330b5634d79fa79a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723329559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5125257a9aa0beaab36a017e9f82750b3aac24f4719374d6cc8e339fc187cdd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.3/nats-streaming-server-v0.24.3-windows-amd64.zip
# Wed, 09 Mar 2022 23:18:48 GMT
ENV NATS_STREAMING_SERVER_SHASUM=7473bfa7efd734ca6984907bc9586260031cca926883b468b4752557ecefaff0
# Wed, 09 Mar 2022 23:19:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:21:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:21:28 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1aac6ec834525c931dc81bbbb6d32996b82fd755a3bd625af11f40b8fc66bb`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d303e56675a80a6fa4eef8ef31d6f93742709f41058dcf6e36b8ba6d71a466f8`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8122e4b6aba607bd3d7b17a847d8ab75da7d7cb7a2bbb035e4a31cfc1b7ce6`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393372fa0a20ba2589a43d177f33a0360245be974d231efaa7ab980bc342b574`  
		Last Modified: Wed, 09 Mar 2022 23:22:13 GMT  
		Size: 349.0 KB (348988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3cf158dc37e43f4d84e520f088e32b2851abbf4a70af92161ab5e0d7e3ecbd`  
		Last Modified: Wed, 09 Mar 2022 23:22:20 GMT  
		Size: 7.5 MB (7516588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fff4072b17e75a66709617708b8b9263dabe4a12c4e0a594fb52e058977fa83`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de86f56dd22fbee61ed7161f763ba9de61d7cbf9623b85a879723ea5670f6e20`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04add3ff0ef25a1f32aab83f90a95cffab3d4b55afd3eb376a861b36094a0b0`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:46f6bc8a055bbcd1b58ffaafc158248686f5851a822f184b5201fd1a38795716
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d12746a51c48aba10e7525afe1d2d1e612c23c12e567bac1a553e0acb30e2557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10169886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c721de8113076f98fcb23b6d322f71d6cc6961d8a9d46d3679595678a23d09b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:10:02 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:10:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:10:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:10:04 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:10:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:10:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1b12db41de2569beb9dcd6e97d377d7cba39c4b53203728e8b6639f55e3c72`  
		Last Modified: Tue, 29 Mar 2022 12:10:31 GMT  
		Size: 7.4 MB (7354954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cb35217e54e379f5c8b6c74c11b655397a50428aad62e14a41028fbd0c8f9f`  
		Last Modified: Tue, 29 Mar 2022 12:10:30 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a996504162f4e1defefdf39b9c815aebedc4b6f2d2368653eaff75b86ac1b32a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9492290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4835a9d80927dd9ffba7d9af4330eba813d53c9e63f04157183b2e05d3bba213`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:11:46 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 08:11:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 08:11:51 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 08:11:52 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 08:11:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:11:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988a41d26b8437b47dc078307d79dfa59992c450ff7d3d77b3aed78aac1e9f23`  
		Last Modified: Tue, 29 Mar 2022 08:13:30 GMT  
		Size: 6.9 MB (6869927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cbde1f81c36c2e615065eefa7eeee2461e95df69f9b125ca0346ab588cdb59`  
		Last Modified: Tue, 29 Mar 2022 08:13:27 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:fbe91d8ff12c500ed54662cf8f8c58c24dc31bbe9e39c6da8a85073b01cbcbcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9286866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b926d3d9d831788c13a302b4722dcea8e9f661c41cd57ff54e435acdb94c11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 02:45:23 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 30 Mar 2022 02:45:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 30 Mar 2022 02:45:28 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 30 Mar 2022 02:45:28 GMT
EXPOSE 4222 8222
# Wed, 30 Mar 2022 02:45:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 02:45:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0161c199af9c847e577fd8dd8ca4fe0e491151ddbc5f639a00e503390f25a`  
		Last Modified: Wed, 30 Mar 2022 02:47:12 GMT  
		Size: 6.9 MB (6862142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4686eb18883d40d09804b1dd68b0562efa06de2e4360a100b0d45c8c20352a`  
		Last Modified: Wed, 30 Mar 2022 02:47:07 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4d5d2d2ac8b13c2832901d028154d57915b444280c14d4245b91d4dc7d40153f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c44957ce449564ad5e2f054dc1d3977b918d450e5ce2fe316b9161ae123a69da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:20:52 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:20:56 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:20:58 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691a8d335004266b96b913aebd2472d7fa602c3dbf4470ed5e37e44442df6c9c`  
		Last Modified: Tue, 29 Mar 2022 12:21:45 GMT  
		Size: 6.8 MB (6783079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12fa80c013fd2dd33c06703fc0d1f756eed95dd0d4487fb239b94ce014ba65f`  
		Last Modified: Tue, 29 Mar 2022 12:21:43 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.15`

```console
$ docker pull nats-streaming@sha256:46f6bc8a055bbcd1b58ffaafc158248686f5851a822f184b5201fd1a38795716
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d12746a51c48aba10e7525afe1d2d1e612c23c12e567bac1a553e0acb30e2557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10169886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c721de8113076f98fcb23b6d322f71d6cc6961d8a9d46d3679595678a23d09b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:10:02 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:10:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:10:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:10:04 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:10:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:10:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1b12db41de2569beb9dcd6e97d377d7cba39c4b53203728e8b6639f55e3c72`  
		Last Modified: Tue, 29 Mar 2022 12:10:31 GMT  
		Size: 7.4 MB (7354954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cb35217e54e379f5c8b6c74c11b655397a50428aad62e14a41028fbd0c8f9f`  
		Last Modified: Tue, 29 Mar 2022 12:10:30 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a996504162f4e1defefdf39b9c815aebedc4b6f2d2368653eaff75b86ac1b32a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9492290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4835a9d80927dd9ffba7d9af4330eba813d53c9e63f04157183b2e05d3bba213`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:11:46 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 08:11:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 08:11:51 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 08:11:52 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 08:11:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:11:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988a41d26b8437b47dc078307d79dfa59992c450ff7d3d77b3aed78aac1e9f23`  
		Last Modified: Tue, 29 Mar 2022 08:13:30 GMT  
		Size: 6.9 MB (6869927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cbde1f81c36c2e615065eefa7eeee2461e95df69f9b125ca0346ab588cdb59`  
		Last Modified: Tue, 29 Mar 2022 08:13:27 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:fbe91d8ff12c500ed54662cf8f8c58c24dc31bbe9e39c6da8a85073b01cbcbcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9286866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b926d3d9d831788c13a302b4722dcea8e9f661c41cd57ff54e435acdb94c11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 02:45:23 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 30 Mar 2022 02:45:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 30 Mar 2022 02:45:28 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 30 Mar 2022 02:45:28 GMT
EXPOSE 4222 8222
# Wed, 30 Mar 2022 02:45:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 02:45:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0161c199af9c847e577fd8dd8ca4fe0e491151ddbc5f639a00e503390f25a`  
		Last Modified: Wed, 30 Mar 2022 02:47:12 GMT  
		Size: 6.9 MB (6862142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4686eb18883d40d09804b1dd68b0562efa06de2e4360a100b0d45c8c20352a`  
		Last Modified: Wed, 30 Mar 2022 02:47:07 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4d5d2d2ac8b13c2832901d028154d57915b444280c14d4245b91d4dc7d40153f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c44957ce449564ad5e2f054dc1d3977b918d450e5ce2fe316b9161ae123a69da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:20:52 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Tue, 29 Mar 2022 12:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3d483a033dd054cf0446ca2c5a5d7c6b7ce58de3155008b2281c50922cbe6426' ;; 		armhf) natsArch='arm6'; sha256='f78977a51901034927264e8087acc05d65aecf77bf9f4e421168a0afd81587c2' ;; 		armv7) natsArch='arm7'; sha256='efb2a459cfef1c08b4041becdc16ae631c4bcd9ec767635051e67e609f4cacef' ;; 		x86_64) natsArch='amd64'; sha256='bf87f5e0ceb95e4fd12b7256cac9149de6f44b60a296547e7dc915c08f05859a' ;; 		x86) natsArch='386'; sha256='e5d0871f4c8c3bafa075e02604be0adc92cba1ebe8da0c7855bff3a4e5cb0ad1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 29 Mar 2022 12:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 29 Mar 2022 12:20:56 GMT
EXPOSE 4222 8222
# Tue, 29 Mar 2022 12:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:20:58 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691a8d335004266b96b913aebd2472d7fa602c3dbf4470ed5e37e44442df6c9c`  
		Last Modified: Tue, 29 Mar 2022 12:21:45 GMT  
		Size: 6.8 MB (6783079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12fa80c013fd2dd33c06703fc0d1f756eed95dd0d4487fb239b94ce014ba65f`  
		Last Modified: Tue, 29 Mar 2022 12:21:43 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:9f8cedbf2e74e6679e9ab44848904ad048f1f9202d1dd72e203002605ba4a331
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eea355922fa3e329228180c171fe18939205a5828944f3c0ec23c0816eef7982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7081263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0f18c883ff929dfaae3de15de5562de5be34b4a941aa05c6d52112b8e4c84`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:21:18 GMT
COPY file:6fcfe62a6cc0951979b80258fb3d207e13828d9234e227e1398cab40548702d7 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:21:18 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:21:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:64b920df5d588d78c6c317a08480a016eb7b6433705c1a3811a22e4e422e61d0`  
		Last Modified: Wed, 09 Mar 2022 23:22:00 GMT  
		Size: 7.1 MB (7081263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:36364386127a72bc130f59fb33c4119222fc6c671e33aea460f694025b82cd46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6597197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a965dc95f8a3e6631c5ca714f0aafd2acc1508a1f6d3298300876536949f11b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:49:55 GMT
COPY file:d62d923585419f7f9d263c0018d56cc159b1092bf7bae749223f339a514a81d9 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:49:56 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:49:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0b00cb53513f9c5bd72363c73ee281128c2cedd1d7653aa7278a2a6536c86a14`  
		Last Modified: Wed, 09 Mar 2022 23:51:50 GMT  
		Size: 6.6 MB (6597197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c786255507edae1bf8167b3adbe962fa9c4ba18fd683462921df662c86e5f36f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6589565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb16b4f9d4a38de66adad0c74fd19049b37e96277e0cd459805b74bdf9474ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:29:51 GMT
COPY file:a5f2524f76b038dc99564d67f8cf6396171fe569b86b60aa9892eca88643b977 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:29:52 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:29:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:29:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:271fefa5e75537e471ab2e96d1b28b6614b2103db059b37f0e60bcc9b8ab40d8`  
		Last Modified: Wed, 09 Mar 2022 23:31:44 GMT  
		Size: 6.6 MB (6589565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb6e16886863d8c84bc6427c4a45c43bca8f97adcddd602756dddc70fa826a6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6510632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd1fc4d49faf17ca5b2a9d116b2758a93de1af0ea5b526e23128bd6bbd00b5f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:41:07 GMT
COPY file:f47e5ea058ace7f6cdb8bca186dec2b15d364fff4ff67303ae8d2cfe38435050 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:41:07 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:41:08 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:41:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9e32cf3eae8c97676148171d71a3cc25149de87eecd89a137222b3b382cdf8f2`  
		Last Modified: Wed, 09 Mar 2022 23:42:13 GMT  
		Size: 6.5 MB (6510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:bf5f4238170d36fdc3b99a4ab8acea5c5755564d3d97131d48d0730dee33bbdc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110249474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68219116c19a9ac4e2603cd23ba4233e15f3ab67ba4a4e9169a2c000801679cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:21:44 GMT
RUN cmd /S /C #(nop) COPY file:2bdfa73d50ba6f64f600945ecab061708a66086f5dd80ec5e00ad93c8bf3b8b6 in C:\nats-streaming-server.exe 
# Wed, 09 Mar 2022 23:21:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:47 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128e56b52a1dd66549cb7830a9bc9f9352ab11829fe936a4bd03858ac830160`  
		Last Modified: Wed, 09 Mar 2022 23:22:35 GMT  
		Size: 7.2 MB (7190251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c581f41ddfe2959d4092845a36fa343eaddd42a160cd818cbca5c31671bff`  
		Last Modified: Wed, 09 Mar 2022 23:22:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba79d16ae428589a386d36328db720a9ac0eb1abd0014da9992cb03cf4df1e`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c567d244b9f979dfa1c24fe471a72b7dc849619f91830d175ca5454f357a2eb`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:4f097bcee579937a2b55f7702298c9d0ccf44bc8fc2820b81ef02b1a9b146e37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eea355922fa3e329228180c171fe18939205a5828944f3c0ec23c0816eef7982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7081263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0f18c883ff929dfaae3de15de5562de5be34b4a941aa05c6d52112b8e4c84`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:21:18 GMT
COPY file:6fcfe62a6cc0951979b80258fb3d207e13828d9234e227e1398cab40548702d7 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:21:18 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:21:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:64b920df5d588d78c6c317a08480a016eb7b6433705c1a3811a22e4e422e61d0`  
		Last Modified: Wed, 09 Mar 2022 23:22:00 GMT  
		Size: 7.1 MB (7081263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:36364386127a72bc130f59fb33c4119222fc6c671e33aea460f694025b82cd46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6597197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a965dc95f8a3e6631c5ca714f0aafd2acc1508a1f6d3298300876536949f11b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:49:55 GMT
COPY file:d62d923585419f7f9d263c0018d56cc159b1092bf7bae749223f339a514a81d9 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:49:56 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:49:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0b00cb53513f9c5bd72363c73ee281128c2cedd1d7653aa7278a2a6536c86a14`  
		Last Modified: Wed, 09 Mar 2022 23:51:50 GMT  
		Size: 6.6 MB (6597197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c786255507edae1bf8167b3adbe962fa9c4ba18fd683462921df662c86e5f36f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6589565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb16b4f9d4a38de66adad0c74fd19049b37e96277e0cd459805b74bdf9474ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:29:51 GMT
COPY file:a5f2524f76b038dc99564d67f8cf6396171fe569b86b60aa9892eca88643b977 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:29:52 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:29:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:29:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:271fefa5e75537e471ab2e96d1b28b6614b2103db059b37f0e60bcc9b8ab40d8`  
		Last Modified: Wed, 09 Mar 2022 23:31:44 GMT  
		Size: 6.6 MB (6589565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb6e16886863d8c84bc6427c4a45c43bca8f97adcddd602756dddc70fa826a6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6510632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd1fc4d49faf17ca5b2a9d116b2758a93de1af0ea5b526e23128bd6bbd00b5f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:41:07 GMT
COPY file:f47e5ea058ace7f6cdb8bca186dec2b15d364fff4ff67303ae8d2cfe38435050 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:41:07 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:41:08 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:41:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9e32cf3eae8c97676148171d71a3cc25149de87eecd89a137222b3b382cdf8f2`  
		Last Modified: Wed, 09 Mar 2022 23:42:13 GMT  
		Size: 6.5 MB (6510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:427167cf68f6cc7da882af2fe3a4b7c8089d370a60bdfb20d1c2f432095618d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:bf5f4238170d36fdc3b99a4ab8acea5c5755564d3d97131d48d0730dee33bbdc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110249474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68219116c19a9ac4e2603cd23ba4233e15f3ab67ba4a4e9169a2c000801679cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:21:44 GMT
RUN cmd /S /C #(nop) COPY file:2bdfa73d50ba6f64f600945ecab061708a66086f5dd80ec5e00ad93c8bf3b8b6 in C:\nats-streaming-server.exe 
# Wed, 09 Mar 2022 23:21:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:47 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128e56b52a1dd66549cb7830a9bc9f9352ab11829fe936a4bd03858ac830160`  
		Last Modified: Wed, 09 Mar 2022 23:22:35 GMT  
		Size: 7.2 MB (7190251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c581f41ddfe2959d4092845a36fa343eaddd42a160cd818cbca5c31671bff`  
		Last Modified: Wed, 09 Mar 2022 23:22:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba79d16ae428589a386d36328db720a9ac0eb1abd0014da9992cb03cf4df1e`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c567d244b9f979dfa1c24fe471a72b7dc849619f91830d175ca5454f357a2eb`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:427167cf68f6cc7da882af2fe3a4b7c8089d370a60bdfb20d1c2f432095618d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:bf5f4238170d36fdc3b99a4ab8acea5c5755564d3d97131d48d0730dee33bbdc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110249474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68219116c19a9ac4e2603cd23ba4233e15f3ab67ba4a4e9169a2c000801679cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:21:44 GMT
RUN cmd /S /C #(nop) COPY file:2bdfa73d50ba6f64f600945ecab061708a66086f5dd80ec5e00ad93c8bf3b8b6 in C:\nats-streaming-server.exe 
# Wed, 09 Mar 2022 23:21:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:47 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128e56b52a1dd66549cb7830a9bc9f9352ab11829fe936a4bd03858ac830160`  
		Last Modified: Wed, 09 Mar 2022 23:22:35 GMT  
		Size: 7.2 MB (7190251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c581f41ddfe2959d4092845a36fa343eaddd42a160cd818cbca5c31671bff`  
		Last Modified: Wed, 09 Mar 2022 23:22:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba79d16ae428589a386d36328db720a9ac0eb1abd0014da9992cb03cf4df1e`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c567d244b9f979dfa1c24fe471a72b7dc849619f91830d175ca5454f357a2eb`  
		Last Modified: Wed, 09 Mar 2022 23:22:32 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:4f097bcee579937a2b55f7702298c9d0ccf44bc8fc2820b81ef02b1a9b146e37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eea355922fa3e329228180c171fe18939205a5828944f3c0ec23c0816eef7982
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7081263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0f18c883ff929dfaae3de15de5562de5be34b4a941aa05c6d52112b8e4c84`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:21:18 GMT
COPY file:6fcfe62a6cc0951979b80258fb3d207e13828d9234e227e1398cab40548702d7 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:21:18 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:21:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:64b920df5d588d78c6c317a08480a016eb7b6433705c1a3811a22e4e422e61d0`  
		Last Modified: Wed, 09 Mar 2022 23:22:00 GMT  
		Size: 7.1 MB (7081263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:36364386127a72bc130f59fb33c4119222fc6c671e33aea460f694025b82cd46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6597197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a965dc95f8a3e6631c5ca714f0aafd2acc1508a1f6d3298300876536949f11b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:49:55 GMT
COPY file:d62d923585419f7f9d263c0018d56cc159b1092bf7bae749223f339a514a81d9 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:49:56 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:49:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0b00cb53513f9c5bd72363c73ee281128c2cedd1d7653aa7278a2a6536c86a14`  
		Last Modified: Wed, 09 Mar 2022 23:51:50 GMT  
		Size: 6.6 MB (6597197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c786255507edae1bf8167b3adbe962fa9c4ba18fd683462921df662c86e5f36f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6589565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb16b4f9d4a38de66adad0c74fd19049b37e96277e0cd459805b74bdf9474ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:29:51 GMT
COPY file:a5f2524f76b038dc99564d67f8cf6396171fe569b86b60aa9892eca88643b977 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:29:52 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:29:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:29:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:271fefa5e75537e471ab2e96d1b28b6614b2103db059b37f0e60bcc9b8ab40d8`  
		Last Modified: Wed, 09 Mar 2022 23:31:44 GMT  
		Size: 6.6 MB (6589565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb6e16886863d8c84bc6427c4a45c43bca8f97adcddd602756dddc70fa826a6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6510632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd1fc4d49faf17ca5b2a9d116b2758a93de1af0ea5b526e23128bd6bbd00b5f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 09 Mar 2022 23:41:07 GMT
COPY file:f47e5ea058ace7f6cdb8bca186dec2b15d364fff4ff67303ae8d2cfe38435050 in /nats-streaming-server 
# Wed, 09 Mar 2022 23:41:07 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:41:08 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 09 Mar 2022 23:41:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9e32cf3eae8c97676148171d71a3cc25149de87eecd89a137222b3b382cdf8f2`  
		Last Modified: Wed, 09 Mar 2022 23:42:13 GMT  
		Size: 6.5 MB (6510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:112510afc4add9efb62621bbcbd4c03a62c4efa7bebfa2854d896a3b81b4822b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:38aa3744b326ea3530932f9ae38c5884a7cc4f4e5e71b77f330b5634d79fa79a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723329559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5125257a9aa0beaab36a017e9f82750b3aac24f4719374d6cc8e339fc187cdd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.3/nats-streaming-server-v0.24.3-windows-amd64.zip
# Wed, 09 Mar 2022 23:18:48 GMT
ENV NATS_STREAMING_SERVER_SHASUM=7473bfa7efd734ca6984907bc9586260031cca926883b468b4752557ecefaff0
# Wed, 09 Mar 2022 23:19:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:21:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:21:28 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1aac6ec834525c931dc81bbbb6d32996b82fd755a3bd625af11f40b8fc66bb`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d303e56675a80a6fa4eef8ef31d6f93742709f41058dcf6e36b8ba6d71a466f8`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8122e4b6aba607bd3d7b17a847d8ab75da7d7cb7a2bbb035e4a31cfc1b7ce6`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393372fa0a20ba2589a43d177f33a0360245be974d231efaa7ab980bc342b574`  
		Last Modified: Wed, 09 Mar 2022 23:22:13 GMT  
		Size: 349.0 KB (348988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3cf158dc37e43f4d84e520f088e32b2851abbf4a70af92161ab5e0d7e3ecbd`  
		Last Modified: Wed, 09 Mar 2022 23:22:20 GMT  
		Size: 7.5 MB (7516588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fff4072b17e75a66709617708b8b9263dabe4a12c4e0a594fb52e058977fa83`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de86f56dd22fbee61ed7161f763ba9de61d7cbf9623b85a879723ea5670f6e20`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04add3ff0ef25a1f32aab83f90a95cffab3d4b55afd3eb376a861b36094a0b0`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:112510afc4add9efb62621bbcbd4c03a62c4efa7bebfa2854d896a3b81b4822b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats-streaming@sha256:38aa3744b326ea3530932f9ae38c5884a7cc4f4e5e71b77f330b5634d79fa79a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723329559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5125257a9aa0beaab36a017e9f82750b3aac24f4719374d6cc8e339fc187cdd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 09 Mar 2022 23:18:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.3/nats-streaming-server-v0.24.3-windows-amd64.zip
# Wed, 09 Mar 2022 23:18:48 GMT
ENV NATS_STREAMING_SERVER_SHASUM=7473bfa7efd734ca6984907bc9586260031cca926883b468b4752557ecefaff0
# Wed, 09 Mar 2022 23:19:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:21:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:21:28 GMT
EXPOSE 4222 8222
# Wed, 09 Mar 2022 23:21:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Mar 2022 23:21:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1aac6ec834525c931dc81bbbb6d32996b82fd755a3bd625af11f40b8fc66bb`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d303e56675a80a6fa4eef8ef31d6f93742709f41058dcf6e36b8ba6d71a466f8`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8122e4b6aba607bd3d7b17a847d8ab75da7d7cb7a2bbb035e4a31cfc1b7ce6`  
		Last Modified: Wed, 09 Mar 2022 23:22:14 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393372fa0a20ba2589a43d177f33a0360245be974d231efaa7ab980bc342b574`  
		Last Modified: Wed, 09 Mar 2022 23:22:13 GMT  
		Size: 349.0 KB (348988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3cf158dc37e43f4d84e520f088e32b2851abbf4a70af92161ab5e0d7e3ecbd`  
		Last Modified: Wed, 09 Mar 2022 23:22:20 GMT  
		Size: 7.5 MB (7516588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fff4072b17e75a66709617708b8b9263dabe4a12c4e0a594fb52e058977fa83`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de86f56dd22fbee61ed7161f763ba9de61d7cbf9623b85a879723ea5670f6e20`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04add3ff0ef25a1f32aab83f90a95cffab3d4b55afd3eb376a861b36094a0b0`  
		Last Modified: Wed, 09 Mar 2022 23:22:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
