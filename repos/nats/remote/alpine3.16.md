## `nats:alpine3.16`

```console
$ docker pull nats@sha256:f576cdc17cc3141858482d6577d6421abd94c7851fafdab5c59c96659930af0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:abb4111e51c329aba5d98f59258cbcbe33991478a70ed25a4c1b5e53a05ab284
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8008197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e5b0f125c55e85f9377c37ccad41b4c8823a8ced89444e49d2166d23db46322`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 09:36:58 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 09:37:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 09:37:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 09:37:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 09:37:02 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 09:37:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 09:37:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507ba89941454589f6119633988d0cf9cdafa9f423297296bc7f140ee6f92a5b`  
		Last Modified: Sat, 12 Nov 2022 09:37:37 GMT  
		Size: 5.2 MB (5200925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5444e99a256eafd521f90c37406f1927399f8a67c7e2881ff3d5531dbe7ffb24`  
		Last Modified: Sat, 12 Nov 2022 09:37:36 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a95b178729cf92d60f3e9402a2bb72412bb6e4fd83677c30cb955ec7e6741c`  
		Last Modified: Sat, 12 Nov 2022 09:37:36 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:aa38aa991628755bb8f27826f3b5688534f871a528f92da8fd5060cdb62ab2c0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7578489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1113f11e09a3840e904549f317a6edc3242bbe3242accbe013893bd63b32342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:56 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:33:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:33:59 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:33:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad55ca795a2109e29efe113d38cf5be22960dc5d72cd19f2deceff57c63a987`  
		Last Modified: Sat, 12 Nov 2022 04:35:17 GMT  
		Size: 5.0 MB (4962411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247b15bed3a4ef31a4163c2d0311131d89ee6e01b7d331462d04b3d916b5260`  
		Last Modified: Sat, 12 Nov 2022 04:35:16 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c487b70d4a43929abb58108b5b9986c238bfc6980a9fb7ef7a56b5f2a93e375e`  
		Last Modified: Sat, 12 Nov 2022 04:35:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:b9d7fe7e72609803812d652259d2edc570eef1a502ddd9a5196fabaf5be71f22
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7375587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b9d7a4b7ce1875f953e199aa24125e40a17b202695250d370547c2530aee67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:24:55 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 05:24:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 05:24:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 05:24:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 05:24:57 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 05:24:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 05:24:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d793b22bfa9da173f6098e3853ecfbb6fadf5361e07945ddc42e79c480df8f6`  
		Last Modified: Sat, 12 Nov 2022 05:26:17 GMT  
		Size: 5.0 MB (4955825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c519ea5fd81d5245127313512123ea30983ad42361c0ecc55a97a0ccac08744d`  
		Last Modified: Sat, 12 Nov 2022 05:26:16 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19726f53fd806d5bcba2dda28bc3d3d5e0a2e5984992ec8ab6c53c1faeb4ea8b`  
		Last Modified: Sat, 12 Nov 2022 05:26:16 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:43063296b032bac846846e4e3dd9208c526aff3b7e3790e66fc18632d764d857
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1f0a1d44d037ccd570d9d7f6ac6a89d12392ecbd6230a4b767d8a6e55b0322`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:54 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:30:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:30:57 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:30:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:30:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c28a3b58a9a32866a0ce5ae0ea96429876fc6e4ddff42f869ae8c90151d137c`  
		Last Modified: Sat, 12 Nov 2022 04:31:29 GMT  
		Size: 4.8 MB (4786484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7cc2d315ec804021165c91007f9bfc3eb67ec28702a59b91256ad2f4e2171d`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a730c28724eff608a152b178885c260fb3bd8dbfd37a226282552a3937384b8`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
