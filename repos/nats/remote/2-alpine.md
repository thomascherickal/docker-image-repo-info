## `nats:2-alpine`

```console
$ docker pull nats@sha256:ba1d3d9564004a89ee20c34f019afcd3683d3221c80602ec95d02e05de5b0aa3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:80f0115de5ee5eb05c78d116eea70cc91aee8fc32a5c590ce7adc083c0ed7c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a3efc6783d934886d9905c35144b3edde805a1f6aadc4e6c520d174a9f1bae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:30:43 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:30:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:30:45 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:30:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc8a4f20a4a5fcb0d7931643204ebba48c8b1b9d6e35cc8b7a43ed267c61a8`  
		Last Modified: Fri, 04 Nov 2022 23:31:19 GMT  
		Size: 5.2 MB (5200906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c061571ab8afcf042cf8999f76ddd700b1f57e48dff2c7e8f0da290ac5870dbe`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e00ff4dd8efc7f40b28e5596b4244c34d719a2d58cec452a23b8e9102b36768`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

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

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9d1bbd448681d703ae510eb6c66dd1b52caf6c36cf08c60a23e9c9e394fdb172
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ab836153e13c3b80d353fdb184e2aa87ca3941b1e99c723fe5bc5a7fbb7baff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 07:15:38 GMT
ENV NATS_SERVER=2.9.6
# Fri, 11 Nov 2022 07:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 11 Nov 2022 07:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 11 Nov 2022 07:15:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 07:15:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f95c291632d48fb04d9cab8d57481a5abad1904dc3a50688ec8f58978d50dba`  
		Last Modified: Fri, 11 Nov 2022 07:17:02 GMT  
		Size: 5.0 MB (4955786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88c6a29511fb518b9e2a560419f0f105a425785049f1ba3b57cf7f3dcf6c63`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a778afa5e25157008d7402637f36cfa4f216f2a5f72e87b7848744a0f40f23`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

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
