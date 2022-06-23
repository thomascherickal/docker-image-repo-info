## `golang:stretch`

```console
$ docker pull golang@sha256:cb52bf472f25983d6fcc1ea8c6a8ceb2acc286b817c3b583e29ab869d0e6d01a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:stretch` - linux; amd64

```console
$ docker pull golang@sha256:3c4f350c0347083f149d5fd7a3180a5de86142472f150d6c9a8dade9371d41d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.5 MB (310470750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ee1deda35bd32b4e08dfd7d0a41f79c14f75afd102507c9ae79a9c10950eb4a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 00:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 18:49:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 18:49:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 18:50:23 GMT
ENV GOLANG_VERSION=1.18.3
# Thu, 23 Jun 2022 18:50:38 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 23 Jun 2022 18:50:39 GMT
ENV GOPATH=/go
# Thu, 23 Jun 2022 18:50:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 18:50:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 23 Jun 2022 18:50:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f576518faec8cbe1e4fdcc36cb9870736c6a0889e0c7db2bde641503f37b6d19`  
		Last Modified: Thu, 23 Jun 2022 01:02:19 GMT  
		Size: 49.8 MB (49765716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90157da0035a3b4845650fbd43b85e258921053f686e2b31926842560efcd9b`  
		Last Modified: Thu, 23 Jun 2022 18:53:54 GMT  
		Size: 57.9 MB (57878913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922e06178296fe50a64cda42e43c42dcdc363e50e507a637c202f4e9aea30fc`  
		Last Modified: Thu, 23 Jun 2022 18:55:51 GMT  
		Size: 141.8 MB (141750097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0461de3b9b38b4cfe5a6079832fb43f79e0d18d8725abc3c765cae4fbd76565b`  
		Last Modified: Thu, 23 Jun 2022 18:55:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:62d5d4d70cf6f52e9bbd3f25acfebda5c305ac6fb5c5361dcea5950679272b88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258427906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a537830a6422a47a2ae03cf0eab29cf287a17ab0509cb3fd5f83ce06cc98d32b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:05:16 GMT
ADD file:f859825c79355490a08b5fd55799cc3eb1643e21abfeebe59a3a4b08e54e3f7f in / 
# Sat, 28 May 2022 01:05:17 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:54:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 02:55:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 20:39:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 20:39:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:00:25 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 23:01:02 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Jun 2022 23:01:04 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 23:01:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 23:01:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 23:01:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ae3d55ab33f9bf9aa2c47629e66da1c4e679da10d83c29941f39b04140996e4b`  
		Last Modified: Sat, 28 May 2022 01:21:38 GMT  
		Size: 42.2 MB (42150781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d277a5551d8d3385d5cf64c67234fe8db9bad96903365595e8c6c61146e48d2b`  
		Last Modified: Sat, 28 May 2022 03:17:39 GMT  
		Size: 10.0 MB (9957035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2055cd14260ece06830786d784271b3008f3ce2ea3279123620a6d78a2afecfa`  
		Last Modified: Sat, 28 May 2022 03:17:36 GMT  
		Size: 3.9 MB (3921757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7574dbdaaad44c5640ade0f5aba1843344998699356f46c27a9d56220564c345`  
		Last Modified: Sat, 28 May 2022 03:18:23 GMT  
		Size: 46.1 MB (46127871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a469840cbf6ac22ee3b08ea9b9fed583abbd14af4334d15183acae1cb67bdf11`  
		Last Modified: Sun, 29 May 2022 20:50:06 GMT  
		Size: 46.2 MB (46210680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f53ac13c096b12e64436b1ace0d92622b17e85337227c49879eff55a8ae233d`  
		Last Modified: Wed, 01 Jun 2022 23:27:44 GMT  
		Size: 110.1 MB (110059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7b9d09389d6f6aab372614382fe666d75fc367a5e8e110e094bf267ea4dcc1`  
		Last Modified: Wed, 01 Jun 2022 23:26:32 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:1c55fabe7b8d5ed791a7d71bfba69abf3ee917ff3dd9524c3b6b8224b6c94834
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (262964377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdaec89312f993d1ede550f041994e5c90e7ca9e5e89fa0045924a07e3dbcbd5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:45 GMT
ADD file:3d8b1da94fcec5d068e3e6465fac70cce404c331bb52e30a5bf7cbd950baa5fe in / 
# Thu, 23 Jun 2022 00:42:45 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:15:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:16:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:16:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 18:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 18:51:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 18:53:15 GMT
ENV GOLANG_VERSION=1.18.3
# Thu, 23 Jun 2022 18:53:27 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 23 Jun 2022 18:53:29 GMT
ENV GOPATH=/go
# Thu, 23 Jun 2022 18:53:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 18:53:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 23 Jun 2022 18:53:32 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d8ccec8a513f896fedd1d9765f3f2abf98bc8264f61cecf17919c80c9aa7ddbc`  
		Last Modified: Thu, 23 Jun 2022 00:51:18 GMT  
		Size: 43.2 MB (43213121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b40625a6bb21cb2cd6b19ef7592951f90da9ea1d8abf359196bf48300c448b2`  
		Last Modified: Thu, 23 Jun 2022 01:25:28 GMT  
		Size: 10.2 MB (10218617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414226169d0f92fdcd77314cbd06ba7613675d62a3afd63aa88afbf0072c44c2`  
		Last Modified: Thu, 23 Jun 2022 01:25:27 GMT  
		Size: 3.9 MB (3874558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb01f37c2a0f6704c7bc0d24baac1a6d5694b5e2fec5ae71f1c257b337a9348`  
		Last Modified: Thu, 23 Jun 2022 01:25:46 GMT  
		Size: 47.7 MB (47736296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187df16cefa0e44ed3f4a74d309d7af745f307d34e97128caac7d900ed5e6ba7`  
		Last Modified: Thu, 23 Jun 2022 18:57:38 GMT  
		Size: 49.0 MB (49042215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0793bab5bfbcf9755723325a341f161011f7eb9e226670437c115b6965b4403`  
		Last Modified: Thu, 23 Jun 2022 18:59:28 GMT  
		Size: 108.9 MB (108879444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f5e97c167c416ca3cff6aee0b760da9b9627f5f1604f5c9ad01d50d090de10`  
		Last Modified: Thu, 23 Jun 2022 18:59:12 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; 386

```console
$ docker pull golang@sha256:55eeadf50812ece1715ecf47a792deed68ed5602311c65f3ec4dd002234c94b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.2 MB (288180699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9842b94af836d1b18cf68efe6375774e294580cb94ad1b18df5c95969986591`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:41:44 GMT
ADD file:ec3ab24d5698ffb1c2c01f4cf088854df8d14de655c3ea1235b3ca4c06864be4 in / 
# Thu, 23 Jun 2022 00:41:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:17:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:17:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:17:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 15:07:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 15:07:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 15:10:25 GMT
ENV GOLANG_VERSION=1.18.3
# Thu, 23 Jun 2022 15:10:40 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 23 Jun 2022 15:10:41 GMT
ENV GOPATH=/go
# Thu, 23 Jun 2022 15:10:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 15:10:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 23 Jun 2022 15:10:45 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:198ad075a14b0fdef3454be69cd94a50c01a286b210867ddfc0a62404bdf34b1`  
		Last Modified: Thu, 23 Jun 2022 00:50:47 GMT  
		Size: 46.2 MB (46150601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaffa0015e0586960116ca5558554b0c37500c89d72de88c1f9d16c4b75f1c3`  
		Last Modified: Thu, 23 Jun 2022 01:25:54 GMT  
		Size: 11.4 MB (11358747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15767d66256ddb61c1d4865abc90dee1afeff18268172fc8e8f0acdc445164ac`  
		Last Modified: Thu, 23 Jun 2022 01:25:53 GMT  
		Size: 4.3 MB (4342258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c04ca75d8a85c2adee31eea858219314e193127787b58a020d53652a7e1487`  
		Last Modified: Thu, 23 Jun 2022 01:26:13 GMT  
		Size: 51.3 MB (51268480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99df1310c4ee589981ff95243e9b531690c9127b55c340967b42939e72bb3f89`  
		Last Modified: Thu, 23 Jun 2022 15:16:30 GMT  
		Size: 62.2 MB (62169937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2db36c4480a7c44fb4b8088754409e8a986f971ed20f2f41abe19d6643cfb8`  
		Last Modified: Thu, 23 Jun 2022 15:18:12 GMT  
		Size: 112.9 MB (112890550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a64550bfcafd9700dbef3cc078d6db297b7dacfd78ba0635d30e534e957537b`  
		Last Modified: Thu, 23 Jun 2022 15:17:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
