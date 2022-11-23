<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.16`](#nats2-alpine316)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.16`](#nats29-alpine316)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.8`](#nats298)
-	[`nats:2.9.8-alpine`](#nats298-alpine)
-	[`nats:2.9.8-alpine3.16`](#nats298-alpine316)
-	[`nats:2.9.8-linux`](#nats298-linux)
-	[`nats:2.9.8-nanoserver`](#nats298-nanoserver)
-	[`nats:2.9.8-nanoserver-1809`](#nats298-nanoserver-1809)
-	[`nats:2.9.8-scratch`](#nats298-scratch)
-	[`nats:2.9.8-windowsservercore`](#nats298-windowsservercore)
-	[`nats:2.9.8-windowsservercore-1809`](#nats298-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.16`](#natsalpine316)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:9b2c3b928d27250178e846061a0523ce812a5f6658bfe0d8f6e3ad6f388d03bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:406dffdd6635f552a4102d89dea2ec47c566a4a3c77a55f174cf7e01163cb935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:c002e5ffb5d05f4d9a26f7713c8c1fe5581901d8f0b8fa3bdf911f5288616710
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8015220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd6fa7a5464783fd1d94dd9177032bd784ebced509022517e078f79333fc8f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:31:32 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:31:35 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:31:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb18394b089809ec14ed5f1896559bbe7011596da8a8a6f514c7f045e3b230a4`  
		Last Modified: Tue, 22 Nov 2022 22:32:07 GMT  
		Size: 5.2 MB (5207950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a351d7adf5fb3b72145eccfb3a99fcdab4e78aad383467bf6bbfc9c60a8d291`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf572efeeb6d7d39f3cb0b6349fa17f9fadac11a3d8faf7d26f1804aacd24c0`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d69b4bc4b5546373c49e12433d97b51d075dadd4dda2ad065e70e2ea7a0a29d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a56e8dab16e0ce21626bdc17bdfabdbd0c0b4c422c2b35c66c4bf87e7eea5c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:58:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:58:32 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:58:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23a73061702a89b02b05f09a230c70a54be68b983232e3089b6341b1f2e24b`  
		Last Modified: Tue, 22 Nov 2022 22:59:47 GMT  
		Size: 5.0 MB (4970356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835dc901364b7df41a2758ac86a456b0198e9c684b9a23d47a65480066e3823a`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045c7ce14372b9d7f23f6620e4f58e1c49492e6acfc20f62680d7f34c7a0e1ef`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:841d2a7ead5c3d3153065d4d57a74824843eba32738c8983e3c5c49ad01d4cb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06e4bfed627d58668b88274e6983919e41bbe1a36b9783c8be726c7886cc721`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 23:07:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 23:07:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 23:07:31 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 23:07:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0406f69480e7e26ebedbcb2f03d5605e2031b167ee8c01189a4c8809603370d4`  
		Last Modified: Tue, 22 Nov 2022 23:08:48 GMT  
		Size: 5.0 MB (4961029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d92bd08d9c3dd7b7a3a2f822dc3e6f2f96c9ebb23a9997d2147d748b1581d3c`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b45cabfa3a1d3c72940738cc484227bd438f269f9734800c5c8e5e6dbab5412`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77a606603f5cfe5a2a8b68de95137357958dc0c807a4e55b634d79c187e96fc4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540ea1800ec43613e42f90ec14f3c0081d20dfb233611c49d193c76022c3ea53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:49:25 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:49:27 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:49:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ac60fca86e18ce46ed8ef28fb8ed256e6a880d4f81833c14825e6407fd1df4`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 4.8 MB (4794414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e36535bf8e34a143d001d45283522f30418a902037dd4212bc15b6d2b00436b`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c251ec8f3740fd168b0c3d843054011d76dfcd6cb4fcd99c0c151c5a81048967`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.16`

```console
$ docker pull nats@sha256:406dffdd6635f552a4102d89dea2ec47c566a4a3c77a55f174cf7e01163cb935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:c002e5ffb5d05f4d9a26f7713c8c1fe5581901d8f0b8fa3bdf911f5288616710
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8015220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd6fa7a5464783fd1d94dd9177032bd784ebced509022517e078f79333fc8f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:31:32 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:31:35 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:31:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb18394b089809ec14ed5f1896559bbe7011596da8a8a6f514c7f045e3b230a4`  
		Last Modified: Tue, 22 Nov 2022 22:32:07 GMT  
		Size: 5.2 MB (5207950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a351d7adf5fb3b72145eccfb3a99fcdab4e78aad383467bf6bbfc9c60a8d291`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf572efeeb6d7d39f3cb0b6349fa17f9fadac11a3d8faf7d26f1804aacd24c0`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:d69b4bc4b5546373c49e12433d97b51d075dadd4dda2ad065e70e2ea7a0a29d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a56e8dab16e0ce21626bdc17bdfabdbd0c0b4c422c2b35c66c4bf87e7eea5c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:58:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:58:32 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:58:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23a73061702a89b02b05f09a230c70a54be68b983232e3089b6341b1f2e24b`  
		Last Modified: Tue, 22 Nov 2022 22:59:47 GMT  
		Size: 5.0 MB (4970356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835dc901364b7df41a2758ac86a456b0198e9c684b9a23d47a65480066e3823a`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045c7ce14372b9d7f23f6620e4f58e1c49492e6acfc20f62680d7f34c7a0e1ef`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:841d2a7ead5c3d3153065d4d57a74824843eba32738c8983e3c5c49ad01d4cb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06e4bfed627d58668b88274e6983919e41bbe1a36b9783c8be726c7886cc721`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 23:07:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 23:07:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 23:07:31 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 23:07:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0406f69480e7e26ebedbcb2f03d5605e2031b167ee8c01189a4c8809603370d4`  
		Last Modified: Tue, 22 Nov 2022 23:08:48 GMT  
		Size: 5.0 MB (4961029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d92bd08d9c3dd7b7a3a2f822dc3e6f2f96c9ebb23a9997d2147d748b1581d3c`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b45cabfa3a1d3c72940738cc484227bd438f269f9734800c5c8e5e6dbab5412`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77a606603f5cfe5a2a8b68de95137357958dc0c807a4e55b634d79c187e96fc4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540ea1800ec43613e42f90ec14f3c0081d20dfb233611c49d193c76022c3ea53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:49:25 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:49:27 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:49:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ac60fca86e18ce46ed8ef28fb8ed256e6a880d4f81833c14825e6407fd1df4`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 4.8 MB (4794414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e36535bf8e34a143d001d45283522f30418a902037dd4212bc15b6d2b00436b`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c251ec8f3740fd168b0c3d843054011d76dfcd6cb4fcd99c0c151c5a81048967`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:25d19360fca54a4146ed9b23c0342b49268f432d6c14a07f8033093ef5f99e22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:7fb77cbb695d71bab663e04d7130c123261b7065b137acf18337e51d0c3098c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:7fb77cbb695d71bab663e04d7130c123261b7065b137acf18337e51d0c3098c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:25d19360fca54a4146ed9b23c0342b49268f432d6c14a07f8033093ef5f99e22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:a13494d3ae8424f9e8472ac512784ef38d22f83a12f52cfad4cf9ee307ae32b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:9e310b8793dffc1390547ff9dd7936f86e81f414392f9a80e0ef7565dd2827f1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15aff17cf4ba484d77c9dc9e11d5354dcde9c549f767baeb8ff1c97614ff4b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:14:31 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:14:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.8/nats-server-v2.9.8-windows-amd64.zip
# Tue, 22 Nov 2022 22:14:34 GMT
ENV NATS_SERVER_SHASUM=b54ada0a61221ad22ce54620655cbb46ea86b1480d25bb63af7161ac3d2ed8e6
# Tue, 22 Nov 2022 22:15:59 GMT
RUN Set-PSDebug -Trace 2
# Tue, 22 Nov 2022 22:17:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 22 Nov 2022 22:17:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:17:57 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:17:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:17:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01edd89b02b20acf3ef0b82fe6d68ee7857211fbfd2ce51b945a2524b04de9d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68618fa193e339baf22d599c372525026a22c68ea90e3b7f7018c16106ad13ba`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be0da56c170d13d53c7e73029f950d42bc1ed0da4700a5e0ff8feefe5fc8f3d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764865c4abdffb4b97742f9ce28ef9005e0f682a330b6757f1baafe347a5599`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 381.1 KB (381090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e135d366a40ec59c87956144f538f0602e356154070123f2c04e5acb040fdab`  
		Last Modified: Tue, 22 Nov 2022 22:18:52 GMT  
		Size: 5.3 MB (5333424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9328cfc6ec5d9c63f420ec1ef7652cd83d4de454aea257298642856543a2cb3a`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 2.0 KB (2002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b171fc4f6c88ea21d028fa578a7e0bc3bef6932abf5d76ee10bd58bcfc56fe`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9333daeeb8fb3e61f534caa0c15c18e1db75c22816963eb61026f49bdfdc76`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01e9ac2760597467c7e3e40ce9e2cecb50d6122cd85176963cd02159596ebf6`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:a13494d3ae8424f9e8472ac512784ef38d22f83a12f52cfad4cf9ee307ae32b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:9e310b8793dffc1390547ff9dd7936f86e81f414392f9a80e0ef7565dd2827f1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15aff17cf4ba484d77c9dc9e11d5354dcde9c549f767baeb8ff1c97614ff4b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:14:31 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:14:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.8/nats-server-v2.9.8-windows-amd64.zip
# Tue, 22 Nov 2022 22:14:34 GMT
ENV NATS_SERVER_SHASUM=b54ada0a61221ad22ce54620655cbb46ea86b1480d25bb63af7161ac3d2ed8e6
# Tue, 22 Nov 2022 22:15:59 GMT
RUN Set-PSDebug -Trace 2
# Tue, 22 Nov 2022 22:17:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 22 Nov 2022 22:17:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:17:57 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:17:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:17:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01edd89b02b20acf3ef0b82fe6d68ee7857211fbfd2ce51b945a2524b04de9d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68618fa193e339baf22d599c372525026a22c68ea90e3b7f7018c16106ad13ba`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be0da56c170d13d53c7e73029f950d42bc1ed0da4700a5e0ff8feefe5fc8f3d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764865c4abdffb4b97742f9ce28ef9005e0f682a330b6757f1baafe347a5599`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 381.1 KB (381090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e135d366a40ec59c87956144f538f0602e356154070123f2c04e5acb040fdab`  
		Last Modified: Tue, 22 Nov 2022 22:18:52 GMT  
		Size: 5.3 MB (5333424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9328cfc6ec5d9c63f420ec1ef7652cd83d4de454aea257298642856543a2cb3a`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 2.0 KB (2002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b171fc4f6c88ea21d028fa578a7e0bc3bef6932abf5d76ee10bd58bcfc56fe`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9333daeeb8fb3e61f534caa0c15c18e1db75c22816963eb61026f49bdfdc76`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01e9ac2760597467c7e3e40ce9e2cecb50d6122cd85176963cd02159596ebf6`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:9b2c3b928d27250178e846061a0523ce812a5f6658bfe0d8f6e3ad6f388d03bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:406dffdd6635f552a4102d89dea2ec47c566a4a3c77a55f174cf7e01163cb935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:c002e5ffb5d05f4d9a26f7713c8c1fe5581901d8f0b8fa3bdf911f5288616710
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8015220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd6fa7a5464783fd1d94dd9177032bd784ebced509022517e078f79333fc8f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:31:32 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:31:35 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:31:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb18394b089809ec14ed5f1896559bbe7011596da8a8a6f514c7f045e3b230a4`  
		Last Modified: Tue, 22 Nov 2022 22:32:07 GMT  
		Size: 5.2 MB (5207950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a351d7adf5fb3b72145eccfb3a99fcdab4e78aad383467bf6bbfc9c60a8d291`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf572efeeb6d7d39f3cb0b6349fa17f9fadac11a3d8faf7d26f1804aacd24c0`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d69b4bc4b5546373c49e12433d97b51d075dadd4dda2ad065e70e2ea7a0a29d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a56e8dab16e0ce21626bdc17bdfabdbd0c0b4c422c2b35c66c4bf87e7eea5c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:58:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:58:32 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:58:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23a73061702a89b02b05f09a230c70a54be68b983232e3089b6341b1f2e24b`  
		Last Modified: Tue, 22 Nov 2022 22:59:47 GMT  
		Size: 5.0 MB (4970356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835dc901364b7df41a2758ac86a456b0198e9c684b9a23d47a65480066e3823a`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045c7ce14372b9d7f23f6620e4f58e1c49492e6acfc20f62680d7f34c7a0e1ef`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:841d2a7ead5c3d3153065d4d57a74824843eba32738c8983e3c5c49ad01d4cb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06e4bfed627d58668b88274e6983919e41bbe1a36b9783c8be726c7886cc721`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 23:07:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 23:07:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 23:07:31 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 23:07:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0406f69480e7e26ebedbcb2f03d5605e2031b167ee8c01189a4c8809603370d4`  
		Last Modified: Tue, 22 Nov 2022 23:08:48 GMT  
		Size: 5.0 MB (4961029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d92bd08d9c3dd7b7a3a2f822dc3e6f2f96c9ebb23a9997d2147d748b1581d3c`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b45cabfa3a1d3c72940738cc484227bd438f269f9734800c5c8e5e6dbab5412`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77a606603f5cfe5a2a8b68de95137357958dc0c807a4e55b634d79c187e96fc4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540ea1800ec43613e42f90ec14f3c0081d20dfb233611c49d193c76022c3ea53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:49:25 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:49:27 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:49:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ac60fca86e18ce46ed8ef28fb8ed256e6a880d4f81833c14825e6407fd1df4`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 4.8 MB (4794414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e36535bf8e34a143d001d45283522f30418a902037dd4212bc15b6d2b00436b`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c251ec8f3740fd168b0c3d843054011d76dfcd6cb4fcd99c0c151c5a81048967`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.16`

```console
$ docker pull nats@sha256:406dffdd6635f552a4102d89dea2ec47c566a4a3c77a55f174cf7e01163cb935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:c002e5ffb5d05f4d9a26f7713c8c1fe5581901d8f0b8fa3bdf911f5288616710
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8015220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd6fa7a5464783fd1d94dd9177032bd784ebced509022517e078f79333fc8f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:31:32 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:31:35 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:31:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb18394b089809ec14ed5f1896559bbe7011596da8a8a6f514c7f045e3b230a4`  
		Last Modified: Tue, 22 Nov 2022 22:32:07 GMT  
		Size: 5.2 MB (5207950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a351d7adf5fb3b72145eccfb3a99fcdab4e78aad383467bf6bbfc9c60a8d291`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf572efeeb6d7d39f3cb0b6349fa17f9fadac11a3d8faf7d26f1804aacd24c0`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:d69b4bc4b5546373c49e12433d97b51d075dadd4dda2ad065e70e2ea7a0a29d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a56e8dab16e0ce21626bdc17bdfabdbd0c0b4c422c2b35c66c4bf87e7eea5c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:58:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:58:32 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:58:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23a73061702a89b02b05f09a230c70a54be68b983232e3089b6341b1f2e24b`  
		Last Modified: Tue, 22 Nov 2022 22:59:47 GMT  
		Size: 5.0 MB (4970356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835dc901364b7df41a2758ac86a456b0198e9c684b9a23d47a65480066e3823a`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045c7ce14372b9d7f23f6620e4f58e1c49492e6acfc20f62680d7f34c7a0e1ef`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:841d2a7ead5c3d3153065d4d57a74824843eba32738c8983e3c5c49ad01d4cb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06e4bfed627d58668b88274e6983919e41bbe1a36b9783c8be726c7886cc721`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 23:07:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 23:07:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 23:07:31 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 23:07:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0406f69480e7e26ebedbcb2f03d5605e2031b167ee8c01189a4c8809603370d4`  
		Last Modified: Tue, 22 Nov 2022 23:08:48 GMT  
		Size: 5.0 MB (4961029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d92bd08d9c3dd7b7a3a2f822dc3e6f2f96c9ebb23a9997d2147d748b1581d3c`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b45cabfa3a1d3c72940738cc484227bd438f269f9734800c5c8e5e6dbab5412`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77a606603f5cfe5a2a8b68de95137357958dc0c807a4e55b634d79c187e96fc4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540ea1800ec43613e42f90ec14f3c0081d20dfb233611c49d193c76022c3ea53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:49:25 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:49:27 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:49:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ac60fca86e18ce46ed8ef28fb8ed256e6a880d4f81833c14825e6407fd1df4`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 4.8 MB (4794414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e36535bf8e34a143d001d45283522f30418a902037dd4212bc15b6d2b00436b`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c251ec8f3740fd168b0c3d843054011d76dfcd6cb4fcd99c0c151c5a81048967`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:25d19360fca54a4146ed9b23c0342b49268f432d6c14a07f8033093ef5f99e22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:7fb77cbb695d71bab663e04d7130c123261b7065b137acf18337e51d0c3098c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:7fb77cbb695d71bab663e04d7130c123261b7065b137acf18337e51d0c3098c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:25d19360fca54a4146ed9b23c0342b49268f432d6c14a07f8033093ef5f99e22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:a13494d3ae8424f9e8472ac512784ef38d22f83a12f52cfad4cf9ee307ae32b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:9e310b8793dffc1390547ff9dd7936f86e81f414392f9a80e0ef7565dd2827f1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15aff17cf4ba484d77c9dc9e11d5354dcde9c549f767baeb8ff1c97614ff4b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:14:31 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:14:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.8/nats-server-v2.9.8-windows-amd64.zip
# Tue, 22 Nov 2022 22:14:34 GMT
ENV NATS_SERVER_SHASUM=b54ada0a61221ad22ce54620655cbb46ea86b1480d25bb63af7161ac3d2ed8e6
# Tue, 22 Nov 2022 22:15:59 GMT
RUN Set-PSDebug -Trace 2
# Tue, 22 Nov 2022 22:17:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 22 Nov 2022 22:17:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:17:57 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:17:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:17:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01edd89b02b20acf3ef0b82fe6d68ee7857211fbfd2ce51b945a2524b04de9d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68618fa193e339baf22d599c372525026a22c68ea90e3b7f7018c16106ad13ba`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be0da56c170d13d53c7e73029f950d42bc1ed0da4700a5e0ff8feefe5fc8f3d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764865c4abdffb4b97742f9ce28ef9005e0f682a330b6757f1baafe347a5599`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 381.1 KB (381090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e135d366a40ec59c87956144f538f0602e356154070123f2c04e5acb040fdab`  
		Last Modified: Tue, 22 Nov 2022 22:18:52 GMT  
		Size: 5.3 MB (5333424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9328cfc6ec5d9c63f420ec1ef7652cd83d4de454aea257298642856543a2cb3a`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 2.0 KB (2002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b171fc4f6c88ea21d028fa578a7e0bc3bef6932abf5d76ee10bd58bcfc56fe`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9333daeeb8fb3e61f534caa0c15c18e1db75c22816963eb61026f49bdfdc76`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01e9ac2760597467c7e3e40ce9e2cecb50d6122cd85176963cd02159596ebf6`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:a13494d3ae8424f9e8472ac512784ef38d22f83a12f52cfad4cf9ee307ae32b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:9e310b8793dffc1390547ff9dd7936f86e81f414392f9a80e0ef7565dd2827f1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15aff17cf4ba484d77c9dc9e11d5354dcde9c549f767baeb8ff1c97614ff4b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:14:31 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:14:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.8/nats-server-v2.9.8-windows-amd64.zip
# Tue, 22 Nov 2022 22:14:34 GMT
ENV NATS_SERVER_SHASUM=b54ada0a61221ad22ce54620655cbb46ea86b1480d25bb63af7161ac3d2ed8e6
# Tue, 22 Nov 2022 22:15:59 GMT
RUN Set-PSDebug -Trace 2
# Tue, 22 Nov 2022 22:17:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 22 Nov 2022 22:17:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:17:57 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:17:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:17:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01edd89b02b20acf3ef0b82fe6d68ee7857211fbfd2ce51b945a2524b04de9d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68618fa193e339baf22d599c372525026a22c68ea90e3b7f7018c16106ad13ba`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be0da56c170d13d53c7e73029f950d42bc1ed0da4700a5e0ff8feefe5fc8f3d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764865c4abdffb4b97742f9ce28ef9005e0f682a330b6757f1baafe347a5599`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 381.1 KB (381090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e135d366a40ec59c87956144f538f0602e356154070123f2c04e5acb040fdab`  
		Last Modified: Tue, 22 Nov 2022 22:18:52 GMT  
		Size: 5.3 MB (5333424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9328cfc6ec5d9c63f420ec1ef7652cd83d4de454aea257298642856543a2cb3a`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 2.0 KB (2002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b171fc4f6c88ea21d028fa578a7e0bc3bef6932abf5d76ee10bd58bcfc56fe`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9333daeeb8fb3e61f534caa0c15c18e1db75c22816963eb61026f49bdfdc76`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01e9ac2760597467c7e3e40ce9e2cecb50d6122cd85176963cd02159596ebf6`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.8`

```console
$ docker pull nats@sha256:9b2c3b928d27250178e846061a0523ce812a5f6658bfe0d8f6e3ad6f388d03bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.8` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.8-alpine`

```console
$ docker pull nats@sha256:406dffdd6635f552a4102d89dea2ec47c566a4a3c77a55f174cf7e01163cb935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.8-alpine` - linux; amd64

```console
$ docker pull nats@sha256:c002e5ffb5d05f4d9a26f7713c8c1fe5581901d8f0b8fa3bdf911f5288616710
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8015220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd6fa7a5464783fd1d94dd9177032bd784ebced509022517e078f79333fc8f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:31:32 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:31:35 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:31:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb18394b089809ec14ed5f1896559bbe7011596da8a8a6f514c7f045e3b230a4`  
		Last Modified: Tue, 22 Nov 2022 22:32:07 GMT  
		Size: 5.2 MB (5207950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a351d7adf5fb3b72145eccfb3a99fcdab4e78aad383467bf6bbfc9c60a8d291`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf572efeeb6d7d39f3cb0b6349fa17f9fadac11a3d8faf7d26f1804aacd24c0`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d69b4bc4b5546373c49e12433d97b51d075dadd4dda2ad065e70e2ea7a0a29d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a56e8dab16e0ce21626bdc17bdfabdbd0c0b4c422c2b35c66c4bf87e7eea5c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:58:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:58:32 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:58:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23a73061702a89b02b05f09a230c70a54be68b983232e3089b6341b1f2e24b`  
		Last Modified: Tue, 22 Nov 2022 22:59:47 GMT  
		Size: 5.0 MB (4970356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835dc901364b7df41a2758ac86a456b0198e9c684b9a23d47a65480066e3823a`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045c7ce14372b9d7f23f6620e4f58e1c49492e6acfc20f62680d7f34c7a0e1ef`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:841d2a7ead5c3d3153065d4d57a74824843eba32738c8983e3c5c49ad01d4cb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06e4bfed627d58668b88274e6983919e41bbe1a36b9783c8be726c7886cc721`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 23:07:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 23:07:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 23:07:31 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 23:07:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0406f69480e7e26ebedbcb2f03d5605e2031b167ee8c01189a4c8809603370d4`  
		Last Modified: Tue, 22 Nov 2022 23:08:48 GMT  
		Size: 5.0 MB (4961029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d92bd08d9c3dd7b7a3a2f822dc3e6f2f96c9ebb23a9997d2147d748b1581d3c`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b45cabfa3a1d3c72940738cc484227bd438f269f9734800c5c8e5e6dbab5412`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77a606603f5cfe5a2a8b68de95137357958dc0c807a4e55b634d79c187e96fc4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540ea1800ec43613e42f90ec14f3c0081d20dfb233611c49d193c76022c3ea53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:49:25 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:49:27 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:49:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ac60fca86e18ce46ed8ef28fb8ed256e6a880d4f81833c14825e6407fd1df4`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 4.8 MB (4794414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e36535bf8e34a143d001d45283522f30418a902037dd4212bc15b6d2b00436b`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c251ec8f3740fd168b0c3d843054011d76dfcd6cb4fcd99c0c151c5a81048967`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.8-alpine3.16`

```console
$ docker pull nats@sha256:406dffdd6635f552a4102d89dea2ec47c566a4a3c77a55f174cf7e01163cb935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.8-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:c002e5ffb5d05f4d9a26f7713c8c1fe5581901d8f0b8fa3bdf911f5288616710
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8015220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd6fa7a5464783fd1d94dd9177032bd784ebced509022517e078f79333fc8f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:31:32 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:31:35 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:31:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb18394b089809ec14ed5f1896559bbe7011596da8a8a6f514c7f045e3b230a4`  
		Last Modified: Tue, 22 Nov 2022 22:32:07 GMT  
		Size: 5.2 MB (5207950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a351d7adf5fb3b72145eccfb3a99fcdab4e78aad383467bf6bbfc9c60a8d291`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf572efeeb6d7d39f3cb0b6349fa17f9fadac11a3d8faf7d26f1804aacd24c0`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:d69b4bc4b5546373c49e12433d97b51d075dadd4dda2ad065e70e2ea7a0a29d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a56e8dab16e0ce21626bdc17bdfabdbd0c0b4c422c2b35c66c4bf87e7eea5c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:58:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:58:32 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:58:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23a73061702a89b02b05f09a230c70a54be68b983232e3089b6341b1f2e24b`  
		Last Modified: Tue, 22 Nov 2022 22:59:47 GMT  
		Size: 5.0 MB (4970356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835dc901364b7df41a2758ac86a456b0198e9c684b9a23d47a65480066e3823a`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045c7ce14372b9d7f23f6620e4f58e1c49492e6acfc20f62680d7f34c7a0e1ef`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:841d2a7ead5c3d3153065d4d57a74824843eba32738c8983e3c5c49ad01d4cb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06e4bfed627d58668b88274e6983919e41bbe1a36b9783c8be726c7886cc721`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 23:07:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 23:07:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 23:07:31 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 23:07:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0406f69480e7e26ebedbcb2f03d5605e2031b167ee8c01189a4c8809603370d4`  
		Last Modified: Tue, 22 Nov 2022 23:08:48 GMT  
		Size: 5.0 MB (4961029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d92bd08d9c3dd7b7a3a2f822dc3e6f2f96c9ebb23a9997d2147d748b1581d3c`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b45cabfa3a1d3c72940738cc484227bd438f269f9734800c5c8e5e6dbab5412`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77a606603f5cfe5a2a8b68de95137357958dc0c807a4e55b634d79c187e96fc4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540ea1800ec43613e42f90ec14f3c0081d20dfb233611c49d193c76022c3ea53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:49:25 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:49:27 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:49:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ac60fca86e18ce46ed8ef28fb8ed256e6a880d4f81833c14825e6407fd1df4`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 4.8 MB (4794414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e36535bf8e34a143d001d45283522f30418a902037dd4212bc15b6d2b00436b`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c251ec8f3740fd168b0c3d843054011d76dfcd6cb4fcd99c0c151c5a81048967`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.8-linux`

```console
$ docker pull nats@sha256:25d19360fca54a4146ed9b23c0342b49268f432d6c14a07f8033093ef5f99e22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.8-linux` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.8-nanoserver`

```console
$ docker pull nats@sha256:7fb77cbb695d71bab663e04d7130c123261b7065b137acf18337e51d0c3098c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.8-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.8-nanoserver-1809`

```console
$ docker pull nats@sha256:7fb77cbb695d71bab663e04d7130c123261b7065b137acf18337e51d0c3098c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.8-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.8-scratch`

```console
$ docker pull nats@sha256:25d19360fca54a4146ed9b23c0342b49268f432d6c14a07f8033093ef5f99e22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.8-scratch` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.8-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.8-windowsservercore`

```console
$ docker pull nats@sha256:a13494d3ae8424f9e8472ac512784ef38d22f83a12f52cfad4cf9ee307ae32b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.8-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:9e310b8793dffc1390547ff9dd7936f86e81f414392f9a80e0ef7565dd2827f1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15aff17cf4ba484d77c9dc9e11d5354dcde9c549f767baeb8ff1c97614ff4b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:14:31 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:14:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.8/nats-server-v2.9.8-windows-amd64.zip
# Tue, 22 Nov 2022 22:14:34 GMT
ENV NATS_SERVER_SHASUM=b54ada0a61221ad22ce54620655cbb46ea86b1480d25bb63af7161ac3d2ed8e6
# Tue, 22 Nov 2022 22:15:59 GMT
RUN Set-PSDebug -Trace 2
# Tue, 22 Nov 2022 22:17:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 22 Nov 2022 22:17:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:17:57 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:17:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:17:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01edd89b02b20acf3ef0b82fe6d68ee7857211fbfd2ce51b945a2524b04de9d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68618fa193e339baf22d599c372525026a22c68ea90e3b7f7018c16106ad13ba`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be0da56c170d13d53c7e73029f950d42bc1ed0da4700a5e0ff8feefe5fc8f3d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764865c4abdffb4b97742f9ce28ef9005e0f682a330b6757f1baafe347a5599`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 381.1 KB (381090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e135d366a40ec59c87956144f538f0602e356154070123f2c04e5acb040fdab`  
		Last Modified: Tue, 22 Nov 2022 22:18:52 GMT  
		Size: 5.3 MB (5333424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9328cfc6ec5d9c63f420ec1ef7652cd83d4de454aea257298642856543a2cb3a`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 2.0 KB (2002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b171fc4f6c88ea21d028fa578a7e0bc3bef6932abf5d76ee10bd58bcfc56fe`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9333daeeb8fb3e61f534caa0c15c18e1db75c22816963eb61026f49bdfdc76`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01e9ac2760597467c7e3e40ce9e2cecb50d6122cd85176963cd02159596ebf6`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.8-windowsservercore-1809`

```console
$ docker pull nats@sha256:a13494d3ae8424f9e8472ac512784ef38d22f83a12f52cfad4cf9ee307ae32b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.8-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:9e310b8793dffc1390547ff9dd7936f86e81f414392f9a80e0ef7565dd2827f1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15aff17cf4ba484d77c9dc9e11d5354dcde9c549f767baeb8ff1c97614ff4b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:14:31 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:14:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.8/nats-server-v2.9.8-windows-amd64.zip
# Tue, 22 Nov 2022 22:14:34 GMT
ENV NATS_SERVER_SHASUM=b54ada0a61221ad22ce54620655cbb46ea86b1480d25bb63af7161ac3d2ed8e6
# Tue, 22 Nov 2022 22:15:59 GMT
RUN Set-PSDebug -Trace 2
# Tue, 22 Nov 2022 22:17:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 22 Nov 2022 22:17:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:17:57 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:17:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:17:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01edd89b02b20acf3ef0b82fe6d68ee7857211fbfd2ce51b945a2524b04de9d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68618fa193e339baf22d599c372525026a22c68ea90e3b7f7018c16106ad13ba`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be0da56c170d13d53c7e73029f950d42bc1ed0da4700a5e0ff8feefe5fc8f3d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764865c4abdffb4b97742f9ce28ef9005e0f682a330b6757f1baafe347a5599`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 381.1 KB (381090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e135d366a40ec59c87956144f538f0602e356154070123f2c04e5acb040fdab`  
		Last Modified: Tue, 22 Nov 2022 22:18:52 GMT  
		Size: 5.3 MB (5333424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9328cfc6ec5d9c63f420ec1ef7652cd83d4de454aea257298642856543a2cb3a`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 2.0 KB (2002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b171fc4f6c88ea21d028fa578a7e0bc3bef6932abf5d76ee10bd58bcfc56fe`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9333daeeb8fb3e61f534caa0c15c18e1db75c22816963eb61026f49bdfdc76`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01e9ac2760597467c7e3e40ce9e2cecb50d6122cd85176963cd02159596ebf6`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:406dffdd6635f552a4102d89dea2ec47c566a4a3c77a55f174cf7e01163cb935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:c002e5ffb5d05f4d9a26f7713c8c1fe5581901d8f0b8fa3bdf911f5288616710
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8015220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd6fa7a5464783fd1d94dd9177032bd784ebced509022517e078f79333fc8f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:31:32 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:31:35 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:31:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb18394b089809ec14ed5f1896559bbe7011596da8a8a6f514c7f045e3b230a4`  
		Last Modified: Tue, 22 Nov 2022 22:32:07 GMT  
		Size: 5.2 MB (5207950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a351d7adf5fb3b72145eccfb3a99fcdab4e78aad383467bf6bbfc9c60a8d291`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf572efeeb6d7d39f3cb0b6349fa17f9fadac11a3d8faf7d26f1804aacd24c0`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d69b4bc4b5546373c49e12433d97b51d075dadd4dda2ad065e70e2ea7a0a29d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a56e8dab16e0ce21626bdc17bdfabdbd0c0b4c422c2b35c66c4bf87e7eea5c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:58:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:58:32 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:58:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23a73061702a89b02b05f09a230c70a54be68b983232e3089b6341b1f2e24b`  
		Last Modified: Tue, 22 Nov 2022 22:59:47 GMT  
		Size: 5.0 MB (4970356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835dc901364b7df41a2758ac86a456b0198e9c684b9a23d47a65480066e3823a`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045c7ce14372b9d7f23f6620e4f58e1c49492e6acfc20f62680d7f34c7a0e1ef`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:841d2a7ead5c3d3153065d4d57a74824843eba32738c8983e3c5c49ad01d4cb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06e4bfed627d58668b88274e6983919e41bbe1a36b9783c8be726c7886cc721`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 23:07:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 23:07:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 23:07:31 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 23:07:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0406f69480e7e26ebedbcb2f03d5605e2031b167ee8c01189a4c8809603370d4`  
		Last Modified: Tue, 22 Nov 2022 23:08:48 GMT  
		Size: 5.0 MB (4961029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d92bd08d9c3dd7b7a3a2f822dc3e6f2f96c9ebb23a9997d2147d748b1581d3c`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b45cabfa3a1d3c72940738cc484227bd438f269f9734800c5c8e5e6dbab5412`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77a606603f5cfe5a2a8b68de95137357958dc0c807a4e55b634d79c187e96fc4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540ea1800ec43613e42f90ec14f3c0081d20dfb233611c49d193c76022c3ea53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:49:25 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:49:27 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:49:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ac60fca86e18ce46ed8ef28fb8ed256e6a880d4f81833c14825e6407fd1df4`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 4.8 MB (4794414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e36535bf8e34a143d001d45283522f30418a902037dd4212bc15b6d2b00436b`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c251ec8f3740fd168b0c3d843054011d76dfcd6cb4fcd99c0c151c5a81048967`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.16`

```console
$ docker pull nats@sha256:406dffdd6635f552a4102d89dea2ec47c566a4a3c77a55f174cf7e01163cb935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:c002e5ffb5d05f4d9a26f7713c8c1fe5581901d8f0b8fa3bdf911f5288616710
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8015220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd6fa7a5464783fd1d94dd9177032bd784ebced509022517e078f79333fc8f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:31:32 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:31:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:31:35 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:31:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb18394b089809ec14ed5f1896559bbe7011596da8a8a6f514c7f045e3b230a4`  
		Last Modified: Tue, 22 Nov 2022 22:32:07 GMT  
		Size: 5.2 MB (5207950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a351d7adf5fb3b72145eccfb3a99fcdab4e78aad383467bf6bbfc9c60a8d291`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf572efeeb6d7d39f3cb0b6349fa17f9fadac11a3d8faf7d26f1804aacd24c0`  
		Last Modified: Tue, 22 Nov 2022 22:32:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:d69b4bc4b5546373c49e12433d97b51d075dadd4dda2ad065e70e2ea7a0a29d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a56e8dab16e0ce21626bdc17bdfabdbd0c0b4c422c2b35c66c4bf87e7eea5c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:58:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:58:32 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:58:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23a73061702a89b02b05f09a230c70a54be68b983232e3089b6341b1f2e24b`  
		Last Modified: Tue, 22 Nov 2022 22:59:47 GMT  
		Size: 5.0 MB (4970356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835dc901364b7df41a2758ac86a456b0198e9c684b9a23d47a65480066e3823a`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045c7ce14372b9d7f23f6620e4f58e1c49492e6acfc20f62680d7f34c7a0e1ef`  
		Last Modified: Tue, 22 Nov 2022 22:59:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:841d2a7ead5c3d3153065d4d57a74824843eba32738c8983e3c5c49ad01d4cb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06e4bfed627d58668b88274e6983919e41bbe1a36b9783c8be726c7886cc721`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 23:07:28 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 23:07:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 23:07:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 23:07:31 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 23:07:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0406f69480e7e26ebedbcb2f03d5605e2031b167ee8c01189a4c8809603370d4`  
		Last Modified: Tue, 22 Nov 2022 23:08:48 GMT  
		Size: 5.0 MB (4961029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d92bd08d9c3dd7b7a3a2f822dc3e6f2f96c9ebb23a9997d2147d748b1581d3c`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b45cabfa3a1d3c72940738cc484227bd438f269f9734800c5c8e5e6dbab5412`  
		Last Modified: Tue, 22 Nov 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77a606603f5cfe5a2a8b68de95137357958dc0c807a4e55b634d79c187e96fc4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540ea1800ec43613e42f90ec14f3c0081d20dfb233611c49d193c76022c3ea53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Tue, 22 Nov 2022 22:49:25 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0d5ed2d72a3b294519ebd9aa109b4a6dde8f6782b080119b074a18e91230475a' ;; 		armhf) natsArch='arm6'; sha256='254c5d3dc48a462ed98fca8903977d4adf07c2ac53032fc8308a65666e90e482' ;; 		armv7) natsArch='arm7'; sha256='5caf555fece68e05d4e93cb128bba8383a24239f6caa45d9b3c7448586b10d29' ;; 		x86_64) natsArch='amd64'; sha256='0f60fe5abfaad53f96eb0f92fbd787bd721255ce67fa8aff3b6a1bf06c85a571' ;; 		x86) natsArch='386'; sha256='37618b46dee7730f233ebc88314e0ac0d387a44da079b5b6394ac817280904a9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 22 Nov 2022 22:49:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 22 Nov 2022 22:49:27 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 22 Nov 2022 22:49:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ac60fca86e18ce46ed8ef28fb8ed256e6a880d4f81833c14825e6407fd1df4`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 4.8 MB (4794414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e36535bf8e34a143d001d45283522f30418a902037dd4212bc15b6d2b00436b`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c251ec8f3740fd168b0c3d843054011d76dfcd6cb4fcd99c0c151c5a81048967`  
		Last Modified: Tue, 22 Nov 2022 22:49:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:9b2c3b928d27250178e846061a0523ce812a5f6658bfe0d8f6e3ad6f388d03bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:25d19360fca54a4146ed9b23c0342b49268f432d6c14a07f8033093ef5f99e22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:7fb77cbb695d71bab663e04d7130c123261b7065b137acf18337e51d0c3098c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:7fb77cbb695d71bab663e04d7130c123261b7065b137acf18337e51d0c3098c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:6b1ff542f9fb4d4b04c96134ed0b1d3182de7cc10771ae93eb8e9cd0026653ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555ae056add88958242b95b50304f6a3ca63354ee793cf4816e522223aff3e03`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:eac6c557838e3e812dc2543f44419eb09e736e014d4fd11024290109e8c1b7c6 in C:\nats-server.exe 
# Tue, 22 Nov 2022 22:18:15 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:18:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0c576d669473b6031dbd52dbfa3697e15df712ddb0b777839009d7213765cb`  
		Last Modified: Tue, 22 Nov 2022 22:19:08 GMT  
		Size: 5.0 MB (4974459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560ff1a6446d5eb02ac4a97069302d9ea27cd774fef66976e43f7d0547bd4f08`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9328f3f99c1115ef08332de8b3476b19c32a1e4b83617fa24a4d9282ab00cf`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ff06f95d61e730590287dee37be6cca689efa50e090e6b483469999653824`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155090c95372447edf0d41ecc014bcb306cef47ef3ddc88714b85c71b24cefa`  
		Last Modified: Tue, 22 Nov 2022 22:19:07 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:25d19360fca54a4146ed9b23c0342b49268f432d6c14a07f8033093ef5f99e22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:68eaddebed013b7050c97b15e75610810dd1ccc4da61e5e4b7f6c1deb7212762
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4919076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba92d67534631043cab89898de0c5d3109c54280ed68a45eaffa8065b909215`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:8d8471f3d0a5ad1e09a2d3bf4f10acd1cf96217322c844e58cdc0a28cfd9ba1b in /nats-server 
# Tue, 22 Nov 2022 22:31:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:31:43 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:31:43 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:31:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d928bc8a30b5ebcb6137cb16aa7072441d3097f07996d86a36a25646201be301`  
		Last Modified: Tue, 22 Nov 2022 22:32:27 GMT  
		Size: 4.9 MB (4918568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcc9cb7dd625d54245d6f042addc9a71a220b27605434b3dedbbce7a4a8b0`  
		Last Modified: Tue, 22 Nov 2022 22:32:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:d012ef66af5ee8140a8a9bc7392313f967bef63df61bc0b92386df3c2bad245a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3779ec3b12b239e250ce8dfa61431ffd22e2a87348d4e096ae9996dc35330d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:58:43 GMT
COPY file:4c7f2f362fd9c0413a9cd227b099a50cfdfeb0339861704cf576f99e7d3e5a53 in /nats-server 
# Tue, 22 Nov 2022 22:58:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:58:44 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:58:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:58:44 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:58:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4c2fef11c8ea15358b5db3041d2b3319c91d75bf9f37c556e752f7ca734e2403`  
		Last Modified: Tue, 22 Nov 2022 23:00:17 GMT  
		Size: 4.7 MB (4682567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d5ad81ab7306b215de72b52058f6e0c25609447e0e754a92aeda4b33678a1c`  
		Last Modified: Tue, 22 Nov 2022 23:00:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:7a95ae636accc6d954364f2620eb3eaa00f476f7a5fcd10cdf7588bc2a5a90d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bb5aae4be9db765115a5493fdd75194cf5813734cc23f848888341801755cc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:4b4a104415c133f8897a95fa42e51ef148fcac45bf008ebb9ea755f725205884 in /nats-server 
# Tue, 22 Nov 2022 23:07:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 23:07:45 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 23:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 23:07:45 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 23:07:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b2b020ee68b6a94e937c4f20581b6ea99a0f0f7c1cee00c0b34727ac50f216db`  
		Last Modified: Tue, 22 Nov 2022 23:09:17 GMT  
		Size: 4.7 MB (4679329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a78a8f4fbe7f308d94d667119ee32694c6bd5f120e182f62f5c5d8f640fc1a`  
		Last Modified: Tue, 22 Nov 2022 23:09:16 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ded04b234d56b1af1c88b73d4052329af8383f5672592552f549357bf91f727e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926324805d1b170c5fe748c5d2464474dc1c660ae18a0336664d8d2bb4bd288`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:d7d85e3bd57fcfc5a244a6ba925eca81e5e6c5f943dc60a416971e267d0bba56 in /nats-server 
# Tue, 22 Nov 2022 22:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 22 Nov 2022 22:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 22 Nov 2022 22:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 22 Nov 2022 22:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f56876685432debe60285d8955aea82f523203ffbed50e1b56e4bc38d5980c03`  
		Last Modified: Tue, 22 Nov 2022 22:50:20 GMT  
		Size: 4.5 MB (4503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7341caf2a309863694c27d5e511f50146f5cfbb8dfbcabff6ffff2073e25d42a`  
		Last Modified: Tue, 22 Nov 2022 22:50:19 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:a13494d3ae8424f9e8472ac512784ef38d22f83a12f52cfad4cf9ee307ae32b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:9e310b8793dffc1390547ff9dd7936f86e81f414392f9a80e0ef7565dd2827f1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15aff17cf4ba484d77c9dc9e11d5354dcde9c549f767baeb8ff1c97614ff4b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:14:31 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:14:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.8/nats-server-v2.9.8-windows-amd64.zip
# Tue, 22 Nov 2022 22:14:34 GMT
ENV NATS_SERVER_SHASUM=b54ada0a61221ad22ce54620655cbb46ea86b1480d25bb63af7161ac3d2ed8e6
# Tue, 22 Nov 2022 22:15:59 GMT
RUN Set-PSDebug -Trace 2
# Tue, 22 Nov 2022 22:17:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 22 Nov 2022 22:17:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:17:57 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:17:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:17:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01edd89b02b20acf3ef0b82fe6d68ee7857211fbfd2ce51b945a2524b04de9d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68618fa193e339baf22d599c372525026a22c68ea90e3b7f7018c16106ad13ba`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be0da56c170d13d53c7e73029f950d42bc1ed0da4700a5e0ff8feefe5fc8f3d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764865c4abdffb4b97742f9ce28ef9005e0f682a330b6757f1baafe347a5599`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 381.1 KB (381090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e135d366a40ec59c87956144f538f0602e356154070123f2c04e5acb040fdab`  
		Last Modified: Tue, 22 Nov 2022 22:18:52 GMT  
		Size: 5.3 MB (5333424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9328cfc6ec5d9c63f420ec1ef7652cd83d4de454aea257298642856543a2cb3a`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 2.0 KB (2002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b171fc4f6c88ea21d028fa578a7e0bc3bef6932abf5d76ee10bd58bcfc56fe`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9333daeeb8fb3e61f534caa0c15c18e1db75c22816963eb61026f49bdfdc76`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01e9ac2760597467c7e3e40ce9e2cecb50d6122cd85176963cd02159596ebf6`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:a13494d3ae8424f9e8472ac512784ef38d22f83a12f52cfad4cf9ee307ae32b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:9e310b8793dffc1390547ff9dd7936f86e81f414392f9a80e0ef7565dd2827f1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15aff17cf4ba484d77c9dc9e11d5354dcde9c549f767baeb8ff1c97614ff4b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Tue, 22 Nov 2022 22:14:31 GMT
ENV NATS_SERVER=2.9.8
# Tue, 22 Nov 2022 22:14:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.8/nats-server-v2.9.8-windows-amd64.zip
# Tue, 22 Nov 2022 22:14:34 GMT
ENV NATS_SERVER_SHASUM=b54ada0a61221ad22ce54620655cbb46ea86b1480d25bb63af7161ac3d2ed8e6
# Tue, 22 Nov 2022 22:15:59 GMT
RUN Set-PSDebug -Trace 2
# Tue, 22 Nov 2022 22:17:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 22 Nov 2022 22:17:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 22 Nov 2022 22:17:57 GMT
EXPOSE 4222 6222 8222
# Tue, 22 Nov 2022 22:17:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 22 Nov 2022 22:17:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01edd89b02b20acf3ef0b82fe6d68ee7857211fbfd2ce51b945a2524b04de9d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68618fa193e339baf22d599c372525026a22c68ea90e3b7f7018c16106ad13ba`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be0da56c170d13d53c7e73029f950d42bc1ed0da4700a5e0ff8feefe5fc8f3d`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764865c4abdffb4b97742f9ce28ef9005e0f682a330b6757f1baafe347a5599`  
		Last Modified: Tue, 22 Nov 2022 22:18:53 GMT  
		Size: 381.1 KB (381090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e135d366a40ec59c87956144f538f0602e356154070123f2c04e5acb040fdab`  
		Last Modified: Tue, 22 Nov 2022 22:18:52 GMT  
		Size: 5.3 MB (5333424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9328cfc6ec5d9c63f420ec1ef7652cd83d4de454aea257298642856543a2cb3a`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 2.0 KB (2002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b171fc4f6c88ea21d028fa578a7e0bc3bef6932abf5d76ee10bd58bcfc56fe`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9333daeeb8fb3e61f534caa0c15c18e1db75c22816963eb61026f49bdfdc76`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01e9ac2760597467c7e3e40ce9e2cecb50d6122cd85176963cd02159596ebf6`  
		Last Modified: Tue, 22 Nov 2022 22:18:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
