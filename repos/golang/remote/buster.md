## `golang:buster`

```console
$ docker pull golang@sha256:6be60119fd752c3ee530cb13f778801af1519a6b40e58539545c546d6e04b610
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:buster` - linux; amd64

```console
$ docker pull golang@sha256:a33d71b6c2bbd1397b1e906c3f7df0a645477d7249f1f034513f1cf4f38ed216
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.9 MB (288923192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e92e76829029d02333d58c05805586b9a8c9049dab54ba4b2459d2f6f2e443c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:24 GMT
ADD file:9d769df745075dbc4cd2c01ca784571a0df008f6b650b895a7f92d3281132807 in / 
# Tue, 23 May 2023 01:20:25 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:50:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:50:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 16:05:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 16:05:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 16:05:14 GMT
ENV GOLANG_VERSION=1.20.4
# Tue, 23 May 2023 16:05:22 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.4.linux-amd64.tar.gz'; 			sha256='698ef3243972a51ddb4028e4a1ac63dc6d60821bf18e59a807e051fee0a385bd'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.4.linux-armv6l.tar.gz'; 			sha256='0b75ca23061a9996840111f5f19092a1bdbc42ec1ae25237ed2eec1c838bd819'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.4.linux-arm64.tar.gz'; 			sha256='105889992ee4b1d40c7c108555222ca70ae43fccb42e20fbf1eebb822f5e72c6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.4.linux-386.tar.gz'; 			sha256='5dfa3db9433ef6a2d3803169fb4bd2f4505414881516eb9972d76ab2e22335a7'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.4.linux-ppc64le.tar.gz'; 			sha256='8c6f44b96c2719c90eebabe2dd866f9c39538648f7897a212cac448587e9a408'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.4.linux-s390x.tar.gz'; 			sha256='57f999a4e605b1dfa4e7e58c7dbae47d370ea240879edba8001ab33c9a963ebf'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.4.src.tar.gz'; 		sha256='9f34ace128764b7a3a4b238b805856cc1b2184304df9e5690825b0710f4202d6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 23 May 2023 16:05:23 GMT
ENV GOPATH=/go
# Tue, 23 May 2023 16:05:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 16:05:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 23 May 2023 16:05:24 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c722db24a050621ee87ea07acd5d066d3d6a94737c32012f27d73a1ad5cc645c`  
		Last Modified: Tue, 23 May 2023 01:24:26 GMT  
		Size: 50.4 MB (50448716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f8e4a0ed530ff1c74aea38be7ec6c725334c7c3a551b417d0f6f9e220a36fb`  
		Last Modified: Tue, 23 May 2023 01:57:08 GMT  
		Size: 17.6 MB (17580817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a739c67a76c3ff201aa979efc9c5deb081a75f5b98390ee176315cb0cb582aa9`  
		Last Modified: Tue, 23 May 2023 01:57:23 GMT  
		Size: 51.9 MB (51878369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb598b4d44cfeea9b42d52f82a4c3ca64bc6044d2264a04c5047a7a3d34e796b`  
		Last Modified: Tue, 23 May 2023 16:06:59 GMT  
		Size: 68.9 MB (68865978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b50c6c10811af772a159c03bf2ecf6f0dd39c9c7771b193015027fda8b09355`  
		Last Modified: Tue, 23 May 2023 16:07:02 GMT  
		Size: 100.1 MB (100149156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02df177330f6fc13e55397c73e5ce07ea69d71e506fda6d1f4670454c14a65a`  
		Last Modified: Tue, 23 May 2023 16:06:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:f4de5e48e73bc2c1c15b8d2f44a7cd856e765d038b53965456cced4065584166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.7 MB (260731229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:733c759af3a37a0b2746a31ab3809c102e4a23bac0c0d95d0945cc5c567d6c82`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:58:06 GMT
ADD file:a1ddba603e505863ad4f9d8c828c3d963fc27fef39de1fee725e8b790a1acfd0 in / 
# Tue, 23 May 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:57:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 09:57:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 17:02:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 17:02:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 17:02:48 GMT
ENV GOLANG_VERSION=1.20.4
# Tue, 23 May 2023 17:03:05 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.4.linux-amd64.tar.gz'; 			sha256='698ef3243972a51ddb4028e4a1ac63dc6d60821bf18e59a807e051fee0a385bd'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.4.linux-armv6l.tar.gz'; 			sha256='0b75ca23061a9996840111f5f19092a1bdbc42ec1ae25237ed2eec1c838bd819'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.4.linux-arm64.tar.gz'; 			sha256='105889992ee4b1d40c7c108555222ca70ae43fccb42e20fbf1eebb822f5e72c6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.4.linux-386.tar.gz'; 			sha256='5dfa3db9433ef6a2d3803169fb4bd2f4505414881516eb9972d76ab2e22335a7'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.4.linux-ppc64le.tar.gz'; 			sha256='8c6f44b96c2719c90eebabe2dd866f9c39538648f7897a212cac448587e9a408'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.4.linux-s390x.tar.gz'; 			sha256='57f999a4e605b1dfa4e7e58c7dbae47d370ea240879edba8001ab33c9a963ebf'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.4.src.tar.gz'; 		sha256='9f34ace128764b7a3a4b238b805856cc1b2184304df9e5690825b0710f4202d6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 23 May 2023 17:03:07 GMT
ENV GOPATH=/go
# Tue, 23 May 2023 17:03:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 17:03:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 23 May 2023 17:03:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ba419081a96034b68934ec792c30825d3deecc56745c9b286bb7637a393c2929`  
		Last Modified: Tue, 23 May 2023 01:02:04 GMT  
		Size: 45.9 MB (45916510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a99cd0a1d29e9b834e64a92aa16a4d9b384c916852eb0adb22894584fb9545`  
		Last Modified: Tue, 23 May 2023 10:05:59 GMT  
		Size: 16.2 MB (16211453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c12024abd2ab6ad6a53e1115837c37361d59bc71f90b3a78372fc21bba14be`  
		Last Modified: Tue, 23 May 2023 10:06:18 GMT  
		Size: 47.4 MB (47392571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7a1dc4d5d2dda7fa63593eff0b7f4a9e4eb6365ca3da1c3ec1c15235a9dd74`  
		Last Modified: Tue, 23 May 2023 17:05:01 GMT  
		Size: 53.3 MB (53341708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ece1ef2ef36174b8d6bf9606c4a2f7d654f97799124ae7878bc06094f6aff1b`  
		Last Modified: Tue, 23 May 2023 17:05:08 GMT  
		Size: 97.9 MB (97868832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550d2a91aa415078a4335e5a8f467f36b13e63bb0a094bfdaba7c9ebfc34b1a4`  
		Last Modified: Tue, 23 May 2023 17:04:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:89f241955d166e1599f51df0d48d76a270e340398c0cba3ed0660855df7bd956
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.1 MB (277085140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea00184d15d34ffd2131b83aa22b4f972e71fc33e9bf80a40f8190eddb0bc891`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:21 GMT
ADD file:a5100e7ed3c2665c1b4dfbb32eb2b47b85783f2a6800e0ae9004db0ce021dfa5 in / 
# Tue, 23 May 2023 00:43:22 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:56:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:57:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 16:51:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 16:51:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 16:51:19 GMT
ENV GOLANG_VERSION=1.20.4
# Tue, 23 May 2023 16:51:32 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.4.linux-amd64.tar.gz'; 			sha256='698ef3243972a51ddb4028e4a1ac63dc6d60821bf18e59a807e051fee0a385bd'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.4.linux-armv6l.tar.gz'; 			sha256='0b75ca23061a9996840111f5f19092a1bdbc42ec1ae25237ed2eec1c838bd819'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.4.linux-arm64.tar.gz'; 			sha256='105889992ee4b1d40c7c108555222ca70ae43fccb42e20fbf1eebb822f5e72c6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.4.linux-386.tar.gz'; 			sha256='5dfa3db9433ef6a2d3803169fb4bd2f4505414881516eb9972d76ab2e22335a7'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.4.linux-ppc64le.tar.gz'; 			sha256='8c6f44b96c2719c90eebabe2dd866f9c39538648f7897a212cac448587e9a408'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.4.linux-s390x.tar.gz'; 			sha256='57f999a4e605b1dfa4e7e58c7dbae47d370ea240879edba8001ab33c9a963ebf'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.4.src.tar.gz'; 		sha256='9f34ace128764b7a3a4b238b805856cc1b2184304df9e5690825b0710f4202d6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 23 May 2023 16:51:33 GMT
ENV GOPATH=/go
# Tue, 23 May 2023 16:51:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 16:51:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 23 May 2023 16:51:34 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5ea482247e9a0d1ae4ed218fb0828063b9cce53822e64fd4621f587ab85a7e6d`  
		Last Modified: Tue, 23 May 2023 00:46:24 GMT  
		Size: 49.2 MB (49238292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b9a832fb21afaa962a9cab69bf1b4044aa29ef4bd4684505838c4c7cabb76f`  
		Last Modified: Tue, 23 May 2023 06:03:52 GMT  
		Size: 17.5 MB (17450452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49fbb768597d28581cacecb6d008fd42c9ce8fe13fb045d488db3f8ac1b8ac9`  
		Last Modified: Tue, 23 May 2023 06:04:06 GMT  
		Size: 52.2 MB (52190742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c8c7f29fc851f5d45c753d49ec8c486cecc4373f52f238b5858e86facd79a3`  
		Last Modified: Tue, 23 May 2023 16:53:05 GMT  
		Size: 62.7 MB (62735744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0344f2fbca42a2619fac0acdfb7e78d3ab0f80fe94a142c05af28e9fe5cb2c5b`  
		Last Modified: Tue, 23 May 2023 16:53:08 GMT  
		Size: 95.5 MB (95469754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a86b2a5cf90bd4b1bc0b26793b7b642384bb4088f88e976f685665a21a318cf`  
		Last Modified: Tue, 23 May 2023 16:52:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; 386

```console
$ docker pull golang@sha256:8ac4385fdcfda836bfc4bc0328590eb682e0f328db6ff3a19f30ada3f72bdcc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297087071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d58338683ac4d79b836f6d8b8616a5a3836f0c69abd2e80c936100b98e96af7a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:45 GMT
ADD file:d82a514985e1c8796d6c5572290d84fdff0dc1c748d7d2e469d3066ac0344c5f in / 
# Tue, 23 May 2023 00:39:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:59:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:59:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:11:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:11:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 20:11:43 GMT
ENV GOLANG_VERSION=1.20.4
# Tue, 23 May 2023 20:11:56 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.4.linux-amd64.tar.gz'; 			sha256='698ef3243972a51ddb4028e4a1ac63dc6d60821bf18e59a807e051fee0a385bd'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.4.linux-armv6l.tar.gz'; 			sha256='0b75ca23061a9996840111f5f19092a1bdbc42ec1ae25237ed2eec1c838bd819'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.4.linux-arm64.tar.gz'; 			sha256='105889992ee4b1d40c7c108555222ca70ae43fccb42e20fbf1eebb822f5e72c6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.4.linux-386.tar.gz'; 			sha256='5dfa3db9433ef6a2d3803169fb4bd2f4505414881516eb9972d76ab2e22335a7'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.4.linux-ppc64le.tar.gz'; 			sha256='8c6f44b96c2719c90eebabe2dd866f9c39538648f7897a212cac448587e9a408'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.4.linux-s390x.tar.gz'; 			sha256='57f999a4e605b1dfa4e7e58c7dbae47d370ea240879edba8001ab33c9a963ebf'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.4.src.tar.gz'; 		sha256='9f34ace128764b7a3a4b238b805856cc1b2184304df9e5690825b0710f4202d6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 23 May 2023 20:11:57 GMT
ENV GOPATH=/go
# Tue, 23 May 2023 20:11:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 20:11:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 23 May 2023 20:11:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5a48e9012f51ff679af95460521da76c7184da775e3adaa39fed65c912ce0a57`  
		Last Modified: Tue, 23 May 2023 00:44:49 GMT  
		Size: 51.2 MB (51205678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bc7a25298904d5eca066c7a365d1c5c9fb1b9d6b1e716ae9a27e37b32a4ad3`  
		Last Modified: Tue, 23 May 2023 02:06:24 GMT  
		Size: 18.1 MB (18097872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de809a24a7c935e1db2594ae9d95cd2a19313955c833a1bd9bbef6dcdf11b43d`  
		Last Modified: Tue, 23 May 2023 02:06:43 GMT  
		Size: 53.5 MB (53472102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fcb9e30491fdb557659262725f64e1fa0e9d8db8d179470dd4550466f15f11`  
		Last Modified: Tue, 23 May 2023 20:14:10 GMT  
		Size: 73.7 MB (73736903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d667447a1554afdfeaa262d71338e2ec065c389825f2d7b87e08d8730b3861`  
		Last Modified: Tue, 23 May 2023 20:14:13 GMT  
		Size: 100.6 MB (100574360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d9d63e1c79a43fa30e47051c51a997b6cf8394c2257b74cf741eab3c35ee02`  
		Last Modified: Tue, 23 May 2023 20:13:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
