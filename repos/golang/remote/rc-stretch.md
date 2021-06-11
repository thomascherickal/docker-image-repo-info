## `golang:rc-stretch`

```console
$ docker pull golang@sha256:196c4d0dc637fec1ee77d38fc4d9b9a3cde4d1d48493abc5e76488b6ea9b65b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:rc-stretch` - linux; amd64

```console
$ docker pull golang@sha256:3b30007c5493f7677c1542771ffc419be21689b33943f592de5875aef5fdc26f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.1 MB (303070490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf49fc180be79214be7d2da9c09d84c675fa7eedfb23e28b3e0b3c4d38652a9d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 02:00:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 19:24:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 19:24:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:20:09 GMT
ENV GOLANG_VERSION=1.17beta1
# Thu, 10 Jun 2021 21:20:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 10 Jun 2021 21:20:25 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:20:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:20:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:20:26 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc05be471d511acb4574f2f3630582527220c59d0abf0b8b905769916b550da7`  
		Last Modified: Wed, 12 May 2021 02:07:47 GMT  
		Size: 49.8 MB (49761958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5f37b059cbbd605939f3fbcfca7a525801e063821b2894ec23a1f3ee438e04`  
		Last Modified: Wed, 12 May 2021 19:26:51 GMT  
		Size: 57.8 MB (57829203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc408783984423c95b8a970893dab1f6d838dbd91ef4a93fd9c1d5d3d874793`  
		Last Modified: Thu, 10 Jun 2021 21:34:00 GMT  
		Size: 134.5 MB (134470225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b4f674571595e8c2c78df1abc2fdb58e710123e7e480705c22dd898d644b63`  
		Last Modified: Thu, 10 Jun 2021 21:33:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:ae01612148ebf3d153792d87b57af6057f5c07f10ba52497044520a3abc06dad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.3 MB (251277472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c61980ac232362c2277aa9d026eb7fb1fa5a0d671f55cb57fec91ce456d3786`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:11:51 GMT
ADD file:81cfd4e746bdfcc19847240b77012487652be22dbd5741ccb2485a4207f2b73f in / 
# Wed, 12 May 2021 01:11:56 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:45:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 00:46:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:06:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:06:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:25:50 GMT
ENV GOLANG_VERSION=1.17beta1
# Thu, 10 Jun 2021 22:26:05 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 10 Jun 2021 22:26:06 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:26:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:26:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:26:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:55b9a6b6b2552c5b2eac0a316e75a7bc18092819ee25c4f1d4d54700bcc1d3dc`  
		Last Modified: Wed, 12 May 2021 01:21:23 GMT  
		Size: 42.1 MB (42120307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba756a0ca8996787a145d62543ecf7cec523a638705be132f442d2013655149`  
		Last Modified: Thu, 27 May 2021 01:06:39 GMT  
		Size: 10.0 MB (9950803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61945aef6a8fee06fbe4dccead7cbad9da46ba174cee1eae1f813541ddb76b3`  
		Last Modified: Thu, 27 May 2021 01:06:38 GMT  
		Size: 3.9 MB (3921169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad0df1f1fa0c631401a3729be99927a3afcaa022e4dd89e0acc026805d6fd2d`  
		Last Modified: Thu, 27 May 2021 01:07:07 GMT  
		Size: 46.1 MB (46125973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f715490688df009fde145956077633ac3ba88d28e792c423c27e175c0b286abb`  
		Last Modified: Thu, 27 May 2021 15:19:02 GMT  
		Size: 46.2 MB (46161293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9617e30b96f91748deed7fd684a97311192d17f0b05006e2df91a81b846e93fb`  
		Last Modified: Thu, 10 Jun 2021 22:51:05 GMT  
		Size: 103.0 MB (102997772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78cf2c2a56e2c302f40a7fe0c16e8076ae89d8cd71111c9ab454e31cc298294`  
		Last Modified: Thu, 10 Jun 2021 22:50:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:5af7a19aa52a5b46c580c7759f478eb73e933d2accb166aac4fc0372ea1ca7ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.0 MB (256983517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff7704243e05d65c440d8450ee79b1309ff7f3db0706a1141309b80fcee74f4b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:56:12 GMT
ADD file:9582243afc9973a3708fda530270ae8f23796b20a532a9f07e4faaf245e2cdc0 in / 
# Wed, 12 May 2021 00:56:18 GMT
CMD ["bash"]
# Thu, 27 May 2021 20:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 20:54:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 20:54:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 22:17:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 22:17:09 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:40:06 GMT
ENV GOLANG_VERSION=1.17beta1
# Thu, 10 Jun 2021 21:40:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 10 Jun 2021 21:40:18 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:40:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:40:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:40:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:41f38ce3010a5142300d74e5e19db4dea7694f4771471c330fff27c633f8ba32`  
		Last Modified: Wed, 12 May 2021 01:04:15 GMT  
		Size: 43.2 MB (43177820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce440adabe2a1239387777b4e56ce06814fe9b17d519fc476a46594611db4f32`  
		Last Modified: Thu, 27 May 2021 21:07:51 GMT  
		Size: 10.2 MB (10214833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c0a158e8c10a9879f2c775b2d7a4483d25019616d9391af775249d584b41e8`  
		Last Modified: Thu, 27 May 2021 21:07:50 GMT  
		Size: 4.1 MB (4096675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82fbf846f6fdcc504df83891d0f286583888d4c91c733ee2395a16ff234988d`  
		Last Modified: Thu, 27 May 2021 21:08:11 GMT  
		Size: 47.7 MB (47736501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507346c86f2bc850d46a0301c496e94608957beb4d31bd613014b560deed639d`  
		Last Modified: Thu, 27 May 2021 22:26:17 GMT  
		Size: 49.2 MB (49224661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283956769da4c94ead9a7cdb6dbeb690477bb1ea35f455fa590191cf3af7553`  
		Last Modified: Thu, 10 Jun 2021 21:53:09 GMT  
		Size: 102.5 MB (102532871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab4c1a3c948928376975cb65dc56f42029d018f85e46560f81018adb9c5eac`  
		Last Modified: Thu, 10 Jun 2021 21:52:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; 386

```console
$ docker pull golang@sha256:761e300a3487364967bd9194591265a95b98a7cb502682ebf95e0cbe0c1d0770
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281148465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d7c1b1b9fc31c9371d8810262824061f8bfbdcb4c1daeef61d938c02f53cc5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:41:41 GMT
ADD file:3b26e2f83a0edf42ea62d20102b47011ee41cd2ab349c9da7487f62ff21b8471 in / 
# Wed, 12 May 2021 00:41:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:12:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:12:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:13:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:28:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:28:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:39:01 GMT
ENV GOLANG_VERSION=1.17beta1
# Thu, 10 Jun 2021 21:39:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 10 Jun 2021 21:39:18 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:39:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:39:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:39:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2a179d76df60628ca372acea241dbf24d4039a86b7dc2ba920d26f64bded15a1`  
		Last Modified: Wed, 12 May 2021 00:49:13 GMT  
		Size: 46.1 MB (46098744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c213a4df67666087b0cfaa22f4d76fa708476c4f91ee848daccd8e1a9059682c`  
		Last Modified: Wed, 12 May 2021 01:21:01 GMT  
		Size: 11.3 MB (11336498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59de6391225c2ff4beecde954f63e31d511a479130b1acd174707008a47f717c`  
		Last Modified: Wed, 12 May 2021 01:20:59 GMT  
		Size: 4.6 MB (4564986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ee2df560b159f574ac071d2b70c54debf87201c8f108268b51b7b83f0cb410`  
		Last Modified: Wed, 12 May 2021 01:21:25 GMT  
		Size: 51.3 MB (51265871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58c622f93a90ae4341900f5fff1ea3fb9752f61cb1bcd4d9c0832b4afe3a2a3`  
		Last Modified: Wed, 12 May 2021 17:32:13 GMT  
		Size: 62.4 MB (62355469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60d8fcf3732df6bdc6496d2c7b39d2175f10851b0d794e62c49a1112bcde9fb`  
		Last Modified: Thu, 10 Jun 2021 22:15:30 GMT  
		Size: 105.5 MB (105526741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef17de9bfeca13204f590940bd911ead5733614bc0fad85dcb61096dae4c6f7d`  
		Last Modified: Thu, 10 Jun 2021 22:15:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
