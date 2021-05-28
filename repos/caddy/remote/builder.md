## `caddy:builder`

```console
$ docker pull caddy@sha256:62214ca98a775d99cd2629949585cb6859b130ce63a5482da19c29decef68626
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:f1d6333d641bfcbc8116821658cc929a658ae32e5d6729608c5bc7bf494b0ab7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116541076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357afcbcbb21ec9cc947a25ef58aa47cd2e00dc0adcaeda6cf3eaedd9b32e832`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:18:07 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:05 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:07 GMT
WORKDIR /go
# Fri, 07 May 2021 01:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:56:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 24 May 2021 18:23:21 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:23:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 24 May 2021 18:23:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 24 May 2021 18:23:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 24 May 2021 18:23:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e7595549f7536d76f08a8a23fb67e3e6fae08ccf3add715c5c1c956f9445d2`  
		Last Modified: Thu, 06 May 2021 23:29:42 GMT  
		Size: 105.7 MB (105745828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df88182f7acff97ffde9f614a0fd86e8a26590e445aa76e442c3a79d9e4c4f4`  
		Last Modified: Thu, 06 May 2021 23:29:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d573d19fd03835237c7687f4f394fa6b1fc1c894a901f2853846256ee7746eb`  
		Last Modified: Fri, 07 May 2021 01:56:57 GMT  
		Size: 6.4 MB (6390123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c2dad00b2cd9137d40a9eb5dd52c93d260659deaf25fdc60a401bbe90e42aa`  
		Last Modified: Mon, 24 May 2021 18:24:01 GMT  
		Size: 1.3 MB (1311168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d7791c92a2caa821eb568fa690da9bccf062429160aa44ae2918f33c8b6f31`  
		Last Modified: Mon, 24 May 2021 18:24:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f845c871e33f6c3255f4f7d019f1662d36c712f735af2744902ffb5fcc146776
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112278587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5a3d9387880aac52af7a922864bf5182d48329c94e6db9f266640a2c5df5609`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:00:55 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:01:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:01:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:24:09 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 21:27:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 21:27:32 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 21:27:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:27:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 21:27:35 GMT
WORKDIR /go
# Wed, 26 May 2021 17:34:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 26 May 2021 17:34:49 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 26 May 2021 17:34:49 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 17:34:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 26 May 2021 17:34:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 26 May 2021 17:34:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 26 May 2021 17:34:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4dea9fd179326b36ea137aad07e06571ffe7ad849e2a13a32354dcfd5d858d`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 281.4 KB (281379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abeb04d84d23abf8470fc95982483a9117a87e55b13c591f5332a460a5233bb`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3721aaa7ffedbec829a557c2d5f99c4661695a51f82632ece4df509b71bc1`  
		Last Modified: Thu, 06 May 2021 21:38:30 GMT  
		Size: 101.9 MB (101925593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298c78bc6b40a671a2f9a64d2cecf253acd10da30924ff687012e02b0307a1a8`  
		Last Modified: Thu, 06 May 2021 21:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882c72e30e7afaacf468b457b8d426d45390b7cf9900c7ba1d592ad8f3c82d54`  
		Last Modified: Wed, 26 May 2021 17:36:33 GMT  
		Size: 6.2 MB (6227097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee74fe4fee80b8596faf1972b5fd89fe534f70d016661f6a841c73f90814f10d`  
		Last Modified: Wed, 26 May 2021 17:36:32 GMT  
		Size: 1.2 MB (1221673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7058461038a87e3fd2ae23f02715aa5b8a39d363208bc0fc1d2f1b8a13fab45`  
		Last Modified: Wed, 26 May 2021 17:36:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8ff9b9d3421d81fcde2b0f225cb0ec5c57113c2c8779b925685168b9c445e4f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111227446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33be917e9f3a75cf094b073a4991144b088bec44378401c5291c2e58feaff4cf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:00:38 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:01:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:01:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:11:51 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:15:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:15:25 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:15:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:15:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:15:29 GMT
WORKDIR /go
# Wed, 26 May 2021 10:59:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 26 May 2021 10:59:47 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 26 May 2021 10:59:47 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 26 May 2021 10:59:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 26 May 2021 10:59:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 26 May 2021 10:59:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 26 May 2021 10:59:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb6bd423db0b63fdc83c72eae7ef401cb2fb9eaa63961c71a867ff26bfe422f`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 280.5 KB (280532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835b667ae68ff940439602ffbabae6e923c687cb56c62a793f23ddca67584049`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5b93a32354ff48887c2e9c4540875b8aa57822ab5c261d95e3c186d27b5c5e`  
		Last Modified: Thu, 06 May 2021 23:28:23 GMT  
		Size: 101.7 MB (101743890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2925b4cee8520caf8150ba3410d1306c50fa326f2fd920488f9e432578fda5`  
		Last Modified: Thu, 06 May 2021 23:27:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704039826a00936d145d8144698d0604e64e325fe6db70f9133f045c9e7a40a7`  
		Last Modified: Wed, 26 May 2021 11:01:29 GMT  
		Size: 5.6 MB (5558661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d917f3583cb3c82edd3cb2e7fa2aa57f79f962d90b759d5d36b24b03c550a53a`  
		Last Modified: Wed, 26 May 2021 11:01:29 GMT  
		Size: 1.2 MB (1219503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2925261ab1b2fbc5d231fcbc8fdfe82ba4b2e122ccd03a06635e05fd50f6b12c`  
		Last Modified: Wed, 26 May 2021 11:01:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9e63193d589111dbbbddfc06e3e97a1bcb1a0136692f3368acc42c562a471626
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111769632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a960c1f125595c92ed07dec6842855feac639cf9a4372533d2381af4c0c44692`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 22:17:28 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 27 May 2021 22:17:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 22:17:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 May 2021 22:17:29 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 27 May 2021 22:18:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 27 May 2021 22:18:49 GMT
ENV GOPATH=/go
# Thu, 27 May 2021 22:18:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 May 2021 22:18:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 27 May 2021 22:18:50 GMT
WORKDIR /go
# Fri, 28 May 2021 12:47:39 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 28 May 2021 12:47:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 28 May 2021 12:47:39 GMT
ENV CADDY_VERSION=v2.4.1
# Fri, 28 May 2021 12:47:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 28 May 2021 12:47:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 28 May 2021 12:47:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 28 May 2021 12:47:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088b5b3c5c0fab79ca41c188d3696a5053778b6c7d602b2aea8084c094608d1`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 281.5 KB (281495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7225fbf94c881dc50b56f5430522fbde8891efa801909d5d9f06261d839cc5`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0040e77a749aa5d95d68f3a9082e206235be5f12e0def7ec7fad9d1bf40e03`  
		Last Modified: Thu, 27 May 2021 22:27:00 GMT  
		Size: 101.1 MB (101089836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a411022a3ea7262d78e11400744e746cf37c77ebdfad3f45c711d635b29e8b2c`  
		Last Modified: Thu, 27 May 2021 22:26:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c8c6dcc536352f1e0b5519fde4e18d6f31c8eb70b81cab8eebd62e8ba1f036`  
		Last Modified: Fri, 28 May 2021 12:48:36 GMT  
		Size: 6.5 MB (6484023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb48cd568d9be4d77da09a0dbed2a1c57e9fc05ceaa6e156e55dfb6e5e8a199`  
		Last Modified: Fri, 28 May 2021 12:48:35 GMT  
		Size: 1.2 MB (1201540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c252c1f483168c461413751eb353a86cf6a7fba145a4e18eea8e1e1ee8af4c1`  
		Last Modified: Fri, 28 May 2021 12:48:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:caf238ee0f7dd40348c019981d8c9afca4dd049746fb8b3ce2887e52ab7879a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110621063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e2fa9c39856cb33440ae51b4e093d9987c613941af358a67354d13cdecf8b66`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:22:47 GMT
ENV GOLANG_VERSION=1.16.4
# Fri, 07 May 2021 00:25:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 07 May 2021 00:25:26 GMT
ENV GOPATH=/go
# Fri, 07 May 2021 00:25:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:25:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 May 2021 00:26:14 GMT
WORKDIR /go
# Fri, 07 May 2021 08:19:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 08:19:57 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 24 May 2021 18:22:40 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:22:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 24 May 2021 18:23:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 24 May 2021 18:23:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 24 May 2021 18:23:11 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d2e93731067b7b48232c826d062ff4fead572dbd98e0a28642db4802342a8e`  
		Last Modified: Fri, 07 May 2021 00:41:39 GMT  
		Size: 99.5 MB (99528032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0e521f95ca5f22fdd4b7917d06aead7df46288885c4fd3ffac0242b96643f`  
		Last Modified: Fri, 07 May 2021 00:41:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9dfa7e81a349fea3e170fbc6f6b9fd3245ee43c53b329a3ae72c9e5ebaddfb`  
		Last Modified: Fri, 07 May 2021 08:22:18 GMT  
		Size: 6.8 MB (6825232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d625a64da01cdb8fe6937a0686a8ff67ceb166adaac170808eb99b4edcc146`  
		Last Modified: Mon, 24 May 2021 18:23:49 GMT  
		Size: 1.2 MB (1170527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1204a6a5f0176b47c8fbc0ec6d80dbfe006135b462867ab000d1b98a2a06c78b`  
		Last Modified: Mon, 24 May 2021 18:23:49 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:afc016693cd73b017fde1ca24659532c594a7bd83ae71e69763a6b3e7e4e3b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115474412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c16686c325c496393f12e7cffacedb198ec1c583fc5896c84c61a98518271ba1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:16:38 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:18 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:21 GMT
WORKDIR /go
# Fri, 07 May 2021 02:02:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:02:35 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 24 May 2021 17:42:04 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 17:42:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 24 May 2021 17:42:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 24 May 2021 17:42:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 24 May 2021 17:42:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dab17b6808078a43afd3d62f1a202857192406e914c33d5ceb5eec1eb05eeb`  
		Last Modified: Thu, 06 May 2021 23:34:08 GMT  
		Size: 104.8 MB (104849388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6059cb089a1bd1108012ddff056f297d814995f95d29d57b15c13d11baede00d`  
		Last Modified: Thu, 06 May 2021 23:33:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84919c1c43955cfb518f179d4f6b541cdfa94579f6f6ef10fdc6e6b3ca4d51a3`  
		Last Modified: Fri, 07 May 2021 02:03:18 GMT  
		Size: 6.5 MB (6475416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9404b24d3fe49a849d0b85fb51abe7d31dc7bf808801d812ad3cd1f5214a6197`  
		Last Modified: Mon, 24 May 2021 17:42:45 GMT  
		Size: 1.3 MB (1264531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e30272b667f3a3c5f48e8b44cec4b2ca1ee2e297780ae37b90a1dbfa446f6`  
		Last Modified: Mon, 24 May 2021 17:42:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:dbfd49e31834bf104bf4f52dd70844272ac6001de57d44c69c605e40068d7aa0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646082577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950a48168b131a24b0cd41fa54d0bb9fa9baa4cbacc4cef550b2bc67925336d4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:26:03 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:28:52 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:28:54 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:01:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:01:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 24 May 2021 18:19:30 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:19:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 24 May 2021 18:19:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 24 May 2021 18:20:00 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421c063618ce27e648851fb286affe0950f7139e757b3df32c000a57be356623`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a33f0b9cbc9b02b55024fe76b7bac201d2b1037026b89c771078012fd84461`  
		Last Modified: Wed, 12 May 2021 12:54:46 GMT  
		Size: 139.3 MB (139340646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0884ee5b71061eefa8cabccdfeea059b656359a6ebc477d6f43284bccbd2057`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388dabb05e13f4119ef08ddb7ab1531da945ae5934f70bf1ead828148c77e9b0`  
		Last Modified: Wed, 12 May 2021 20:07:41 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39998044c69992575089510bbe2da6af14ac95b838cdd6ff78ded4896c641cb`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587cc65ea1b6c91915c81424d0599bd2aa48865018c44ba9de874f1f9db1b754`  
		Last Modified: Mon, 24 May 2021 18:23:41 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf0ac59e42b9f8d046f7911683ea53ad1c404df591a45e9a4ac89b9982f65fb`  
		Last Modified: Mon, 24 May 2021 18:23:41 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a4738133b86db0435f5acd7b0af60e3245e5add085bea2c6dd0bc1340bd2b`  
		Last Modified: Mon, 24 May 2021 18:23:44 GMT  
		Size: 1.7 MB (1732041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2cf4d3a8873d041f1605fe9b471eae135c06d51cd95480ad52598e2a53c6d5`  
		Last Modified: Mon, 24 May 2021 18:23:42 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:720d9e386ec0d8e76a8a135e2422f7edbfd3838d9c27e6ea6e4f2a2e0e18110c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988476112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e769ccbb03ee6c0eab147d2b597b0853321655b026df4231f63f5266892eb39`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:33:11 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:37:08 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:37:10 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:02:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:02:17 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 24 May 2021 18:20:08 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:20:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 24 May 2021 18:21:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 24 May 2021 18:21:37 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d753db33d9475a781a71db67226b6c2805f1e71108748b94dfdd610bb33137d`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16cf5cfefdc254a6ea68d79ebf521696de46090dd4d38c207ff2e301ff621d2`  
		Last Modified: Wed, 12 May 2021 12:55:48 GMT  
		Size: 149.2 MB (149178430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924854b0100f624a921d0d3d2922ca97fd7cca3d49cdc1dd677d10f628a122c`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d1201ff9263b27c3203fb740b420dfc811d03d441859aefe187732f9f4f54`  
		Last Modified: Wed, 12 May 2021 20:08:00 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ea4eae8e32e10e3ec07876a089c1bc058b7360f4cbe858bb6555f86da0b198`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda8f5ffb0b7c85547351f95a0039858879defbd257658f2d5562901c14e692e`  
		Last Modified: Mon, 24 May 2021 18:23:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2524c38952768fcd8503ffbcd6b5c3494480e3e95ec71e4e4fd3cfa5e05c78ab`  
		Last Modified: Mon, 24 May 2021 18:23:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8110088623447f637fdd1087b533db1edbd3dbab67f2a686de22582461cd99`  
		Last Modified: Mon, 24 May 2021 18:24:06 GMT  
		Size: 7.0 MB (7042281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34ca45a6484361983c9f1fa4ffd6dbeeb866cecc5baca55d06fe6736911c356`  
		Last Modified: Mon, 24 May 2021 18:23:58 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
