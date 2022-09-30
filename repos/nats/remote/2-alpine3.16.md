## `nats:2-alpine3.16`

```console
$ docker pull nats@sha256:4b4a742e09bfa2c39b2b1f52d9bcc57c8ab9e32fb187e5048c11f3e341176418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:93b6c178034659b624ec39316bec9daeb14b38f690a531eaf5687c8f9a6420f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5068a20fcd0f44c75cc992b50a0c9406d62900af1d7756407b98f67a5aff6049`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:24:33 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:24:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:24:35 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:24:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cfb9d9ea4605961cdb87b6f9e44cdcfdf68501e6502197a61ba80d7fa2cf3`  
		Last Modified: Fri, 30 Sep 2022 00:25:27 GMT  
		Size: 5.2 MB (5191367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19aac431077ee9634be9f5879d95e018b853fe9f4355edfb009578928af4a8b`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d803ce9173785ad956d0980594d07b7c002d401ec4f7038696cea1a816f8eeba`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:1b1b13874064770ee71ee054d372744f61509858d4e2f0e728f4f7e3d0c96979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca1a0478849efea10188e490a19d87485a7e44be7adeb5a71abc150e21ad71b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:15:00 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:15:03 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:15:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e3a299d439ca160a2da5bc72a2fbdfe0d669e0251c6c9ca166ab1f6572234f`  
		Last Modified: Fri, 30 Sep 2022 00:16:18 GMT  
		Size: 5.0 MB (4954323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c24ad6cbf82b17aa717ce52a3630fce897bdc317f1cd90fa28a0b18ec0132`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569952349d4aaee564b407fc4a769f8afee1973b746dbc535f7ec1d82ee711f`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:43a4795e7153c524620b43f9cf744659f5f32f1eb37326b2259be4f06dc7a959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7367096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eadfdcca40f49ba08c9b57db4711db2b88b1027405154bb190abd16686cc4c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 22 Sep 2022 23:57:45 GMT
ENV NATS_SERVER=2.9.1
# Thu, 22 Sep 2022 23:57:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d0aa00133c68e3dd1c791272fe352ba5d5ec097c58991946c5a0e66e06fdca4c' ;; 		armhf) natsArch='arm6'; sha256='794267eb36c86034b8f800fda1a60019538ac79788ca3e060cbe737dcbe6e8b8' ;; 		armv7) natsArch='arm7'; sha256='22c9d0304daf83d8ed08431121f4e389954ea9447c39b407d07eee588ac31dc5' ;; 		x86_64) natsArch='amd64'; sha256='7d2d6a245f3c42b0ac5a75a6cf345235bef534a0baeabeb374b328e08b60a25b' ;; 		x86) natsArch='386'; sha256='f63cbffde08a8c6716a1dba464a52df48265186e8b0386a4815e7c549143599a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 22 Sep 2022 23:57:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 22 Sep 2022 23:57:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 22 Sep 2022 23:57:48 GMT
EXPOSE 4222 6222 8222
# Thu, 22 Sep 2022 23:57:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Sep 2022 23:57:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28148b83a7e0626bede5387abe8640718cde573f4e7e2fc013b181c07a8b21a`  
		Last Modified: Thu, 22 Sep 2022 23:59:04 GMT  
		Size: 4.9 MB (4949037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb4b374b15114a9cee11f09286b893ca3cc79d82fab81fb81921ca5969142ae`  
		Last Modified: Thu, 22 Sep 2022 23:59:03 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704470fff25768fb506edddc3efac7a081fbeb8c379a243a84a60554c121062e`  
		Last Modified: Thu, 22 Sep 2022 23:59:03 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:af501466b5b4748dd58d6a01314dc8b52929cc19ede83b48599b301569f1cfc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7483893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e0f52297bec9c9125da3427bf806b078a28bc0afc58dcf442110dc6f5455c18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 22 Sep 2022 23:40:04 GMT
ENV NATS_SERVER=2.9.1
# Thu, 22 Sep 2022 23:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d0aa00133c68e3dd1c791272fe352ba5d5ec097c58991946c5a0e66e06fdca4c' ;; 		armhf) natsArch='arm6'; sha256='794267eb36c86034b8f800fda1a60019538ac79788ca3e060cbe737dcbe6e8b8' ;; 		armv7) natsArch='arm7'; sha256='22c9d0304daf83d8ed08431121f4e389954ea9447c39b407d07eee588ac31dc5' ;; 		x86_64) natsArch='amd64'; sha256='7d2d6a245f3c42b0ac5a75a6cf345235bef534a0baeabeb374b328e08b60a25b' ;; 		x86) natsArch='386'; sha256='f63cbffde08a8c6716a1dba464a52df48265186e8b0386a4815e7c549143599a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 22 Sep 2022 23:40:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 22 Sep 2022 23:40:09 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 22 Sep 2022 23:40:09 GMT
EXPOSE 4222 6222 8222
# Thu, 22 Sep 2022 23:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Sep 2022 23:40:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08937f059ddd40b2696cabb3fc09473c8f136f25a55e1818bd8cd11177bb5b0`  
		Last Modified: Thu, 22 Sep 2022 23:41:12 GMT  
		Size: 4.8 MB (4775257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8b44164b339cf12c411012651587f34f3451b6c3161b0f6c18d64d2a28d84a`  
		Last Modified: Thu, 22 Sep 2022 23:41:12 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6a983c21365eff677a992cc5781a1ae47afd965f00abe6bd59ee79649c0c13`  
		Last Modified: Thu, 22 Sep 2022 23:41:12 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
