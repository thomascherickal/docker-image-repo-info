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
