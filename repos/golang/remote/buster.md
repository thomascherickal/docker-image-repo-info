## `golang:buster`

```console
$ docker pull golang@sha256:c1695ea86ac2454c5d3830184094690db92aee367f41e7a9e3420d812b3ebbd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `golang:buster` - linux; amd64

```console
$ docker pull golang@sha256:504366de834ff066f79a83f394cf3b3221f751d26524e6d8527c8aeec16818a4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.7 MB (309695727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f9d35ce5cfe925757feb4d5d264863ec3547058de5a9499b7631565e5f4f783`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 16:58:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 20:33:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 20:33:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 20:33:05 GMT
ENV GOLANG_VERSION=1.15.6
# Thu, 17 Dec 2020 20:33:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 17 Dec 2020 20:33:16 GMT
ENV GOPATH=/go
# Thu, 17 Dec 2020 20:33:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 20:33:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Dec 2020 20:33:18 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d599c07d28e6c920ef615f4f9b5cd0d52eb106fcd20c3a7daef389f14edd4ef5`  
		Last Modified: Thu, 17 Dec 2020 17:26:19 GMT  
		Size: 51.8 MB (51829485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c616e0dda35f18bc9c0826279139808008b102035043926b1229cd641a4d2146`  
		Last Modified: Thu, 17 Dec 2020 20:35:14 GMT  
		Size: 68.7 MB (68708455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e68d0e3d3c7ffdfde9af883ccdf892375c53a8e1555b34ef47b080b663cb45a`  
		Last Modified: Thu, 17 Dec 2020 20:35:21 GMT  
		Size: 121.0 MB (120951441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dea2301be074c83aa3db569cf6f8ac7101ca5ba3d18c530a9f71b35d438fb97`  
		Last Modified: Thu, 17 Dec 2020 20:35:00 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:ed5418c8f935db65f521291e0a572a021e173dfb66e816c2e0c89b58dff12817
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.7 MB (269706515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b676c24ca9d826a4ff0904daa8b5dedf4979ab748b706491cf682b5b1f70f68f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:09 GMT
ADD file:6bb5740487b2a3dbdcfe226dc1b844c4b3586f92824989273c94f58a7be61521 in / 
# Tue, 12 Jan 2021 00:51:11 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:28:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:28:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:29:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 13:14:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 13:14:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 13:18:45 GMT
ENV GOLANG_VERSION=1.15.6
# Tue, 12 Jan 2021 13:21:42 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 12 Jan 2021 13:21:46 GMT
ENV GOPATH=/go
# Tue, 12 Jan 2021 13:21:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 13:21:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jan 2021 13:21:49 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2663f95eeaf3e5f20b51c12003bb968c3590794bc6eb385f9e448a620c063beb`  
		Last Modified: Tue, 12 Jan 2021 00:59:39 GMT  
		Size: 48.1 MB (48112596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00face3f5d2c20e2d27bb8a18bc2970f142fcd36b1aa94a95004cb93990e3bf`  
		Last Modified: Tue, 12 Jan 2021 01:43:36 GMT  
		Size: 7.4 MB (7362263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a678d54f3a9324d0c090e05019af611bbe80cf104f7762f5034da6ac4257ea`  
		Last Modified: Tue, 12 Jan 2021 01:43:36 GMT  
		Size: 9.7 MB (9687427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c227fef8ac09a8d6728bb05fe2d2bab3a83fd4dccbee20b5f35d988cbb53a01b`  
		Last Modified: Tue, 12 Jan 2021 01:44:10 GMT  
		Size: 49.6 MB (49572388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f310365a5b4be0622861b4cc6f45181da167de3e3675f9f5998456c04976154`  
		Last Modified: Tue, 12 Jan 2021 13:26:08 GMT  
		Size: 52.0 MB (52017415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7461e1e91909a33ce449974477110c3c7005258f29c785bc06f098e388d8e6a9`  
		Last Modified: Tue, 12 Jan 2021 13:27:06 GMT  
		Size: 103.0 MB (102954270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554d66700d41c271327d3a2ba27d25cc42615569b2e66288fe034a1bd1e3794a`  
		Last Modified: Tue, 12 Jan 2021 13:26:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:1cb13f55dc37563d96ae9f11dbfa5e13df20bd90926b10c670a5acdd14e17ea3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.7 MB (260697417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43119d2de81fbb92aec9471031815248cef5f5b8bd4ee0291058ad4949bcc58f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:08 GMT
ADD file:af46f686172bae3034ad0b34cc26081a2f8db0f5d4704ef63abb7eeaf06c75e0 in / 
# Fri, 11 Dec 2020 02:23:11 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 08:16:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 08:16:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 08:17:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:05:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:05:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 11:05:11 GMT
ENV GOLANG_VERSION=1.15.6
# Thu, 17 Dec 2020 11:05:36 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 17 Dec 2020 11:05:38 GMT
ENV GOPATH=/go
# Thu, 17 Dec 2020 11:05:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 11:05:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Dec 2020 11:05:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:709549ab8c597dac59777a5a3666600f3dd986b5f05389aa7b15bd5f9281f809`  
		Last Modified: Fri, 11 Dec 2020 02:32:43 GMT  
		Size: 45.9 MB (45867902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47835026e1df0ff27d1071162b8ee6183c6c06f3880f788d360330f95d426f3`  
		Last Modified: Thu, 17 Dec 2020 08:52:24 GMT  
		Size: 7.1 MB (7099204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9aa96a1a673a07b6f8f0936ce1fb5521c14b566ea503a69342bd56e5e115e20`  
		Last Modified: Thu, 17 Dec 2020 08:52:24 GMT  
		Size: 9.3 MB (9343453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e19bdda1d2f3319ac9fbe5b8b2a9a62eba6a49e13e6846089d4d85f3b6d256`  
		Last Modified: Thu, 17 Dec 2020 08:52:49 GMT  
		Size: 47.4 MB (47355631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934ecff420e3c2954c7b0594c8910402c8593ea152d0282b00c7f870d3f64692`  
		Last Modified: Thu, 17 Dec 2020 11:08:50 GMT  
		Size: 53.2 MB (53177674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b4dfb5128594a9225d54b730d4a84d0b5e029c4dd39dc84ec98430e80d41dc`  
		Last Modified: Thu, 17 Dec 2020 11:09:09 GMT  
		Size: 97.9 MB (97853398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44c15dc193f67d4eaad79e792b228743af2ce952c03ebe47b4db1790280be82`  
		Last Modified: Thu, 17 Dec 2020 11:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:4e8d5b8651f6ad69d9d15cf14ae8cfbc94fa33269f521e42598a2c7dbe2cfedd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.2 MB (279178241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:020877ec5337a67c7186bcc7f2dc3fc2910e45f913d5ab19ab45c0aee70aa743`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:23 GMT
ADD file:b08f373022952dba7d08b7fc02909d9e369c9727e0e4f62d6110e41e70e668cc in / 
# Fri, 11 Dec 2020 02:45:25 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 10:05:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:06:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 10:06:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 14:52:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 14:52:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 14:52:13 GMT
ENV GOLANG_VERSION=1.15.6
# Thu, 17 Dec 2020 14:52:29 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 17 Dec 2020 14:52:32 GMT
ENV GOPATH=/go
# Thu, 17 Dec 2020 14:52:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 14:52:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Dec 2020 14:52:35 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:99e5136f81cd2a8cc226c42435d6f4f30584d168cc51f4d4afd2d5611e4d2215`  
		Last Modified: Fri, 11 Dec 2020 02:52:45 GMT  
		Size: 49.2 MB (49180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e84abcfad00e501f51bf9945429b6856c10fe31c1504e62c6520d85fff4382`  
		Last Modified: Thu, 17 Dec 2020 10:38:12 GMT  
		Size: 7.7 MB (7682276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97012cb1831f37b45ec32c7b23a4a1bbd2d92d45324067362d15f9c5ed5341b0`  
		Last Modified: Thu, 17 Dec 2020 10:38:13 GMT  
		Size: 10.0 MB (9984302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ab763a154e0e4765c5e67269e4bb776478e2abfb52f24bae39ee817ad26bbc`  
		Last Modified: Thu, 17 Dec 2020 10:38:37 GMT  
		Size: 52.2 MB (52163991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e622b12525cf72c0b9d160909bdd668e261a84e9e4b0635497b0ef18fdbf60`  
		Last Modified: Thu, 17 Dec 2020 14:55:30 GMT  
		Size: 62.6 MB (62577196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d96ce22fb1263175afb7c01345ea271a2ffefff779a7b8105a736b92d440a2`  
		Last Modified: Thu, 17 Dec 2020 14:55:39 GMT  
		Size: 97.6 MB (97590004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360dea20c58ddb8f3cee4fd531ff4cdf1fe2dd0b61ad8bf2b78ec39842e43f65`  
		Last Modified: Thu, 17 Dec 2020 14:55:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; 386

```console
$ docker pull golang@sha256:87d833f81bc4d33d6e1b68e15ed2dcd2ad6b8062ffcb337011f3e33d55c70b1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.9 MB (296907325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14375eddfc3f5562da49d4c56a14861663701da07ccc2a862c1cb3fee38dca96`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:20 GMT
ADD file:a9adff9550f58602df592d7afdcf7dead81207490f94d5119ce09d6a3a35c856 in / 
# Tue, 12 Jan 2021 00:39:20 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:18:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:18:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 03:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 17:14:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 17:14:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 17:17:36 GMT
ENV GOLANG_VERSION=1.15.6
# Tue, 12 Jan 2021 17:17:54 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 12 Jan 2021 17:17:54 GMT
ENV GOPATH=/go
# Tue, 12 Jan 2021 17:17:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 17:17:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jan 2021 17:17:55 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0766cf79c8928aa3f896ef392c35c2447301aec0dbac55ac6da9a6efde011fd6`  
		Last Modified: Tue, 12 Jan 2021 00:45:56 GMT  
		Size: 51.2 MB (51163652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e3049e9c61bd8ec7a11a8d511e6e49314335b9483bebb284233b813718076b`  
		Last Modified: Tue, 12 Jan 2021 03:31:21 GMT  
		Size: 8.0 MB (7981772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e60415ae2910cd4250c2204e52a34fb01fd20439269ee1cb768e195de279c3`  
		Last Modified: Tue, 12 Jan 2021 03:31:21 GMT  
		Size: 10.3 MB (10338765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb1f672cb3a4e1913fc3656c4c8fc50ef5f7c6290fc38830ccac36ef778eecd`  
		Last Modified: Tue, 12 Jan 2021 03:31:48 GMT  
		Size: 53.4 MB (53432011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeb8be618f9696ece093704140db318f0d3b29e70a2fef5d00049281b0da824`  
		Last Modified: Tue, 12 Jan 2021 17:20:54 GMT  
		Size: 73.6 MB (73574515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f499835aeaa695369325582c5cf147587b6661c272ccc1f3dd5afb2a8edf9b3`  
		Last Modified: Tue, 12 Jan 2021 17:21:35 GMT  
		Size: 100.4 MB (100416486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea0031acbbfd786a5a993caf8d55bd5cef41406d5a8bb171f155f42925f09b1`  
		Last Modified: Tue, 12 Jan 2021 17:21:13 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; mips64le

```console
$ docker pull golang@sha256:d7f8b3e570a2c860f607e44023fd1bdbd5eb834d88c0deaef2bd9505ccaec4a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.3 MB (272328152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e2ace25b741791cef8dbd93b5fd18a383790c8f2bac6c00e534ef151400b4e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 01:15:58 GMT
ADD file:1ea3ca1d00229eb0be06bc2fa54f95822e906deb654f8f3bf5d6aa49dd884f6f in / 
# Tue, 12 Jan 2021 01:15:59 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:50:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:50:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:51:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:12:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:12:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 16:21:01 GMT
ENV GOLANG_VERSION=1.15.6
# Tue, 12 Jan 2021 16:28:29 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 12 Jan 2021 16:28:31 GMT
ENV GOPATH=/go
# Tue, 12 Jan 2021 16:28:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 16:28:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jan 2021 16:28:33 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:1d0e08cc8efbf09ece45929fdb6f02d6bf57202bf8653e71adc6e782f0e67c68`  
		Last Modified: Tue, 12 Jan 2021 01:22:21 GMT  
		Size: 49.0 MB (49025676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999a474ffc3c8bea221f1d8cd6242dede4fd59e39591c684e2e1a3f175dfaabd`  
		Last Modified: Tue, 12 Jan 2021 02:02:15 GMT  
		Size: 7.2 MB (7232200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba100e51ff51674e6e530f33b8b3dab47d6c95c36fb384daf75f67cfa1d36de`  
		Last Modified: Tue, 12 Jan 2021 02:02:16 GMT  
		Size: 10.0 MB (10016222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e406dcf9e8aa8be41fcde4b18a0478cad031260659d026dd4e43ae5dc99b80`  
		Last Modified: Tue, 12 Jan 2021 02:03:10 GMT  
		Size: 50.8 MB (50842117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6339e0b01cf74f963b4dac47fc8c21200d20e5ca2c2f6960442abd8e5fdeb876`  
		Last Modified: Tue, 12 Jan 2021 16:37:49 GMT  
		Size: 54.6 MB (54620955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967eaceafc27fab6bb82d94ef81eba60a39ab7254392e41e8832a19e4e8d8ccc`  
		Last Modified: Tue, 12 Jan 2021 16:39:51 GMT  
		Size: 100.6 MB (100590856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39765e440505a9358049865f9848453ea9d1751875038c461f1d3939c67b1c90`  
		Last Modified: Tue, 12 Jan 2021 16:38:42 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; ppc64le

```console
$ docker pull golang@sha256:048cf7abac107fca26ecd7f3ace8ae1caf2eb17f8bdc1975f371dac343ec71f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300480257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e145621d346031997bf0d5cdc32a2d60f260d6cbf775cb5c187b17ebdc9b6c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 03:33:14 GMT
ADD file:3f6d74a3193dcc81fb8d9c0a830337812d5ed7618d5f16c8eb193d30f827c49d in / 
# Fri, 11 Dec 2020 03:33:24 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 11:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:35:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 11:37:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 21:16:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 21:16:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 21:16:32 GMT
ENV GOLANG_VERSION=1.15.6
# Thu, 17 Dec 2020 21:17:11 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 17 Dec 2020 21:17:26 GMT
ENV GOPATH=/go
# Thu, 17 Dec 2020 21:17:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 21:17:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Dec 2020 21:17:53 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:fbe5c9ac66677a4494c2d36707222498adce02d2dcb8e08d2f8a59a0f10b2582`  
		Last Modified: Fri, 11 Dec 2020 03:41:06 GMT  
		Size: 54.1 MB (54142548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ec43513b23f6fdf7966a25f8c07ddf163a83eecd7793ff3508c4c280091fba`  
		Last Modified: Thu, 17 Dec 2020 13:37:25 GMT  
		Size: 8.3 MB (8255775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d8dd70933f639bb084c14461d159384654d788cec2e4c66bef8c451f55207f`  
		Last Modified: Thu, 17 Dec 2020 13:37:24 GMT  
		Size: 10.7 MB (10727587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92278c25b4d152f837c7a5038f1a925f0e92765d08e01c91c4d5b74824b37f4`  
		Last Modified: Thu, 17 Dec 2020 13:38:28 GMT  
		Size: 57.5 MB (57455306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cbea48f4439e5a9bdbd42f016346e11b6575a9d43a241dbbc4ab3ee022b173`  
		Last Modified: Thu, 17 Dec 2020 21:21:17 GMT  
		Size: 73.6 MB (73612847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb827a757725a1f99148b265d8851dcfa3e78503e7a965990e34bbf4523a45b`  
		Last Modified: Thu, 17 Dec 2020 21:21:22 GMT  
		Size: 96.3 MB (96286039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416f692fa040553b5176745bad039f3cbe6a521d3b3ac60b182f6fbf9c184ccb`  
		Last Modified: Thu, 17 Dec 2020 21:21:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; s390x

```console
$ docker pull golang@sha256:1c8d37f9a3d21d9bef6cb7604a6df8b9f2027be221ff4132621794507f709878
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.4 MB (275445583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fc493d2320b8ce0a03297b7041d7108170460a87e0cc26ecd31f7b0b5c62e16`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:07 GMT
ADD file:7d0e79f65f07030b440bfbb8e3fac979eddeed967c5e47ac30b5c2aa5e0144b1 in / 
# Tue, 12 Jan 2021 00:42:09 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:10:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:10:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 02:10:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:12:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:12:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 15:13:02 GMT
ENV GOLANG_VERSION=1.15.6
# Tue, 12 Jan 2021 15:13:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 12 Jan 2021 15:13:33 GMT
ENV GOPATH=/go
# Tue, 12 Jan 2021 15:13:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 15:13:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jan 2021 15:13:34 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:15e71c2ae22f7fff5a03d5a2c1ccbee8b2526b04a21e1cff46ad70648272e773`  
		Last Modified: Tue, 12 Jan 2021 00:49:15 GMT  
		Size: 49.0 MB (48970492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aaa59f720edfbbd3dceca4a0253274b1730139ee512333e7ec6c74c77ae1a59`  
		Last Modified: Tue, 12 Jan 2021 02:20:09 GMT  
		Size: 7.4 MB (7386423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d930b55daa1d1253012758814d63e3c45e1eda80229b838a38e804e1aa47bbe2`  
		Last Modified: Tue, 12 Jan 2021 02:20:10 GMT  
		Size: 9.9 MB (9883004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950e64959dfb388a9874bb74ace538bd9da65024ea4fd0f99e2b995c57f1d976`  
		Last Modified: Tue, 12 Jan 2021 02:21:49 GMT  
		Size: 51.4 MB (51380119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fdb6f58c92c31b8a36f673fb66b9a831535bb25837f4f9f4b625fdd7c7cb96`  
		Last Modified: Tue, 12 Jan 2021 15:16:10 GMT  
		Size: 56.8 MB (56778961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feefcb4cb8875e1e49f2ef6daa3dbea29db786ed1b8b1ea8066b591bd2de3213`  
		Last Modified: Tue, 12 Jan 2021 15:18:16 GMT  
		Size: 101.0 MB (101046429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd3934ea0a961a15496e47638e8e426d7b59eb8483155abdccc46b642b6a662`  
		Last Modified: Tue, 12 Jan 2021 15:18:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
