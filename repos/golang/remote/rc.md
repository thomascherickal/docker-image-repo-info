## `golang:rc`

```console
$ docker pull golang@sha256:d82f9e20b4f771a64482d3924d823746b0fab3c64cdaad6b78425b326885a99f
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
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `golang:rc` - linux; amd64

```console
$ docker pull golang@sha256:d9016519ab0ac9aea149ed1e30a2ca8dd74b33ae12cd79dab729dc7f93489d08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.2 MB (320241434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84043852736f0b2b6900324ab23e237d5b124e5f1f6df4ed31c5b84317b8148b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 03:57:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:22:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:22:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:33:24 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 22:33:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-amd64.tar.gz'; 			sha256='6a62610f56a04bae8702cd2bd73bfea34645c1b89ded3f0b81a841393b6f1f14'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-armv6l.tar.gz'; 			sha256='ab8d1447a2d74ab61aadbbed8229d9d0cf465959290a55fd5b82824a25aae2cf'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-arm64.tar.gz'; 			sha256='ba6769f0e2051fcb5418c4ba9b3f12fe7776f865e8ae8692d71efed74c4373fa'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-386.tar.gz'; 			sha256='53eb05c57a5e0deb8ac12fa10e7452c1395a500cae40acbdcd90b5f94218b36c'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-ppc64le.tar.gz'; 			sha256='c99498c31e41dd6478a9f0326d75c9ac44e8a994564d9eedee30cb40f5ae273c'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-s390x.tar.gz'; 			sha256='d3819118e8e3696776e9dc0abfedb701b38db1c4d40480a0a162c2be5df96062'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 			sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 28 Jan 2021 22:33:39 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 22:33:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:33:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 22:33:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fd949ed9338da3c1e09f9b75408c214368c637c448e0fd839467f6f7717b5`  
		Last Modified: Tue, 12 Jan 2021 04:06:20 GMT  
		Size: 51.8 MB (51830144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547cc43be03d30dadf175bfd9e0e67b4ee2ba5bc2b948a071c1181566f700b7c`  
		Last Modified: Tue, 12 Jan 2021 23:25:17 GMT  
		Size: 68.7 MB (68708498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959a73be579abf072bebf4bdfc63291b99f7fe954dfb72b3d421d3697ac0c603`  
		Last Modified: Thu, 28 Jan 2021 22:40:33 GMT  
		Size: 131.5 MB (131495102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3486d0e5e2aef7f66c3957b7a83e9095d9e0fc85bdca2b2d7265dc3675edd97a`  
		Last Modified: Thu, 28 Jan 2021 22:40:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; arm variant v5

```console
$ docker pull golang@sha256:0d81d22646d87b5730eba05e7a65731f0396ada8574c2d08d8d828c8f5a2b001
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271750680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9066e7e4502cb38d46013c87c02a40a33fed4ec43e6cc98193883ecb54a5c583`
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
# Thu, 28 Jan 2021 21:48:31 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 21:52:04 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-amd64.tar.gz'; 			sha256='6a62610f56a04bae8702cd2bd73bfea34645c1b89ded3f0b81a841393b6f1f14'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-armv6l.tar.gz'; 			sha256='ab8d1447a2d74ab61aadbbed8229d9d0cf465959290a55fd5b82824a25aae2cf'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-arm64.tar.gz'; 			sha256='ba6769f0e2051fcb5418c4ba9b3f12fe7776f865e8ae8692d71efed74c4373fa'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-386.tar.gz'; 			sha256='53eb05c57a5e0deb8ac12fa10e7452c1395a500cae40acbdcd90b5f94218b36c'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-ppc64le.tar.gz'; 			sha256='c99498c31e41dd6478a9f0326d75c9ac44e8a994564d9eedee30cb40f5ae273c'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-s390x.tar.gz'; 			sha256='d3819118e8e3696776e9dc0abfedb701b38db1c4d40480a0a162c2be5df96062'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 			sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 28 Jan 2021 21:52:09 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 21:52:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 21:52:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 21:52:12 GMT
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
	-	`sha256:6ee894253f7263c55db13715992a0f0475361f9d962764adb125280ce28e32b7`  
		Last Modified: Thu, 28 Jan 2021 21:53:23 GMT  
		Size: 105.0 MB (104998436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f87752f558b7ac28e5fa6fd6ed691c41da3d0158401475d6a9616912a299fe7`  
		Last Modified: Thu, 28 Jan 2021 21:52:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; arm variant v7

```console
$ docker pull golang@sha256:87e64e1b0cf091d931c4123ea671db3c9126a1c059f08c2ea1192a25e6398bec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.6 MB (265593475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb161d9a67dc78dbc0660281c218e21eaf723629104881543f3ebd1c2f8c813`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:00:37 GMT
ADD file:216371f6fe8c803a0191f84e555c809a3301d1344c62b831dddb5e0c595fe0ef in / 
# Tue, 12 Jan 2021 00:00:46 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:14:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:15:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 19:49:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 19:49:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:01:40 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 22:02:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-amd64.tar.gz'; 			sha256='6a62610f56a04bae8702cd2bd73bfea34645c1b89ded3f0b81a841393b6f1f14'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-armv6l.tar.gz'; 			sha256='ab8d1447a2d74ab61aadbbed8229d9d0cf465959290a55fd5b82824a25aae2cf'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-arm64.tar.gz'; 			sha256='ba6769f0e2051fcb5418c4ba9b3f12fe7776f865e8ae8692d71efed74c4373fa'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-386.tar.gz'; 			sha256='53eb05c57a5e0deb8ac12fa10e7452c1395a500cae40acbdcd90b5f94218b36c'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-ppc64le.tar.gz'; 			sha256='c99498c31e41dd6478a9f0326d75c9ac44e8a994564d9eedee30cb40f5ae273c'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-s390x.tar.gz'; 			sha256='d3819118e8e3696776e9dc0abfedb701b38db1c4d40480a0a162c2be5df96062'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 			sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 28 Jan 2021 22:02:06 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 22:02:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:02:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 22:02:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d8925d905dadf63fa0ff74be912443a1cf8cd72ea5543317b0e22067d39ef948`  
		Last Modified: Tue, 12 Jan 2021 00:10:42 GMT  
		Size: 45.9 MB (45870031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd9c5a6d77413d17345fcf1f89b9dde2f3d9d6157bd070d4093cfef30107add`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 7.1 MB (7099141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e1f8e87a65e3a71764ea79b951f915c90a885dfd516f61e57d81745acaf272`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 9.3 MB (9343447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43213eb5a44e08394e2dfcfb96a0577df6dea9ae20ef636053cf840a14d7cad`  
		Last Modified: Tue, 12 Jan 2021 01:30:16 GMT  
		Size: 47.4 MB (47355871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e230a9dc5b7d6af1fad8076c109e8ff819f32761931cd9ddef1356053f6ed3db`  
		Last Modified: Tue, 12 Jan 2021 19:54:07 GMT  
		Size: 53.2 MB (53177068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036e217301329b264e9171b6d87f1e0b3f429961640cf63fa3d21dc6df67cc25`  
		Last Modified: Thu, 28 Jan 2021 22:09:38 GMT  
		Size: 102.7 MB (102747761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b941e668039f44810484fa6810193fcce90cdb9174a2c2a9e1b811b4c1ea0c`  
		Last Modified: Thu, 28 Jan 2021 22:09:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:6babbff133294be528988eb8b50d06b720c552375475b9cd36453c3eba32d675
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.6 MB (283648745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb898697d99114c3e2d42b02cc82640c0610491d4c84a9a00974cc3939724a6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:40:39 GMT
ADD file:849d424ecc8572facb3ca68eff836dce211bc677cb32d3c3eaa129d364d33878 in / 
# Tue, 12 Jan 2021 00:40:43 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:24:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 20:17:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 20:17:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 21:43:09 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 21:43:26 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-amd64.tar.gz'; 			sha256='6a62610f56a04bae8702cd2bd73bfea34645c1b89ded3f0b81a841393b6f1f14'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-armv6l.tar.gz'; 			sha256='ab8d1447a2d74ab61aadbbed8229d9d0cf465959290a55fd5b82824a25aae2cf'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-arm64.tar.gz'; 			sha256='ba6769f0e2051fcb5418c4ba9b3f12fe7776f865e8ae8692d71efed74c4373fa'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-386.tar.gz'; 			sha256='53eb05c57a5e0deb8ac12fa10e7452c1395a500cae40acbdcd90b5f94218b36c'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-ppc64le.tar.gz'; 			sha256='c99498c31e41dd6478a9f0326d75c9ac44e8a994564d9eedee30cb40f5ae273c'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-s390x.tar.gz'; 			sha256='d3819118e8e3696776e9dc0abfedb701b38db1c4d40480a0a162c2be5df96062'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 			sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 28 Jan 2021 21:43:30 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 21:43:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 21:43:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 21:43:34 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6e5587ff5efa4e647ae927194fac9b961a68d46b23b68a3119c90016e58f17aa`  
		Last Modified: Tue, 12 Jan 2021 00:51:18 GMT  
		Size: 49.2 MB (49183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439dbbb05ea0aa8484ae8a51d0fbb1c7609176a1b0d3f15dad69d52e9a83af66`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 7.7 MB (7682325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b89c8b4e5b232c040d5905808ee62cdfcc9d697de10183d6bc4767468859d92`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 10.0 MB (9984327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53f70a43c3c83782c39cad75aa09ccddb893b3fd54762416fca4d48a3b44b5`  
		Last Modified: Tue, 12 Jan 2021 01:38:54 GMT  
		Size: 52.2 MB (52163502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56052def468cb5c58be8e760350fc9a45d39c59eee37508312766e5c982dd99`  
		Last Modified: Tue, 12 Jan 2021 20:21:42 GMT  
		Size: 62.6 MB (62577187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c54060fd5372ef959a53157b33e7206ee9c8375208c5e752983375496f9b3c`  
		Last Modified: Thu, 28 Jan 2021 21:50:23 GMT  
		Size: 102.1 MB (102057513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789fb76bdbb61b06cb23947ac7b9fafc3595c6220f9baa5884a5774cde4f879c`  
		Last Modified: Thu, 28 Jan 2021 21:49:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; 386

```console
$ docker pull golang@sha256:81cd7b615d3e8b3a08b599b95462d3ce3a131e89f5f2ade9762caa637c6bcce7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.0 MB (302036859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a78c6a240e0da041fa9ce6eaa358dcdb44ea3ab0f46ff01c2b329efa765bd0`
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
# Thu, 28 Jan 2021 21:41:12 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 21:41:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-amd64.tar.gz'; 			sha256='6a62610f56a04bae8702cd2bd73bfea34645c1b89ded3f0b81a841393b6f1f14'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-armv6l.tar.gz'; 			sha256='ab8d1447a2d74ab61aadbbed8229d9d0cf465959290a55fd5b82824a25aae2cf'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-arm64.tar.gz'; 			sha256='ba6769f0e2051fcb5418c4ba9b3f12fe7776f865e8ae8692d71efed74c4373fa'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-386.tar.gz'; 			sha256='53eb05c57a5e0deb8ac12fa10e7452c1395a500cae40acbdcd90b5f94218b36c'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-ppc64le.tar.gz'; 			sha256='c99498c31e41dd6478a9f0326d75c9ac44e8a994564d9eedee30cb40f5ae273c'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-s390x.tar.gz'; 			sha256='d3819118e8e3696776e9dc0abfedb701b38db1c4d40480a0a162c2be5df96062'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 			sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 28 Jan 2021 21:41:28 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 21:41:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 21:41:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 21:41:29 GMT
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
	-	`sha256:dbe29120c3e220f0a71475c1e6043b71421f34a0f76ffa641ee373df37fa493d`  
		Last Modified: Thu, 28 Jan 2021 21:44:20 GMT  
		Size: 105.5 MB (105546018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b4acaf1c099c7fc6b3bc2fef84705ee4d1a86c9fe7e993a19a5aac804a268b`  
		Last Modified: Thu, 28 Jan 2021 21:43:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; mips64le

```console
$ docker pull golang@sha256:f3d80c4a11f8b13e3c5f7384a07769d0016e9b6905d010ad2017f955f6ea8fc0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.8 MB (273782065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1197ac14bb161c6ca8f95055f8a2274c36e4c58643baebe50f614c65f5752bd3`
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
# Thu, 28 Jan 2021 22:07:22 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 22:15:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-amd64.tar.gz'; 			sha256='6a62610f56a04bae8702cd2bd73bfea34645c1b89ded3f0b81a841393b6f1f14'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-armv6l.tar.gz'; 			sha256='ab8d1447a2d74ab61aadbbed8229d9d0cf465959290a55fd5b82824a25aae2cf'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-arm64.tar.gz'; 			sha256='ba6769f0e2051fcb5418c4ba9b3f12fe7776f865e8ae8692d71efed74c4373fa'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-386.tar.gz'; 			sha256='53eb05c57a5e0deb8ac12fa10e7452c1395a500cae40acbdcd90b5f94218b36c'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-ppc64le.tar.gz'; 			sha256='c99498c31e41dd6478a9f0326d75c9ac44e8a994564d9eedee30cb40f5ae273c'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-s390x.tar.gz'; 			sha256='d3819118e8e3696776e9dc0abfedb701b38db1c4d40480a0a162c2be5df96062'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 			sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 28 Jan 2021 22:15:18 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 22:15:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:15:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 22:15:20 GMT
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
	-	`sha256:d62fd64c0a5841baef33eb3d60d96d2e23c5896e827359af6697617a863b23fc`  
		Last Modified: Thu, 28 Jan 2021 22:17:06 GMT  
		Size: 102.0 MB (102044769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115d44c47ce40cd884e033f4e285813c92154ef7a88f61bed32a6bf7b8cd8889`  
		Last Modified: Thu, 28 Jan 2021 22:15:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; ppc64le

```console
$ docker pull golang@sha256:093ad61ddd1b6293d44a96e2921857f084a8b2f12bde03f7ade86de978912f4a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.7 MB (304740380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36161c6efcbfd8410c5fa148b6f97c861b8ca9963337896c557811f80f01e204`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:24:16 GMT
ADD file:cebd019e462ded2318bdc6bbfa649ddd11dc15d005b0f330876282e08143e069 in / 
# Tue, 12 Jan 2021 00:24:28 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:59:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:00:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 02:03:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 19:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 19:57:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:31:38 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 22:32:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-amd64.tar.gz'; 			sha256='6a62610f56a04bae8702cd2bd73bfea34645c1b89ded3f0b81a841393b6f1f14'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-armv6l.tar.gz'; 			sha256='ab8d1447a2d74ab61aadbbed8229d9d0cf465959290a55fd5b82824a25aae2cf'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-arm64.tar.gz'; 			sha256='ba6769f0e2051fcb5418c4ba9b3f12fe7776f865e8ae8692d71efed74c4373fa'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-386.tar.gz'; 			sha256='53eb05c57a5e0deb8ac12fa10e7452c1395a500cae40acbdcd90b5f94218b36c'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-ppc64le.tar.gz'; 			sha256='c99498c31e41dd6478a9f0326d75c9ac44e8a994564d9eedee30cb40f5ae273c'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-s390x.tar.gz'; 			sha256='d3819118e8e3696776e9dc0abfedb701b38db1c4d40480a0a162c2be5df96062'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 			sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 28 Jan 2021 22:32:47 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 22:32:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:33:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 22:33:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f55666525fdfb3052e2a27209639b4e83b4d5c8ca7cfcff8525f50f63345cc0d`  
		Last Modified: Tue, 12 Jan 2021 00:33:32 GMT  
		Size: 54.1 MB (54144733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a708f84b552354f6bd7c8b378ef1e6115050807ae6691c9d0673313a9bc6efe`  
		Last Modified: Tue, 12 Jan 2021 02:39:01 GMT  
		Size: 8.3 MB (8255846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7316456c5112c2c378cba4cdaa76f5ef1a261726c4c1bbbb78d3e55412bdcbbb`  
		Last Modified: Tue, 12 Jan 2021 02:39:02 GMT  
		Size: 10.7 MB (10727570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f5c800c03748ea756d5667879a46f6fc464545603bff606353bb4fc2039985`  
		Last Modified: Tue, 12 Jan 2021 02:39:31 GMT  
		Size: 57.5 MB (57455589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9020b6f08e528d8da40ae076803bb543c9c9124f9c9cb7374f0600c82f03c42d`  
		Last Modified: Tue, 12 Jan 2021 20:03:55 GMT  
		Size: 73.6 MB (73612260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737560bd2173a94b5e39f860cc230658889fd5152338bc59efe50854b77a6d04`  
		Last Modified: Thu, 28 Jan 2021 23:01:55 GMT  
		Size: 100.5 MB (100544227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcb4beba88720a966ae3045ae071f6ce31daf2f4084098603ec1790bb5712d8`  
		Last Modified: Thu, 28 Jan 2021 23:01:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; s390x

```console
$ docker pull golang@sha256:9ced73f90c57b0159d2bb6eeedd66c6d29bdb5f88992fdb8cda63c643062e04b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.1 MB (280080528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f26104cc33543f18de31c0efaff177146b088e71a234db597a32aa1300bb7c99`
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
# Thu, 28 Jan 2021 21:44:08 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 21:44:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-amd64.tar.gz'; 			sha256='6a62610f56a04bae8702cd2bd73bfea34645c1b89ded3f0b81a841393b6f1f14'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-armv6l.tar.gz'; 			sha256='ab8d1447a2d74ab61aadbbed8229d9d0cf465959290a55fd5b82824a25aae2cf'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-arm64.tar.gz'; 			sha256='ba6769f0e2051fcb5418c4ba9b3f12fe7776f865e8ae8692d71efed74c4373fa'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-386.tar.gz'; 			sha256='53eb05c57a5e0deb8ac12fa10e7452c1395a500cae40acbdcd90b5f94218b36c'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-ppc64le.tar.gz'; 			sha256='c99498c31e41dd6478a9f0326d75c9ac44e8a994564d9eedee30cb40f5ae273c'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16rc1.linux-s390x.tar.gz'; 			sha256='d3819118e8e3696776e9dc0abfedb701b38db1c4d40480a0a162c2be5df96062'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 			sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 28 Jan 2021 21:44:59 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 21:45:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 21:45:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 21:45:03 GMT
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
	-	`sha256:56f56466658f2b7545abbf85abb18d0d6b224a0c2bc096ee2b4b9ccdd11b89c1`  
		Last Modified: Thu, 28 Jan 2021 21:52:12 GMT  
		Size: 105.7 MB (105681374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620d8e9c93356a561e0de576ffe6a2632017fe78f74fb73467f5f60bf62848fd`  
		Last Modified: Thu, 28 Jan 2021 21:51:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - windows version 10.0.17763.1697; amd64

```console
$ docker pull golang@sha256:eab1fee81cddd149939e0a49487d014199c014f7a8a540ef86c5e1500e035b9b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2616732158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05dbe6a3dcd326f4cf6d902d71e986cac57b3419f253b3cb0126df059498695c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:32:54 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:32:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:34:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:34:01 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:34:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 28 Jan 2021 22:15:09 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 22:17:54 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16rc1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ff765c31cf321b431f9a11ec42e61d42ec87d56333c847f5a87d30e01aaed3df'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 28 Jan 2021 22:17:56 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad72ac4b6931b207a545d6d62fda35143222f3144778d4338ba25345066dce83`  
		Last Modified: Wed, 13 Jan 2021 15:07:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa315e63f98a74b6d8eaa632289849e8ec86de24cc05b5a05e0f5e60fef47ca1`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32646dc4c31ba7b4756ec7a55372b0b826608da90c73a1b0e70be1ec400e5cd9`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e012143f550ba0c16a6368ae3695a74a56b153468e98d9c463221448e557b`  
		Last Modified: Wed, 13 Jan 2021 15:07:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de36418fb6d968516c8374e5baf49e2bce6bbab4a107753c235e67c36187e16`  
		Last Modified: Wed, 13 Jan 2021 15:07:25 GMT  
		Size: 34.5 MB (34452685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349aa2cb74f5d5cc343c42d6ba9fec62a6885cedcc0f07995fa77e3f68c6ac75`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384ca1dabb9f23cb13f29f907b3a436e7676da86a825631d876e4a204898b47`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 300.8 KB (300786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b6a6481463d674e2541f9548437b0694c6b21040ac95394b5db9a251182957`  
		Last Modified: Thu, 28 Jan 2021 22:25:56 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0cf59654e1fe2f990fb20368543d37a620de732f3052fa3cc52d760ef60d6c`  
		Last Modified: Thu, 28 Jan 2021 22:26:25 GMT  
		Size: 146.2 MB (146196885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca46333b7a04ad7c15c641dcc90ab7ee13975652aaf02db11b001b29d9357aa`  
		Last Modified: Thu, 28 Jan 2021 22:25:56 GMT  
		Size: 1.5 KB (1486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - windows version 10.0.14393.4169; amd64

```console
$ docker pull golang@sha256:eeccbf3e2365acd6ce8525219c19308812d2c442819e9bb0dfbd7015efd857e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5986364949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29fc242d897dacfcf033bf3a964b505a82962acac655439673900199bdff39ca`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:37:07 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:37:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:39:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:39:19 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:40:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 28 Jan 2021 22:18:05 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 22:21:46 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16rc1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ff765c31cf321b431f9a11ec42e61d42ec87d56333c847f5a87d30e01aaed3df'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 28 Jan 2021 22:21:48 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7c74b9f7bda8494c06b61f172b711267512a7eef464aae2946fa79f14fbc6c`  
		Last Modified: Wed, 13 Jan 2021 15:10:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16980afcb11d4373e2ced6b4e81c79cdc57071c5b2d049925d8103e3b1685c0a`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b769faccdc304e663d15a124104d2aaa3ac8f722d364a8196f27a3cb7485cd`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee85b465f4b2c47a1ed4af61a17e4f6bd1f26c42b26eeba881f2a5fdf182619`  
		Last Modified: Wed, 13 Jan 2021 15:10:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a900fab54fda5407bf2c34f918f84f42c2ba78c89b79b10e5a8059a642814c5`  
		Last Modified: Wed, 13 Jan 2021 15:10:31 GMT  
		Size: 35.2 MB (35242884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4728bca9e3e0ca560fb0489af700986254ac669509fff4e8e8e208dde2bf3`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7738a5c4a381adacded290e0ed60fb37c9afa472ca097aae390199b16f444d`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 5.6 MB (5599196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3840ef2f76151d14cd1b058810702944fea5dddaa28265ed3e6d70c881080978`  
		Last Modified: Thu, 28 Jan 2021 22:26:39 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85eb243014ffd4c407fb8175909b09652d871d8f4decaf4ab33e57b26b256584`  
		Last Modified: Thu, 28 Jan 2021 22:27:10 GMT  
		Size: 151.6 MB (151619100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23d2a83ddae0accffbd23b03defe4408e46b93247a42e4b22d4b43db04b3b1d`  
		Last Modified: Thu, 28 Jan 2021 22:26:39 GMT  
		Size: 1.5 KB (1487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
