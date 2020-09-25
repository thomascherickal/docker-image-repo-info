## `caddy:alpine`

```console
$ docker pull caddy@sha256:7367adca165f92427bf9f63732334d37213e92b1d8800da194dbd7bfbcb87452
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:alpine` - linux; amd64

```console
$ docker pull caddy@sha256:7210e033f1b7846a51ad4e7e0412f5eecff286aa706500698fbea1f89c316357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14632306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6f01784bcc9de68ae349a8c782c82c8d54f642f6cbadb2472567ea33e69cf0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:27:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:27:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:27:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:27:35 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:27:36 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:27:38 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:27:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5bea3a62f2eb8bdd91cf1d01de5e62aa88dbcd8e5834f5dd686a4f1a482531`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 5.8 KB (5761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863c6d72ce944f51161d2c13a01dde2210e77bb69c72cbd54e3125a34d60d899`  
		Last Modified: Fri, 25 Sep 2020 22:28:11 GMT  
		Size: 11.5 MB (11528869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e626bfeb2f84ef9a852704892ac16a98c0562469db9c76430725e5c18a998ddb`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c8ad488eec7c77aa1c7781b7a72a8d945481bdd0cb7ccb70880d9b925873048
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13780578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f98716bd7a8a9c2ef8aa29c6650238e67c38bdb8293c65fee78840359abf69`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:50:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:50:11 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:50:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:50:17 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:50:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:50:20 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:50:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:50:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:50:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:50:27 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:50:28 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:50:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdf9fef63ad932b076740c7fd4eac18d505c2e815b2b27093fae4a1037c1f83`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4febe5cd2333cc513bb8556e642ebf16c47e8b19d55ca0a5ea133b0ac51ffb6`  
		Last Modified: Fri, 25 Sep 2020 22:51:22 GMT  
		Size: 10.9 MB (10871161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a4a456aa5012b57a14ca79cf84c1fcadb9921dacbceabaa51276b470026164`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f7cf9f964eeea33eafd618e61be6df5924aeb7554b18ebf67553d7b6b4b87c4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13563595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9c246982f6b6958d5da2a3fd34536f8ac51c0bb7d8b9f5dac90402a50362ae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:58:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:58:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:58:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:58:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:58:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:58:40 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:58:40 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:58:41 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:58:42 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:58:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:58:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:58:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:58:51 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:58:51 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:58:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429f21378d6028fa7cda0d5b592cd8b633c405139cc47eee9863c2b21da4378b`  
		Last Modified: Fri, 25 Sep 2020 22:59:48 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93665bdf05fdd3470eab6a6ffbc672a036b9fd454b448b462f016d7ca8ef6948`  
		Last Modified: Fri, 25 Sep 2020 22:59:51 GMT  
		Size: 10.9 MB (10851606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff23fb2f1e176ebd5c38157ac164416de40bede15eda73c657fcd72ab44cbf4`  
		Last Modified: Fri, 25 Sep 2020 22:59:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:fd7be1e3e7e8f22025c4c7c932ed959e20a042800583b99d221d49210d2256b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13537918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdda1ab60a0a087288e1096da6b835d6d0492ace07c13f12b7ae57fc0aa31fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:18 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:40:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:40:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:40:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:40:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:40:26 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:40:27 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:40:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:40:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:40:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:40:33 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:40:34 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:40:35 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:40:35 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:40:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bbc79642b3dde186ddb45804729b84a8d010ca521d5c376311e2f613371675`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2737d74b46f3ab6089d70958b2003334d319108e095e574ccb5513b8df65957b`  
		Last Modified: Fri, 25 Sep 2020 22:41:26 GMT  
		Size: 10.5 MB (10523576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bccfced4019a7c0a8f4727d9564f261cc2cea2f152604c090c8e1534648917`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1f9ba55d19fd2ec980dbaeab620562f227dcf0d7ced312dc989d275783c346eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13288765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3fce9822eca46a2dd633cf719e3ed86a1381b29ecaf6869f8959e53899d0e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:41 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:09 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:38 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:47 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:42:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:42:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:42:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:42:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:42:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:42:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:42:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:42:53 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:42:59 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:43:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6899a5c1a337a29052e5f09180d092a86821dcf3d513b96fdf5db876ec3d6368`  
		Last Modified: Fri, 25 Sep 2020 22:45:34 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5fe5c56024bfb32687701ff11f9c64f76889469f8562abad35c6b11862a8cb`  
		Last Modified: Fri, 25 Sep 2020 22:45:35 GMT  
		Size: 10.2 MB (10175209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb09e4037c29b877b9d6dc22577ae3f8283f506d76525794858646d23a4c596`  
		Last Modified: Fri, 25 Sep 2020 22:45:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:aab2bff384d7eeaac65e97fe65c9f60f11a3515ae789192681455c483e7849d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14069343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036d0863bbc70fc945f1013ac5fc1b1ffa1f292eafc9e5cb9b6167ae03031199`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:41:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:41:44 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:47 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:48 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:41:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:41:50 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:41:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b62d245db5345045e7a29f409c7a0109545e93366793659a9538d863745398`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd84433ce0180dc40fb2dfc528d8186c247a35a24b5868a7b6065989bf0ee684`  
		Last Modified: Fri, 25 Sep 2020 22:42:26 GMT  
		Size: 11.2 MB (11196639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b4a42908e611c3b87202fd7fa709303806890837e261ae5a76d427925c7825`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
