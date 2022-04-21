## `golang:1-bullseye`

```console
$ docker pull golang@sha256:9d12facef9179ef91d2b3fcefed178c6780515b0b700e4a03a60991b097a422e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `golang:1-bullseye` - linux; amd64

```console
$ docker pull golang@sha256:5b75b529da0f2196ee8561a90e5b99aceee56e125c6ef09a3da4e32cf3cc6c20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.1 MB (353087793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65375c930b214d93a4c09a1db748e6979ef53ad585ec864dbe837108d48d8d14`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:15 GMT
ADD file:3a81c181c66f226bd6abd48d0c7ed8a9c599c9f521ec7229286c83161afec8c2 in / 
# Wed, 20 Apr 2022 04:43:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:57:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:57:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:58:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:27:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:27:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:27:43 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 20 Apr 2022 22:27:55 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 20 Apr 2022 22:27:57 GMT
ENV GOPATH=/go
# Wed, 20 Apr 2022 22:27:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:27:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Apr 2022 22:27:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6aefca2dc61dcbcd268b8a9861e552f9cdb69e57242faec64ac120d2355a9c1a`  
		Last Modified: Wed, 20 Apr 2022 04:47:57 GMT  
		Size: 54.9 MB (54941777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967757d5652770cfa81b6cc7577d65e06d336173da116d1fb5b2d349d5d44127`  
		Last Modified: Wed, 20 Apr 2022 07:05:43 GMT  
		Size: 5.2 MB (5155716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c357e2c68cb3bf1e98dcb3eb6ceb16837253db71535921d6993c594588bffe04`  
		Last Modified: Wed, 20 Apr 2022 07:05:45 GMT  
		Size: 10.9 MB (10874928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c766e27afb21eddf9ab3e4349700ebe697c32a4c6ada6af4f08282277a291a28`  
		Last Modified: Wed, 20 Apr 2022 07:06:05 GMT  
		Size: 54.6 MB (54578663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a8ea6bd5f867dbdf5bad1c42bc569afacf062a0241c1a8b45718fc8ae26fba`  
		Last Modified: Wed, 20 Apr 2022 22:31:00 GMT  
		Size: 85.8 MB (85835412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a9b904f7423b8b1f02a99df065ceb2de067207d626915b84776bb0c918ed0f`  
		Last Modified: Wed, 20 Apr 2022 22:31:08 GMT  
		Size: 141.7 MB (141701141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3447e3508f49d81eb14b0cf466950f15126161f20f2d70b8d429017d2b08a74f`  
		Last Modified: Wed, 20 Apr 2022 22:30:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v5

```console
$ docker pull golang@sha256:1d7e627c26ac2803cc82358e59878d2d1da21485384d0ffd924e2eadca335960
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.7 MB (301663358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:504069d8fe72929b065fbc64a67aee7a0212e375b6a955ab8c4e8adc3b78aa0d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:50:03 GMT
ADD file:6cca5eca42975074f53a45a9b4ba83d1f06b95182dd4d8d95622d63cbc206574 in / 
# Tue, 29 Mar 2022 00:50:04 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:42:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:43:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 07:43:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 15:09:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 15:09:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:31 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 13 Apr 2022 02:53:07 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 13 Apr 2022 02:53:08 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:53:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:53:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:53:11 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cfb93eae062e68427eb7e96f51a690313db08e4118ca20b5a644c29fecb784db`  
		Last Modified: Tue, 29 Mar 2022 01:04:42 GMT  
		Size: 52.5 MB (52475868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d69db2a0aac9ea7e48801a42d0b5e9e3a116bd0cdc20079aea745dd5653a7a`  
		Last Modified: Tue, 29 Mar 2022 08:05:43 GMT  
		Size: 5.1 MB (5065379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcddb47fa9924cdf33c6afa828fb4fa1365d464069ed1a63a5063b7daabbabe1`  
		Last Modified: Tue, 29 Mar 2022 08:05:45 GMT  
		Size: 10.6 MB (10572944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a5b09c9df3962b241df6ed71a37e9f3febeec33fcff083e6417ada9551f79c`  
		Last Modified: Tue, 29 Mar 2022 08:06:39 GMT  
		Size: 52.3 MB (52316733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d448eaf3e3a3b08e5c04bef6900e3783b50ad674b4d05c81e0987016512b3754`  
		Last Modified: Wed, 30 Mar 2022 15:29:08 GMT  
		Size: 68.8 MB (68766145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f7125635f0a0acefa08f2b3bdc25bee4c4a4cf84c39993d2976749e0758d97`  
		Last Modified: Wed, 13 Apr 2022 03:08:40 GMT  
		Size: 112.5 MB (112466133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9b50ea7305bd094875e1df3e4dfa9fd3ae0585688640d70242d3f209a57ac6`  
		Last Modified: Wed, 13 Apr 2022 03:07:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:92f6794c9968bf14c0aadd6032c0c43ab64e485ec6069b40a9b94dfa31645e9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.4 MB (290410849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73871b0bb7a0f2abe029dc072c99d5dbde322bf1d9ce8b2428fe029ac93f4d34`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:17:58 GMT
ADD file:d8d3280d101d611090968c237af923598174e090c533c24bcee805d174e4a6f5 in / 
# Tue, 29 Mar 2022 02:17:59 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:06:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 20:07:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 23:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 23:29:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:14:09 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 13 Apr 2022 04:14:43 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 13 Apr 2022 04:14:45 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 04:14:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:14:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 04:14:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:fc87a15f2d540adb88546a549e56aa0a378d5719bbfd07399e467a095e27d5df`  
		Last Modified: Tue, 29 Mar 2022 02:33:28 GMT  
		Size: 50.1 MB (50133868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991e015792e592929b68328873d303aff48f6941208e2954283895889e665b3`  
		Last Modified: Wed, 30 Mar 2022 20:30:28 GMT  
		Size: 4.9 MB (4924893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4aa6896142430c96d4b31e28c4d0e3c383d9ae671ce052f26fc7cf68189c058`  
		Last Modified: Wed, 30 Mar 2022 20:30:30 GMT  
		Size: 10.2 MB (10217881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e907cedb6582c6203cece538aac031ac66936e9249b00577dfd745a466ff936c`  
		Last Modified: Wed, 30 Mar 2022 21:30:51 GMT  
		Size: 50.3 MB (50328564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40dbe001d369848fb66eaefb3e91b9b90a56d0255de1aa23eeb28f9be23e195b`  
		Last Modified: Thu, 31 Mar 2022 23:39:20 GMT  
		Size: 64.8 MB (64787857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4b16d41f059fb5c011d6e9ee0ea05595608f70b5cf5d2db26f567c11d8431f`  
		Last Modified: Wed, 13 Apr 2022 04:38:01 GMT  
		Size: 110.0 MB (110017630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51b6e66f2e8870c24e1afaffcdedccc386f3d03905a5357314028b12ad3c1e1`  
		Last Modified: Wed, 13 Apr 2022 04:36:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:2e1a0c4b36e65643e4d737797036644ead11609ba3f006d1cf7a5ad151b3f849
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313649870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27959cb699fc4755876c72ab969ed067fd9e05a32869f99805107273549a5336`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:28:55 GMT
ADD file:ece192802cbdaf1a141d04f0c2e90cfd3479e5e3e82c6a00206970684494cf48 in / 
# Wed, 20 Apr 2022 04:28:56 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:44:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:00:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:00:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:00:35 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 20 Apr 2022 22:00:47 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 20 Apr 2022 22:00:48 GMT
ENV GOPATH=/go
# Wed, 20 Apr 2022 22:00:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:00:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Apr 2022 22:00:51 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:83d5dcfea08e6927083bc886bf182fc39d87bb04b54b63002ac0c4c0b9aab682`  
		Last Modified: Wed, 20 Apr 2022 04:35:19 GMT  
		Size: 53.6 MB (53633096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfa86b7b1aca6d694057e4d42ee1440527f41c00b9e577df729244380c9eba`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 4.9 MB (4938663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79b19335f27cc78840bf9159e875322f3252ac06113c73756f9d4fba905f9b`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 10.7 MB (10656971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350ecaf08eac09037b05465ab97a1b8f7bc9b7a9b1fcef900dedd7dba9bbcf4d`  
		Last Modified: Wed, 20 Apr 2022 06:54:32 GMT  
		Size: 54.7 MB (54672934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8129b50beeb587c45b07bd0fc9db983c8384eba20c8f87784f5456c1e7935b5`  
		Last Modified: Wed, 20 Apr 2022 22:04:57 GMT  
		Size: 81.0 MB (81049736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1beb8c2043eb5ed94ec703523a402deaa54b6d8202ba1126fe275ad9985018d`  
		Last Modified: Wed, 20 Apr 2022 22:05:03 GMT  
		Size: 108.7 MB (108698344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba5e8425c8eef2b5564b4f8ba179b65bb133b3408a82585d01158858c9124fa`  
		Last Modified: Wed, 20 Apr 2022 22:04:47 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; 386

```console
$ docker pull golang@sha256:3b7fa1bed1510cfdadbbd839ab1c2c4ca5ee86bc259d2cb71142f6bd4e70b59f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.9 MB (327884996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a24dbf0d7fe4860603ce52b04c59577a585979561b1c59dc31fcd9cd7c53f40`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:18 GMT
ADD file:81b79bac6ad02f2b0e2d30c005dac5f38d58fc7e12d7466c6704bc8a8980a0ef in / 
# Wed, 20 Apr 2022 07:37:19 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:16:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:16:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 10:16:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:07:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:07:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:07:20 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 20 Apr 2022 22:07:37 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 20 Apr 2022 22:07:38 GMT
ENV GOPATH=/go
# Wed, 20 Apr 2022 22:07:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:07:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Apr 2022 22:07:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:03830d6b0d2ecb0a7f823997ff6629d0ff36a821ec317f6d5644d08b1870d936`  
		Last Modified: Wed, 20 Apr 2022 07:44:23 GMT  
		Size: 55.9 MB (55940721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5cb7d3850c1f11597dc2fec3a9db47da0cf01b07710d9db78b1bef55ee2868`  
		Last Modified: Wed, 20 Apr 2022 10:27:18 GMT  
		Size: 5.1 MB (5080236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d496dba7030d724d160a2e22c59274cbb50c0ef8459868c1606869acc1e547dc`  
		Last Modified: Wed, 20 Apr 2022 10:27:18 GMT  
		Size: 11.0 MB (11033707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b150f765b11c7498c1cef2cfc444847ca96a2c66714988c44157d31e39ba0ca8`  
		Last Modified: Wed, 20 Apr 2022 10:27:41 GMT  
		Size: 55.9 MB (55914454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a39b7fcaba420ffc8f17adf72a0742dd285cf26d096690f283ad963c56683d`  
		Last Modified: Wed, 20 Apr 2022 22:12:19 GMT  
		Size: 87.1 MB (87059885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009349f28afe3e66d95629f796cb205aae62dd6a857195f86c9ca50670e0e9e7`  
		Last Modified: Wed, 20 Apr 2022 22:12:21 GMT  
		Size: 112.9 MB (112855869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bfe833c39fa01fc2b0864424163d64567ce6a1d72f387e13640905a6183501`  
		Last Modified: Wed, 20 Apr 2022 22:12:06 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:e139e689507eb71b946b5bd7ac89e9b42635163b4fc0454361d910d62adf04cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297467552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa49472658c3e1463040ec08cb54ce1f850459eca04deee5f8ef95a06de82aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:41:51 GMT
ADD file:40fc6f06ccce55e9889d1c94556c29242d1ac62870cb9895da64d37bac45ab5e in / 
# Tue, 29 Mar 2022 07:41:56 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:27:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:27:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 08:29:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 01:47:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 01:47:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:07:26 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 13 Apr 2022 02:19:09 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 13 Apr 2022 02:19:17 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:19:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:19:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:19:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:efb90a274e1b19eec263e44f7fbc1f9c9c6c393210c27b03ebde7c2b0a2b6482`  
		Last Modified: Tue, 29 Mar 2022 07:52:16 GMT  
		Size: 53.2 MB (53199386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7959b932ae1363e586ef79fc1ab6afdaee0b7a9f97e0a507c1868cfc6dd47778`  
		Last Modified: Tue, 29 Mar 2022 08:57:32 GMT  
		Size: 4.9 MB (4912295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3b22f54d8b49fd2d7d246274c6016cdcff9377c15befaa4323d44c3b1e75ac`  
		Last Modified: Tue, 29 Mar 2022 08:57:35 GMT  
		Size: 10.7 MB (10660105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d388c5955683d48c342f8d6b2291b7cedf59d2fcfb9343f5aa240f4b5f56da3`  
		Last Modified: Tue, 29 Mar 2022 08:58:23 GMT  
		Size: 53.3 MB (53297457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e978f1552505ee0749721ea9d15cea9c7bdcfec2486a888d0f42104c476513`  
		Last Modified: Thu, 31 Mar 2022 02:37:01 GMT  
		Size: 66.7 MB (66736753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2264854fd070c3191d53e3ebb7e1a728cb5c563d4d825c1d4aadc28228169aa8`  
		Last Modified: Wed, 13 Apr 2022 02:56:18 GMT  
		Size: 108.7 MB (108661430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79083f084a68eb86a8f8650ebad60bd217b164c06376c32e645cda52840f6347`  
		Last Modified: Wed, 13 Apr 2022 02:55:10 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; ppc64le

```console
$ docker pull golang@sha256:3d833a08e829e4a9da7873b2391d839ff29db6c59462a145b171a04da2adfc32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.9 MB (323918426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f86f74db99f2ccbb4a6b5060d10ba429f1d3f680fab58c3a2b192ae28a4226c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:21:35 GMT
ADD file:32dd723ee02b792cb3de67b78d352e79bdb52bf9d23fa5190ce764956b1e3884 in / 
# Tue, 29 Mar 2022 00:21:42 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:47:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:48:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 05:50:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 13:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 13:31:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:40:30 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 13 Apr 2022 02:41:07 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 13 Apr 2022 02:41:14 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:41:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:41:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:41:27 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c632eeaf13829ddb578e0545ba882dab1aee70ee0cf3069a1fc9eefd23c3e0a8`  
		Last Modified: Tue, 29 Mar 2022 00:32:02 GMT  
		Size: 58.8 MB (58834937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762034bf4e697addca3a77a00590017f45c852584700ffabe39eed10a6c58083`  
		Last Modified: Wed, 30 Mar 2022 06:25:30 GMT  
		Size: 5.4 MB (5405164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c92df217f6ce5e8db50ab0c999242f4d0fbefce03ed9a33195642d3c86ce17`  
		Last Modified: Wed, 30 Mar 2022 06:25:31 GMT  
		Size: 11.6 MB (11627455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543ec63f3430a7907602f65d568921eac8baffc304cc47afd544b1d44996285f`  
		Last Modified: Wed, 30 Mar 2022 06:25:58 GMT  
		Size: 58.9 MB (58854169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7ba7ad317c2e615ec8a60451c28111c6feef1be0090a403822e3dbd1b716c9`  
		Last Modified: Thu, 31 Mar 2022 13:42:53 GMT  
		Size: 80.3 MB (80318194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db9efeaba138a2395c86950e9e17a81d49fc905aba84bae02230603b5e88afe`  
		Last Modified: Wed, 13 Apr 2022 02:56:25 GMT  
		Size: 108.9 MB (108878351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2db06209de29e0cf000a9f486159a2d53757d8afe812f894beb6e19152b24c7`  
		Last Modified: Wed, 13 Apr 2022 02:55:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; s390x

```console
$ docker pull golang@sha256:b4004430fa7f61cc530de1f5617a4829bbc860daf979bb00c73f43054cb971c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.3 MB (300330321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd7fc24ad62c9f3bdcde247f58030a327e241ee10e3b0ef07a834631ffba47b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:39:00 GMT
ADD file:82d4840cdb4b0211b2191ba71ea2698d8dc1b05554d7ed1499aca9cbafaa3fc8 in / 
# Wed, 20 Apr 2022 08:39:07 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:14:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:14:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 11:15:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:48:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:48:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:48:44 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 20 Apr 2022 22:49:04 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 20 Apr 2022 22:49:10 GMT
ENV GOPATH=/go
# Wed, 20 Apr 2022 22:49:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:49:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Apr 2022 22:49:11 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:bec7f58dd40ec15934a767db84e5e9b88704cefe60ebe4d7f5abc1583f6c060c`  
		Last Modified: Wed, 20 Apr 2022 08:49:18 GMT  
		Size: 53.2 MB (53207374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3218063f6607544274f51ec8c2c55ce1aded6957be3971daff89994bdda6a2cf`  
		Last Modified: Wed, 20 Apr 2022 11:28:09 GMT  
		Size: 5.1 MB (5140662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0a6f99a2efe32d3a43fb003ae9ecc029a6ee042cf8dd86a02575641ae1f2f`  
		Last Modified: Wed, 20 Apr 2022 11:28:10 GMT  
		Size: 10.8 MB (10765408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1541dbd7cbb77f6f94e9662dd72fda7406d1f327090e791168c3b7a8bdce5e2a`  
		Last Modified: Wed, 20 Apr 2022 11:28:27 GMT  
		Size: 54.0 MB (54045497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7684862853e6ceb672882b9f7d0a31cbc73574dfa2bdceeac664fe3125e1d8`  
		Last Modified: Wed, 20 Apr 2022 22:53:03 GMT  
		Size: 65.6 MB (65561017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150f64c9182844944421d88df411e8acdbe7d5854ea450a1df6c0be961c8e4e0`  
		Last Modified: Wed, 20 Apr 2022 22:53:08 GMT  
		Size: 111.6 MB (111610207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c3c415b60fbeeae4f414ff6329193cbadbbd2015a11abc7da3b474c3608550`  
		Last Modified: Wed, 20 Apr 2022 22:52:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
