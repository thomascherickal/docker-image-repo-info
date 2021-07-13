## `golang:1-stretch`

```console
$ docker pull golang@sha256:f5a98edf4e233fb0b6f69fa85f322fe558e385731952a6cebb0a25939ed61d7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:1-stretch` - linux; amd64

```console
$ docker pull golang@sha256:32775517ca9a60baf836716662a52560242597b6440cf10cfbc3d4578524ca9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297676347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aaa19e09590ea120e0e7b37a7ea16c39ac02ced89088ae92891aafe554e1c26`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:56:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 00:29:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 00:29:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:42:07 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 00:42:21 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 13 Jul 2021 00:42:22 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 00:42:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:42:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 00:42:24 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6154ac87d7f3d5133865f50f67a37cc0687318bb4f422ba4f2d65057e9c266fd`  
		Last Modified: Wed, 23 Jun 2021 01:04:53 GMT  
		Size: 49.8 MB (49761580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0641dfa685bcc52e5444aa58819feb552705d7eda96704b89d29325443bb4943`  
		Last Modified: Thu, 24 Jun 2021 00:34:47 GMT  
		Size: 57.8 MB (57846790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8d02371c0ff571b5b170f782a8ca41b9aac1c61414b76920379bc2fcfbb1d1`  
		Last Modified: Tue, 13 Jul 2021 00:56:57 GMT  
		Size: 129.1 MB (129050875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bb5f8c7fc38e72654285bed94a4ac8ae5fe847b638a7417f566e6cde32ee41`  
		Last Modified: Tue, 13 Jul 2021 00:56:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:f92eca948c3e397999d65c06407af73fc974ccbb393ea97aa6d100f697572688
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.6 MB (248577700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97945139b1236bbc3046052e97b1a96c3bc7a1abce914af3a846589d3825eaaf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:06 GMT
ADD file:8c289b4c3c40ee076e3b3563f38ccd72dee8b2ee3122170cf1bdd417ae9e03c0 in / 
# Wed, 23 Jun 2021 00:23:08 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:53:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 17:37:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 17:37:09 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:03:59 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 06:04:26 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 13 Jul 2021 06:04:27 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 06:04:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:04:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 06:04:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d2f34e8839b40d84b70d62e2c8a6909422dad9688919bf387ad4a092d38ab62f`  
		Last Modified: Wed, 23 Jun 2021 00:36:08 GMT  
		Size: 42.1 MB (42119988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327954c584e8a66a22440b9a731a29ecccc047aa5f3477d6191e1c7167a37503`  
		Last Modified: Wed, 23 Jun 2021 06:24:47 GMT  
		Size: 10.0 MB (9950929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7274a619e45e9e714e599f6ae62b529f504ec947a07a58908ad99c464907420`  
		Last Modified: Wed, 23 Jun 2021 06:24:44 GMT  
		Size: 3.9 MB (3921297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9912efc947692ebde57dca8997537ddf30def320f8ba3667b58994d42617114`  
		Last Modified: Wed, 23 Jun 2021 06:25:35 GMT  
		Size: 46.1 MB (46125750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0295fb82aaa7b9c871b876986d1bdf5460f8ab71a6d812bad588e17cce1b4f`  
		Last Modified: Thu, 24 Jun 2021 17:57:38 GMT  
		Size: 46.2 MB (46178266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e30d0c2a15bb9f1388e814960c4e4d61235a51242751c673e53d4c37aa0125`  
		Last Modified: Tue, 13 Jul 2021 06:29:35 GMT  
		Size: 100.3 MB (100281314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa157c5d6d5aa93e946c283fa9e4137b60e53a97d71889c58fb666b7435ab983`  
		Last Modified: Tue, 13 Jul 2021 06:28:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:55a996b066eb99f5a52752a3cfc112de3f7c8f6a4f938a212b10626a4743143d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.1 MB (254084970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:039b52eb51d1fa7707c1dbbbec48d7ec3e91fb9125931eef64a7caf87a60fbf8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:55 GMT
ADD file:02285d0bd3ea996a7ebbe069a83e508701cbaf14f53fdeaa123775acd7e0537f in / 
# Tue, 22 Jun 2021 23:50:56 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:27:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:53:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:53:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:41:32 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:41:42 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 13 Jul 2021 01:41:43 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:41:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:41:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:41:44 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0789e4a342a11c7c57a241829a41af53fbd194e6dede60c6d6f63d69e403b2cd`  
		Last Modified: Tue, 22 Jun 2021 23:57:52 GMT  
		Size: 43.2 MB (43177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd2ed69368e8a7d296f1c91060e897753bed4a79ab68ed47c544e1f4d6fadcd`  
		Last Modified: Wed, 23 Jun 2021 00:35:58 GMT  
		Size: 10.2 MB (10214577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c76e514669ff971481e0d19dc0581f90d72eab2d0e117a5761ae016e14f213`  
		Last Modified: Wed, 23 Jun 2021 00:35:57 GMT  
		Size: 4.1 MB (4096534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa19114dc4cc7157e619bb778418a2fadbc86acafe444fd2066e1412d2a7fb8`  
		Last Modified: Wed, 23 Jun 2021 00:36:18 GMT  
		Size: 47.7 MB (47732823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587bc22d217c19df4528c956b00cdcf815df2701e8ede693376ccf8ba1fe466a`  
		Last Modified: Wed, 23 Jun 2021 12:59:26 GMT  
		Size: 49.2 MB (49237288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5d31b589e7cc3f449439da9c40481a4d0d2a7fad7a9ff366d461e3e622a890`  
		Last Modified: Tue, 13 Jul 2021 01:53:52 GMT  
		Size: 99.6 MB (99626171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc5dc960eb959d5640a51815a09d8aaa5faf73d091a8813335e92d519047629`  
		Last Modified: Tue, 13 Jul 2021 01:53:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; 386

```console
$ docker pull golang@sha256:f8ce9b2883e8c955cfbfd9e6670322c0fe2aa22d158abef991cdb0d6a0386157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.7 MB (278749696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a29ac66a38d6d2e6cdaf08ed511b88f3cf112b3365a7a4988ac1d2c160deab86`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:41:10 GMT
ADD file:80feef1b55f2f1e39986ac669152a7a209e2fa5a097a8dfa16ca7e1118159830 in / 
# Tue, 22 Jun 2021 23:41:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:12:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:12:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:13:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:16:05 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:16:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 13 Jul 2021 01:16:19 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:16:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:16:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:16:21 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3497549dbcdd02a0f25068f37e6950ad5b608b1791d0c79236abdfe13b8e3f02`  
		Last Modified: Tue, 22 Jun 2021 23:49:21 GMT  
		Size: 46.1 MB (46096990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908bab0e9cd5e81a3e8bb8d6a886f1f7d5058bed177f7d72aaa41cbc1be07c78`  
		Last Modified: Wed, 23 Jun 2021 00:21:09 GMT  
		Size: 11.4 MB (11352293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d81c9417ef64635e730e26eed1f82f02fa869f476770ef658a95fddfc192319`  
		Last Modified: Wed, 23 Jun 2021 00:21:07 GMT  
		Size: 4.6 MB (4564980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec9dd8c9a561c924b995bbee8e6986503521fd6ce2ce66ce18c154371379e11`  
		Last Modified: Wed, 23 Jun 2021 00:21:34 GMT  
		Size: 51.3 MB (51265677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ddf2e60d5bb49788a3f3ded7c2c09b5a75dcb25c1a80ce967efc736d79bdcb`  
		Last Modified: Wed, 23 Jun 2021 17:15:54 GMT  
		Size: 62.4 MB (62371452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be93a4bd59fb4a4449c098e4e2f69f062b96229d4b295231594999875bb74552`  
		Last Modified: Tue, 13 Jul 2021 01:35:53 GMT  
		Size: 103.1 MB (103098149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990122c98a490e7dbca2546abb7ca26db4b1ccdcebc2fd35d259bbd5ced83d49`  
		Last Modified: Tue, 13 Jul 2021 01:35:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
