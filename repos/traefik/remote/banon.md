## `traefik:banon`

```console
$ docker pull traefik@sha256:426f5d4e1432a1d1780a0fe081715d70c667345df1e50b02be57872f3e410628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:banon` - linux; amd64

```console
$ docker pull traefik@sha256:3eaf50b7874f63567ee5d18498536928faef199302c805cb6b766e06b649302d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33416269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6de8578b2384107d9e08f90be5d6cf43472e369ba98dca46373b336b83fdbd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:18 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:18 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62b4fe8af5e2bd23c9c1a5303b1d320706bc52330058f23c4725df3dadc9cad`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 673.4 KB (673371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b954c2c3b6c35a716c65a53d1bb120db920d2cdc90267d260674af3965a5b68`  
		Last Modified: Fri, 07 Oct 2022 04:22:00 GMT  
		Size: 29.9 MB (29919018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857fadab46062ec62a3b8f3183843ff14b05f3ec377ccbe51a5296f86eacce5f`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm variant v6

```console
$ docker pull traefik@sha256:95960ed785badbe47cd0ec5bfc0833db6502043a7c83d1a14fa495615bd7dbd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31543171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1030c56c08192fde82ebb2fef3c8b57f7d8d340ac8463f7e563f4637caa60a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 03 Oct 2022 22:49:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 03 Oct 2022 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 03 Oct 2022 22:49:33 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:49:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 03 Oct 2022 22:49:33 GMT
CMD ["traefik"]
# Mon, 03 Oct 2022 22:49:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ecdfbf7665eeb46df55d94a2322221d8d1de9cebdc0f97c05affd0aa619f0`  
		Last Modified: Thu, 11 Aug 2022 01:15:26 GMT  
		Size: 686.0 KB (686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d29799c16bfd82dab22b9850857fb3488e2dc721c763c4bcc4fde280c30872`  
		Last Modified: Mon, 03 Oct 2022 22:50:37 GMT  
		Size: 28.2 MB (28225634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ee8605f9b04da07ee4ce0161573fc9e64faccb9a768733f7222a40ad141c2`  
		Last Modified: Mon, 03 Oct 2022 22:50:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3e90150cae10bbf88c2c186563c6307a0a4e7d169d2f640ac04fdda6b08b9b36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb461c4c2d15f33277f220c17547fd45eb0d588862147433c0d11afe2bfc1c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:38:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:38:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:38:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:38:56 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:38:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:38:58 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:38:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e179f025e9fd053dccf5cf01e48636e8a4fa642091186bc0a736693adbc34f`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 673.7 KB (673749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b59dd829100bd144172d2c8d6fa0e5c7c4b18b3f5e621012734841e8b803f7`  
		Last Modified: Fri, 07 Oct 2022 07:40:11 GMT  
		Size: 27.3 MB (27311746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7e56d00862713d11472648e728636220fa3aab656c706e800aba3b9be7687`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; s390x

```console
$ docker pull traefik@sha256:86ff93cc178de9b8f86436b83bc6e896c65edb55cda098b94882253afdd3eb1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32112411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0174719729d126f9205e2bd2f9d55bdd430ac98c573cb2f2b92d2e5c12bcf9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 09:57:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 09:57:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 09:57:11 GMT
EXPOSE 80
# Fri, 07 Oct 2022 09:57:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 09:57:12 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 09:57:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a1ec6f28225d3ff13bc2defe049a19ceecab6d949a0e69884c44e7e28279b`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 677.5 KB (677512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1d229f8b015fe7609ece81d9725b607d8ca5314d0f08667adfd7c13a5d5daf`  
		Last Modified: Fri, 07 Oct 2022 09:57:46 GMT  
		Size: 28.8 MB (28828444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd924ce12d473d0268c58ca23de4965014be194f51da2ab5fa66fbb94384d8e5`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
