## `golang:latest`

```console
$ docker pull golang@sha256:3049cdf48ea2d2a0d9bb4621c0b22245c0e471fde2975416b58f4462c3b3de3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 10
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.20348.1970; amd64
	-	windows version 10.0.17763.4851; amd64

### `golang:latest` - linux; amd64

```console
$ docker pull golang@sha256:e63f8cf91f5b59ce217f2804936132b2964b04bb5b06c0a79b9e37990a6ab148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (296994950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6285f5529f1ba8755fd2469d255fa9e0429d5fa8c6003d52da5ea09838aea548`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:26 GMT
ADD file:ce04d6a354feaef93795269c859f36667fce9efda23c61b37d7060263b66ed4e in / 
# Wed, 20 Sep 2023 04:55:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:20:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:21:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:28:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:28:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:19:54 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:20:03 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.2.linux-mips64le.tar.gz'; 			sha256='9b7e03ae43bd55bbbecd0a4c8928961488eb1ba404324ce80b606efc5f486a77'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 05 Oct 2023 21:20:04 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:20:04 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:20:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:20:05 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:167b8a53ca4504bc6aa3182e336fa96f4ef76875d158c1933d3e2fa19c57e0c3`  
		Last Modified: Wed, 20 Sep 2023 04:59:55 GMT  
		Size: 49.6 MB (49557601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47a222d28fa95680198398973d0a29b82a968f03e7ef361cc8ded562e4d84a3`  
		Last Modified: Wed, 20 Sep 2023 09:29:57 GMT  
		Size: 24.0 MB (24030522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debce5f9f3a9709885f7f2ad3cf41f036a3b57b406b27ba3a883928315787042`  
		Last Modified: Wed, 20 Sep 2023 09:30:18 GMT  
		Size: 64.1 MB (64112257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b457aaf04f424db4f223ea7aad4b196d4a62da58d6f45938233e0f54bd162c`  
		Last Modified: Thu, 21 Sep 2023 03:30:49 GMT  
		Size: 92.3 MB (92300511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab90286b1543edaec4dd9402a487a164307c216d646369c8e59248fb92da4767`  
		Last Modified: Thu, 05 Oct 2023 21:25:32 GMT  
		Size: 67.0 MB (66993903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcec06b980f5d54c94a469aeb286627475f645205140fb3ed0514e32cebede2`  
		Last Modified: Thu, 05 Oct 2023 21:25:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v5

```console
$ docker pull golang@sha256:6a4ebdc53138118f67b4a36690b10508b590379e1e5a2f894162dc8494fc042e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.2 MB (271237478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ef00a799c72ef69a0f31d92a39d795e6119be98f2adfdbba97b6b2813444b31`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:41 GMT
ADD file:4c262e2fcc04b6144cc529b2b0dbd984b5f44ecf09bd87707631cb5cad3012f0 in / 
# Wed, 20 Sep 2023 00:49:42 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:54:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:55:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 00:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 00:15:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:48:16 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:50:28 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.2.linux-mips64le.tar.gz'; 			sha256='9b7e03ae43bd55bbbecd0a4c8928961488eb1ba404324ce80b606efc5f486a77'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 05 Oct 2023 21:50:31 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:50:31 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:50:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:50:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:50:32 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c2e728ebba2eb6503d5975d2d8245f959ffad36ab8a83164e1c7e45956c36080`  
		Last Modified: Wed, 20 Sep 2023 00:54:16 GMT  
		Size: 47.4 MB (47415014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19620991f32e48616e52febc5b55b219fc0e07a38ce2edc871e4e75601582812`  
		Last Modified: Wed, 20 Sep 2023 10:04:59 GMT  
		Size: 22.7 MB (22709714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a754c9ac0c66ea612dd3e7313134a3f8bbc17850295990e81eb1848b34eabf4`  
		Last Modified: Wed, 20 Sep 2023 10:05:22 GMT  
		Size: 61.6 MB (61554233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ed0c8ce21012cf47c922e84bc09759ceef7f27c83430797575015e3fe79894`  
		Last Modified: Thu, 21 Sep 2023 00:25:27 GMT  
		Size: 71.3 MB (71279766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b259003110d7acae61bf1b03358b65445eacae46454944f07ee8fdb315a2622`  
		Last Modified: Thu, 05 Oct 2023 21:58:03 GMT  
		Size: 68.3 MB (68278595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518f1438dc340deb182b292b67e4de4fd8dfa4a59904c57852cd27b661c41ab`  
		Last Modified: Thu, 05 Oct 2023 21:57:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v7

```console
$ docker pull golang@sha256:e8e1464f60c1b7eeb912966b15cee00eb3c093490526d8845f337c57a1558b95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.3 MB (258337842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61602eb26c6bb488fe14299710ced67f2b3545f6ae2cc3f7ba6c575948879762`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:08 GMT
ADD file:e8c98b19a39772b96a8bfa0f38abfc620498f040012f9b9906640975ac01ce0d in / 
# Wed, 20 Sep 2023 04:57:09 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:24:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:24:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 05:40:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 05:40:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:02:35 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 22:02:46 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.2.linux-mips64le.tar.gz'; 			sha256='9b7e03ae43bd55bbbecd0a4c8928961488eb1ba404324ce80b606efc5f486a77'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 05 Oct 2023 22:02:47 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 22:02:47 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 22:02:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:02:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 22:02:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:013e3017888216ce95d0ffe3d0fb039c509402dc99800465157f56e7520abd4a`  
		Last Modified: Wed, 20 Sep 2023 05:00:53 GMT  
		Size: 45.2 MB (45232576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b45aaa3d8d542a2281410c108a016f367f050793bb029d35cca677cc0d500f1`  
		Last Modified: Wed, 20 Sep 2023 15:35:12 GMT  
		Size: 21.9 MB (21936768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecb66b8eee4d1eb823c09a41799c3f25f6ef9f31c3ef273c3b37419d8c39606`  
		Last Modified: Wed, 20 Sep 2023 15:35:36 GMT  
		Size: 59.3 MB (59262478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac4e9eaf20db5c51937cb9caa0088ad77a7e31803d12d467f8baea23e670539`  
		Last Modified: Thu, 21 Sep 2023 05:42:21 GMT  
		Size: 66.1 MB (66148892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac45c6c3cc1ae8e7dc5a4420f0898748cc3dcadd46e622da61fe872f2079b29`  
		Last Modified: Thu, 05 Oct 2023 22:08:45 GMT  
		Size: 65.8 MB (65756972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20883fb641b822fff55b6c2fc00bd148aa68928d8d7771ec2dec10de9edb50c9`  
		Last Modified: Thu, 05 Oct 2023 22:08:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:013ebb36af72d90db0175b077ffa6469ecccfe10ba2a2389cbbc4c1010a83b96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.6 MB (287578611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a89fc427b1e667e4af990d2dad9293774963c8a5728960d85a0a5cf5f23501`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:04 GMT
ADD file:7a0adbde6e967e2bcaafa69f04fabdec993025645c8d0d51acc991a31b404eed in / 
# Wed, 20 Sep 2023 02:44:05 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:23:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:23:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:19:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:19:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:39:31 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:39:38 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.2.linux-mips64le.tar.gz'; 			sha256='9b7e03ae43bd55bbbecd0a4c8928961488eb1ba404324ce80b606efc5f486a77'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 05 Oct 2023 21:39:40 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:39:40 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:39:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:39:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:39:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:796cc43785ac3cd0081892bd48e545a0615415265b60c794fdf81ac95b034213`  
		Last Modified: Wed, 20 Sep 2023 02:47:15 GMT  
		Size: 49.6 MB (49591881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91290b4a059080b4227746016e1a8f32a290271d8712b213834e9296a38bfea9`  
		Last Modified: Wed, 20 Sep 2023 09:32:11 GMT  
		Size: 23.6 MB (23570121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8d278f2f731ceff5e8c6f5010bef6b1bf18c555a80663ca612e3e42d013779`  
		Last Modified: Wed, 20 Sep 2023 09:32:29 GMT  
		Size: 64.0 MB (63988033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bd3fde148c3ad9659f4843f0b27408919e0c24b954ff14165c0edb811e2c72`  
		Last Modified: Wed, 20 Sep 2023 22:21:36 GMT  
		Size: 86.3 MB (86331594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207a4a626d340a9ded5da454b9f353db8ea64106b91ccc73f4a332df11d1ba6d`  
		Last Modified: Thu, 05 Oct 2023 21:44:08 GMT  
		Size: 64.1 MB (64096827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f88b0dac11c75b9909a031ea4e9b1ec6afd2f70caae9fb8c2c43154780164a3`  
		Last Modified: Thu, 05 Oct 2023 21:44:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; 386

```console
$ docker pull golang@sha256:cba2b286a758ce023de8b5280ffbd67dbdfaca0fd30c66d98bc25f10e7ad7d1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296558178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f98d9f4135ba33b947401f272fb1a91534927c4110044ac8ed14abe6a04672f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:41:42 GMT
ADD file:23c52eb6ca90f95eb3fff17deef5cfb900f1807fd50deae367183075f49aa81d in / 
# Wed, 20 Sep 2023 00:41:45 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:25:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 08:41:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 08:41:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:38:23 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:38:37 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.2.linux-mips64le.tar.gz'; 			sha256='9b7e03ae43bd55bbbecd0a4c8928961488eb1ba404324ce80b606efc5f486a77'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 05 Oct 2023 21:38:39 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:38:39 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:38:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:38:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:38:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b3de420baafed4c606a756da9f1ab4e930a007eb8cb0a1104bc280c0b7820cbf`  
		Last Modified: Wed, 20 Sep 2023 00:46:20 GMT  
		Size: 50.6 MB (50568965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4c8b4e1e9e09c6062a8931a468a599c126b11dde5f26fc56c31c3de3f4cf68`  
		Last Modified: Wed, 20 Sep 2023 11:36:56 GMT  
		Size: 24.9 MB (24869713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd965fff65d218c5dd30176fa6be9fe57accd5e588e2173f509ea58bf7d44ab8`  
		Last Modified: Wed, 20 Sep 2023 11:37:22 GMT  
		Size: 66.0 MB (65972489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe1a98aa621dac0c0a2816b958ba064727ca06b16f200cab0d764976693bbfe`  
		Last Modified: Thu, 21 Sep 2023 08:44:21 GMT  
		Size: 89.7 MB (89703716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfeaa1eeeb776b7093a109233b4a8f6f3f876cb3440813d4a61d596a9ef7a08`  
		Last Modified: Thu, 05 Oct 2023 21:47:27 GMT  
		Size: 65.4 MB (65443139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24b35e6783c67d1ea9a7a6bda79d4e679b56c8d76e15d892c6349ce6882ca49`  
		Last Modified: Thu, 05 Oct 2023 21:47:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; mips64le

```console
$ docker pull golang@sha256:54fafabdd0171283a17b6d88460eec45b4c6f09c8e1320fdd05a2265c7be0fe0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.9 MB (267894134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b01d990a2df68b832ac1d0320dd470532c8b12ecf19a08ebeab9fcad176bdc4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 03:09:14 GMT
ADD file:fcce6589274e33563988a8b5cf9be10cd70df7b83bdf6713a5162f272a6c801f in / 
# Wed, 20 Sep 2023 03:09:19 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 21:45:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 21:47:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Sep 2023 04:43:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Sep 2023 04:43:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:07:36 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 22:08:24 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.2.linux-mips64le.tar.gz'; 			sha256='9b7e03ae43bd55bbbecd0a4c8928961488eb1ba404324ce80b606efc5f486a77'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 05 Oct 2023 22:08:32 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 22:08:39 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 22:08:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:08:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 22:09:01 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d60e76f86e60c0c2ec7b83df437d97bc329aab62315d63446e73d0ccc6bed0b5`  
		Last Modified: Wed, 20 Sep 2023 03:20:16 GMT  
		Size: 49.5 MB (49542389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcc2e2248e2cc36baf3ee5daf0facc6ebb4ffbfeacea598d0236469d9f6573b`  
		Last Modified: Wed, 20 Sep 2023 22:20:35 GMT  
		Size: 23.6 MB (23612726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270da23f34a3d46cf64368c2f1574be74de69879d2f3d04ce465cae23dee66f7`  
		Last Modified: Wed, 20 Sep 2023 22:21:28 GMT  
		Size: 63.0 MB (62950631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d373fd66bd4c02c145c832d57a1a6c692c958b3e4278608b83f83e4fdac6724`  
		Last Modified: Fri, 22 Sep 2023 05:14:51 GMT  
		Size: 69.7 MB (69657359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb5a38e0e3fbc9241c8e4552a34fe7072d274065fb7ff678148448d308f1cae`  
		Last Modified: Thu, 05 Oct 2023 22:37:30 GMT  
		Size: 62.1 MB (62130905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cee7681c735e4318a81b0f6106aa60d94fcd043bdd9ef77cdc292f8925029b`  
		Last Modified: Thu, 05 Oct 2023 22:36:43 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; ppc64le

```console
$ docker pull golang@sha256:833e2e51ced9d631edc86d8bc4487ec28cd4f4962a7bb2d797dd3eb0f509a48b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.2 MB (303195329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f763b1b30911ab0bae017b3924bb18766a05533cc79032ad27616af1fb9ad577`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:31 GMT
ADD file:dc6a80175c6d467f50c4ff816701171cd27bd98fc9bb7292161e476ada0cfed1 in / 
# Wed, 20 Sep 2023 07:52:34 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 07:30:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 07:30:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:17:03 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:17:34 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.2.linux-mips64le.tar.gz'; 			sha256='9b7e03ae43bd55bbbecd0a4c8928961488eb1ba404324ce80b606efc5f486a77'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 05 Oct 2023 21:17:39 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:17:39 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:17:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:17:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:17:42 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:dacd41a2ee8a7a272473dd20943e3e5c0ddac0964f5610239dd5ae6c807c000c`  
		Last Modified: Wed, 20 Sep 2023 08:49:21 GMT  
		Size: 53.5 MB (53544796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ec766d4028b01ee907aa2c7c4460d2a3a7b6046a77e25177450d4c40b848a9`  
		Last Modified: Wed, 20 Sep 2023 10:20:30 GMT  
		Size: 25.7 MB (25680962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a962ae127ab04dc4b0c1dc7a9f6ce9d0f64cb5981c0e114caaec07fd9c8c5e`  
		Last Modified: Wed, 20 Sep 2023 10:20:59 GMT  
		Size: 69.6 MB (69570258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975e986e3e2f60555f542951ba79f9315607751e1f8121f632ab75691c4ecf83`  
		Last Modified: Thu, 21 Sep 2023 07:34:21 GMT  
		Size: 90.3 MB (90283618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e63506bc5204d0a5c340ad9b61ce5c992a5f3e6f9a9bcd0ed902d6542ce0f0`  
		Last Modified: Thu, 05 Oct 2023 21:29:25 GMT  
		Size: 64.1 MB (64115540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21054dcb97b824f4206bd5cac48faad8902d302eb696681d12363677dad9e21e`  
		Last Modified: Thu, 05 Oct 2023 21:29:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; s390x

```console
$ docker pull golang@sha256:1e115e02a0126302de1c9d5a137e9182fb8636bf36e453f83551581a9ce32952
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.1 MB (270137600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ddad6b414074c3f5ed9ac4f66d6dd69ca4747c80fdf5c160e5b9d86d67a55c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:09 GMT
ADD file:988f82e85974ad63522cfbd8ca56dddd8dd9825ed628600e9a5037d77d1bd890 in / 
# Wed, 20 Sep 2023 02:54:12 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:49:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:49:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:53:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 17:53:42 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 20 Sep 2023 17:53:55 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.1.linux-mips64le.tar.gz'; 			sha256='3aa007a41f533b50eae2491bbd29926ada09357367a8aa05e7e50ec50c78acf9'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 27 Sep 2023 00:44:57 GMT
ENV GOTOOLCHAIN=local
# Wed, 27 Sep 2023 00:44:57 GMT
ENV GOPATH=/go
# Wed, 27 Sep 2023 00:44:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Sep 2023 00:44:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 27 Sep 2023 00:44:59 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ca5551f4914a3e8f0c34772f4d772442cbf259e6ee48db35d827776924e556bf`  
		Last Modified: Wed, 20 Sep 2023 02:59:30 GMT  
		Size: 47.9 MB (47921769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d1899ef7b4679dca64e2b81a7d1bc3c4b48e9813dc2fa8cae7a5106d1ce073`  
		Last Modified: Wed, 20 Sep 2023 09:58:27 GMT  
		Size: 24.0 MB (24028736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b068b7dafac8638b610a6cb2e2a91a3aa7ca68a443fa93992af5f0fe704f55a`  
		Last Modified: Wed, 20 Sep 2023 09:58:48 GMT  
		Size: 63.1 MB (63113324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d5b5bc595db7cf7c489ea22ae8705ae5650d03252cc774bf59e53ef4f7d2bd`  
		Last Modified: Wed, 20 Sep 2023 17:56:55 GMT  
		Size: 68.9 MB (68870246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b2e774f51ce625f46ead9707285996576cde314c52392b9e84bbedb599bce`  
		Last Modified: Wed, 20 Sep 2023 17:56:56 GMT  
		Size: 66.2 MB (66203370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bb307c127dd15d66f22505d2ea99f29f5ba27452ec3a90b63a4e14ebd47521`  
		Last Modified: Wed, 27 Sep 2023 00:46:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.20348.1970; amd64

```console
$ docker pull golang@sha256:1cd9f2f77f9b09098c36343b1932f512f26c8c506c55f4773701b73605df2124
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1932440194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e080fdef39b18484bdd95724cb782c85afda97e56d69751260c57da484209ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:35:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:35:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:35:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:35:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:36:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:36:16 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:36:38 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 05 Oct 2023 21:14:54 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:16:51 GMT
RUN $url = 'https://dl.google.com/go/go1.21.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2cd46db02477f33559a4ebf8a176c22879b43fdcfddb1542a23876054f26a83f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 05 Oct 2023 21:16:52 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a846e03791bc3a58cfed3f02e65f87e18a5f5f416405456368e8a0ec4f9364`  
		Last Modified: Wed, 13 Sep 2023 02:15:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc2015fc36cda903dca8edfdc1c87b219753af24c4ff5a95db324fb0e1cc0c`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1910b6e6c60b5b71a12c43af94e08cf0ba20718d9a6c16ad07734f4977311`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46353fb4c6176aee49921617b1cd3ac7dcbca49d4d7a734cb5ddef177b8354b2`  
		Last Modified: Wed, 13 Sep 2023 02:15:20 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f70d11added5b27b9707831ac76b04e95d4fa92b406f09532472fa350df630`  
		Last Modified: Wed, 13 Sep 2023 02:15:25 GMT  
		Size: 25.6 MB (25551011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892bff3fc5428691c1922057d675611c2b50e50cf3c6d22c2054b270861bc53c`  
		Last Modified: Wed, 13 Sep 2023 02:15:17 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ee07c029ab53a292bbb7320390d24d86b21159530b1b77d968b2b5416e8f67`  
		Last Modified: Wed, 13 Sep 2023 02:15:18 GMT  
		Size: 277.5 KB (277484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4d621af92887896386a876f8789ba88e1775bdaec7b6c0e379b2be5b984f5a`  
		Last Modified: Thu, 05 Oct 2023 21:34:23 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c735a32d40b515348db5b026968d1323ec6df5586bced97fe2f1d529a2ed6dc6`  
		Last Modified: Thu, 05 Oct 2023 21:34:40 GMT  
		Size: 69.3 MB (69326685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae63a289eb9500bb81e265921deb90189c8844fe68e1099de64230f575e5b2c2`  
		Last Modified: Thu, 05 Oct 2023 21:34:23 GMT  
		Size: 1.5 KB (1535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.17763.4851; amd64

```console
$ docker pull golang@sha256:278a095f7d525d8e3364d9cdcc5a0a5d603f4f2ca361f3069661453bfee8f6c3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2111475208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88991f923167af7330f709a4ef1f078962f0d7a3d6995239db0cbe2b196c9f8c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 01:39:14 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Sep 2023 01:39:15 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Sep 2023 01:39:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Sep 2023 01:40:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 01:40:50 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:41:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 05 Oct 2023 21:17:07 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:19:45 GMT
RUN $url = 'https://dl.google.com/go/go1.21.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2cd46db02477f33559a4ebf8a176c22879b43fdcfddb1542a23876054f26a83f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 05 Oct 2023 21:19:46 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdfacf538899a08fcbb1c6b92df02725dbfcc05c593d6f310371baf9cc5c28b`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa9f7bc4f06074cd41e4c8f38f9019d00b30116cc81e7e57bb201a2cddbe76`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa369f25c61f03e75b9090231c21b059562345a9aa5b4710c1d4bd043232a46`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1338c790efe798520cb633291aa3dbf3b37552cfbd91737d2539bad7bcac882c`  
		Last Modified: Wed, 13 Sep 2023 02:16:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af230316f5f5bdfd37af05e436ffaadf28ac7a31d97f315dbfb2924c4d1ca3c`  
		Last Modified: Wed, 13 Sep 2023 02:16:54 GMT  
		Size: 25.6 MB (25567707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606d89c5df48922aee4ed7b88afc9f9fc270b462891c28d20b75199f2726201e`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f90ec51ca481c33d4e3887adf74f8b37c2f82af9e60290d2755f34c55b70e9c`  
		Last Modified: Wed, 13 Sep 2023 02:16:46 GMT  
		Size: 220.5 KB (220461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994a4ab81cb0f8c53c8efd244a7cc436a374a06734ef049bce28de32188a2a8e`  
		Last Modified: Thu, 05 Oct 2023 21:34:54 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d12633d4fa4f7a275ac52083283b6b48414f25b3cd2000e2be75a2d35413f3`  
		Last Modified: Thu, 05 Oct 2023 21:35:10 GMT  
		Size: 69.3 MB (69345652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cafecdd9c7a4af7f37d5646f597539b5c560428abe7bab151f7394cc274085`  
		Last Modified: Thu, 05 Oct 2023 21:34:54 GMT  
		Size: 1.5 KB (1541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
