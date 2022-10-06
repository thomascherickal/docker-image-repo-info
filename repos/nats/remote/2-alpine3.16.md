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
