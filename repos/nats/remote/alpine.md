## `nats:alpine`

```console
$ docker pull nats@sha256:45faf7fef5f78d815f712b8a05a2a0ded8793d777a0fb7640b0b0e6ff58e0009
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e995bfdd6f9247dbf1b305adc029a95e72e8630251d8d19a9023c63dcbc47318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7109895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae75c35e1d2e6f686fde0a0cfaea0aff2d58dcdf3e52a8ecba5ffc3dea3fe0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 02:48:29 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 02:48:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 02:48:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 02:48:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 02:48:35 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 02:48:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5abfce067d7bc34edb53d2ef3b851fb6750f2f165d88e6b7c1751a372637cf9`  
		Last Modified: Fri, 27 Aug 2021 02:50:40 GMT  
		Size: 4.5 MB (4482575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915f8f45a2be36433373b63850ff3ca8ec9eb622ab7d74dd908284a971539307`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcbfc2ac16592f5503b1b3f59404245367a0082b75af6bd79a2b48e8c45a762`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
