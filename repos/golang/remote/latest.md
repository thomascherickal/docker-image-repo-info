## `golang:latest`

```console
$ docker pull golang@sha256:83171007a297bc768813be384eeff7ed7b475fc14b4d8593d85161a50ec70a9f
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
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `golang:latest` - linux; amd64

```console
$ docker pull golang@sha256:27a4178f1a02c2a2ca0070bd4be92b95fd9cbdd76eb49b54a688c08003bcb26f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.7 MB (309685389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e2ffcb73e11be90ae4bc6aabd584b9311c4ee1ce863001852954f6e63b202a6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:58 GMT
ADD file:9a4fd72d749f4a791e75e0f6fc6028d0771e3381b6d84a8d0b07a4887bc7c641 in / 
# Tue, 17 Nov 2020 20:20:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:30:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:30:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:31:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 02:09:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 02:09:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:36 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:21:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 04 Dec 2020 00:21:48 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:21:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:21:49 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:756975cb9c7e7933d824af9319b512dd72a50894232761d06ef3be59981df838`  
		Last Modified: Tue, 17 Nov 2020 20:27:06 GMT  
		Size: 50.4 MB (50397725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77915b4e630d47296770ce4cf481894885978072432456615172af463433cc5`  
		Last Modified: Wed, 18 Nov 2020 00:49:42 GMT  
		Size: 7.8 MB (7811717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f37a0a41b6b03489dd7de0aa2a79e369fd8b219bbc36b52f3f9790dc128e74b`  
		Last Modified: Wed, 18 Nov 2020 00:49:42 GMT  
		Size: 10.0 MB (9996233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b2c1e36db5f5910f58da2ca4f9311b0690810c7107fb055ee1541498b5061f`  
		Last Modified: Wed, 18 Nov 2020 00:50:25 GMT  
		Size: 51.8 MB (51829318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145393847161fdd9e821a7c92b53d37c33c5cc43d2e7fbe3391be04225418690`  
		Last Modified: Thu, 19 Nov 2020 02:12:35 GMT  
		Size: 68.7 MB (68698832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8843661db98315d49df0bcba0cc5044f5197d3f844fefb7f897d9e72ca3a08`  
		Last Modified: Fri, 04 Dec 2020 00:30:42 GMT  
		Size: 121.0 MB (120951438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218d240e42d495dd8ecd5d62e3ea9ba154c9cf22cb15e1438142a5d63b6127e7`  
		Last Modified: Fri, 04 Dec 2020 00:30:20 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v5

```console
$ docker pull golang@sha256:a8ce38b9a3a1f498610db9304a9253c81b8930794174e2bdede5f621465ffed1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.7 MB (269704069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d9d2679a7c7ce9d157ffaecb5cfbf44badda7832fef6f6877c86f4aea2643a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:16 GMT
ADD file:955829a14d270d20f9903754a57858fd2dbe3bcf8845491c1cdccae1e4896249 in / 
# Fri, 11 Dec 2020 02:04:20 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:44:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:45:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 02:46:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 13:15:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 13:15:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 13:15:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 13:18:59 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 11 Dec 2020 13:19:03 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 13:19:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 13:19:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 13:19:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d0f09cc3b3e26671eb372263913148f5c37e856980aa747129a90a3e14610461`  
		Last Modified: Fri, 11 Dec 2020 02:14:15 GMT  
		Size: 48.1 MB (48110951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6dfd2752660733cb28140557883aebafb300f8d5feb54cd866371882826509`  
		Last Modified: Fri, 11 Dec 2020 03:06:59 GMT  
		Size: 7.4 MB (7362304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70af9e49905885803a3a9fb626687874b912388320ca5bc2ab1f9ee2576787f1`  
		Last Modified: Fri, 11 Dec 2020 03:06:59 GMT  
		Size: 9.7 MB (9687464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7a4c35c3d9812b61f1c67d568bd52e4772ae28fe061416d94a4f1fe75c4e8e`  
		Last Modified: Fri, 11 Dec 2020 03:07:26 GMT  
		Size: 49.6 MB (49571487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8ce08bb2af7c8c6c5631b494cea2534aaee91d878e487bd9508631089f5ea3`  
		Last Modified: Fri, 11 Dec 2020 13:23:09 GMT  
		Size: 52.0 MB (52017456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685bc36dd16022b0d672cb824b421002f74285c5f476c98c04dc06ae5f48bd9f`  
		Last Modified: Fri, 11 Dec 2020 13:23:25 GMT  
		Size: 103.0 MB (102954251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a438fed67ffccc0534cdacf3fa56860c7107e0a9e25b2bbbf4a223b279dbfc`  
		Last Modified: Fri, 11 Dec 2020 13:22:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v7

```console
$ docker pull golang@sha256:6ab6b95325d829585d9aecf20e4d04aea14fc14a5d3420da767e81f65f0da832
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.7 MB (260697576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe33c3e9d8df6296b37eba5eaa1f87b190fd596063a4e6880f97672ad667813`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:08 GMT
ADD file:af46f686172bae3034ad0b34cc26081a2f8db0f5d4704ef63abb7eeaf06c75e0 in / 
# Fri, 11 Dec 2020 02:23:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:24:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:24:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:25:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 07:07:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 07:07:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Dec 2020 07:07:46 GMT
ENV GOLANG_VERSION=1.15.6
# Sat, 12 Dec 2020 07:08:09 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Sat, 12 Dec 2020 07:08:13 GMT
ENV GOPATH=/go
# Sat, 12 Dec 2020 07:08:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Dec 2020 07:08:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 12 Dec 2020 07:08:18 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:709549ab8c597dac59777a5a3666600f3dd986b5f05389aa7b15bd5f9281f809`  
		Last Modified: Fri, 11 Dec 2020 02:32:43 GMT  
		Size: 45.9 MB (45867902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ebb34ef82f207f1fe2804f394d61205a909e4ec6256fc1aa3a30b484c3176f`  
		Last Modified: Fri, 11 Dec 2020 16:43:39 GMT  
		Size: 7.1 MB (7099238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc4c14c5eea8f2b3009ee1de8df43fcf61c0a0d73af4efa97923119eae19bf`  
		Last Modified: Fri, 11 Dec 2020 16:43:38 GMT  
		Size: 9.3 MB (9343469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2d9bc5b9d534ac062b6fe74080e2674bdd0caef2d6c12cd1018d79ad0b02a`  
		Last Modified: Fri, 11 Dec 2020 16:44:04 GMT  
		Size: 47.4 MB (47356031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d510f956ca19e7e5e011500ac69859bb3f0ec5d9644a189a9da029499b4a2a`  
		Last Modified: Sat, 12 Dec 2020 07:11:37 GMT  
		Size: 53.2 MB (53177370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0264b1bfb1f5692ff335de9d9703c23977de3d4f09444b47bc070fe114fb2f3`  
		Last Modified: Sat, 12 Dec 2020 07:11:53 GMT  
		Size: 97.9 MB (97853411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f56cd943920d060011d4e2d75f10fb4f044cd7b8db279ec062be2a8f1827ed`  
		Last Modified: Sat, 12 Dec 2020 07:11:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:e2bf7b19b77d76173f838d071354190e3cd0f4171321a2ecdcb97bca41daa2dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.2 MB (279178700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1062e6aa0f48eccc9e1e3332be1114d5e02260ee9ef27a768032bb3ce163d782`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:23 GMT
ADD file:b08f373022952dba7d08b7fc02909d9e369c9727e0e4f62d6110e41e70e668cc in / 
# Fri, 11 Dec 2020 02:45:25 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 18:52:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 18:53:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 18:53:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 07:05:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 07:05:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Dec 2020 07:05:21 GMT
ENV GOLANG_VERSION=1.15.6
# Sat, 12 Dec 2020 07:05:36 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Sat, 12 Dec 2020 07:05:38 GMT
ENV GOPATH=/go
# Sat, 12 Dec 2020 07:05:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Dec 2020 07:05:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 12 Dec 2020 07:05:42 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:99e5136f81cd2a8cc226c42435d6f4f30584d168cc51f4d4afd2d5611e4d2215`  
		Last Modified: Fri, 11 Dec 2020 02:52:45 GMT  
		Size: 49.2 MB (49180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c9f56ed15888e5a0a9a8738d53044b1d62ff9f3c8c2857e5cebf782039305`  
		Last Modified: Fri, 11 Dec 2020 19:07:21 GMT  
		Size: 7.7 MB (7682310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33292316eac7d9491a0980a8cc9ba5f3e9cde7e2af0014f8dc10cdae5706b9d8`  
		Last Modified: Fri, 11 Dec 2020 19:07:22 GMT  
		Size: 10.0 MB (9984305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3287f43f5d44b20fe250f2683c57f0330bb0451261ad1d0c3eab9b116b0da52b`  
		Last Modified: Fri, 11 Dec 2020 19:07:44 GMT  
		Size: 52.2 MB (52164628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bade970b1e16ea06e96462b37c7f1d584e887ae47e2e43f081339e87057e15`  
		Last Modified: Sat, 12 Dec 2020 07:08:21 GMT  
		Size: 62.6 MB (62576989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5786ca6e9ad382561a85ef99b1f1355dd6d996e80de88cd065d263b6aaead6cc`  
		Last Modified: Sat, 12 Dec 2020 07:08:34 GMT  
		Size: 97.6 MB (97589996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6515b7c47497d5312d750a8c747e05354bb62e4d9327408f6e7f30e4696ececb`  
		Last Modified: Sat, 12 Dec 2020 07:08:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; 386

```console
$ docker pull golang@sha256:28ef9a17b8cefebb3cf12d09fed9f2a6d5dae791ab2d83800e35a8b4662dffcf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.9 MB (296890126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dd759c29a00a4c268c6473af0cf9beb7e4b1c28926e3ff6fa1820ab1fe2b4f4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:39 GMT
ADD file:4805e11ec22df9454eb4759523111e031e84c8078bcaef178f089baca9e83cdb in / 
# Tue, 17 Nov 2020 20:19:40 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:03:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:50:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:50:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:40:59 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:41:12 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 04 Dec 2020 00:41:13 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:41:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:41:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:41:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:21c39c42a8e082b1b164b44e463e4752c74821dbc51451f2ac2518ae6f29dff3`  
		Last Modified: Tue, 17 Nov 2020 20:26:25 GMT  
		Size: 51.2 MB (51159492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afab7b21aa8cddd140983ed21a34965621db1efb35f635bc756479b30c3deaf3`  
		Last Modified: Tue, 17 Nov 2020 21:23:47 GMT  
		Size: 8.0 MB (7981231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a1ce1fcda982662c6c9be38bac7b53e9fd405b0b367fa902cfd957be683731`  
		Last Modified: Tue, 17 Nov 2020 21:23:46 GMT  
		Size: 10.3 MB (10338498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a190a57cc81d3d40833225fd0b5e6bf1d793a9c09ba842367e28f584fc4ab5e7`  
		Last Modified: Tue, 17 Nov 2020 21:24:09 GMT  
		Size: 53.4 MB (53433407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9921dd4e18de5f4248d57558b544ccae22ed7928531aaeb12fd47f5b655ec179`  
		Last Modified: Wed, 18 Nov 2020 15:53:07 GMT  
		Size: 73.6 MB (73560882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea36b59455560748b01381a08c5e1c321f45e9cb03e7250d509f6467abe7a686`  
		Last Modified: Fri, 04 Dec 2020 00:51:19 GMT  
		Size: 100.4 MB (100416491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6602721803f0a26ddbb4a24708276f6ddf1db6c0615a6dfcc1ad88220db4cd6b`  
		Last Modified: Fri, 04 Dec 2020 00:50:54 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; mips64le

```console
$ docker pull golang@sha256:2f8ede076c295e61ddca4cf85f363fcab90459aa7564b301922dca8eeb7f29c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.3 MB (272325336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a5591b8466468733f09f670e5d9eb4a475314ed642c2dd6f1f1dc85a722af59`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:06 GMT
ADD file:de28e706af92bb73003a6ea1969c51666f52e0cd0286cbd99c624f3bc49e4666 in / 
# Fri, 11 Dec 2020 02:03:07 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:50:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:50:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 02:51:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:58:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:58:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:58:24 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 17:06:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 11 Dec 2020 17:06:04 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 17:06:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 17:06:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 17:06:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6057d98f1b0dc943648ced0ad33983792fadf9f1b0eaac90fd62165829122340`  
		Last Modified: Fri, 11 Dec 2020 02:09:27 GMT  
		Size: 49.0 MB (49022625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e90ff301a3d0d856fb4e7e6911036aa68b68b2c71f3be423ef654b42f0be98`  
		Last Modified: Fri, 11 Dec 2020 03:02:19 GMT  
		Size: 7.2 MB (7232151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9b5cb9bd92be17ad45be69b85a627b3fc368a8486765bd25f83e7916c0484`  
		Last Modified: Fri, 11 Dec 2020 03:02:18 GMT  
		Size: 10.0 MB (10016229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4576e15dbb62b557fb4030dd6fbc86324c2c98d2409f9b1fe6409accacd47f6a`  
		Last Modified: Fri, 11 Dec 2020 03:03:10 GMT  
		Size: 50.8 MB (50842772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04525548ecd8b3d9c70d8909b2c810df97eb5d72030517e62da2189c065ba1bb`  
		Last Modified: Fri, 11 Dec 2020 17:15:13 GMT  
		Size: 54.6 MB (54620725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b42083189cc0e7579b3bce993e0e922a645b2423dc40edee2fa68d53b0b1d0`  
		Last Modified: Fri, 11 Dec 2020 17:15:42 GMT  
		Size: 100.6 MB (100590709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709bba12a2e91d7dd71b46db36a4924c5f295c3889ee1a3f8438ab8f0b5e4d8`  
		Last Modified: Fri, 11 Dec 2020 17:14:32 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; ppc64le

```console
$ docker pull golang@sha256:77851ae23b2f5a4e82aefbbd09e06f5b20041abd88b9382b015ae6135eb31077
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300470638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e200bfc848f5d079e33718a11e32c81ee10ab4d4208d8b8da1fe00f0e61b5320`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 23:22:28 GMT
ADD file:b5112ae3b22de1d8a373191ad01151a6c1cdde605887b1836672be39787e2213 in / 
# Tue, 17 Nov 2020 23:22:37 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:55:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:57:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:59:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 17:14:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 17:14:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:54:47 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:55:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 04 Dec 2020 01:55:52 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:55:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:56:09 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:94e00adb98ff1f971add74025ff2a8ca87e003568d828bdb0df26ecd46c269a2`  
		Last Modified: Tue, 17 Nov 2020 23:31:43 GMT  
		Size: 54.1 MB (54143125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a46d858a6e31a5aa25fd9c527cdee95fe08fc11f45038212d1c5c7e52dc7b40`  
		Last Modified: Wed, 18 Nov 2020 01:53:05 GMT  
		Size: 8.3 MB (8255326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfab907b4d9fde9fb35f17a366b653e709c31cbce8602a2ae23c23d39524820`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 10.7 MB (10727375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157cce210a3874859c02d469911ddfc967ed435c3c04ebf12cdad81fe199cef0`  
		Last Modified: Wed, 18 Nov 2020 01:54:24 GMT  
		Size: 57.5 MB (57455140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a6669b63d2a6b953f45b160375ac1195d8a6206ece43030bc20b3c29b96f10`  
		Last Modified: Wed, 18 Nov 2020 17:18:16 GMT  
		Size: 73.6 MB (73603478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468b4de5736c75cf8fec17fcee21e22d2254d98240547e95f405d79d3381cc5c`  
		Last Modified: Fri, 04 Dec 2020 02:06:33 GMT  
		Size: 96.3 MB (96286038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cedacec81b58974781bbfd25f93bd3f7fc32603fb67e5ef5af877bcaf53976`  
		Last Modified: Fri, 04 Dec 2020 02:06:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; s390x

```console
$ docker pull golang@sha256:489b58c97d6f0d2b744745b420921da899f71c8cfbe6d48ded25bfab18fbc9f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.4 MB (275443746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dbe8f8115ca89e79b2458a2e19359c0f8102feba9aa71c8e7190c5782e319bf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:11:47 GMT
ADD file:b48379f9d2c111607924e8c59c2769c735341a59df0d6819d8a4b3e44f5457b0 in / 
# Fri, 11 Dec 2020 02:11:54 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:02:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:03:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:03:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:25:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:25:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 21:25:34 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 21:26:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-amd64.tar.gz'; 			sha256='3918e6cc85e7eaaa6f859f1bdbaac772e7a825b0eb423c63d3ae68b21f84b844'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-armv6l.tar.gz'; 			sha256='40ba9a57764e374195018ef37c38a5fbac9bbce908eab436370631a84bfc5788'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-arm64.tar.gz'; 			sha256='f87515b9744154ffe31182da9341d0a61eb0795551173d242c8cad209239e492'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-386.tar.gz'; 			sha256='ad187f02158b9a9013ef03f41d14aa69c402477f178825a3940280814bcbb755'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-ppc64le.tar.gz'; 			sha256='d4174fc217e749ac049eacc8827df879689f2246ac230d04991ae7df336f7cb2'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.6.linux-s390x.tar.gz'; 			sha256='839cc6b67687d8bb7cb044e4a9a2eac0c090765cc8ec55ffe714dfb7cd51cf3a'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 			sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 11 Dec 2020 21:26:17 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 21:26:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 21:26:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 21:26:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b8cd59e115fe85cdffdb9750beb150c189e768249dc100d22cab4733fb0c7247`  
		Last Modified: Fri, 11 Dec 2020 02:16:44 GMT  
		Size: 49.0 MB (48968242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0eb33d878287686bed77cfef9cecb3fd540caf075a646ed34afdb64288ae74`  
		Last Modified: Fri, 11 Dec 2020 16:15:45 GMT  
		Size: 7.4 MB (7386652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7571827f1162945abd5d70aa40ae2489e866f25a600c027f482c4dbd5bfc88`  
		Last Modified: Fri, 11 Dec 2020 16:15:45 GMT  
		Size: 9.9 MB (9883064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9e36ebe77bd8ffdf1d40b3ce51f765116b1fdc5aa75b3bd774c9388233fc72`  
		Last Modified: Fri, 11 Dec 2020 16:16:04 GMT  
		Size: 51.4 MB (51379787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a6ea024810aa241b2b42c85d54a291e96bb88745b234d7bf45ed0d5fd51dcd`  
		Last Modified: Fri, 11 Dec 2020 21:28:49 GMT  
		Size: 56.8 MB (56779372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef7214cb47029597e0a31303f202968cad8153d8241038efba74854a2a935fe`  
		Last Modified: Fri, 11 Dec 2020 21:28:55 GMT  
		Size: 101.0 MB (101046473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8078310c9c2c3ba6296df8f2f28ce5d8acdff2bf1d6297cfa278603305e0a1`  
		Last Modified: Fri, 11 Dec 2020 21:28:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.17763.1637; amd64

```console
$ docker pull golang@sha256:9dd287a431b6f190ada80d11313382a195de99dec346306fc51361ebda507cf2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2563861826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:568e89632cb13746350f24e35ff0017b56fd1446e0ec3f89bfe0b82c9c51fdda`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:30:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:30:19 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:31:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:31:35 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:31:57 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:31:58 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:34:28 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:34:29 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea5287e7eabe2989764541d2d84c4676b838a30a6cf7582ae1634e551b3ef2f`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588b553e313f50806677aefb0ecff1b14bc3bf2af3502007ed9a8d56a8583fc5`  
		Last Modified: Wed, 09 Dec 2020 13:54:35 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dbdf38d85835112bbd66c15c88fa10af5cc452590f50bed5c4eb114aef12e9`  
		Last Modified: Wed, 09 Dec 2020 13:54:34 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b50f011f5bd2ab0eaef775ba7b2f9a5fbb8d05f53f675cfb55480847fa80c3`  
		Last Modified: Wed, 09 Dec 2020 13:54:27 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9000bff3ee5b419217d7c208139db32357708f5e042073232d013021b9648`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 34.3 MB (34329902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb549abdec7bb8d4debb3e8d9c2220fe8a39c707f3b55ca0041105f451407112`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766c92af76c17356f7a58754b35eef18ba39be13fac5c7122c2fdcf092668de`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 293.7 KB (293711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316565f55d31523fdfcb01911fc30d22ac533ba7caf3a6b1b1c82d4e5a1ba3ab`  
		Last Modified: Wed, 09 Dec 2020 13:54:25 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0d077fdd4cfce06b53ec657234fc70f93c76e7b88bbaa5e2688abfc5690507`  
		Last Modified: Wed, 09 Dec 2020 13:54:59 GMT  
		Size: 138.4 MB (138354476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b3459f90d7ddb0bf00cf559125df32dad069cd1666c5ed6303f427233fcb`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.14393.4104; amd64

```console
$ docker pull golang@sha256:be19477f781e64be6143e4e80358a52808f2fb31e6729f60f5acc715932b3734
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5953139280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3751933261827e2b3d0c44ba90b254be833fc9f97b484d41e53976eb933d6cde`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:34:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:34:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:36:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:36:54 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:38:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:38:11 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:41:41 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:41:43 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f374b7a81d8d1da3ea2e749c7510b6aa8464f5cf9cfd8635eee23c26c264186`  
		Last Modified: Wed, 09 Dec 2020 13:55:32 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c2e54f8832483cbe5f46ec46fd2932e9656680f47c5811d036e1f9c60f9b79`  
		Last Modified: Wed, 09 Dec 2020 13:55:30 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a357d7b727e3e4efaec8f4443236eb37c1fed68ca863b98d5b19ad17395225`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0785c68a2876dc32a5ff5aea8c9dbaddcea68864db06f5af609f3f65240a9`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661765d49c7f605a23d3caa9a99455ce231aa2576dd72ff0b8eab7a5e2ec7ce6`  
		Last Modified: Wed, 09 Dec 2020 13:56:06 GMT  
		Size: 35.1 MB (35137422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4862d1f955bf7fa5325ae4ff054954789b3895bf8fab9ecc625537f8f673abd5`  
		Last Modified: Wed, 09 Dec 2020 13:55:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc55fb10a0bab3af9f2e63e7fcb33ba85af44f9e4877a85c0301a6114533edd`  
		Last Modified: Wed, 09 Dec 2020 13:55:26 GMT  
		Size: 5.5 MB (5497159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8203b1d27b0d111a6fbb09e09707cebb1991dc96c22cb61122d7b3a11c9ee`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa19bd5b077ef4c72c70c3a038e75d69dcf133835ba71839ee690433c01736f`  
		Last Modified: Wed, 09 Dec 2020 13:55:58 GMT  
		Size: 143.7 MB (143651420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5437279258059e7b08038e7ec5bd346c95f4bf73e1cb030bdd90ecd1128a7870`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
