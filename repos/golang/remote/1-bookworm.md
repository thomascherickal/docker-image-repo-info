## `golang:1-bookworm`

```console
$ docker pull golang@sha256:114b9cc39f435cfc34e2d48d0cb12cba2015a87f359f5dbf3ee3b6cf3591b7fb
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

### `golang:1-bookworm` - linux; amd64

```console
$ docker pull golang@sha256:2ae8b80bcf4937fbfc88c17b1c1177a99d347630af5c463a832d16100958dd57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (296990321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ac27c2c245ecf28861e52185d49533841550460cb8a571f1c2e7bc412410de0`
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
# Thu, 21 Sep 2023 03:28:49 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 21 Sep 2023 03:28:57 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.1.linux-mips64le.tar.gz'; 			sha256='3aa007a41f533b50eae2491bbd29926ada09357367a8aa05e7e50ec50c78acf9'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 21 Sep 2023 03:28:58 GMT
ENV GOPATH=/go
# Thu, 21 Sep 2023 03:28:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Sep 2023 03:28:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 21 Sep 2023 03:28:59 GMT
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
	-	`sha256:b0ed6cc9b50977796e8eb9b270ad9c62922003c0090aa3e5ec26a165cfcb9c02`  
		Last Modified: Thu, 21 Sep 2023 03:30:48 GMT  
		Size: 67.0 MB (66989274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd4529ba4b39e200f288cf7fd82159d3e157647d88356a488cfeea532bb284`  
		Last Modified: Thu, 21 Sep 2023 03:30:36 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bookworm` - linux; arm variant v5

```console
$ docker pull golang@sha256:653bee805527574cce36c9a476fd000f81dcc086fe59ed124e441e92198e2771
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.2 MB (271228868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9d7e38136a1f11828c0a3a26bae6bbb6c0f52c33d801f41182777d702bfcefc`
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
# Thu, 21 Sep 2023 00:15:22 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 21 Sep 2023 00:17:28 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.1.linux-mips64le.tar.gz'; 			sha256='3aa007a41f533b50eae2491bbd29926ada09357367a8aa05e7e50ec50c78acf9'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 21 Sep 2023 00:17:29 GMT
ENV GOPATH=/go
# Thu, 21 Sep 2023 00:17:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Sep 2023 00:17:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 21 Sep 2023 00:17:30 GMT
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
	-	`sha256:24b2d547b57a2f02f3ffd85722f612528547c35035b42ddcc9b68a63b925521f`  
		Last Modified: Thu, 21 Sep 2023 00:25:30 GMT  
		Size: 68.3 MB (68269984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71c013df6c24608d3ac432dabd94f6ec8b0c6df27cacd30c946f6dbd7e4d74d`  
		Last Modified: Thu, 21 Sep 2023 00:25:16 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bookworm` - linux; arm variant v7

```console
$ docker pull golang@sha256:545c18db0250cdbc70be3a19214eb9f942dfe3847e5d90303b15f74876284ab1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.3 MB (258329531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebdad0e32b46c3ae0efb8728e2899f08f68b1d9561cfacb8a73a3dbdccd977b0`
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
# Thu, 21 Sep 2023 05:40:19 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 21 Sep 2023 05:40:30 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.1.linux-mips64le.tar.gz'; 			sha256='3aa007a41f533b50eae2491bbd29926ada09357367a8aa05e7e50ec50c78acf9'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 21 Sep 2023 05:40:31 GMT
ENV GOPATH=/go
# Thu, 21 Sep 2023 05:40:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Sep 2023 05:40:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 21 Sep 2023 05:40:32 GMT
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
	-	`sha256:843ac29859021a1f6c2c7412168181379fcb4779d05022d4ca0b8880bc2e7873`  
		Last Modified: Thu, 21 Sep 2023 05:42:26 GMT  
		Size: 65.7 MB (65748660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec82b881b9d54bfe2f8cf90fdaa49fab0c64eb4fc46896d3bc8d6f6dd9a40549`  
		Last Modified: Thu, 21 Sep 2023 05:42:12 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:5b8d45bb27a2a83a3da96cda1e33d4d8b2fbd547888ead8bd7ef2a5e67d6cb1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.6 MB (287571026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:391000e01baea9d141ef853112cdf125415086eba5ee94c377d6b95d8b0fd602`
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
# Wed, 20 Sep 2023 22:19:55 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 20 Sep 2023 22:20:03 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.1.linux-mips64le.tar.gz'; 			sha256='3aa007a41f533b50eae2491bbd29926ada09357367a8aa05e7e50ec50c78acf9'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 20 Sep 2023 22:20:04 GMT
ENV GOPATH=/go
# Wed, 20 Sep 2023 22:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 22:20:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 20 Sep 2023 22:20:05 GMT
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
	-	`sha256:82e8ac953ea22bd1cc7b54bab2980bd3695cbd9b3767031df371d0cae0b200b5`  
		Last Modified: Wed, 20 Sep 2023 22:21:36 GMT  
		Size: 64.1 MB (64089241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ae7d75210d2e022f723016e144f6240357570c6b0539f7bc8bdff78774ea65`  
		Last Modified: Wed, 20 Sep 2023 22:21:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bookworm` - linux; 386

```console
$ docker pull golang@sha256:cc86a7b9edadbd36edbd993cd4f186e5e215c16e3b28fd1a7083805f00dc85f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296557650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5c1002c0680aa0401e5246116a990bee99fee1f4db7bc05a4c03a3775fa6c8e`
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
# Thu, 21 Sep 2023 08:41:54 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 21 Sep 2023 08:42:06 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.1.linux-mips64le.tar.gz'; 			sha256='3aa007a41f533b50eae2491bbd29926ada09357367a8aa05e7e50ec50c78acf9'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 21 Sep 2023 08:42:08 GMT
ENV GOPATH=/go
# Thu, 21 Sep 2023 08:42:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Sep 2023 08:42:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 21 Sep 2023 08:42:08 GMT
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
	-	`sha256:1efdc6435cd54f11f1f64273d427f5becc6d5e7a943d964f61aeca0850a9e4fc`  
		Last Modified: Thu, 21 Sep 2023 08:44:18 GMT  
		Size: 65.4 MB (65442611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4add66066f8f08396c48a7e9f14b3a7e462d59e67c60fc34adb715a5b5e4891`  
		Last Modified: Thu, 21 Sep 2023 08:43:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bookworm` - linux; mips64le

```console
$ docker pull golang@sha256:40dfc8cc4540046db7e11093522a65af79b173080a15b30ede7b9142a36da47a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.9 MB (267859009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:182788069f5664aa30d67bb35103ca98a5213195edeac8b7fe393950e55d4b85`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:08:33 GMT
ADD file:b12d5f9bfd6066e8e4df916aff636c5fc50b1cbd9011b061f050f9616c5a4700 in / 
# Thu, 07 Sep 2023 01:08:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:43:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:45:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 08 Sep 2023 15:47:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Sep 2023 15:47:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Sep 2023 15:47:31 GMT
ENV GOLANG_VERSION=1.21.1
# Fri, 08 Sep 2023 15:48:21 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.1.linux-mips64le.tar.gz'; 			sha256='3aa007a41f533b50eae2491bbd29926ada09357367a8aa05e7e50ec50c78acf9'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Fri, 08 Sep 2023 15:48:29 GMT
ENV GOPATH=/go
# Fri, 08 Sep 2023 15:48:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Sep 2023 15:48:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 08 Sep 2023 15:48:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5432e7fe6622506d41a4904c6c8f24ffc691cc53e107e3188eb4e22c6a42f952`  
		Last Modified: Thu, 07 Sep 2023 01:19:30 GMT  
		Size: 49.5 MB (49542026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b895bf089727243ca906ccf5751e80977f9fde47782ad42ea0d1f280ea17d8`  
		Last Modified: Thu, 07 Sep 2023 04:19:54 GMT  
		Size: 23.6 MB (23612690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3231d7a773fc731df8f91925b53693b6f8793d340f9b469b5d8fac4ce40f9ac`  
		Last Modified: Thu, 07 Sep 2023 04:20:48 GMT  
		Size: 63.0 MB (62950915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e94def153d26085585fcc3fef80ab28bf21fd20341f644edb744c8c791397d`  
		Last Modified: Fri, 08 Sep 2023 16:18:52 GMT  
		Size: 69.6 MB (69624242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07458f52411c20d66a273018ba9dc51b078990bc835e8822e8a4dbea92c56aa`  
		Last Modified: Fri, 08 Sep 2023 16:18:58 GMT  
		Size: 62.1 MB (62129012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2cabc0b2306bebe59e376cf4cdb43c655e1dfe6ad8089252d39e65433b88e6`  
		Last Modified: Fri, 08 Sep 2023 16:18:05 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bookworm` - linux; ppc64le

```console
$ docker pull golang@sha256:46c5272e124fa207a29bc279d496640caa25fc14218f505a8f885d8347a6e4c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.2 MB (303191054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b4b02691007b5a432c28c1860c33ddd6f3289dd1fb0009d397706513859c28a`
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
# Thu, 21 Sep 2023 07:30:06 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 21 Sep 2023 07:31:18 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.1.linux-mips64le.tar.gz'; 			sha256='3aa007a41f533b50eae2491bbd29926ada09357367a8aa05e7e50ec50c78acf9'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 21 Sep 2023 07:31:22 GMT
ENV GOPATH=/go
# Thu, 21 Sep 2023 07:31:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Sep 2023 07:31:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 21 Sep 2023 07:31:23 GMT
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
	-	`sha256:f76e75d32632712e31647ab6492d64eb9d46abcfa384bf6b647fb5f01cafc43d`  
		Last Modified: Thu, 21 Sep 2023 07:34:18 GMT  
		Size: 64.1 MB (64111263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddfc156ff13fe3133054564962367e05852d58cccf8def2732c23b776d968f2`  
		Last Modified: Thu, 21 Sep 2023 07:33:59 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bookworm` - linux; s390x

```console
$ docker pull golang@sha256:258fe81e46e186b58f79abf7cb6720c89972232287c9e0373d6b4e0ed1077144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.1 MB (270137601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e0327895ea11b175b648d2ff352fe4ccba2c30367cf214ac298882a4a83e063`
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
# Wed, 20 Sep 2023 17:54:01 GMT
ENV GOPATH=/go
# Wed, 20 Sep 2023 17:54:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 17:54:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 20 Sep 2023 17:54:01 GMT
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
	-	`sha256:0a988f8013f03a614c7755a22d11c9e767b46935526e5d75c51e2e86e062b828`  
		Last Modified: Wed, 20 Sep 2023 17:56:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
