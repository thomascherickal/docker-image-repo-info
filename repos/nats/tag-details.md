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
-	[`nats:2.9.2`](#nats292)
-	[`nats:2.9.2-alpine`](#nats292-alpine)
-	[`nats:2.9.2-alpine3.16`](#nats292-alpine316)
-	[`nats:2.9.2-linux`](#nats292-linux)
-	[`nats:2.9.2-nanoserver`](#nats292-nanoserver)
-	[`nats:2.9.2-nanoserver-1809`](#nats292-nanoserver-1809)
-	[`nats:2.9.2-scratch`](#nats292-scratch)
-	[`nats:2.9.2-windowsservercore`](#nats292-windowsservercore)
-	[`nats:2.9.2-windowsservercore-1809`](#nats292-windowsservercore-1809)
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
$ docker pull nats@sha256:15bde806d8c135ca8a7a789530c3b5161e18e1f19ddfdbdf406e7736432e5968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3406; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:d6c92962d43c160cce9e24dde0e4788f762eaf0b5266f074cc7d85dda2eb6269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:71df66b207236cd907eb0beb1e74fea7fbc878937d9205d3973823e26458d214
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:790052334b67e37157a63c702821e5f4c0057ebdc221a323a74d6eb3d4c973b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:08:02 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 23:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 23:08:05 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:08:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72b599605c80147166a744d5aace3e9c34f50cbc78416059d48f5a1763e93e`  
		Last Modified: Thu, 06 Oct 2022 23:08:48 GMT  
		Size: 5.2 MB (5191377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42824359a649e4b243dd40103638fe7ce202ad8a3e64ae9f675f1575a1b6db`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7feb8eb8b712b8d5e4da1b5d434b56f4138fd50531deb1be40cae5acc10d5f0`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:85c672503d1215a58c6827b2cd3e7df1148ce29383784a0b5933f7f21fe6c939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff6e1498edb7d6bfc2558857cc2eab2d87ca36f3ca63891deecf31d9cc3eb16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:59:38 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 20:59:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 20:59:41 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:59:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d42068ce179e3552dc7a37baf291d30dca05c3b8e0d8483c47152ad7733e03`  
		Last Modified: Thu, 06 Oct 2022 21:00:52 GMT  
		Size: 5.0 MB (4954383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8d3ead1dd51d69a06b5270278f51d402937b1489767c3166f4815a6afefcad`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad27f5c47894f5e7041b7b29d19235924fbeda41839143e7bf48d0cbb075374`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:83484abdba02a228e9c6a108991021188e4878321ba9adc46f13e3534ac89990
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916074e87b4b8b556d435f2a48f9e2766fc0eeebef17bf6246c33975b8668c8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:34:09 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 22:34:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 22:34:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 22:34:14 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:34:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bbfe71df3a30e72fa617788e2443134d13258d259fed638d0502eea0e0f872`  
		Last Modified: Thu, 06 Oct 2022 22:35:18 GMT  
		Size: 4.8 MB (4776561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed2a39bad08dae24ff6cc3cb0eb7efa192b524fa6c0932c5e8f53773085769`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e410dcfcf3b7e6fe1fd25a07673b7a39428ea0830441bd7769ca9b2dcf5f7`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.16`

```console
$ docker pull nats@sha256:d6c92962d43c160cce9e24dde0e4788f762eaf0b5266f074cc7d85dda2eb6269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:71df66b207236cd907eb0beb1e74fea7fbc878937d9205d3973823e26458d214
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:790052334b67e37157a63c702821e5f4c0057ebdc221a323a74d6eb3d4c973b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:08:02 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 23:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 23:08:05 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:08:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72b599605c80147166a744d5aace3e9c34f50cbc78416059d48f5a1763e93e`  
		Last Modified: Thu, 06 Oct 2022 23:08:48 GMT  
		Size: 5.2 MB (5191377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42824359a649e4b243dd40103638fe7ce202ad8a3e64ae9f675f1575a1b6db`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7feb8eb8b712b8d5e4da1b5d434b56f4138fd50531deb1be40cae5acc10d5f0`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:85c672503d1215a58c6827b2cd3e7df1148ce29383784a0b5933f7f21fe6c939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff6e1498edb7d6bfc2558857cc2eab2d87ca36f3ca63891deecf31d9cc3eb16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:59:38 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 20:59:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 20:59:41 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:59:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d42068ce179e3552dc7a37baf291d30dca05c3b8e0d8483c47152ad7733e03`  
		Last Modified: Thu, 06 Oct 2022 21:00:52 GMT  
		Size: 5.0 MB (4954383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8d3ead1dd51d69a06b5270278f51d402937b1489767c3166f4815a6afefcad`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad27f5c47894f5e7041b7b29d19235924fbeda41839143e7bf48d0cbb075374`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:83484abdba02a228e9c6a108991021188e4878321ba9adc46f13e3534ac89990
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916074e87b4b8b556d435f2a48f9e2766fc0eeebef17bf6246c33975b8668c8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:34:09 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 22:34:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 22:34:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 22:34:14 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:34:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bbfe71df3a30e72fa617788e2443134d13258d259fed638d0502eea0e0f872`  
		Last Modified: Thu, 06 Oct 2022 22:35:18 GMT  
		Size: 4.8 MB (4776561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed2a39bad08dae24ff6cc3cb0eb7efa192b524fa6c0932c5e8f53773085769`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e410dcfcf3b7e6fe1fd25a07673b7a39428ea0830441bd7769ca9b2dcf5f7`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:e4828e278542dac16268f0886f5db9a68b28db92dc41b5c5fbadb3b9d2c3f8b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:e4828e278542dac16268f0886f5db9a68b28db92dc41b5c5fbadb3b9d2c3f8b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:15bde806d8c135ca8a7a789530c3b5161e18e1f19ddfdbdf406e7736432e5968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:d6c92962d43c160cce9e24dde0e4788f762eaf0b5266f074cc7d85dda2eb6269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:71df66b207236cd907eb0beb1e74fea7fbc878937d9205d3973823e26458d214
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:790052334b67e37157a63c702821e5f4c0057ebdc221a323a74d6eb3d4c973b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:08:02 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 23:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 23:08:05 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:08:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72b599605c80147166a744d5aace3e9c34f50cbc78416059d48f5a1763e93e`  
		Last Modified: Thu, 06 Oct 2022 23:08:48 GMT  
		Size: 5.2 MB (5191377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42824359a649e4b243dd40103638fe7ce202ad8a3e64ae9f675f1575a1b6db`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7feb8eb8b712b8d5e4da1b5d434b56f4138fd50531deb1be40cae5acc10d5f0`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:85c672503d1215a58c6827b2cd3e7df1148ce29383784a0b5933f7f21fe6c939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff6e1498edb7d6bfc2558857cc2eab2d87ca36f3ca63891deecf31d9cc3eb16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:59:38 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 20:59:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 20:59:41 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:59:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d42068ce179e3552dc7a37baf291d30dca05c3b8e0d8483c47152ad7733e03`  
		Last Modified: Thu, 06 Oct 2022 21:00:52 GMT  
		Size: 5.0 MB (4954383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8d3ead1dd51d69a06b5270278f51d402937b1489767c3166f4815a6afefcad`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad27f5c47894f5e7041b7b29d19235924fbeda41839143e7bf48d0cbb075374`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:83484abdba02a228e9c6a108991021188e4878321ba9adc46f13e3534ac89990
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916074e87b4b8b556d435f2a48f9e2766fc0eeebef17bf6246c33975b8668c8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:34:09 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 22:34:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 22:34:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 22:34:14 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:34:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bbfe71df3a30e72fa617788e2443134d13258d259fed638d0502eea0e0f872`  
		Last Modified: Thu, 06 Oct 2022 22:35:18 GMT  
		Size: 4.8 MB (4776561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed2a39bad08dae24ff6cc3cb0eb7efa192b524fa6c0932c5e8f53773085769`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e410dcfcf3b7e6fe1fd25a07673b7a39428ea0830441bd7769ca9b2dcf5f7`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.16`

```console
$ docker pull nats@sha256:d6c92962d43c160cce9e24dde0e4788f762eaf0b5266f074cc7d85dda2eb6269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:71df66b207236cd907eb0beb1e74fea7fbc878937d9205d3973823e26458d214
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:790052334b67e37157a63c702821e5f4c0057ebdc221a323a74d6eb3d4c973b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:08:02 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 23:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 23:08:05 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:08:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72b599605c80147166a744d5aace3e9c34f50cbc78416059d48f5a1763e93e`  
		Last Modified: Thu, 06 Oct 2022 23:08:48 GMT  
		Size: 5.2 MB (5191377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42824359a649e4b243dd40103638fe7ce202ad8a3e64ae9f675f1575a1b6db`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7feb8eb8b712b8d5e4da1b5d434b56f4138fd50531deb1be40cae5acc10d5f0`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:85c672503d1215a58c6827b2cd3e7df1148ce29383784a0b5933f7f21fe6c939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff6e1498edb7d6bfc2558857cc2eab2d87ca36f3ca63891deecf31d9cc3eb16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:59:38 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 20:59:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 20:59:41 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:59:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d42068ce179e3552dc7a37baf291d30dca05c3b8e0d8483c47152ad7733e03`  
		Last Modified: Thu, 06 Oct 2022 21:00:52 GMT  
		Size: 5.0 MB (4954383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8d3ead1dd51d69a06b5270278f51d402937b1489767c3166f4815a6afefcad`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad27f5c47894f5e7041b7b29d19235924fbeda41839143e7bf48d0cbb075374`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:83484abdba02a228e9c6a108991021188e4878321ba9adc46f13e3534ac89990
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916074e87b4b8b556d435f2a48f9e2766fc0eeebef17bf6246c33975b8668c8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:34:09 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 22:34:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 22:34:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 22:34:14 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:34:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bbfe71df3a30e72fa617788e2443134d13258d259fed638d0502eea0e0f872`  
		Last Modified: Thu, 06 Oct 2022 22:35:18 GMT  
		Size: 4.8 MB (4776561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed2a39bad08dae24ff6cc3cb0eb7efa192b524fa6c0932c5e8f53773085769`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e410dcfcf3b7e6fe1fd25a07673b7a39428ea0830441bd7769ca9b2dcf5f7`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:e4828e278542dac16268f0886f5db9a68b28db92dc41b5c5fbadb3b9d2c3f8b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:e4828e278542dac16268f0886f5db9a68b28db92dc41b5c5fbadb3b9d2c3f8b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2`

```console
$ docker pull nats@sha256:15bde806d8c135ca8a7a789530c3b5161e18e1f19ddfdbdf406e7736432e5968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9.2` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-alpine`

```console
$ docker pull nats@sha256:d6c92962d43c160cce9e24dde0e4788f762eaf0b5266f074cc7d85dda2eb6269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:71df66b207236cd907eb0beb1e74fea7fbc878937d9205d3973823e26458d214
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:790052334b67e37157a63c702821e5f4c0057ebdc221a323a74d6eb3d4c973b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:08:02 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 23:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 23:08:05 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:08:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72b599605c80147166a744d5aace3e9c34f50cbc78416059d48f5a1763e93e`  
		Last Modified: Thu, 06 Oct 2022 23:08:48 GMT  
		Size: 5.2 MB (5191377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42824359a649e4b243dd40103638fe7ce202ad8a3e64ae9f675f1575a1b6db`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7feb8eb8b712b8d5e4da1b5d434b56f4138fd50531deb1be40cae5acc10d5f0`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:85c672503d1215a58c6827b2cd3e7df1148ce29383784a0b5933f7f21fe6c939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff6e1498edb7d6bfc2558857cc2eab2d87ca36f3ca63891deecf31d9cc3eb16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:59:38 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 20:59:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 20:59:41 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:59:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d42068ce179e3552dc7a37baf291d30dca05c3b8e0d8483c47152ad7733e03`  
		Last Modified: Thu, 06 Oct 2022 21:00:52 GMT  
		Size: 5.0 MB (4954383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8d3ead1dd51d69a06b5270278f51d402937b1489767c3166f4815a6afefcad`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad27f5c47894f5e7041b7b29d19235924fbeda41839143e7bf48d0cbb075374`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:83484abdba02a228e9c6a108991021188e4878321ba9adc46f13e3534ac89990
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916074e87b4b8b556d435f2a48f9e2766fc0eeebef17bf6246c33975b8668c8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:34:09 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 22:34:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 22:34:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 22:34:14 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:34:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bbfe71df3a30e72fa617788e2443134d13258d259fed638d0502eea0e0f872`  
		Last Modified: Thu, 06 Oct 2022 22:35:18 GMT  
		Size: 4.8 MB (4776561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed2a39bad08dae24ff6cc3cb0eb7efa192b524fa6c0932c5e8f53773085769`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e410dcfcf3b7e6fe1fd25a07673b7a39428ea0830441bd7769ca9b2dcf5f7`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-alpine3.16`

```console
$ docker pull nats@sha256:d6c92962d43c160cce9e24dde0e4788f762eaf0b5266f074cc7d85dda2eb6269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.2-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:71df66b207236cd907eb0beb1e74fea7fbc878937d9205d3973823e26458d214
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:790052334b67e37157a63c702821e5f4c0057ebdc221a323a74d6eb3d4c973b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:08:02 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 23:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 23:08:05 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:08:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72b599605c80147166a744d5aace3e9c34f50cbc78416059d48f5a1763e93e`  
		Last Modified: Thu, 06 Oct 2022 23:08:48 GMT  
		Size: 5.2 MB (5191377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42824359a649e4b243dd40103638fe7ce202ad8a3e64ae9f675f1575a1b6db`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7feb8eb8b712b8d5e4da1b5d434b56f4138fd50531deb1be40cae5acc10d5f0`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:85c672503d1215a58c6827b2cd3e7df1148ce29383784a0b5933f7f21fe6c939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff6e1498edb7d6bfc2558857cc2eab2d87ca36f3ca63891deecf31d9cc3eb16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:59:38 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 20:59:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 20:59:41 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:59:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d42068ce179e3552dc7a37baf291d30dca05c3b8e0d8483c47152ad7733e03`  
		Last Modified: Thu, 06 Oct 2022 21:00:52 GMT  
		Size: 5.0 MB (4954383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8d3ead1dd51d69a06b5270278f51d402937b1489767c3166f4815a6afefcad`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad27f5c47894f5e7041b7b29d19235924fbeda41839143e7bf48d0cbb075374`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:83484abdba02a228e9c6a108991021188e4878321ba9adc46f13e3534ac89990
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916074e87b4b8b556d435f2a48f9e2766fc0eeebef17bf6246c33975b8668c8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:34:09 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 22:34:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 22:34:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 22:34:14 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:34:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bbfe71df3a30e72fa617788e2443134d13258d259fed638d0502eea0e0f872`  
		Last Modified: Thu, 06 Oct 2022 22:35:18 GMT  
		Size: 4.8 MB (4776561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed2a39bad08dae24ff6cc3cb0eb7efa192b524fa6c0932c5e8f53773085769`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e410dcfcf3b7e6fe1fd25a07673b7a39428ea0830441bd7769ca9b2dcf5f7`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-linux`

```console
$ docker pull nats@sha256:e4828e278542dac16268f0886f5db9a68b28db92dc41b5c5fbadb3b9d2c3f8b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-nanoserver`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9.2-nanoserver` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-nanoserver-1809`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9.2-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-scratch`

```console
$ docker pull nats@sha256:e4828e278542dac16268f0886f5db9a68b28db92dc41b5c5fbadb3b9d2c3f8b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-windowsservercore`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9.2-windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9.2-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:d6c92962d43c160cce9e24dde0e4788f762eaf0b5266f074cc7d85dda2eb6269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:71df66b207236cd907eb0beb1e74fea7fbc878937d9205d3973823e26458d214
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:790052334b67e37157a63c702821e5f4c0057ebdc221a323a74d6eb3d4c973b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:08:02 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 23:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 23:08:05 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:08:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72b599605c80147166a744d5aace3e9c34f50cbc78416059d48f5a1763e93e`  
		Last Modified: Thu, 06 Oct 2022 23:08:48 GMT  
		Size: 5.2 MB (5191377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42824359a649e4b243dd40103638fe7ce202ad8a3e64ae9f675f1575a1b6db`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7feb8eb8b712b8d5e4da1b5d434b56f4138fd50531deb1be40cae5acc10d5f0`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:85c672503d1215a58c6827b2cd3e7df1148ce29383784a0b5933f7f21fe6c939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff6e1498edb7d6bfc2558857cc2eab2d87ca36f3ca63891deecf31d9cc3eb16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:59:38 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 20:59:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 20:59:41 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:59:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d42068ce179e3552dc7a37baf291d30dca05c3b8e0d8483c47152ad7733e03`  
		Last Modified: Thu, 06 Oct 2022 21:00:52 GMT  
		Size: 5.0 MB (4954383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8d3ead1dd51d69a06b5270278f51d402937b1489767c3166f4815a6afefcad`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad27f5c47894f5e7041b7b29d19235924fbeda41839143e7bf48d0cbb075374`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:83484abdba02a228e9c6a108991021188e4878321ba9adc46f13e3534ac89990
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916074e87b4b8b556d435f2a48f9e2766fc0eeebef17bf6246c33975b8668c8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:34:09 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 22:34:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 22:34:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 22:34:14 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:34:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bbfe71df3a30e72fa617788e2443134d13258d259fed638d0502eea0e0f872`  
		Last Modified: Thu, 06 Oct 2022 22:35:18 GMT  
		Size: 4.8 MB (4776561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed2a39bad08dae24ff6cc3cb0eb7efa192b524fa6c0932c5e8f53773085769`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e410dcfcf3b7e6fe1fd25a07673b7a39428ea0830441bd7769ca9b2dcf5f7`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.16`

```console
$ docker pull nats@sha256:d6c92962d43c160cce9e24dde0e4788f762eaf0b5266f074cc7d85dda2eb6269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:71df66b207236cd907eb0beb1e74fea7fbc878937d9205d3973823e26458d214
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:790052334b67e37157a63c702821e5f4c0057ebdc221a323a74d6eb3d4c973b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:08:02 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 23:08:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 23:08:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 23:08:05 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:08:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a72b599605c80147166a744d5aace3e9c34f50cbc78416059d48f5a1763e93e`  
		Last Modified: Thu, 06 Oct 2022 23:08:48 GMT  
		Size: 5.2 MB (5191377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42824359a649e4b243dd40103638fe7ce202ad8a3e64ae9f675f1575a1b6db`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7feb8eb8b712b8d5e4da1b5d434b56f4138fd50531deb1be40cae5acc10d5f0`  
		Last Modified: Thu, 06 Oct 2022 23:08:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:85c672503d1215a58c6827b2cd3e7df1148ce29383784a0b5933f7f21fe6c939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff6e1498edb7d6bfc2558857cc2eab2d87ca36f3ca63891deecf31d9cc3eb16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:59:38 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 20:59:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 20:59:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 20:59:41 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:59:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d42068ce179e3552dc7a37baf291d30dca05c3b8e0d8483c47152ad7733e03`  
		Last Modified: Thu, 06 Oct 2022 21:00:52 GMT  
		Size: 5.0 MB (4954383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8d3ead1dd51d69a06b5270278f51d402937b1489767c3166f4815a6afefcad`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad27f5c47894f5e7041b7b29d19235924fbeda41839143e7bf48d0cbb075374`  
		Last Modified: Thu, 06 Oct 2022 21:00:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:83484abdba02a228e9c6a108991021188e4878321ba9adc46f13e3534ac89990
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916074e87b4b8b556d435f2a48f9e2766fc0eeebef17bf6246c33975b8668c8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:34:09 GMT
ENV NATS_SERVER=2.9.2
# Thu, 06 Oct 2022 22:34:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 06 Oct 2022 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 06 Oct 2022 22:34:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 06 Oct 2022 22:34:14 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:34:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bbfe71df3a30e72fa617788e2443134d13258d259fed638d0502eea0e0f872`  
		Last Modified: Thu, 06 Oct 2022 22:35:18 GMT  
		Size: 4.8 MB (4776561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed2a39bad08dae24ff6cc3cb0eb7efa192b524fa6c0932c5e8f53773085769`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e410dcfcf3b7e6fe1fd25a07673b7a39428ea0830441bd7769ca9b2dcf5f7`  
		Last Modified: Thu, 06 Oct 2022 22:35:17 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:15bde806d8c135ca8a7a789530c3b5161e18e1f19ddfdbdf406e7736432e5968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3406; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:e4828e278542dac16268f0886f5db9a68b28db92dc41b5c5fbadb3b9d2c3f8b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:nanoserver` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:e4828e278542dac16268f0886f5db9a68b28db92dc41b5c5fbadb3b9d2c3f8b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:2fc4d1c8a2712885129651633bdd213c5bb5dcb912d38302b08a7b70e9e7b42e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55143ff5b854445dd60e5e53664bce0ca2671d1c5e4ab5aa1c49dc10d38b521a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Thu, 06 Oct 2022 23:08:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 23:08:23 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 23:08:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 23:08:23 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 23:08:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d8d38665a16b2976bd0c59d31dfeafd94c13bbe50fdecda4df3e1f43f6ce9`  
		Last Modified: Thu, 06 Oct 2022 23:09:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4458cb2668004b0c75afea742d887ec189e06deb15e27c2eede54f701ee2045d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e862314d3d2559e998ad6f0a055310fe2a7625fc50b006fdbab40a48821cf1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Thu, 06 Oct 2022 20:59:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 20:59:51 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 20:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 20:59:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 20:59:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6d87d82f400ed0a9c4b08b92aa8e9aacfbed9d586b6e276392346aa2aecce5`  
		Last Modified: Thu, 06 Oct 2022 21:01:25 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:248659b214730aa4f17ad77f40d6de6ff17b92cc230be4ac8d734da10c333d27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d301488e86b33080fab2ac79a1f633d3ed7db3d26bc28035708c1e77b718464b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Oct 2022 22:34:25 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Thu, 06 Oct 2022 22:34:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 06 Oct 2022 22:34:27 GMT
EXPOSE 4222 6222 8222
# Thu, 06 Oct 2022 22:34:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 06 Oct 2022 22:34:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 06 Oct 2022 22:34:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e53bccfa1af888074ecb423a2285c59977062531adce07e120c21e1cf0aff76`  
		Last Modified: Thu, 06 Oct 2022 22:35:46 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
