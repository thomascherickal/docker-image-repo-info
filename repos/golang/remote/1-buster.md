## `golang:1-buster`

```console
$ docker pull golang@sha256:267cd0d6449f47031b4a6b386e5652ee572ced4ee7e2ec846352b0132bf0d3e5
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

### `golang:1-buster` - linux; amd64

```console
$ docker pull golang@sha256:645084f761154b6f9509f4f558993baceece127d9143371c3e6986cd0f777b59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.8 MB (323791648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a154fd32f606d9cdf136acb3cda97619f5ded7782b59a717f63c24bc0d3382`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:41 GMT
ADD file:e8b516b464e535b435a6ed8609bac98acc90ee30e2a0667f68932f0d924f6e49 in / 
# Tue, 01 Mar 2022 02:13:42 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:27:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:28:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 06:28:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 17:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 17:53:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 01:03:36 GMT
ENV GOLANG_VERSION=1.17.8
# Fri, 04 Mar 2022 01:04:34 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.8.linux-amd64.tar.gz'; 			sha256='980e65a863377e69fd9b67df9d8395fd8e93858e7a24c9f55803421e453f4f99'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.8.linux-armv6l.tar.gz'; 			sha256='3287ca2fe6819fa87af95182d5942bf4fa565aff8f145812c6c70c0466ce25ae'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.8.linux-arm64.tar.gz'; 			sha256='57a9171682e297df1a5bd287be056ed0280195ad079af90af16dcad4f64710cb'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.8.linux-386.tar.gz'; 			sha256='a826cd599828aeefc86d742e1a8ce8ab7e0251b2429568ad5633e21c8a769053'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.8.linux-ppc64le.tar.gz'; 			sha256='2077dd2fc57a74b0630b0c239ae4e3114607311778effd43fcfe5174133ee188'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.8.linux-s390x.tar.gz'; 			sha256='3fac23801644a2f93a1643acecd5a94a5ea05d88e19467092fb6e64205710f61'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 04 Mar 2022 01:04:35 GMT
ENV GOPATH=/go
# Fri, 04 Mar 2022 01:04:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 01:04:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Mar 2022 01:04:36 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:1c9a8b42b5780ac49c71f392c9512c0167ecc23de9b30b1b5f38747b73097d1a`  
		Last Modified: Tue, 01 Mar 2022 02:19:43 GMT  
		Size: 50.4 MB (50437046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163066942b43a00ba7f4674c4c1ca90eccc8d99366a3dc47cb64e06ad79c36e5`  
		Last Modified: Tue, 01 Mar 2022 06:37:36 GMT  
		Size: 7.8 MB (7834052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf70e03a8272d87e65c7b1592f97f6e739cf1f5d13cc536670f41c28b086b4cb`  
		Last Modified: Tue, 01 Mar 2022 06:37:37 GMT  
		Size: 10.0 MB (9997298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c5ff33549498a7154441116b5843e184c1f4441df2eab519ad2c498cb8a716`  
		Last Modified: Tue, 01 Mar 2022 06:37:56 GMT  
		Size: 51.8 MB (51843267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398bdb7b0a5ae8eb0b39b1c5624619d48f54dda97ee695a49b721773626fa1da`  
		Last Modified: Wed, 02 Mar 2022 18:06:51 GMT  
		Size: 68.8 MB (68776617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2239c4fc855a17007b941f50392a4b0ab8693c47a488d84123e762460166ae4`  
		Last Modified: Fri, 04 Mar 2022 01:20:25 GMT  
		Size: 134.9 MB (134903212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b6dc998a91f7ae5c9d96e3b916fdcdd67863da0fc617a174fb93d696a38f1`  
		Last Modified: Fri, 04 Mar 2022 01:20:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:5e4a826ebe2cb990617cce0e03410d15e7bca86c6f77465fe9f7ef7202fa3822
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.3 MB (272346009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce2e2f8df3678efcdb29a5a3852f060063d1a910995a1ca6535251b57193fa55`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:21 GMT
ADD file:67f3f7e89901c5f16436fda6f05f959b01ce2654ab6b4cd9d53b597d1a30a97d in / 
# Tue, 01 Mar 2022 02:03:23 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:06:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 03:07:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:45:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:45:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 22:53:39 GMT
ENV GOLANG_VERSION=1.17.8
# Thu, 03 Mar 2022 22:57:39 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.8.linux-amd64.tar.gz'; 			sha256='980e65a863377e69fd9b67df9d8395fd8e93858e7a24c9f55803421e453f4f99'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.8.linux-armv6l.tar.gz'; 			sha256='3287ca2fe6819fa87af95182d5942bf4fa565aff8f145812c6c70c0466ce25ae'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.8.linux-arm64.tar.gz'; 			sha256='57a9171682e297df1a5bd287be056ed0280195ad079af90af16dcad4f64710cb'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.8.linux-386.tar.gz'; 			sha256='a826cd599828aeefc86d742e1a8ce8ab7e0251b2429568ad5633e21c8a769053'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.8.linux-ppc64le.tar.gz'; 			sha256='2077dd2fc57a74b0630b0c239ae4e3114607311778effd43fcfe5174133ee188'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.8.linux-s390x.tar.gz'; 			sha256='3fac23801644a2f93a1643acecd5a94a5ea05d88e19467092fb6e64205710f61'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 03 Mar 2022 22:57:41 GMT
ENV GOPATH=/go
# Thu, 03 Mar 2022 22:57:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 22:57:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 03 Mar 2022 22:57:44 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cce169e928830f476b72f6fb2bd7ce1b80e59d3bd3d24202f5fbd7a9535fd48c`  
		Last Modified: Tue, 01 Mar 2022 02:19:20 GMT  
		Size: 48.2 MB (48154229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d57d0b9b76245f122bedc54cfb401efe4ae73525e3e5096c640b38010ce60e`  
		Last Modified: Tue, 01 Mar 2022 03:27:49 GMT  
		Size: 7.4 MB (7377224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657cd7a4baa440bfbce8ec469123713e5b5d23c6629f9fa5b6dd0e75ce50d3a`  
		Last Modified: Tue, 01 Mar 2022 03:27:49 GMT  
		Size: 9.7 MB (9687611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc7ca897fec0f5641e72195c9642b35a822abea245e98700f0e566cb0196407`  
		Last Modified: Tue, 01 Mar 2022 03:28:37 GMT  
		Size: 49.6 MB (49578751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d195b774893b0bb28cca3f5618d2a43afc3bcc8fbc74b8ccd5e2e31487303bbf`  
		Last Modified: Wed, 02 Mar 2022 08:10:03 GMT  
		Size: 52.1 MB (52085868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935ed299ba483f081572b8d0b87f85a3cb1e464f865f390ed0e6f6b7575b6ed3`  
		Last Modified: Thu, 03 Mar 2022 23:09:44 GMT  
		Size: 105.5 MB (105462169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012a53b13e0ccd7bdf5e90836fa1e8072c9a2c385edab7aff66c2e53c626ee52`  
		Last Modified: Thu, 03 Mar 2022 23:08:34 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:fa97aaa80a96474fcee5b5b2c73bcb73b5ae7f1c87420a9b3c9385835517e9f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.1 MB (266123340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72171491fffface85fa3c823252efc71ca5d69a58a19787decae33845738b812`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:29 GMT
ADD file:49ab7c627696d55c8512392867bee4593a377d34c5c4f75aac1eb176a56b672c in / 
# Tue, 01 Mar 2022 02:03:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 09:29:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 09:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 09:30:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 22:00:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 22:00:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 00:49:34 GMT
ENV GOLANG_VERSION=1.17.8
# Fri, 04 Mar 2022 00:50:21 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.8.linux-amd64.tar.gz'; 			sha256='980e65a863377e69fd9b67df9d8395fd8e93858e7a24c9f55803421e453f4f99'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.8.linux-armv6l.tar.gz'; 			sha256='3287ca2fe6819fa87af95182d5942bf4fa565aff8f145812c6c70c0466ce25ae'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.8.linux-arm64.tar.gz'; 			sha256='57a9171682e297df1a5bd287be056ed0280195ad079af90af16dcad4f64710cb'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.8.linux-386.tar.gz'; 			sha256='a826cd599828aeefc86d742e1a8ce8ab7e0251b2429568ad5633e21c8a769053'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.8.linux-ppc64le.tar.gz'; 			sha256='2077dd2fc57a74b0630b0c239ae4e3114607311778effd43fcfe5174133ee188'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.8.linux-s390x.tar.gz'; 			sha256='3fac23801644a2f93a1643acecd5a94a5ea05d88e19467092fb6e64205710f61'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 04 Mar 2022 00:50:23 GMT
ENV GOPATH=/go
# Fri, 04 Mar 2022 00:50:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 00:50:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Mar 2022 00:50:26 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5e77565ce5247d53df5dcb65e54c6d6e73e60996d11fbc1ce5ee34bf80dfa1f2`  
		Last Modified: Tue, 01 Mar 2022 02:19:53 GMT  
		Size: 45.9 MB (45918104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b40356d157bf4856aec771f3f51360d39ebb8715ba13f6f19d8153416eced08`  
		Last Modified: Tue, 01 Mar 2022 09:53:58 GMT  
		Size: 7.1 MB (7125246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02534a5c6a025b55da20b42dc333e67684e4ef06a3b2d46d0b0f00543548e29`  
		Last Modified: Tue, 01 Mar 2022 09:53:59 GMT  
		Size: 9.3 MB (9343821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee494db552973674b15404f408d37e26afac1a9202a409e16f59441f0ccaa6c2`  
		Last Modified: Tue, 01 Mar 2022 09:54:42 GMT  
		Size: 47.4 MB (47357696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7934b614d9a4c199eb37b678fe6f37b690a16ce7d56334136c3c5f9dfe3526`  
		Last Modified: Wed, 02 Mar 2022 22:23:44 GMT  
		Size: 53.2 MB (53240892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872b7c2be86fadda4032852cd065af49f0163bbc2480344bedecf3f8e919490f`  
		Last Modified: Fri, 04 Mar 2022 01:16:23 GMT  
		Size: 103.1 MB (103137425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf37c81a12513c71f440d9f3bdc349294a8e798733ce48934f8c3b606139b6d`  
		Last Modified: Fri, 04 Mar 2022 01:15:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:a6fb95e3372bd02a2af21c895acc7f15f48b279a254d29ec845cccfe34893f9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.0 MB (283973543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be2184728fcc0301aab8f50eac5ad91df546915c5f2536295884e332c8c097a8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:41 GMT
ADD file:ec3d90624857dbfae217c1372a38966f453fcd51282379652f07d2ccf6fcc67e in / 
# Tue, 01 Mar 2022 02:11:42 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:35:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 10:35:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 06:57:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 06:57:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 02:28:33 GMT
ENV GOLANG_VERSION=1.17.8
# Fri, 04 Mar 2022 02:29:06 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.8.linux-amd64.tar.gz'; 			sha256='980e65a863377e69fd9b67df9d8395fd8e93858e7a24c9f55803421e453f4f99'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.8.linux-armv6l.tar.gz'; 			sha256='3287ca2fe6819fa87af95182d5942bf4fa565aff8f145812c6c70c0466ce25ae'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.8.linux-arm64.tar.gz'; 			sha256='57a9171682e297df1a5bd287be056ed0280195ad079af90af16dcad4f64710cb'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.8.linux-386.tar.gz'; 			sha256='a826cd599828aeefc86d742e1a8ce8ab7e0251b2429568ad5633e21c8a769053'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.8.linux-ppc64le.tar.gz'; 			sha256='2077dd2fc57a74b0630b0c239ae4e3114607311778effd43fcfe5174133ee188'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.8.linux-s390x.tar.gz'; 			sha256='3fac23801644a2f93a1643acecd5a94a5ea05d88e19467092fb6e64205710f61'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 04 Mar 2022 02:29:07 GMT
ENV GOPATH=/go
# Fri, 04 Mar 2022 02:29:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 02:29:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Mar 2022 02:29:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:72f0eb753e825356fa0fef854ac259cc8eefdb0f689516f29b13da8b1595c342`  
		Last Modified: Tue, 01 Mar 2022 02:18:46 GMT  
		Size: 49.2 MB (49223022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93053a54416be8288cbcc300d0a929f1279cceff9eb11ad9c080fe5439d62dbd`  
		Last Modified: Tue, 01 Mar 2022 10:45:39 GMT  
		Size: 7.7 MB (7695236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2387f0e2dcc6f4271b34d3158d1768015e4424839f06ae428f4e22de8a5c1542`  
		Last Modified: Tue, 01 Mar 2022 10:45:40 GMT  
		Size: 9.8 MB (9767253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d8752c30aea58b7ac6dd29ed3dee03ac8ecb3aedcc6e23ba5ddaac39d89f0b`  
		Last Modified: Tue, 01 Mar 2022 10:45:58 GMT  
		Size: 52.2 MB (52174602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950f61f24f60a2947ceec6c4f3a247c07661917d317b88c05cb7c2df9591646f`  
		Last Modified: Wed, 02 Mar 2022 07:11:36 GMT  
		Size: 62.4 MB (62419725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d37f2cb5438694ec1a291235a8bcc6c79c0b7b7b678d0327b0f83bb366c2d34`  
		Last Modified: Fri, 04 Mar 2022 02:40:47 GMT  
		Size: 102.7 MB (102693579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a392329948f01677d026aa553336f582e7a0b568a496d1ce691bc3199cc13`  
		Last Modified: Fri, 04 Mar 2022 02:40:32 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:366076f8807c7705d1cf81f9289910f2ba4876ea3249d422b2db29b63f3cfd60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.3 MB (302307129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35b1929c25dbe316d50da35ec91d4771a9c7508ae5fa45342b25e76469aeeee3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:47 GMT
ADD file:bdcedc0826a512fa5720a5481555b67977a75cc3a2c76cf5525f4067f6e30f78 in / 
# Tue, 01 Mar 2022 02:07:47 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:42:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:42:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 05:43:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 04:39:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 04:39:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 22:40:37 GMT
ENV GOLANG_VERSION=1.17.8
# Thu, 03 Mar 2022 22:41:14 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.8.linux-amd64.tar.gz'; 			sha256='980e65a863377e69fd9b67df9d8395fd8e93858e7a24c9f55803421e453f4f99'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.8.linux-armv6l.tar.gz'; 			sha256='3287ca2fe6819fa87af95182d5942bf4fa565aff8f145812c6c70c0466ce25ae'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.8.linux-arm64.tar.gz'; 			sha256='57a9171682e297df1a5bd287be056ed0280195ad079af90af16dcad4f64710cb'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.8.linux-386.tar.gz'; 			sha256='a826cd599828aeefc86d742e1a8ce8ab7e0251b2429568ad5633e21c8a769053'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.8.linux-ppc64le.tar.gz'; 			sha256='2077dd2fc57a74b0630b0c239ae4e3114607311778effd43fcfe5174133ee188'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.8.linux-s390x.tar.gz'; 			sha256='3fac23801644a2f93a1643acecd5a94a5ea05d88e19467092fb6e64205710f61'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 03 Mar 2022 22:41:15 GMT
ENV GOPATH=/go
# Thu, 03 Mar 2022 22:41:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 22:41:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 03 Mar 2022 22:41:16 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:476db560471d1237921e304e3ff8f4080b6678e161577b3284ac8cc10eeacb64`  
		Last Modified: Tue, 01 Mar 2022 02:16:20 GMT  
		Size: 51.2 MB (51207695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c26a779ac27dbfd1d496436ab636b45a1a0157570daf0fe074b2b128251084`  
		Last Modified: Tue, 01 Mar 2022 05:53:41 GMT  
		Size: 8.0 MB (8000492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f554cfd6e25d31263311f533991fee169f308525eac5bfd2a37a744aca5580`  
		Last Modified: Tue, 01 Mar 2022 05:53:41 GMT  
		Size: 10.3 MB (10340017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a9779cb01b98555fd465f4f1e10c4a014e406cf5e9f662ca5522c871ae253d`  
		Last Modified: Tue, 01 Mar 2022 05:54:05 GMT  
		Size: 53.4 MB (53439729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6244980614610e7e627489981ae72e4100912171b55200aa3ad80a474c0015f3`  
		Last Modified: Wed, 02 Mar 2022 04:55:39 GMT  
		Size: 73.6 MB (73640235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05a29aa5fd8455b61c05a758528ddb26757e2ab59365116f506d5d5702e92e0`  
		Last Modified: Thu, 03 Mar 2022 23:00:42 GMT  
		Size: 105.7 MB (105678805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e94f5081168503b66a482cd17b65bfbfa18e103d2f0da20c095b4bb2fbf850f`  
		Last Modified: Thu, 03 Mar 2022 23:00:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; mips64le

```console
$ docker pull golang@sha256:f3e2089409983f631a1f4b6382dc565995786e230e9f83fbcecea6d0d0e6b19d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.1 MB (274149684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b8d5310479cf22d2f2e228acb16c863c5c2d61f73f916898bf6f7f4ef03391`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:19 GMT
ADD file:3571860386733ca996c3c4d7a49193aeb8e67693a3d526fceb67acd916ed1d06 in / 
# Tue, 01 Mar 2022 02:03:20 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:08:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:08:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 03:09:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 Mar 2022 08:07:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 05 Mar 2022 08:07:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Mar 2022 08:31:12 GMT
ENV GOLANG_VERSION=1.17.8
# Sat, 05 Mar 2022 08:41:28 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.8.linux-amd64.tar.gz'; 			sha256='980e65a863377e69fd9b67df9d8395fd8e93858e7a24c9f55803421e453f4f99'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.8.linux-armv6l.tar.gz'; 			sha256='3287ca2fe6819fa87af95182d5942bf4fa565aff8f145812c6c70c0466ce25ae'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.8.linux-arm64.tar.gz'; 			sha256='57a9171682e297df1a5bd287be056ed0280195ad079af90af16dcad4f64710cb'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.8.linux-386.tar.gz'; 			sha256='a826cd599828aeefc86d742e1a8ce8ab7e0251b2429568ad5633e21c8a769053'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.8.linux-ppc64le.tar.gz'; 			sha256='2077dd2fc57a74b0630b0c239ae4e3114607311778effd43fcfe5174133ee188'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.8.linux-s390x.tar.gz'; 			sha256='3fac23801644a2f93a1643acecd5a94a5ea05d88e19467092fb6e64205710f61'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Sat, 05 Mar 2022 08:41:35 GMT
ENV GOPATH=/go
# Sat, 05 Mar 2022 08:41:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Mar 2022 08:41:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 05 Mar 2022 08:41:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:474e1e24c547862b41e95f278b833c2fe32cf9c18a4d6b9d60bb4693d4deabc3`  
		Last Modified: Tue, 01 Mar 2022 02:13:06 GMT  
		Size: 49.1 MB (49079524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92112e67de2237a86e384a0b009d17d7a4bf3303fa948d3204a1069a9625d91`  
		Last Modified: Tue, 01 Mar 2022 03:24:23 GMT  
		Size: 7.3 MB (7253758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40614a0b9d501b650586d48df88bbe0b9b8c667aa7e9caa3597967c89127e0e`  
		Last Modified: Tue, 01 Mar 2022 03:24:24 GMT  
		Size: 10.0 MB (10016358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76be8a996d30253c5206186efb3cadbe915fbecb1ea9c1e67d6fe70fd916779`  
		Last Modified: Tue, 01 Mar 2022 03:25:07 GMT  
		Size: 50.9 MB (50852934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d557016fbbe3941b45a63b42a480133085ed0ff55c676d480d8248dfd67f3e`  
		Last Modified: Sat, 05 Mar 2022 09:03:04 GMT  
		Size: 54.5 MB (54464622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e280c8567deb9912d4f39c078facba49988eae11d11d87b41f5a2a8b21ada84`  
		Last Modified: Sat, 05 Mar 2022 09:06:20 GMT  
		Size: 102.5 MB (102482362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e95108c42c92aeda7c7ad18ed160192ea8d2b2fb18a2d249a8dab65387cdb2`  
		Last Modified: Sat, 05 Mar 2022 09:05:12 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:525a7c0279ca4ce85df828b4300de153c9f0e75851dddfaebd692ca5cb4f61b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.4 MB (305413213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f0ceebc70836c719ba71e33529da9ca435c6e01ea748fe1078d0396b610bde`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:05:31 GMT
ADD file:b0fccd713cf7d422b1caea3a5d8c8bc230da590e6004fb58a27f2e53589bb87e in / 
# Tue, 01 Mar 2022 02:05:38 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 07:18:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 07:18:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 07:21:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 17:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 17:03:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 00:11:19 GMT
ENV GOLANG_VERSION=1.17.8
# Fri, 04 Mar 2022 00:12:08 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.8.linux-amd64.tar.gz'; 			sha256='980e65a863377e69fd9b67df9d8395fd8e93858e7a24c9f55803421e453f4f99'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.8.linux-armv6l.tar.gz'; 			sha256='3287ca2fe6819fa87af95182d5942bf4fa565aff8f145812c6c70c0466ce25ae'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.8.linux-arm64.tar.gz'; 			sha256='57a9171682e297df1a5bd287be056ed0280195ad079af90af16dcad4f64710cb'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.8.linux-386.tar.gz'; 			sha256='a826cd599828aeefc86d742e1a8ce8ab7e0251b2429568ad5633e21c8a769053'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.8.linux-ppc64le.tar.gz'; 			sha256='2077dd2fc57a74b0630b0c239ae4e3114607311778effd43fcfe5174133ee188'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.8.linux-s390x.tar.gz'; 			sha256='3fac23801644a2f93a1643acecd5a94a5ea05d88e19467092fb6e64205710f61'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 04 Mar 2022 00:12:15 GMT
ENV GOPATH=/go
# Fri, 04 Mar 2022 00:12:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 00:12:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Mar 2022 00:12:24 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3af27652881c17f6980cd7f32718c45cc6047a3391b74b55f499341c8efb5ec5`  
		Last Modified: Tue, 01 Mar 2022 02:15:48 GMT  
		Size: 54.2 MB (54183617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2afaad5be738f67c67e6b3d540b5a3dcad788dcd8f5180f494ca1465ac0c03f`  
		Last Modified: Tue, 01 Mar 2022 07:43:43 GMT  
		Size: 8.3 MB (8273085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd41299687186ba7a9a5ca4d29f672f8a2ef6047cbb81a80e5c8b78fd082580`  
		Last Modified: Tue, 01 Mar 2022 07:43:43 GMT  
		Size: 10.7 MB (10727782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7ff69cbc600643af29c318ec272c395ba5acdb3ec94fbf3ee6222336909324`  
		Last Modified: Tue, 01 Mar 2022 07:44:06 GMT  
		Size: 57.5 MB (57458037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001811638c356c2fd30207de2ef15342984b2c8ef36be5c27c8db4d9fd5e19f7`  
		Last Modified: Tue, 01 Mar 2022 17:34:51 GMT  
		Size: 73.7 MB (73682090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff40a3d4ef856807140ff34b11bdecfe73a46fc7a50d904fd2b34de00fedd3d`  
		Last Modified: Fri, 04 Mar 2022 00:32:55 GMT  
		Size: 101.1 MB (101088446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0398bcfd268df9e209c6eb28c6cbbfdd87e43b4c815f5a1727f06e78366ff733`  
		Last Modified: Fri, 04 Mar 2022 00:32:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; s390x

```console
$ docker pull golang@sha256:df286b22d49dc3786fc1377e4114b403e182356c0a2628fb3ed614985b2de3aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280370574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7baf4c68a2afcff2061c4af882345f2696526ab2ab9f04b5cec64fb01c9d034`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:09 GMT
ADD file:d42860e0eaa59b8efe33f2b9046be595efe776263ed470e4020317e451efbc47 in / 
# Tue, 01 Mar 2022 02:02:11 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:52:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:52:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 03:53:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 15:43:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 15:43:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 23:08:24 GMT
ENV GOLANG_VERSION=1.17.8
# Thu, 03 Mar 2022 23:09:42 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.8.linux-amd64.tar.gz'; 			sha256='980e65a863377e69fd9b67df9d8395fd8e93858e7a24c9f55803421e453f4f99'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.8.linux-armv6l.tar.gz'; 			sha256='3287ca2fe6819fa87af95182d5942bf4fa565aff8f145812c6c70c0466ce25ae'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.8.linux-arm64.tar.gz'; 			sha256='57a9171682e297df1a5bd287be056ed0280195ad079af90af16dcad4f64710cb'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.8.linux-386.tar.gz'; 			sha256='a826cd599828aeefc86d742e1a8ce8ab7e0251b2429568ad5633e21c8a769053'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.8.linux-ppc64le.tar.gz'; 			sha256='2077dd2fc57a74b0630b0c239ae4e3114607311778effd43fcfe5174133ee188'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.8.linux-s390x.tar.gz'; 			sha256='3fac23801644a2f93a1643acecd5a94a5ea05d88e19467092fb6e64205710f61'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 03 Mar 2022 23:09:48 GMT
ENV GOPATH=/go
# Thu, 03 Mar 2022 23:09:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 23:09:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 03 Mar 2022 23:09:49 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:05bdf937590b731e3ffabc77f5871a8a9c7e597b417485eb87bc8541e791026b`  
		Last Modified: Tue, 01 Mar 2022 02:07:47 GMT  
		Size: 49.0 MB (49005374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb8877d9e145f9b36d4b6ce925bfba017d214117b3a9ffdded7895c9e5f07ad`  
		Last Modified: Tue, 01 Mar 2022 04:00:50 GMT  
		Size: 7.4 MB (7401505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39f0fcec69d1c8fe79f586cfff15fbfb251a666eb3bd6f16ec55c24d4392017`  
		Last Modified: Tue, 01 Mar 2022 04:00:50 GMT  
		Size: 9.9 MB (9883076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712b9a603e5ec96f647d7c70f8627b53e05bdb787d56a8cd518f70181b04ca3e`  
		Last Modified: Tue, 01 Mar 2022 04:01:04 GMT  
		Size: 51.4 MB (51381386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e5b1db3d5592b1dc22ec8edb23c1faa5425ae6a3be67677bd0ae6e41e6660f`  
		Last Modified: Tue, 01 Mar 2022 15:54:40 GMT  
		Size: 56.8 MB (56845780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6c0187015c63e57c6cdf00cf12791c1aac3a502cae705a729fa50ccc9141bd`  
		Last Modified: Thu, 03 Mar 2022 23:25:46 GMT  
		Size: 105.9 MB (105853297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056af4f345c3ae5cf2599e7657c4827f042eced783038a61ead968fbb10f6a79`  
		Last Modified: Thu, 03 Mar 2022 23:25:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
