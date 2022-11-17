## `nats:alpine`

```console
$ docker pull nats@sha256:400adfffe0df7f2df0e76d34d6e25a0fb8eb68cfdc10d404afbbb31f818d0276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:d4698031a0afeb1ed37b240a9632b22a2d0fcea5fd48af3c8b28e1eba3348033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8014859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c26ee116aa283ae59469d995e49cce15bb982559c777e32f06933e315898c54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:21:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:21:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:21:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:21:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94acb566bf3ae8a5a3c0747075e8b16df167a9694bfb5ac6ccdea4e5558e2a01`  
		Last Modified: Thu, 17 Nov 2022 20:22:12 GMT  
		Size: 5.2 MB (5207590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e759e667a2c2d6d67aaf3491e124f07a1afc8de774d7973958b32b81ff7a0304`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e8173963a2be8b30df5827fcfc01a70e5c95ab186696e43d9f624884cee41`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:221c14c269fed109042c154935b6cd22b270dda8b66b30e48f734f5fb50ffb87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8f37497160e12532b20e7eaca7e50daa1304f46b7002848dfae699b06743ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:49:34 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:49:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5728111a27515c16eb46117bf3339ccefc8af39e7c1508951d9286a3c3891c`  
		Last Modified: Thu, 17 Nov 2022 20:50:52 GMT  
		Size: 5.0 MB (4970331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e171e5c82f413b32d409f4fce9c56e3a429da91e068be34239e7c8c856576`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699b733f623013826c3dee6862aac2f7cb12bc97712d445dcf79191ba87875f6`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:bf2175af45ce04af8a4d8a8c810eb98dbbdf0208010f248234803a56346e7492
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af540a578654dbc22e31a00269e904f93dae199d3a57c7b588311595cd8c326c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:57:48 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6aab4ebcc741288db0b5a719ef99f393d0fd90552b7131f9391a1f1bb37575`  
		Last Modified: Thu, 17 Nov 2022 20:59:09 GMT  
		Size: 5.0 MB (4960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4be9c1201790ef36f0543a1ad75a874f321b98fb2053e0b742e2f74e72338e`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f34e641f8406d256e755f8e058c5e957c85a985209c0e0021a18e1aab450c9`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:173181d8057b550ed4e321336b885f0ada263273ebc6cba24563f43578c00c23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f949bc183512a9594a4bcf404727a905c6e76f0ac0318a03cf0e2b93ccf1de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:40:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:40:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:40:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46474a86907df61c3b68bfcfc04ccf1b583ae765e82a80c581951fb9f5e8a104`  
		Last Modified: Thu, 17 Nov 2022 20:41:10 GMT  
		Size: 4.8 MB (4794340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf9fbe300cc2e491de01ad75e29bc228c5e706a5140594a1c29c565216b00e`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323da261341d5d9bbcca4222e4b1c77ff87a4bd0aae38eb7e003bc530717bd2`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
