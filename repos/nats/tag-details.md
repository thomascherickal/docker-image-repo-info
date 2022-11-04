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
-	[`nats:2.9.6`](#nats296)
-	[`nats:2.9.6-alpine`](#nats296-alpine)
-	[`nats:2.9.6-alpine3.16`](#nats296-alpine316)
-	[`nats:2.9.6-linux`](#nats296-linux)
-	[`nats:2.9.6-nanoserver`](#nats296-nanoserver)
-	[`nats:2.9.6-nanoserver-1809`](#nats296-nanoserver-1809)
-	[`nats:2.9.6-scratch`](#nats296-scratch)
-	[`nats:2.9.6-windowsservercore`](#nats296-windowsservercore)
-	[`nats:2.9.6-windowsservercore-1809`](#nats296-windowsservercore-1809)
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
$ docker pull nats@sha256:38cf02118dd5f875345011c712c01b337d93d6ba53ad405e554071971ddc96aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3532; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:93861bcaeec03b3ea77060e14e384d56bf43a20406a131547f741c9fb450ed9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4911489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d6c505fda05f49d5495b187a61f43d54e6d2c28f0b3ac8580cf7a0e3799058`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:fc8a71e7647a1153d30c11b86b96696357a82358286c206f04f09a1d0b01c26d in /nats-server 
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:56:36 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:56:36 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:56:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a241e0574e89ace91503f96ef69e43113479ea62d48263238c3278998139cfa7`  
		Last Modified: Wed, 02 Nov 2022 00:57:25 GMT  
		Size: 4.9 MB (4910981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4f5b84be1c29282b0d6580ec613179f0dcc5dc57cdbb562e6d613df08a24ae`  
		Last Modified: Wed, 02 Nov 2022 00:57:24 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:526012301d2a5498900afa30c7a2f2c1504d63000eaa9fbdb5110de20a97afa6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4678332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37c22cb1d3dae3bb00768485dea1a9ab57158c8b02017a0a46366aaf22ddc20`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:08:18 GMT
COPY file:bbc13cd2b910904563c88c430693025307c46d6a649c9c8bc65e4804db00de30 in /nats-server 
# Wed, 02 Nov 2022 00:08:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:08:19 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:08:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:08:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd0c038cbd2ad2c43ed500c9294ebd89b5275a293c403709e9c211465cfdef87`  
		Last Modified: Wed, 02 Nov 2022 00:09:56 GMT  
		Size: 4.7 MB (4677824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6a1f9044fd1eb13edd75e07c50e5c6e65f6b9e8e009180a73cc657481095a4`  
		Last Modified: Wed, 02 Nov 2022 00:09:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:ce273a7b73864fdddfc207bd265f8677afe39ef92c1cab2c06cba957bc99aa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4670550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2c93c2c0a5487edec047944085da7c0588d6fb522131ba60026d2ccaa77d42`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:21:26 GMT
COPY file:0566bc820f488437cfd3b1975d6edbcfffd3a48619964eca98d1e17a3ba034d0 in /nats-server 
# Wed, 02 Nov 2022 00:21:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:21:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:21:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:21:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cf37db33ebaa16eea964e96fb841d5dc472c329955da0d19b104026e4bbd9a9`  
		Last Modified: Wed, 02 Nov 2022 00:23:10 GMT  
		Size: 4.7 MB (4670042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c09ee262d1e8dc86b07fce75dc53eeaeb202174876aba05eddad97b3fda0f7a`  
		Last Modified: Wed, 02 Nov 2022 00:23:09 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3eb536b111d97bb89b35a9188e4c7ce6a5ec2f9ddad47f9c64ead1314b6d9fd4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4498550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa65ab166f9d05e530b3f151e35c31f992c2db9cf4e913dc8c8ffc33e3c486a5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:501b37b1133c20e9a1f4c5f4b27cb7c8dc0d825a0fc035df37aba209279077d8 in /nats-server 
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 01 Nov 2022 23:53:59 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 01 Nov 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 01 Nov 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:87c14cfbbbaa392bfe5b0af729955338eed477736790f057c64af1eef178e8e7`  
		Last Modified: Tue, 01 Nov 2022 23:54:49 GMT  
		Size: 4.5 MB (4498041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a40a934e5ce1a49e45b1fec3dc93c91173cc60d94ad49cbb23711e801f78685`  
		Last Modified: Tue, 01 Nov 2022 23:54:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:7a4708b3472be80d1090192110656adb3902f3152d5f8778fd96121e72d10c0b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111745442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc18527cfa55e481d723721cccdf73b138dee3173cb9aa2e42c27f5b3e1d0f0f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:19:03 GMT
RUN cmd /S /C #(nop) COPY file:65b3e40a5360689cebd70d8ad0bf1a0f64c10095a7245da46f8edce1b068ffce in C:\nats-server.exe 
# Wed, 02 Nov 2022 00:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc22e1d8ebc97d5b89ec9ff01a8ce44a7b760979db5f448526034afc5803ee48`  
		Last Modified: Wed, 02 Nov 2022 00:20:01 GMT  
		Size: 5.0 MB (4965227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8811e98534493c1911a5abfcd13fb711c59a30848835e3081054615ec5a9bab`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c0961ffa08780e8c5ec100d27acba026f5c7f83c078873964a4ddacd3bfa9`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da95ec42c571a9748d1810f3382600b7c8561a35ab1a3d3bb071bb583eb2d34`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a6a96d3a7442170ddfffa9f35c2d61c1f7ce3b2d2f338f51e3a5934c381c07`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:8c528ac1ecb3a4dc05d7d97c4af97aa95cc3bcac98c9957343eba30da6714d65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b961cb563a3c05e116ece911ad75c0dca8580521e1dc744f63fa78b2543e0aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ddca7bf9721da25b144954f6e7f84a0a12a42fc3e9308c660d8c9605ab0437`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:56:24 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:56:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:56:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:56:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302e87da6070ff379d961db7b481279218ed389beb3926c73d8eb5beed4e33bb`  
		Last Modified: Wed, 02 Nov 2022 00:57:01 GMT  
		Size: 5.2 MB (5200291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a220c8fb007e3187e497790e78b3c83a11125f9d984957b3cde03ff8b92823e7`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e1546352df384b16589539ff410d5a98559a08e25644c6b945d5ddf789b1f`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:8b60ed6ab24342ee724be5dbbd651cf22fc52787094b890197707af8c7898493
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7575822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab3e46d1547f7d198946fe8f001c5907d76c05e567caf17815a704499e4393c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:08:02 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:08:05 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:08:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd0d5ffca28edfa48b20f5823dcc114ef35b779965e8f8db21014b43157a3ff`  
		Last Modified: Wed, 02 Nov 2022 00:09:22 GMT  
		Size: 5.0 MB (4960884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1336fce1b4cb453c724a5cdc8b7664478b3c055bd3bba1752017ad2b2217fc6`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef2dd33e0e2e06539f636a8262aeb4cb98629e49d39799d94f8f7cb421b449c`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:0662be9bd4d5b559514ab09716ee1e33ab6c0537089a6ad99e6db47c233de0ba
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb51fc1a5a45ada65d2b86a95fbfcd8ed466b2e3532a4182811e93d19c2c4960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:21:04 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:21:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:21:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:21:08 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:21:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864e5340595c6879a6ead752a501201f8125830a520057c5b16f6b4ffa868b97`  
		Last Modified: Wed, 02 Nov 2022 00:22:35 GMT  
		Size: 5.0 MB (4955004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39c5c2d6544f552d996cebb05e4926c27a90a9cc9f5dbcf253ba523329ed504`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf2041c02640b63c0165501e872d53b000862c2cdc58cbc9938f6268594dd2`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:98e77de239f1bd3f91e43a552663637aca23ddfa8455a200090001fa56dafb1e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7491902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852fc53f0e44485b1cd1c57bbc335a359eee42d8d7e4fd70bdf162242ad1c77a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 23:53:52 GMT
ENV NATS_SERVER=2.9.5
# Tue, 01 Nov 2022 23:53:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 01 Nov 2022 23:53:54 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Nov 2022 23:53:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea762a6e49b5a10ed11c1f96e5b4df611123037738c753150aabf290a4f48c84`  
		Last Modified: Tue, 01 Nov 2022 23:54:26 GMT  
		Size: 4.8 MB (4783239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fcfec87094fe5e7b6306cf2251de83273c271b57e89b4928f6184897c93bfc`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cc486385827ce20e788b5eaf825120c671bd87491e4f50f68971809f5ff257`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.16`

```console
$ docker pull nats@sha256:8c528ac1ecb3a4dc05d7d97c4af97aa95cc3bcac98c9957343eba30da6714d65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:b961cb563a3c05e116ece911ad75c0dca8580521e1dc744f63fa78b2543e0aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ddca7bf9721da25b144954f6e7f84a0a12a42fc3e9308c660d8c9605ab0437`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:56:24 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:56:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:56:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:56:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302e87da6070ff379d961db7b481279218ed389beb3926c73d8eb5beed4e33bb`  
		Last Modified: Wed, 02 Nov 2022 00:57:01 GMT  
		Size: 5.2 MB (5200291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a220c8fb007e3187e497790e78b3c83a11125f9d984957b3cde03ff8b92823e7`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e1546352df384b16589539ff410d5a98559a08e25644c6b945d5ddf789b1f`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:8b60ed6ab24342ee724be5dbbd651cf22fc52787094b890197707af8c7898493
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7575822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab3e46d1547f7d198946fe8f001c5907d76c05e567caf17815a704499e4393c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:08:02 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:08:05 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:08:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd0d5ffca28edfa48b20f5823dcc114ef35b779965e8f8db21014b43157a3ff`  
		Last Modified: Wed, 02 Nov 2022 00:09:22 GMT  
		Size: 5.0 MB (4960884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1336fce1b4cb453c724a5cdc8b7664478b3c055bd3bba1752017ad2b2217fc6`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef2dd33e0e2e06539f636a8262aeb4cb98629e49d39799d94f8f7cb421b449c`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:0662be9bd4d5b559514ab09716ee1e33ab6c0537089a6ad99e6db47c233de0ba
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb51fc1a5a45ada65d2b86a95fbfcd8ed466b2e3532a4182811e93d19c2c4960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:21:04 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:21:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:21:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:21:08 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:21:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864e5340595c6879a6ead752a501201f8125830a520057c5b16f6b4ffa868b97`  
		Last Modified: Wed, 02 Nov 2022 00:22:35 GMT  
		Size: 5.0 MB (4955004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39c5c2d6544f552d996cebb05e4926c27a90a9cc9f5dbcf253ba523329ed504`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf2041c02640b63c0165501e872d53b000862c2cdc58cbc9938f6268594dd2`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:98e77de239f1bd3f91e43a552663637aca23ddfa8455a200090001fa56dafb1e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7491902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852fc53f0e44485b1cd1c57bbc335a359eee42d8d7e4fd70bdf162242ad1c77a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 23:53:52 GMT
ENV NATS_SERVER=2.9.5
# Tue, 01 Nov 2022 23:53:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 01 Nov 2022 23:53:54 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Nov 2022 23:53:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea762a6e49b5a10ed11c1f96e5b4df611123037738c753150aabf290a4f48c84`  
		Last Modified: Tue, 01 Nov 2022 23:54:26 GMT  
		Size: 4.8 MB (4783239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fcfec87094fe5e7b6306cf2251de83273c271b57e89b4928f6184897c93bfc`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cc486385827ce20e788b5eaf825120c671bd87491e4f50f68971809f5ff257`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:3a6a6e93d2fde4db16a35477ae17f68d184d37fb642982a233e0197f34035583
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:93861bcaeec03b3ea77060e14e384d56bf43a20406a131547f741c9fb450ed9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4911489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d6c505fda05f49d5495b187a61f43d54e6d2c28f0b3ac8580cf7a0e3799058`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:fc8a71e7647a1153d30c11b86b96696357a82358286c206f04f09a1d0b01c26d in /nats-server 
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:56:36 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:56:36 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:56:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a241e0574e89ace91503f96ef69e43113479ea62d48263238c3278998139cfa7`  
		Last Modified: Wed, 02 Nov 2022 00:57:25 GMT  
		Size: 4.9 MB (4910981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4f5b84be1c29282b0d6580ec613179f0dcc5dc57cdbb562e6d613df08a24ae`  
		Last Modified: Wed, 02 Nov 2022 00:57:24 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:526012301d2a5498900afa30c7a2f2c1504d63000eaa9fbdb5110de20a97afa6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4678332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37c22cb1d3dae3bb00768485dea1a9ab57158c8b02017a0a46366aaf22ddc20`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:08:18 GMT
COPY file:bbc13cd2b910904563c88c430693025307c46d6a649c9c8bc65e4804db00de30 in /nats-server 
# Wed, 02 Nov 2022 00:08:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:08:19 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:08:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:08:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd0c038cbd2ad2c43ed500c9294ebd89b5275a293c403709e9c211465cfdef87`  
		Last Modified: Wed, 02 Nov 2022 00:09:56 GMT  
		Size: 4.7 MB (4677824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6a1f9044fd1eb13edd75e07c50e5c6e65f6b9e8e009180a73cc657481095a4`  
		Last Modified: Wed, 02 Nov 2022 00:09:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ce273a7b73864fdddfc207bd265f8677afe39ef92c1cab2c06cba957bc99aa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4670550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2c93c2c0a5487edec047944085da7c0588d6fb522131ba60026d2ccaa77d42`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:21:26 GMT
COPY file:0566bc820f488437cfd3b1975d6edbcfffd3a48619964eca98d1e17a3ba034d0 in /nats-server 
# Wed, 02 Nov 2022 00:21:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:21:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:21:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:21:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cf37db33ebaa16eea964e96fb841d5dc472c329955da0d19b104026e4bbd9a9`  
		Last Modified: Wed, 02 Nov 2022 00:23:10 GMT  
		Size: 4.7 MB (4670042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c09ee262d1e8dc86b07fce75dc53eeaeb202174876aba05eddad97b3fda0f7a`  
		Last Modified: Wed, 02 Nov 2022 00:23:09 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3eb536b111d97bb89b35a9188e4c7ce6a5ec2f9ddad47f9c64ead1314b6d9fd4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4498550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa65ab166f9d05e530b3f151e35c31f992c2db9cf4e913dc8c8ffc33e3c486a5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:501b37b1133c20e9a1f4c5f4b27cb7c8dc0d825a0fc035df37aba209279077d8 in /nats-server 
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 01 Nov 2022 23:53:59 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 01 Nov 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 01 Nov 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:87c14cfbbbaa392bfe5b0af729955338eed477736790f057c64af1eef178e8e7`  
		Last Modified: Tue, 01 Nov 2022 23:54:49 GMT  
		Size: 4.5 MB (4498041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a40a934e5ce1a49e45b1fec3dc93c91173cc60d94ad49cbb23711e801f78685`  
		Last Modified: Tue, 01 Nov 2022 23:54:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:ebae1b3153e43950c72497335ab46f90f39daf9535fe9e09e2b99b40adfdbd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:7a4708b3472be80d1090192110656adb3902f3152d5f8778fd96121e72d10c0b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111745442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc18527cfa55e481d723721cccdf73b138dee3173cb9aa2e42c27f5b3e1d0f0f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:19:03 GMT
RUN cmd /S /C #(nop) COPY file:65b3e40a5360689cebd70d8ad0bf1a0f64c10095a7245da46f8edce1b068ffce in C:\nats-server.exe 
# Wed, 02 Nov 2022 00:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc22e1d8ebc97d5b89ec9ff01a8ce44a7b760979db5f448526034afc5803ee48`  
		Last Modified: Wed, 02 Nov 2022 00:20:01 GMT  
		Size: 5.0 MB (4965227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8811e98534493c1911a5abfcd13fb711c59a30848835e3081054615ec5a9bab`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c0961ffa08780e8c5ec100d27acba026f5c7f83c078873964a4ddacd3bfa9`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da95ec42c571a9748d1810f3382600b7c8561a35ab1a3d3bb071bb583eb2d34`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a6a96d3a7442170ddfffa9f35c2d61c1f7ce3b2d2f338f51e3a5934c381c07`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:ebae1b3153e43950c72497335ab46f90f39daf9535fe9e09e2b99b40adfdbd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:7a4708b3472be80d1090192110656adb3902f3152d5f8778fd96121e72d10c0b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111745442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc18527cfa55e481d723721cccdf73b138dee3173cb9aa2e42c27f5b3e1d0f0f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:19:03 GMT
RUN cmd /S /C #(nop) COPY file:65b3e40a5360689cebd70d8ad0bf1a0f64c10095a7245da46f8edce1b068ffce in C:\nats-server.exe 
# Wed, 02 Nov 2022 00:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc22e1d8ebc97d5b89ec9ff01a8ce44a7b760979db5f448526034afc5803ee48`  
		Last Modified: Wed, 02 Nov 2022 00:20:01 GMT  
		Size: 5.0 MB (4965227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8811e98534493c1911a5abfcd13fb711c59a30848835e3081054615ec5a9bab`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c0961ffa08780e8c5ec100d27acba026f5c7f83c078873964a4ddacd3bfa9`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da95ec42c571a9748d1810f3382600b7c8561a35ab1a3d3bb071bb583eb2d34`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a6a96d3a7442170ddfffa9f35c2d61c1f7ce3b2d2f338f51e3a5934c381c07`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:3a6a6e93d2fde4db16a35477ae17f68d184d37fb642982a233e0197f34035583
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:93861bcaeec03b3ea77060e14e384d56bf43a20406a131547f741c9fb450ed9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4911489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d6c505fda05f49d5495b187a61f43d54e6d2c28f0b3ac8580cf7a0e3799058`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:fc8a71e7647a1153d30c11b86b96696357a82358286c206f04f09a1d0b01c26d in /nats-server 
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:56:36 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:56:36 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:56:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a241e0574e89ace91503f96ef69e43113479ea62d48263238c3278998139cfa7`  
		Last Modified: Wed, 02 Nov 2022 00:57:25 GMT  
		Size: 4.9 MB (4910981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4f5b84be1c29282b0d6580ec613179f0dcc5dc57cdbb562e6d613df08a24ae`  
		Last Modified: Wed, 02 Nov 2022 00:57:24 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:526012301d2a5498900afa30c7a2f2c1504d63000eaa9fbdb5110de20a97afa6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4678332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37c22cb1d3dae3bb00768485dea1a9ab57158c8b02017a0a46366aaf22ddc20`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:08:18 GMT
COPY file:bbc13cd2b910904563c88c430693025307c46d6a649c9c8bc65e4804db00de30 in /nats-server 
# Wed, 02 Nov 2022 00:08:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:08:19 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:08:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:08:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd0c038cbd2ad2c43ed500c9294ebd89b5275a293c403709e9c211465cfdef87`  
		Last Modified: Wed, 02 Nov 2022 00:09:56 GMT  
		Size: 4.7 MB (4677824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6a1f9044fd1eb13edd75e07c50e5c6e65f6b9e8e009180a73cc657481095a4`  
		Last Modified: Wed, 02 Nov 2022 00:09:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ce273a7b73864fdddfc207bd265f8677afe39ef92c1cab2c06cba957bc99aa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4670550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2c93c2c0a5487edec047944085da7c0588d6fb522131ba60026d2ccaa77d42`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:21:26 GMT
COPY file:0566bc820f488437cfd3b1975d6edbcfffd3a48619964eca98d1e17a3ba034d0 in /nats-server 
# Wed, 02 Nov 2022 00:21:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:21:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:21:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:21:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cf37db33ebaa16eea964e96fb841d5dc472c329955da0d19b104026e4bbd9a9`  
		Last Modified: Wed, 02 Nov 2022 00:23:10 GMT  
		Size: 4.7 MB (4670042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c09ee262d1e8dc86b07fce75dc53eeaeb202174876aba05eddad97b3fda0f7a`  
		Last Modified: Wed, 02 Nov 2022 00:23:09 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3eb536b111d97bb89b35a9188e4c7ce6a5ec2f9ddad47f9c64ead1314b6d9fd4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4498550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa65ab166f9d05e530b3f151e35c31f992c2db9cf4e913dc8c8ffc33e3c486a5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:501b37b1133c20e9a1f4c5f4b27cb7c8dc0d825a0fc035df37aba209279077d8 in /nats-server 
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 01 Nov 2022 23:53:59 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 01 Nov 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 01 Nov 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:87c14cfbbbaa392bfe5b0af729955338eed477736790f057c64af1eef178e8e7`  
		Last Modified: Tue, 01 Nov 2022 23:54:49 GMT  
		Size: 4.5 MB (4498041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a40a934e5ce1a49e45b1fec3dc93c91173cc60d94ad49cbb23711e801f78685`  
		Last Modified: Tue, 01 Nov 2022 23:54:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:c892e8d423eb9100e66d518f443dc34c909d61cbb9ddf3e915d1b2b01ebe751e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:5571861cd5b0f6018aa7855af4e2404c0ce18c6c84998469f37d20ff2b3c1904
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779175732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:531ff1eed7b103984ec29d81ea6f77943f8d3a711b1f4a6369022382a699d410`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:15:11 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.5/nats-server-v2.9.5-windows-amd64.zip
# Wed, 02 Nov 2022 00:15:17 GMT
ENV NATS_SERVER_SHASUM=86c963d3780234e6fecdaf72b9c89c9ecc2fc534d21c8e3ae855d0c062e41842
# Wed, 02 Nov 2022 00:16:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 02 Nov 2022 00:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 02 Nov 2022 00:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:18:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:18:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008b3979e40adbc80493c35e40a541ee0cd9f8cfb0d21f0dbb615b61a5800f3c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04f2cde91cfc04742cc431a646b0a0497d5cb0ac69c47f4530a16661f2eaca7`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf94dd1d2f43db680e22d0f214cd977185845f10df9bc06e7482c0eb43fb738`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a68e7f32692839720ce6bc41b42930a1fb73553533f3126fda5f90e7aacf45c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 358.3 KB (358324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db97038ec690106eede5d444866ae33a36d942485fd573db39c19207af3241e5`  
		Last Modified: Wed, 02 Nov 2022 00:19:42 GMT  
		Size: 5.3 MB (5305782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f237153f81ef2cffd83842993b4adbfa6bd1bc6e93f4775bef663d5564b28b8`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0660057acb9a90d1ec48107439058b6de0b482644e12a14859cda3f5db0fee4a`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596407afbadde38cf9b8f7a01869e6a2df90f9db2bfc93a669b60b263856927`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a537a0f8dced04ed22fcf2ceade81c6a0f2e2c1e31a8ece5416bb3673b5b7e9`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:c892e8d423eb9100e66d518f443dc34c909d61cbb9ddf3e915d1b2b01ebe751e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:5571861cd5b0f6018aa7855af4e2404c0ce18c6c84998469f37d20ff2b3c1904
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779175732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:531ff1eed7b103984ec29d81ea6f77943f8d3a711b1f4a6369022382a699d410`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:15:11 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.5/nats-server-v2.9.5-windows-amd64.zip
# Wed, 02 Nov 2022 00:15:17 GMT
ENV NATS_SERVER_SHASUM=86c963d3780234e6fecdaf72b9c89c9ecc2fc534d21c8e3ae855d0c062e41842
# Wed, 02 Nov 2022 00:16:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 02 Nov 2022 00:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 02 Nov 2022 00:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:18:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:18:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008b3979e40adbc80493c35e40a541ee0cd9f8cfb0d21f0dbb615b61a5800f3c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04f2cde91cfc04742cc431a646b0a0497d5cb0ac69c47f4530a16661f2eaca7`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf94dd1d2f43db680e22d0f214cd977185845f10df9bc06e7482c0eb43fb738`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a68e7f32692839720ce6bc41b42930a1fb73553533f3126fda5f90e7aacf45c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 358.3 KB (358324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db97038ec690106eede5d444866ae33a36d942485fd573db39c19207af3241e5`  
		Last Modified: Wed, 02 Nov 2022 00:19:42 GMT  
		Size: 5.3 MB (5305782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f237153f81ef2cffd83842993b4adbfa6bd1bc6e93f4775bef663d5564b28b8`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0660057acb9a90d1ec48107439058b6de0b482644e12a14859cda3f5db0fee4a`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596407afbadde38cf9b8f7a01869e6a2df90f9db2bfc93a669b60b263856927`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a537a0f8dced04ed22fcf2ceade81c6a0f2e2c1e31a8ece5416bb3673b5b7e9`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:38cf02118dd5f875345011c712c01b337d93d6ba53ad405e554071971ddc96aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:93861bcaeec03b3ea77060e14e384d56bf43a20406a131547f741c9fb450ed9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4911489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d6c505fda05f49d5495b187a61f43d54e6d2c28f0b3ac8580cf7a0e3799058`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:fc8a71e7647a1153d30c11b86b96696357a82358286c206f04f09a1d0b01c26d in /nats-server 
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:56:36 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:56:36 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:56:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a241e0574e89ace91503f96ef69e43113479ea62d48263238c3278998139cfa7`  
		Last Modified: Wed, 02 Nov 2022 00:57:25 GMT  
		Size: 4.9 MB (4910981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4f5b84be1c29282b0d6580ec613179f0dcc5dc57cdbb562e6d613df08a24ae`  
		Last Modified: Wed, 02 Nov 2022 00:57:24 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:526012301d2a5498900afa30c7a2f2c1504d63000eaa9fbdb5110de20a97afa6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4678332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37c22cb1d3dae3bb00768485dea1a9ab57158c8b02017a0a46366aaf22ddc20`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:08:18 GMT
COPY file:bbc13cd2b910904563c88c430693025307c46d6a649c9c8bc65e4804db00de30 in /nats-server 
# Wed, 02 Nov 2022 00:08:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:08:19 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:08:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:08:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd0c038cbd2ad2c43ed500c9294ebd89b5275a293c403709e9c211465cfdef87`  
		Last Modified: Wed, 02 Nov 2022 00:09:56 GMT  
		Size: 4.7 MB (4677824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6a1f9044fd1eb13edd75e07c50e5c6e65f6b9e8e009180a73cc657481095a4`  
		Last Modified: Wed, 02 Nov 2022 00:09:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:ce273a7b73864fdddfc207bd265f8677afe39ef92c1cab2c06cba957bc99aa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4670550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2c93c2c0a5487edec047944085da7c0588d6fb522131ba60026d2ccaa77d42`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:21:26 GMT
COPY file:0566bc820f488437cfd3b1975d6edbcfffd3a48619964eca98d1e17a3ba034d0 in /nats-server 
# Wed, 02 Nov 2022 00:21:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:21:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:21:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:21:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cf37db33ebaa16eea964e96fb841d5dc472c329955da0d19b104026e4bbd9a9`  
		Last Modified: Wed, 02 Nov 2022 00:23:10 GMT  
		Size: 4.7 MB (4670042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c09ee262d1e8dc86b07fce75dc53eeaeb202174876aba05eddad97b3fda0f7a`  
		Last Modified: Wed, 02 Nov 2022 00:23:09 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3eb536b111d97bb89b35a9188e4c7ce6a5ec2f9ddad47f9c64ead1314b6d9fd4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4498550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa65ab166f9d05e530b3f151e35c31f992c2db9cf4e913dc8c8ffc33e3c486a5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:501b37b1133c20e9a1f4c5f4b27cb7c8dc0d825a0fc035df37aba209279077d8 in /nats-server 
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 01 Nov 2022 23:53:59 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 01 Nov 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 01 Nov 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:87c14cfbbbaa392bfe5b0af729955338eed477736790f057c64af1eef178e8e7`  
		Last Modified: Tue, 01 Nov 2022 23:54:49 GMT  
		Size: 4.5 MB (4498041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a40a934e5ce1a49e45b1fec3dc93c91173cc60d94ad49cbb23711e801f78685`  
		Last Modified: Tue, 01 Nov 2022 23:54:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:7a4708b3472be80d1090192110656adb3902f3152d5f8778fd96121e72d10c0b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111745442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc18527cfa55e481d723721cccdf73b138dee3173cb9aa2e42c27f5b3e1d0f0f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:19:03 GMT
RUN cmd /S /C #(nop) COPY file:65b3e40a5360689cebd70d8ad0bf1a0f64c10095a7245da46f8edce1b068ffce in C:\nats-server.exe 
# Wed, 02 Nov 2022 00:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc22e1d8ebc97d5b89ec9ff01a8ce44a7b760979db5f448526034afc5803ee48`  
		Last Modified: Wed, 02 Nov 2022 00:20:01 GMT  
		Size: 5.0 MB (4965227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8811e98534493c1911a5abfcd13fb711c59a30848835e3081054615ec5a9bab`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c0961ffa08780e8c5ec100d27acba026f5c7f83c078873964a4ddacd3bfa9`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da95ec42c571a9748d1810f3382600b7c8561a35ab1a3d3bb071bb583eb2d34`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a6a96d3a7442170ddfffa9f35c2d61c1f7ce3b2d2f338f51e3a5934c381c07`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:8c528ac1ecb3a4dc05d7d97c4af97aa95cc3bcac98c9957343eba30da6714d65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b961cb563a3c05e116ece911ad75c0dca8580521e1dc744f63fa78b2543e0aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ddca7bf9721da25b144954f6e7f84a0a12a42fc3e9308c660d8c9605ab0437`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:56:24 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:56:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:56:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:56:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302e87da6070ff379d961db7b481279218ed389beb3926c73d8eb5beed4e33bb`  
		Last Modified: Wed, 02 Nov 2022 00:57:01 GMT  
		Size: 5.2 MB (5200291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a220c8fb007e3187e497790e78b3c83a11125f9d984957b3cde03ff8b92823e7`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e1546352df384b16589539ff410d5a98559a08e25644c6b945d5ddf789b1f`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:8b60ed6ab24342ee724be5dbbd651cf22fc52787094b890197707af8c7898493
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7575822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab3e46d1547f7d198946fe8f001c5907d76c05e567caf17815a704499e4393c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:08:02 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:08:05 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:08:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd0d5ffca28edfa48b20f5823dcc114ef35b779965e8f8db21014b43157a3ff`  
		Last Modified: Wed, 02 Nov 2022 00:09:22 GMT  
		Size: 5.0 MB (4960884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1336fce1b4cb453c724a5cdc8b7664478b3c055bd3bba1752017ad2b2217fc6`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef2dd33e0e2e06539f636a8262aeb4cb98629e49d39799d94f8f7cb421b449c`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:0662be9bd4d5b559514ab09716ee1e33ab6c0537089a6ad99e6db47c233de0ba
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb51fc1a5a45ada65d2b86a95fbfcd8ed466b2e3532a4182811e93d19c2c4960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:21:04 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:21:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:21:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:21:08 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:21:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864e5340595c6879a6ead752a501201f8125830a520057c5b16f6b4ffa868b97`  
		Last Modified: Wed, 02 Nov 2022 00:22:35 GMT  
		Size: 5.0 MB (4955004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39c5c2d6544f552d996cebb05e4926c27a90a9cc9f5dbcf253ba523329ed504`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf2041c02640b63c0165501e872d53b000862c2cdc58cbc9938f6268594dd2`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:98e77de239f1bd3f91e43a552663637aca23ddfa8455a200090001fa56dafb1e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7491902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852fc53f0e44485b1cd1c57bbc335a359eee42d8d7e4fd70bdf162242ad1c77a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 23:53:52 GMT
ENV NATS_SERVER=2.9.5
# Tue, 01 Nov 2022 23:53:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 01 Nov 2022 23:53:54 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Nov 2022 23:53:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea762a6e49b5a10ed11c1f96e5b4df611123037738c753150aabf290a4f48c84`  
		Last Modified: Tue, 01 Nov 2022 23:54:26 GMT  
		Size: 4.8 MB (4783239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fcfec87094fe5e7b6306cf2251de83273c271b57e89b4928f6184897c93bfc`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cc486385827ce20e788b5eaf825120c671bd87491e4f50f68971809f5ff257`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.16`

```console
$ docker pull nats@sha256:8c528ac1ecb3a4dc05d7d97c4af97aa95cc3bcac98c9957343eba30da6714d65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:b961cb563a3c05e116ece911ad75c0dca8580521e1dc744f63fa78b2543e0aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ddca7bf9721da25b144954f6e7f84a0a12a42fc3e9308c660d8c9605ab0437`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:56:24 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:56:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:56:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:56:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302e87da6070ff379d961db7b481279218ed389beb3926c73d8eb5beed4e33bb`  
		Last Modified: Wed, 02 Nov 2022 00:57:01 GMT  
		Size: 5.2 MB (5200291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a220c8fb007e3187e497790e78b3c83a11125f9d984957b3cde03ff8b92823e7`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e1546352df384b16589539ff410d5a98559a08e25644c6b945d5ddf789b1f`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:8b60ed6ab24342ee724be5dbbd651cf22fc52787094b890197707af8c7898493
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7575822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab3e46d1547f7d198946fe8f001c5907d76c05e567caf17815a704499e4393c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:08:02 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:08:05 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:08:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd0d5ffca28edfa48b20f5823dcc114ef35b779965e8f8db21014b43157a3ff`  
		Last Modified: Wed, 02 Nov 2022 00:09:22 GMT  
		Size: 5.0 MB (4960884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1336fce1b4cb453c724a5cdc8b7664478b3c055bd3bba1752017ad2b2217fc6`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef2dd33e0e2e06539f636a8262aeb4cb98629e49d39799d94f8f7cb421b449c`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:0662be9bd4d5b559514ab09716ee1e33ab6c0537089a6ad99e6db47c233de0ba
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb51fc1a5a45ada65d2b86a95fbfcd8ed466b2e3532a4182811e93d19c2c4960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:21:04 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:21:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:21:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:21:08 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:21:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864e5340595c6879a6ead752a501201f8125830a520057c5b16f6b4ffa868b97`  
		Last Modified: Wed, 02 Nov 2022 00:22:35 GMT  
		Size: 5.0 MB (4955004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39c5c2d6544f552d996cebb05e4926c27a90a9cc9f5dbcf253ba523329ed504`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf2041c02640b63c0165501e872d53b000862c2cdc58cbc9938f6268594dd2`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:98e77de239f1bd3f91e43a552663637aca23ddfa8455a200090001fa56dafb1e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7491902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852fc53f0e44485b1cd1c57bbc335a359eee42d8d7e4fd70bdf162242ad1c77a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 23:53:52 GMT
ENV NATS_SERVER=2.9.5
# Tue, 01 Nov 2022 23:53:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 01 Nov 2022 23:53:54 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Nov 2022 23:53:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea762a6e49b5a10ed11c1f96e5b4df611123037738c753150aabf290a4f48c84`  
		Last Modified: Tue, 01 Nov 2022 23:54:26 GMT  
		Size: 4.8 MB (4783239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fcfec87094fe5e7b6306cf2251de83273c271b57e89b4928f6184897c93bfc`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cc486385827ce20e788b5eaf825120c671bd87491e4f50f68971809f5ff257`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:3a6a6e93d2fde4db16a35477ae17f68d184d37fb642982a233e0197f34035583
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:93861bcaeec03b3ea77060e14e384d56bf43a20406a131547f741c9fb450ed9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4911489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d6c505fda05f49d5495b187a61f43d54e6d2c28f0b3ac8580cf7a0e3799058`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:fc8a71e7647a1153d30c11b86b96696357a82358286c206f04f09a1d0b01c26d in /nats-server 
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:56:36 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:56:36 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:56:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a241e0574e89ace91503f96ef69e43113479ea62d48263238c3278998139cfa7`  
		Last Modified: Wed, 02 Nov 2022 00:57:25 GMT  
		Size: 4.9 MB (4910981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4f5b84be1c29282b0d6580ec613179f0dcc5dc57cdbb562e6d613df08a24ae`  
		Last Modified: Wed, 02 Nov 2022 00:57:24 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:526012301d2a5498900afa30c7a2f2c1504d63000eaa9fbdb5110de20a97afa6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4678332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37c22cb1d3dae3bb00768485dea1a9ab57158c8b02017a0a46366aaf22ddc20`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:08:18 GMT
COPY file:bbc13cd2b910904563c88c430693025307c46d6a649c9c8bc65e4804db00de30 in /nats-server 
# Wed, 02 Nov 2022 00:08:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:08:19 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:08:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:08:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd0c038cbd2ad2c43ed500c9294ebd89b5275a293c403709e9c211465cfdef87`  
		Last Modified: Wed, 02 Nov 2022 00:09:56 GMT  
		Size: 4.7 MB (4677824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6a1f9044fd1eb13edd75e07c50e5c6e65f6b9e8e009180a73cc657481095a4`  
		Last Modified: Wed, 02 Nov 2022 00:09:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ce273a7b73864fdddfc207bd265f8677afe39ef92c1cab2c06cba957bc99aa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4670550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2c93c2c0a5487edec047944085da7c0588d6fb522131ba60026d2ccaa77d42`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:21:26 GMT
COPY file:0566bc820f488437cfd3b1975d6edbcfffd3a48619964eca98d1e17a3ba034d0 in /nats-server 
# Wed, 02 Nov 2022 00:21:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:21:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:21:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:21:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cf37db33ebaa16eea964e96fb841d5dc472c329955da0d19b104026e4bbd9a9`  
		Last Modified: Wed, 02 Nov 2022 00:23:10 GMT  
		Size: 4.7 MB (4670042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c09ee262d1e8dc86b07fce75dc53eeaeb202174876aba05eddad97b3fda0f7a`  
		Last Modified: Wed, 02 Nov 2022 00:23:09 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3eb536b111d97bb89b35a9188e4c7ce6a5ec2f9ddad47f9c64ead1314b6d9fd4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4498550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa65ab166f9d05e530b3f151e35c31f992c2db9cf4e913dc8c8ffc33e3c486a5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:501b37b1133c20e9a1f4c5f4b27cb7c8dc0d825a0fc035df37aba209279077d8 in /nats-server 
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 01 Nov 2022 23:53:59 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 01 Nov 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 01 Nov 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:87c14cfbbbaa392bfe5b0af729955338eed477736790f057c64af1eef178e8e7`  
		Last Modified: Tue, 01 Nov 2022 23:54:49 GMT  
		Size: 4.5 MB (4498041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a40a934e5ce1a49e45b1fec3dc93c91173cc60d94ad49cbb23711e801f78685`  
		Last Modified: Tue, 01 Nov 2022 23:54:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:ebae1b3153e43950c72497335ab46f90f39daf9535fe9e09e2b99b40adfdbd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:7a4708b3472be80d1090192110656adb3902f3152d5f8778fd96121e72d10c0b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111745442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc18527cfa55e481d723721cccdf73b138dee3173cb9aa2e42c27f5b3e1d0f0f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:19:03 GMT
RUN cmd /S /C #(nop) COPY file:65b3e40a5360689cebd70d8ad0bf1a0f64c10095a7245da46f8edce1b068ffce in C:\nats-server.exe 
# Wed, 02 Nov 2022 00:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc22e1d8ebc97d5b89ec9ff01a8ce44a7b760979db5f448526034afc5803ee48`  
		Last Modified: Wed, 02 Nov 2022 00:20:01 GMT  
		Size: 5.0 MB (4965227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8811e98534493c1911a5abfcd13fb711c59a30848835e3081054615ec5a9bab`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c0961ffa08780e8c5ec100d27acba026f5c7f83c078873964a4ddacd3bfa9`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da95ec42c571a9748d1810f3382600b7c8561a35ab1a3d3bb071bb583eb2d34`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a6a96d3a7442170ddfffa9f35c2d61c1f7ce3b2d2f338f51e3a5934c381c07`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:ebae1b3153e43950c72497335ab46f90f39daf9535fe9e09e2b99b40adfdbd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:7a4708b3472be80d1090192110656adb3902f3152d5f8778fd96121e72d10c0b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111745442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc18527cfa55e481d723721cccdf73b138dee3173cb9aa2e42c27f5b3e1d0f0f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:19:03 GMT
RUN cmd /S /C #(nop) COPY file:65b3e40a5360689cebd70d8ad0bf1a0f64c10095a7245da46f8edce1b068ffce in C:\nats-server.exe 
# Wed, 02 Nov 2022 00:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc22e1d8ebc97d5b89ec9ff01a8ce44a7b760979db5f448526034afc5803ee48`  
		Last Modified: Wed, 02 Nov 2022 00:20:01 GMT  
		Size: 5.0 MB (4965227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8811e98534493c1911a5abfcd13fb711c59a30848835e3081054615ec5a9bab`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c0961ffa08780e8c5ec100d27acba026f5c7f83c078873964a4ddacd3bfa9`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da95ec42c571a9748d1810f3382600b7c8561a35ab1a3d3bb071bb583eb2d34`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a6a96d3a7442170ddfffa9f35c2d61c1f7ce3b2d2f338f51e3a5934c381c07`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:3a6a6e93d2fde4db16a35477ae17f68d184d37fb642982a233e0197f34035583
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:93861bcaeec03b3ea77060e14e384d56bf43a20406a131547f741c9fb450ed9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4911489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d6c505fda05f49d5495b187a61f43d54e6d2c28f0b3ac8580cf7a0e3799058`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:fc8a71e7647a1153d30c11b86b96696357a82358286c206f04f09a1d0b01c26d in /nats-server 
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:56:36 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:56:36 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:56:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a241e0574e89ace91503f96ef69e43113479ea62d48263238c3278998139cfa7`  
		Last Modified: Wed, 02 Nov 2022 00:57:25 GMT  
		Size: 4.9 MB (4910981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4f5b84be1c29282b0d6580ec613179f0dcc5dc57cdbb562e6d613df08a24ae`  
		Last Modified: Wed, 02 Nov 2022 00:57:24 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:526012301d2a5498900afa30c7a2f2c1504d63000eaa9fbdb5110de20a97afa6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4678332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37c22cb1d3dae3bb00768485dea1a9ab57158c8b02017a0a46366aaf22ddc20`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:08:18 GMT
COPY file:bbc13cd2b910904563c88c430693025307c46d6a649c9c8bc65e4804db00de30 in /nats-server 
# Wed, 02 Nov 2022 00:08:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:08:19 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:08:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:08:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd0c038cbd2ad2c43ed500c9294ebd89b5275a293c403709e9c211465cfdef87`  
		Last Modified: Wed, 02 Nov 2022 00:09:56 GMT  
		Size: 4.7 MB (4677824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6a1f9044fd1eb13edd75e07c50e5c6e65f6b9e8e009180a73cc657481095a4`  
		Last Modified: Wed, 02 Nov 2022 00:09:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ce273a7b73864fdddfc207bd265f8677afe39ef92c1cab2c06cba957bc99aa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4670550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2c93c2c0a5487edec047944085da7c0588d6fb522131ba60026d2ccaa77d42`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:21:26 GMT
COPY file:0566bc820f488437cfd3b1975d6edbcfffd3a48619964eca98d1e17a3ba034d0 in /nats-server 
# Wed, 02 Nov 2022 00:21:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:21:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:21:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:21:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cf37db33ebaa16eea964e96fb841d5dc472c329955da0d19b104026e4bbd9a9`  
		Last Modified: Wed, 02 Nov 2022 00:23:10 GMT  
		Size: 4.7 MB (4670042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c09ee262d1e8dc86b07fce75dc53eeaeb202174876aba05eddad97b3fda0f7a`  
		Last Modified: Wed, 02 Nov 2022 00:23:09 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3eb536b111d97bb89b35a9188e4c7ce6a5ec2f9ddad47f9c64ead1314b6d9fd4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4498550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa65ab166f9d05e530b3f151e35c31f992c2db9cf4e913dc8c8ffc33e3c486a5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:501b37b1133c20e9a1f4c5f4b27cb7c8dc0d825a0fc035df37aba209279077d8 in /nats-server 
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 01 Nov 2022 23:53:59 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 01 Nov 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 01 Nov 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:87c14cfbbbaa392bfe5b0af729955338eed477736790f057c64af1eef178e8e7`  
		Last Modified: Tue, 01 Nov 2022 23:54:49 GMT  
		Size: 4.5 MB (4498041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a40a934e5ce1a49e45b1fec3dc93c91173cc60d94ad49cbb23711e801f78685`  
		Last Modified: Tue, 01 Nov 2022 23:54:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:c892e8d423eb9100e66d518f443dc34c909d61cbb9ddf3e915d1b2b01ebe751e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:5571861cd5b0f6018aa7855af4e2404c0ce18c6c84998469f37d20ff2b3c1904
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779175732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:531ff1eed7b103984ec29d81ea6f77943f8d3a711b1f4a6369022382a699d410`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:15:11 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.5/nats-server-v2.9.5-windows-amd64.zip
# Wed, 02 Nov 2022 00:15:17 GMT
ENV NATS_SERVER_SHASUM=86c963d3780234e6fecdaf72b9c89c9ecc2fc534d21c8e3ae855d0c062e41842
# Wed, 02 Nov 2022 00:16:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 02 Nov 2022 00:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 02 Nov 2022 00:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:18:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:18:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008b3979e40adbc80493c35e40a541ee0cd9f8cfb0d21f0dbb615b61a5800f3c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04f2cde91cfc04742cc431a646b0a0497d5cb0ac69c47f4530a16661f2eaca7`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf94dd1d2f43db680e22d0f214cd977185845f10df9bc06e7482c0eb43fb738`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a68e7f32692839720ce6bc41b42930a1fb73553533f3126fda5f90e7aacf45c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 358.3 KB (358324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db97038ec690106eede5d444866ae33a36d942485fd573db39c19207af3241e5`  
		Last Modified: Wed, 02 Nov 2022 00:19:42 GMT  
		Size: 5.3 MB (5305782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f237153f81ef2cffd83842993b4adbfa6bd1bc6e93f4775bef663d5564b28b8`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0660057acb9a90d1ec48107439058b6de0b482644e12a14859cda3f5db0fee4a`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596407afbadde38cf9b8f7a01869e6a2df90f9db2bfc93a669b60b263856927`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a537a0f8dced04ed22fcf2ceade81c6a0f2e2c1e31a8ece5416bb3673b5b7e9`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:c892e8d423eb9100e66d518f443dc34c909d61cbb9ddf3e915d1b2b01ebe751e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:5571861cd5b0f6018aa7855af4e2404c0ce18c6c84998469f37d20ff2b3c1904
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779175732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:531ff1eed7b103984ec29d81ea6f77943f8d3a711b1f4a6369022382a699d410`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:15:11 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.5/nats-server-v2.9.5-windows-amd64.zip
# Wed, 02 Nov 2022 00:15:17 GMT
ENV NATS_SERVER_SHASUM=86c963d3780234e6fecdaf72b9c89c9ecc2fc534d21c8e3ae855d0c062e41842
# Wed, 02 Nov 2022 00:16:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 02 Nov 2022 00:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 02 Nov 2022 00:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:18:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:18:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008b3979e40adbc80493c35e40a541ee0cd9f8cfb0d21f0dbb615b61a5800f3c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04f2cde91cfc04742cc431a646b0a0497d5cb0ac69c47f4530a16661f2eaca7`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf94dd1d2f43db680e22d0f214cd977185845f10df9bc06e7482c0eb43fb738`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a68e7f32692839720ce6bc41b42930a1fb73553533f3126fda5f90e7aacf45c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 358.3 KB (358324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db97038ec690106eede5d444866ae33a36d942485fd573db39c19207af3241e5`  
		Last Modified: Wed, 02 Nov 2022 00:19:42 GMT  
		Size: 5.3 MB (5305782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f237153f81ef2cffd83842993b4adbfa6bd1bc6e93f4775bef663d5564b28b8`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0660057acb9a90d1ec48107439058b6de0b482644e12a14859cda3f5db0fee4a`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596407afbadde38cf9b8f7a01869e6a2df90f9db2bfc93a669b60b263856927`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a537a0f8dced04ed22fcf2ceade81c6a0f2e2c1e31a8ece5416bb3673b5b7e9`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6`

**does not exist** (yet?)

## `nats:2.9.6-alpine`

**does not exist** (yet?)

## `nats:2.9.6-alpine3.16`

**does not exist** (yet?)

## `nats:2.9.6-linux`

**does not exist** (yet?)

## `nats:2.9.6-nanoserver`

**does not exist** (yet?)

## `nats:2.9.6-nanoserver-1809`

**does not exist** (yet?)

## `nats:2.9.6-scratch`

**does not exist** (yet?)

## `nats:2.9.6-windowsservercore`

**does not exist** (yet?)

## `nats:2.9.6-windowsservercore-1809`

**does not exist** (yet?)

## `nats:alpine`

```console
$ docker pull nats@sha256:8c528ac1ecb3a4dc05d7d97c4af97aa95cc3bcac98c9957343eba30da6714d65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:b961cb563a3c05e116ece911ad75c0dca8580521e1dc744f63fa78b2543e0aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ddca7bf9721da25b144954f6e7f84a0a12a42fc3e9308c660d8c9605ab0437`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:56:24 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:56:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:56:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:56:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302e87da6070ff379d961db7b481279218ed389beb3926c73d8eb5beed4e33bb`  
		Last Modified: Wed, 02 Nov 2022 00:57:01 GMT  
		Size: 5.2 MB (5200291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a220c8fb007e3187e497790e78b3c83a11125f9d984957b3cde03ff8b92823e7`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e1546352df384b16589539ff410d5a98559a08e25644c6b945d5ddf789b1f`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:8b60ed6ab24342ee724be5dbbd651cf22fc52787094b890197707af8c7898493
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7575822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab3e46d1547f7d198946fe8f001c5907d76c05e567caf17815a704499e4393c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:08:02 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:08:05 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:08:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd0d5ffca28edfa48b20f5823dcc114ef35b779965e8f8db21014b43157a3ff`  
		Last Modified: Wed, 02 Nov 2022 00:09:22 GMT  
		Size: 5.0 MB (4960884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1336fce1b4cb453c724a5cdc8b7664478b3c055bd3bba1752017ad2b2217fc6`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef2dd33e0e2e06539f636a8262aeb4cb98629e49d39799d94f8f7cb421b449c`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:0662be9bd4d5b559514ab09716ee1e33ab6c0537089a6ad99e6db47c233de0ba
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb51fc1a5a45ada65d2b86a95fbfcd8ed466b2e3532a4182811e93d19c2c4960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:21:04 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:21:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:21:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:21:08 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:21:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864e5340595c6879a6ead752a501201f8125830a520057c5b16f6b4ffa868b97`  
		Last Modified: Wed, 02 Nov 2022 00:22:35 GMT  
		Size: 5.0 MB (4955004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39c5c2d6544f552d996cebb05e4926c27a90a9cc9f5dbcf253ba523329ed504`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf2041c02640b63c0165501e872d53b000862c2cdc58cbc9938f6268594dd2`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:98e77de239f1bd3f91e43a552663637aca23ddfa8455a200090001fa56dafb1e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7491902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852fc53f0e44485b1cd1c57bbc335a359eee42d8d7e4fd70bdf162242ad1c77a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 23:53:52 GMT
ENV NATS_SERVER=2.9.5
# Tue, 01 Nov 2022 23:53:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 01 Nov 2022 23:53:54 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Nov 2022 23:53:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea762a6e49b5a10ed11c1f96e5b4df611123037738c753150aabf290a4f48c84`  
		Last Modified: Tue, 01 Nov 2022 23:54:26 GMT  
		Size: 4.8 MB (4783239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fcfec87094fe5e7b6306cf2251de83273c271b57e89b4928f6184897c93bfc`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cc486385827ce20e788b5eaf825120c671bd87491e4f50f68971809f5ff257`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.16`

```console
$ docker pull nats@sha256:8c528ac1ecb3a4dc05d7d97c4af97aa95cc3bcac98c9957343eba30da6714d65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:b961cb563a3c05e116ece911ad75c0dca8580521e1dc744f63fa78b2543e0aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ddca7bf9721da25b144954f6e7f84a0a12a42fc3e9308c660d8c9605ab0437`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:56:24 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:56:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:56:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:56:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:56:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302e87da6070ff379d961db7b481279218ed389beb3926c73d8eb5beed4e33bb`  
		Last Modified: Wed, 02 Nov 2022 00:57:01 GMT  
		Size: 5.2 MB (5200291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a220c8fb007e3187e497790e78b3c83a11125f9d984957b3cde03ff8b92823e7`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e1546352df384b16589539ff410d5a98559a08e25644c6b945d5ddf789b1f`  
		Last Modified: Wed, 02 Nov 2022 00:57:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:8b60ed6ab24342ee724be5dbbd651cf22fc52787094b890197707af8c7898493
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7575822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab3e46d1547f7d198946fe8f001c5907d76c05e567caf17815a704499e4393c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:08:02 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:08:05 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:08:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd0d5ffca28edfa48b20f5823dcc114ef35b779965e8f8db21014b43157a3ff`  
		Last Modified: Wed, 02 Nov 2022 00:09:22 GMT  
		Size: 5.0 MB (4960884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1336fce1b4cb453c724a5cdc8b7664478b3c055bd3bba1752017ad2b2217fc6`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef2dd33e0e2e06539f636a8262aeb4cb98629e49d39799d94f8f7cb421b449c`  
		Last Modified: Wed, 02 Nov 2022 00:09:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:0662be9bd4d5b559514ab09716ee1e33ab6c0537089a6ad99e6db47c233de0ba
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb51fc1a5a45ada65d2b86a95fbfcd8ed466b2e3532a4182811e93d19c2c4960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 02 Nov 2022 00:21:04 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 02 Nov 2022 00:21:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 02 Nov 2022 00:21:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 02 Nov 2022 00:21:08 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 00:21:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864e5340595c6879a6ead752a501201f8125830a520057c5b16f6b4ffa868b97`  
		Last Modified: Wed, 02 Nov 2022 00:22:35 GMT  
		Size: 5.0 MB (4955004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39c5c2d6544f552d996cebb05e4926c27a90a9cc9f5dbcf253ba523329ed504`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf2041c02640b63c0165501e872d53b000862c2cdc58cbc9938f6268594dd2`  
		Last Modified: Wed, 02 Nov 2022 00:22:34 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:98e77de239f1bd3f91e43a552663637aca23ddfa8455a200090001fa56dafb1e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7491902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852fc53f0e44485b1cd1c57bbc335a359eee42d8d7e4fd70bdf162242ad1c77a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 23:53:52 GMT
ENV NATS_SERVER=2.9.5
# Tue, 01 Nov 2022 23:53:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='490821b628421ce516ca8ed4d31e25e88577aa530a1eac53df51366ebcf6149b' ;; 		armhf) natsArch='arm6'; sha256='d8b1e79ad136dc381b86192110531b2bae716408baf57d8ade3000fbbd957810' ;; 		armv7) natsArch='arm7'; sha256='e9cd21a0f203448b6816fbeaa73a63028bfa48bede37549c4dcc1c9311755e5b' ;; 		x86_64) natsArch='amd64'; sha256='3e488e579c091da8fd628db69795cc4cdc8b376c516561e4a7c5fa5ff3874ec7' ;; 		x86) natsArch='386'; sha256='8606cafb62a5957abf720baeb1217b1adcd336d75a263d8b61528c03e34e04b9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 01 Nov 2022 23:53:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 01 Nov 2022 23:53:54 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Nov 2022 23:53:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea762a6e49b5a10ed11c1f96e5b4df611123037738c753150aabf290a4f48c84`  
		Last Modified: Tue, 01 Nov 2022 23:54:26 GMT  
		Size: 4.8 MB (4783239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fcfec87094fe5e7b6306cf2251de83273c271b57e89b4928f6184897c93bfc`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cc486385827ce20e788b5eaf825120c671bd87491e4f50f68971809f5ff257`  
		Last Modified: Tue, 01 Nov 2022 23:54:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:38cf02118dd5f875345011c712c01b337d93d6ba53ad405e554071971ddc96aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3532; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:93861bcaeec03b3ea77060e14e384d56bf43a20406a131547f741c9fb450ed9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4911489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d6c505fda05f49d5495b187a61f43d54e6d2c28f0b3ac8580cf7a0e3799058`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:fc8a71e7647a1153d30c11b86b96696357a82358286c206f04f09a1d0b01c26d in /nats-server 
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:56:36 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:56:36 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:56:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a241e0574e89ace91503f96ef69e43113479ea62d48263238c3278998139cfa7`  
		Last Modified: Wed, 02 Nov 2022 00:57:25 GMT  
		Size: 4.9 MB (4910981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4f5b84be1c29282b0d6580ec613179f0dcc5dc57cdbb562e6d613df08a24ae`  
		Last Modified: Wed, 02 Nov 2022 00:57:24 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:526012301d2a5498900afa30c7a2f2c1504d63000eaa9fbdb5110de20a97afa6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4678332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37c22cb1d3dae3bb00768485dea1a9ab57158c8b02017a0a46366aaf22ddc20`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:08:18 GMT
COPY file:bbc13cd2b910904563c88c430693025307c46d6a649c9c8bc65e4804db00de30 in /nats-server 
# Wed, 02 Nov 2022 00:08:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:08:19 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:08:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:08:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd0c038cbd2ad2c43ed500c9294ebd89b5275a293c403709e9c211465cfdef87`  
		Last Modified: Wed, 02 Nov 2022 00:09:56 GMT  
		Size: 4.7 MB (4677824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6a1f9044fd1eb13edd75e07c50e5c6e65f6b9e8e009180a73cc657481095a4`  
		Last Modified: Wed, 02 Nov 2022 00:09:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:ce273a7b73864fdddfc207bd265f8677afe39ef92c1cab2c06cba957bc99aa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4670550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2c93c2c0a5487edec047944085da7c0588d6fb522131ba60026d2ccaa77d42`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:21:26 GMT
COPY file:0566bc820f488437cfd3b1975d6edbcfffd3a48619964eca98d1e17a3ba034d0 in /nats-server 
# Wed, 02 Nov 2022 00:21:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:21:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:21:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:21:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cf37db33ebaa16eea964e96fb841d5dc472c329955da0d19b104026e4bbd9a9`  
		Last Modified: Wed, 02 Nov 2022 00:23:10 GMT  
		Size: 4.7 MB (4670042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c09ee262d1e8dc86b07fce75dc53eeaeb202174876aba05eddad97b3fda0f7a`  
		Last Modified: Wed, 02 Nov 2022 00:23:09 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3eb536b111d97bb89b35a9188e4c7ce6a5ec2f9ddad47f9c64ead1314b6d9fd4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4498550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa65ab166f9d05e530b3f151e35c31f992c2db9cf4e913dc8c8ffc33e3c486a5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:501b37b1133c20e9a1f4c5f4b27cb7c8dc0d825a0fc035df37aba209279077d8 in /nats-server 
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 01 Nov 2022 23:53:59 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 01 Nov 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 01 Nov 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:87c14cfbbbaa392bfe5b0af729955338eed477736790f057c64af1eef178e8e7`  
		Last Modified: Tue, 01 Nov 2022 23:54:49 GMT  
		Size: 4.5 MB (4498041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a40a934e5ce1a49e45b1fec3dc93c91173cc60d94ad49cbb23711e801f78685`  
		Last Modified: Tue, 01 Nov 2022 23:54:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:7a4708b3472be80d1090192110656adb3902f3152d5f8778fd96121e72d10c0b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111745442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc18527cfa55e481d723721cccdf73b138dee3173cb9aa2e42c27f5b3e1d0f0f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:19:03 GMT
RUN cmd /S /C #(nop) COPY file:65b3e40a5360689cebd70d8ad0bf1a0f64c10095a7245da46f8edce1b068ffce in C:\nats-server.exe 
# Wed, 02 Nov 2022 00:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc22e1d8ebc97d5b89ec9ff01a8ce44a7b760979db5f448526034afc5803ee48`  
		Last Modified: Wed, 02 Nov 2022 00:20:01 GMT  
		Size: 5.0 MB (4965227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8811e98534493c1911a5abfcd13fb711c59a30848835e3081054615ec5a9bab`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c0961ffa08780e8c5ec100d27acba026f5c7f83c078873964a4ddacd3bfa9`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da95ec42c571a9748d1810f3382600b7c8561a35ab1a3d3bb071bb583eb2d34`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a6a96d3a7442170ddfffa9f35c2d61c1f7ce3b2d2f338f51e3a5934c381c07`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:3a6a6e93d2fde4db16a35477ae17f68d184d37fb642982a233e0197f34035583
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:93861bcaeec03b3ea77060e14e384d56bf43a20406a131547f741c9fb450ed9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4911489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d6c505fda05f49d5495b187a61f43d54e6d2c28f0b3ac8580cf7a0e3799058`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:fc8a71e7647a1153d30c11b86b96696357a82358286c206f04f09a1d0b01c26d in /nats-server 
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:56:36 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:56:36 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:56:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a241e0574e89ace91503f96ef69e43113479ea62d48263238c3278998139cfa7`  
		Last Modified: Wed, 02 Nov 2022 00:57:25 GMT  
		Size: 4.9 MB (4910981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4f5b84be1c29282b0d6580ec613179f0dcc5dc57cdbb562e6d613df08a24ae`  
		Last Modified: Wed, 02 Nov 2022 00:57:24 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:526012301d2a5498900afa30c7a2f2c1504d63000eaa9fbdb5110de20a97afa6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4678332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37c22cb1d3dae3bb00768485dea1a9ab57158c8b02017a0a46366aaf22ddc20`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:08:18 GMT
COPY file:bbc13cd2b910904563c88c430693025307c46d6a649c9c8bc65e4804db00de30 in /nats-server 
# Wed, 02 Nov 2022 00:08:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:08:19 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:08:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:08:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd0c038cbd2ad2c43ed500c9294ebd89b5275a293c403709e9c211465cfdef87`  
		Last Modified: Wed, 02 Nov 2022 00:09:56 GMT  
		Size: 4.7 MB (4677824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6a1f9044fd1eb13edd75e07c50e5c6e65f6b9e8e009180a73cc657481095a4`  
		Last Modified: Wed, 02 Nov 2022 00:09:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ce273a7b73864fdddfc207bd265f8677afe39ef92c1cab2c06cba957bc99aa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4670550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2c93c2c0a5487edec047944085da7c0588d6fb522131ba60026d2ccaa77d42`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:21:26 GMT
COPY file:0566bc820f488437cfd3b1975d6edbcfffd3a48619964eca98d1e17a3ba034d0 in /nats-server 
# Wed, 02 Nov 2022 00:21:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:21:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:21:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:21:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cf37db33ebaa16eea964e96fb841d5dc472c329955da0d19b104026e4bbd9a9`  
		Last Modified: Wed, 02 Nov 2022 00:23:10 GMT  
		Size: 4.7 MB (4670042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c09ee262d1e8dc86b07fce75dc53eeaeb202174876aba05eddad97b3fda0f7a`  
		Last Modified: Wed, 02 Nov 2022 00:23:09 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3eb536b111d97bb89b35a9188e4c7ce6a5ec2f9ddad47f9c64ead1314b6d9fd4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4498550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa65ab166f9d05e530b3f151e35c31f992c2db9cf4e913dc8c8ffc33e3c486a5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:501b37b1133c20e9a1f4c5f4b27cb7c8dc0d825a0fc035df37aba209279077d8 in /nats-server 
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 01 Nov 2022 23:53:59 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 01 Nov 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 01 Nov 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:87c14cfbbbaa392bfe5b0af729955338eed477736790f057c64af1eef178e8e7`  
		Last Modified: Tue, 01 Nov 2022 23:54:49 GMT  
		Size: 4.5 MB (4498041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a40a934e5ce1a49e45b1fec3dc93c91173cc60d94ad49cbb23711e801f78685`  
		Last Modified: Tue, 01 Nov 2022 23:54:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:ebae1b3153e43950c72497335ab46f90f39daf9535fe9e09e2b99b40adfdbd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:nanoserver` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:7a4708b3472be80d1090192110656adb3902f3152d5f8778fd96121e72d10c0b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111745442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc18527cfa55e481d723721cccdf73b138dee3173cb9aa2e42c27f5b3e1d0f0f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:19:03 GMT
RUN cmd /S /C #(nop) COPY file:65b3e40a5360689cebd70d8ad0bf1a0f64c10095a7245da46f8edce1b068ffce in C:\nats-server.exe 
# Wed, 02 Nov 2022 00:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc22e1d8ebc97d5b89ec9ff01a8ce44a7b760979db5f448526034afc5803ee48`  
		Last Modified: Wed, 02 Nov 2022 00:20:01 GMT  
		Size: 5.0 MB (4965227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8811e98534493c1911a5abfcd13fb711c59a30848835e3081054615ec5a9bab`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c0961ffa08780e8c5ec100d27acba026f5c7f83c078873964a4ddacd3bfa9`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da95ec42c571a9748d1810f3382600b7c8561a35ab1a3d3bb071bb583eb2d34`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a6a96d3a7442170ddfffa9f35c2d61c1f7ce3b2d2f338f51e3a5934c381c07`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:ebae1b3153e43950c72497335ab46f90f39daf9535fe9e09e2b99b40adfdbd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:7a4708b3472be80d1090192110656adb3902f3152d5f8778fd96121e72d10c0b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111745442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc18527cfa55e481d723721cccdf73b138dee3173cb9aa2e42c27f5b3e1d0f0f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:19:03 GMT
RUN cmd /S /C #(nop) COPY file:65b3e40a5360689cebd70d8ad0bf1a0f64c10095a7245da46f8edce1b068ffce in C:\nats-server.exe 
# Wed, 02 Nov 2022 00:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:19:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc22e1d8ebc97d5b89ec9ff01a8ce44a7b760979db5f448526034afc5803ee48`  
		Last Modified: Wed, 02 Nov 2022 00:20:01 GMT  
		Size: 5.0 MB (4965227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8811e98534493c1911a5abfcd13fb711c59a30848835e3081054615ec5a9bab`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c0961ffa08780e8c5ec100d27acba026f5c7f83c078873964a4ddacd3bfa9`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da95ec42c571a9748d1810f3382600b7c8561a35ab1a3d3bb071bb583eb2d34`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a6a96d3a7442170ddfffa9f35c2d61c1f7ce3b2d2f338f51e3a5934c381c07`  
		Last Modified: Wed, 02 Nov 2022 00:20:00 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:3a6a6e93d2fde4db16a35477ae17f68d184d37fb642982a233e0197f34035583
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:93861bcaeec03b3ea77060e14e384d56bf43a20406a131547f741c9fb450ed9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4911489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d6c505fda05f49d5495b187a61f43d54e6d2c28f0b3ac8580cf7a0e3799058`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:fc8a71e7647a1153d30c11b86b96696357a82358286c206f04f09a1d0b01c26d in /nats-server 
# Wed, 02 Nov 2022 00:56:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:56:36 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:56:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:56:36 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:56:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a241e0574e89ace91503f96ef69e43113479ea62d48263238c3278998139cfa7`  
		Last Modified: Wed, 02 Nov 2022 00:57:25 GMT  
		Size: 4.9 MB (4910981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4f5b84be1c29282b0d6580ec613179f0dcc5dc57cdbb562e6d613df08a24ae`  
		Last Modified: Wed, 02 Nov 2022 00:57:24 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:526012301d2a5498900afa30c7a2f2c1504d63000eaa9fbdb5110de20a97afa6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4678332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37c22cb1d3dae3bb00768485dea1a9ab57158c8b02017a0a46366aaf22ddc20`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:08:18 GMT
COPY file:bbc13cd2b910904563c88c430693025307c46d6a649c9c8bc65e4804db00de30 in /nats-server 
# Wed, 02 Nov 2022 00:08:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:08:19 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:08:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:08:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:08:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd0c038cbd2ad2c43ed500c9294ebd89b5275a293c403709e9c211465cfdef87`  
		Last Modified: Wed, 02 Nov 2022 00:09:56 GMT  
		Size: 4.7 MB (4677824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6a1f9044fd1eb13edd75e07c50e5c6e65f6b9e8e009180a73cc657481095a4`  
		Last Modified: Wed, 02 Nov 2022 00:09:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ce273a7b73864fdddfc207bd265f8677afe39ef92c1cab2c06cba957bc99aa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4670550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2c93c2c0a5487edec047944085da7c0588d6fb522131ba60026d2ccaa77d42`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Nov 2022 00:21:26 GMT
COPY file:0566bc820f488437cfd3b1975d6edbcfffd3a48619964eca98d1e17a3ba034d0 in /nats-server 
# Wed, 02 Nov 2022 00:21:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 02 Nov 2022 00:21:27 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:21:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 02 Nov 2022 00:21:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 02 Nov 2022 00:21:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cf37db33ebaa16eea964e96fb841d5dc472c329955da0d19b104026e4bbd9a9`  
		Last Modified: Wed, 02 Nov 2022 00:23:10 GMT  
		Size: 4.7 MB (4670042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c09ee262d1e8dc86b07fce75dc53eeaeb202174876aba05eddad97b3fda0f7a`  
		Last Modified: Wed, 02 Nov 2022 00:23:09 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3eb536b111d97bb89b35a9188e4c7ce6a5ec2f9ddad47f9c64ead1314b6d9fd4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4498550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa65ab166f9d05e530b3f151e35c31f992c2db9cf4e913dc8c8ffc33e3c486a5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:501b37b1133c20e9a1f4c5f4b27cb7c8dc0d825a0fc035df37aba209279077d8 in /nats-server 
# Tue, 01 Nov 2022 23:53:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 01 Nov 2022 23:53:59 GMT
EXPOSE 4222 6222 8222
# Tue, 01 Nov 2022 23:53:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 01 Nov 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 01 Nov 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:87c14cfbbbaa392bfe5b0af729955338eed477736790f057c64af1eef178e8e7`  
		Last Modified: Tue, 01 Nov 2022 23:54:49 GMT  
		Size: 4.5 MB (4498041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a40a934e5ce1a49e45b1fec3dc93c91173cc60d94ad49cbb23711e801f78685`  
		Last Modified: Tue, 01 Nov 2022 23:54:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:c892e8d423eb9100e66d518f443dc34c909d61cbb9ddf3e915d1b2b01ebe751e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:5571861cd5b0f6018aa7855af4e2404c0ce18c6c84998469f37d20ff2b3c1904
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779175732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:531ff1eed7b103984ec29d81ea6f77943f8d3a711b1f4a6369022382a699d410`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:15:11 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.5/nats-server-v2.9.5-windows-amd64.zip
# Wed, 02 Nov 2022 00:15:17 GMT
ENV NATS_SERVER_SHASUM=86c963d3780234e6fecdaf72b9c89c9ecc2fc534d21c8e3ae855d0c062e41842
# Wed, 02 Nov 2022 00:16:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 02 Nov 2022 00:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 02 Nov 2022 00:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:18:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:18:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008b3979e40adbc80493c35e40a541ee0cd9f8cfb0d21f0dbb615b61a5800f3c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04f2cde91cfc04742cc431a646b0a0497d5cb0ac69c47f4530a16661f2eaca7`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf94dd1d2f43db680e22d0f214cd977185845f10df9bc06e7482c0eb43fb738`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a68e7f32692839720ce6bc41b42930a1fb73553533f3126fda5f90e7aacf45c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 358.3 KB (358324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db97038ec690106eede5d444866ae33a36d942485fd573db39c19207af3241e5`  
		Last Modified: Wed, 02 Nov 2022 00:19:42 GMT  
		Size: 5.3 MB (5305782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f237153f81ef2cffd83842993b4adbfa6bd1bc6e93f4775bef663d5564b28b8`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0660057acb9a90d1ec48107439058b6de0b482644e12a14859cda3f5db0fee4a`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596407afbadde38cf9b8f7a01869e6a2df90f9db2bfc93a669b60b263856927`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a537a0f8dced04ed22fcf2ceade81c6a0f2e2c1e31a8ece5416bb3673b5b7e9`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:c892e8d423eb9100e66d518f443dc34c909d61cbb9ddf3e915d1b2b01ebe751e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:5571861cd5b0f6018aa7855af4e2404c0ce18c6c84998469f37d20ff2b3c1904
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779175732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:531ff1eed7b103984ec29d81ea6f77943f8d3a711b1f4a6369022382a699d410`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:15:11 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.5/nats-server-v2.9.5-windows-amd64.zip
# Wed, 02 Nov 2022 00:15:17 GMT
ENV NATS_SERVER_SHASUM=86c963d3780234e6fecdaf72b9c89c9ecc2fc534d21c8e3ae855d0c062e41842
# Wed, 02 Nov 2022 00:16:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 02 Nov 2022 00:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 02 Nov 2022 00:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:18:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:18:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008b3979e40adbc80493c35e40a541ee0cd9f8cfb0d21f0dbb615b61a5800f3c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04f2cde91cfc04742cc431a646b0a0497d5cb0ac69c47f4530a16661f2eaca7`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf94dd1d2f43db680e22d0f214cd977185845f10df9bc06e7482c0eb43fb738`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a68e7f32692839720ce6bc41b42930a1fb73553533f3126fda5f90e7aacf45c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 358.3 KB (358324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db97038ec690106eede5d444866ae33a36d942485fd573db39c19207af3241e5`  
		Last Modified: Wed, 02 Nov 2022 00:19:42 GMT  
		Size: 5.3 MB (5305782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f237153f81ef2cffd83842993b4adbfa6bd1bc6e93f4775bef663d5564b28b8`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0660057acb9a90d1ec48107439058b6de0b482644e12a14859cda3f5db0fee4a`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596407afbadde38cf9b8f7a01869e6a2df90f9db2bfc93a669b60b263856927`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a537a0f8dced04ed22fcf2ceade81c6a0f2e2c1e31a8ece5416bb3673b5b7e9`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
