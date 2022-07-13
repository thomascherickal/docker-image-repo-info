## `golang:buster`

```console
$ docker pull golang@sha256:55bb0affc48c86f081c2fdafce579ba236f4327f9ed2bc58b71e54b372d2926c
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

### `golang:buster` - linux; amd64

```console
$ docker pull golang@sha256:d966ce343c1efa8bf9200a87d202f9873f2146951c4165058e09b663e30171a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330782435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e87973a8632a8aefa3f02be25be90794b0ab0b5c640b13cb117dc481008625b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:20 GMT
ADD file:d738977543f4afc4c3040c6fca3e3f15388ec3b7263a29a6aa83f9a4bf05fed1 in / 
# Tue, 12 Jul 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:49:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:49:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:49:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 23:55:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 23:55:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 23:59:54 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 00:00:07 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.4.linux-amd64.tar.gz'; 			sha256='c9b099b68d93f5c5c8a8844a89f8db07eaa58270e3a1e01804f17f4cf8df02f5'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.4.linux-armv6l.tar.gz'; 			sha256='7dfeab572e49638b0f3d9901457f0622c27b73301c2b99db9f5e9568ff40460c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.4.linux-arm64.tar.gz'; 			sha256='35014d92b50d97da41dade965df7ebeb9a715da600206aa59ce1b2d05527421f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.4.linux-386.tar.gz'; 			sha256='418232d905e18ece6cb13c4884bb1c68963d7d3b4d889671b3e5be8bd4059862'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.4.linux-ppc64le.tar.gz'; 			sha256='f80acc4dc054ddc89ccc4869664e331bf16e0ac6e07830e94554162e66f66961'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.4.linux-s390x.tar.gz'; 			sha256='7e932f36e8f347feea2e706dcd32c1a464b1e5767ab2928ae460a37a975fe4a3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 13 Jul 2022 00:00:08 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 00:00:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:00:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 00:00:09 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:80b89a2b88b24e7be7c8038e2cbff99ad4fd2f07ad914da4bab80dabaadf8a99`  
		Last Modified: Tue, 12 Jul 2022 01:24:55 GMT  
		Size: 50.4 MB (50440555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0405f798f5b335d83b02371187f3be0ce2092aa0c6b6178ff11290ee6a14c9`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 7.9 MB (7856888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab80b2b0494ab26b41941fb73a028292e2e5d2070c56b3488e890eda20e04641`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 10.0 MB (9998095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb827974c1cb152eae96a7b67abce3afa75353dec7790c0c07fdbb8906925921`  
		Last Modified: Tue, 12 Jul 2022 02:56:31 GMT  
		Size: 51.8 MB (51843739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107910070fddb285b7efcd0059371a3e6390693a973af12e3dc7588fa1d4630e`  
		Last Modified: Wed, 13 Jul 2022 00:09:17 GMT  
		Size: 68.8 MB (68828758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d86d53e142ee8a4a08899aa8a23fd0296958a0c7a167d8d16d6959b8ea17f73`  
		Last Modified: Wed, 13 Jul 2022 00:11:33 GMT  
		Size: 141.8 MB (141814245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc048aab24e0527d2849a5de7feb0d3a17b2042bec0d0d426a249a12c55a22ff`  
		Last Modified: Wed, 13 Jul 2022 00:11:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:b12e0250be32f8748d4548785e8777fb24e772123b4d30e546185e88922540d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.1 MB (279149118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:753681e69d0bc15c0d67be44a15abe432992ec17a40984540ad7023446d5182a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:51:06 GMT
ADD file:29a86a4b70e0fb7454a1325b875ec05d02fe02c2dd72a61a0b9476e7f1f3fb78 in / 
# Thu, 23 Jun 2022 00:51:07 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:41:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:41:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:42:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 10:56:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 10:56:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jun 2022 11:06:11 GMT
ENV GOLANG_VERSION=1.18.3
# Fri, 24 Jun 2022 11:10:19 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Fri, 24 Jun 2022 11:10:21 GMT
ENV GOPATH=/go
# Fri, 24 Jun 2022 11:10:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jun 2022 11:10:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 24 Jun 2022 11:10:23 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:dad2005e84922efa5686f4921c83f828452891153e5fad381514bbdbd3b2b8fa`  
		Last Modified: Thu, 23 Jun 2022 01:06:27 GMT  
		Size: 48.2 MB (48160705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e32e30ed2717efe58bd73d7a7469de69e97c528d2402897d3f6d326ca6af4`  
		Last Modified: Thu, 23 Jun 2022 02:04:39 GMT  
		Size: 7.4 MB (7400800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd283a4314a89d71392745ece238ed63888f508f2dd55f513099cfe5d8748eeb`  
		Last Modified: Thu, 23 Jun 2022 02:04:39 GMT  
		Size: 9.7 MB (9687650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8287fbf741a3acfdcc7dae55783cb6450c99e052448a3e31549e333a036e58d`  
		Last Modified: Thu, 23 Jun 2022 02:05:28 GMT  
		Size: 49.6 MB (49584208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22705a1933515fe24a14518f18bd842b2429ba6fd6be941b2d4777ae2a1b4bf1`  
		Last Modified: Fri, 24 Jun 2022 11:22:26 GMT  
		Size: 52.1 MB (52110082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f640519f690dce86c758e475d5248ac33b4f051cb5f4adda4b60270b037bc77e`  
		Last Modified: Fri, 24 Jun 2022 11:26:14 GMT  
		Size: 112.2 MB (112205517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c34d7ab1b36858ac47c69278f58536f9c11d144b061e224897645533033cc4`  
		Last Modified: Fri, 24 Jun 2022 11:24:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:a511064471275696769f7b41cf6ce4d3a1c9fe8ced25bd2835c24c0df288d2f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.1 MB (273101303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e75a6fa79021cb04d878876a25f4607b50a106d5834db27b1a489e9c15ca1535`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:00:14 GMT
ADD file:b8401862d74ac67a61f764c5dcc54fde231623bf55d2299665eab35dccd25114 in / 
# Thu, 23 Jun 2022 01:00:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:50:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:50:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:51:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 19:25:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 19:25:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jun 2022 19:29:24 GMT
ENV GOLANG_VERSION=1.18.3
# Fri, 24 Jun 2022 19:30:05 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Fri, 24 Jun 2022 19:30:06 GMT
ENV GOPATH=/go
# Fri, 24 Jun 2022 19:30:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jun 2022 19:30:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 24 Jun 2022 19:30:08 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0555d003e6ef528480fa5625ca8ff9a45d899a62b5c20ab7547a42c64d7c1d4c`  
		Last Modified: Thu, 23 Jun 2022 01:16:07 GMT  
		Size: 45.9 MB (45915761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67b659cf86b06bd457cf205d2cfded55fd9654e275d3ec128f15fb94099c21f`  
		Last Modified: Thu, 23 Jun 2022 02:16:11 GMT  
		Size: 7.1 MB (7145400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6da167dadbe348ebfc7cbe4152eae80fb72e14b28b417ffa2bc6adf87034179`  
		Last Modified: Thu, 23 Jun 2022 02:16:12 GMT  
		Size: 9.3 MB (9343917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034ac9bc2920b12499948ed10c17ffdc5b34b7e5bff76a6b5735dbddcd25233f`  
		Last Modified: Thu, 23 Jun 2022 02:16:49 GMT  
		Size: 47.4 MB (47359583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1890f5ae12567562c802dd823d296117598a1473bb92d549d36661f3ac2b5a3a`  
		Last Modified: Fri, 24 Jun 2022 19:40:38 GMT  
		Size: 53.3 MB (53276843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3432b8eb3ffa63df36ddf122497f6dcd08907c239448a84d18f6644d23dae57`  
		Last Modified: Fri, 24 Jun 2022 19:46:00 GMT  
		Size: 110.1 MB (110059645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e089c07371c33791f69fc9f144619d0802b0c6ed4ecbd6149e198915337da107`  
		Last Modified: Fri, 24 Jun 2022 19:44:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:e27f68813b00f1f8adaf1bc43164baddb4775c51d70b4e1f47f41a5fbfbcafdf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.3 MB (290299476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2983818360cf6ff885b568f1a06ec5a076c2d6537d67e45b59bd4f2b29749c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:46 GMT
ADD file:ea39534c5e9a548d7938f6b0e2459383caaf3906f3cc5eafe8bf66053b19f2d5 in / 
# Tue, 12 Jul 2022 00:40:47 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:34:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:35:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 21:22:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 21:22:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:23:03 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:23:14 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.4.linux-amd64.tar.gz'; 			sha256='c9b099b68d93f5c5c8a8844a89f8db07eaa58270e3a1e01804f17f4cf8df02f5'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.4.linux-armv6l.tar.gz'; 			sha256='7dfeab572e49638b0f3d9901457f0622c27b73301c2b99db9f5e9568ff40460c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.4.linux-arm64.tar.gz'; 			sha256='35014d92b50d97da41dade965df7ebeb9a715da600206aa59ce1b2d05527421f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.4.linux-386.tar.gz'; 			sha256='418232d905e18ece6cb13c4884bb1c68963d7d3b4d889671b3e5be8bd4059862'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.4.linux-ppc64le.tar.gz'; 			sha256='f80acc4dc054ddc89ccc4869664e331bf16e0ac6e07830e94554162e66f66961'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.4.linux-s390x.tar.gz'; 			sha256='7e932f36e8f347feea2e706dcd32c1a464b1e5767ab2928ae460a37a975fe4a3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 12 Jul 2022 22:23:15 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:23:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:23:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:23:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:891a1587d3644a8b4b6dab3726ef380a725a0e19bfbf0eac02a275f711985862`  
		Last Modified: Tue, 12 Jul 2022 00:46:46 GMT  
		Size: 49.2 MB (49228928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d1ed6a27dab15e77b7afa9c8697a170f017a73ec9ea8f3f00d5f322e1d3ab`  
		Last Modified: Tue, 12 Jul 2022 02:43:49 GMT  
		Size: 7.7 MB (7720027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186afd5d5e89c602b988d31dd5210c9e3c19435f849f6cc4a6a22a2388e83cf`  
		Last Modified: Tue, 12 Jul 2022 02:43:46 GMT  
		Size: 9.8 MB (9768648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5359768b018a374b04e8bf19e97c814527cb448f87c25de12fbabbb2ff3556d`  
		Last Modified: Tue, 12 Jul 2022 02:44:07 GMT  
		Size: 52.2 MB (52174846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa18f8501e4d284a9ce0729c6bb2aea70693faccddb329e9852ab4280adf3ab`  
		Last Modified: Tue, 12 Jul 2022 21:27:48 GMT  
		Size: 62.5 MB (62470498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f2ca3bb5a5257c6f5ed9e32bcc7ad905eb20058d32c53d390545dbc5a1ccc4`  
		Last Modified: Tue, 12 Jul 2022 22:33:13 GMT  
		Size: 108.9 MB (108936403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f6cdb30ea8ed8bfe5d22b95dec1169a701b5cbb2dd9000f395b97a32159c4`  
		Last Modified: Tue, 12 Jul 2022 22:32:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; 386

```console
$ docker pull golang@sha256:66e8f7dc1145623649dcda06b8bab6277feddb929df64fc0325a386f3babb991
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.2 MB (309190853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9540f25b1907c98b071df420247d257e79cdd3a7866ca0d42688d77247408612`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:39 GMT
ADD file:0f1020fa1fb5b3518ec765b21180056cc802ac9258d1eed5e109edd83e0038d9 in / 
# Tue, 12 Jul 2022 00:39:40 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:28:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:28:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 04:29:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 18:40:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 18:41:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:25:31 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:26:45 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.4.linux-amd64.tar.gz'; 			sha256='c9b099b68d93f5c5c8a8844a89f8db07eaa58270e3a1e01804f17f4cf8df02f5'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.4.linux-armv6l.tar.gz'; 			sha256='7dfeab572e49638b0f3d9901457f0622c27b73301c2b99db9f5e9568ff40460c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.4.linux-arm64.tar.gz'; 			sha256='35014d92b50d97da41dade965df7ebeb9a715da600206aa59ce1b2d05527421f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.4.linux-386.tar.gz'; 			sha256='418232d905e18ece6cb13c4884bb1c68963d7d3b4d889671b3e5be8bd4059862'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.4.linux-ppc64le.tar.gz'; 			sha256='f80acc4dc054ddc89ccc4869664e331bf16e0ac6e07830e94554162e66f66961'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.4.linux-s390x.tar.gz'; 			sha256='7e932f36e8f347feea2e706dcd32c1a464b1e5767ab2928ae460a37a975fe4a3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 12 Jul 2022 22:26:46 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:26:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:26:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:26:50 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:87a13c20a9000f48185a3819712d2a14a8ddd6111bd1392856609aa18a233847`  
		Last Modified: Tue, 12 Jul 2022 00:45:40 GMT  
		Size: 51.2 MB (51204001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798a6241824db4c4cb7e4997fe37c17a97c4d76bf1fb544730ccdbbbc9aaf8e0`  
		Last Modified: Tue, 12 Jul 2022 04:37:13 GMT  
		Size: 8.0 MB (8022957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a99684560fe738e37dc34fae618fb12d6be36f03ccc22266fe649cb7bbb61c4`  
		Last Modified: Tue, 12 Jul 2022 04:37:14 GMT  
		Size: 10.1 MB (10123633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1585b0c9e22a13d5d87725ff1930fdb45614aee7c6e4e100407baf92a6bf7511`  
		Last Modified: Tue, 12 Jul 2022 04:37:36 GMT  
		Size: 53.4 MB (53443224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bedb340d7b534bdb03b61ee8d2f2389843f8726c1e0ed6faa07d088e85742d10`  
		Last Modified: Tue, 12 Jul 2022 18:47:21 GMT  
		Size: 73.5 MB (73463846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93c3f3d6e03e3d01ef191c6c3c1c786385e8705c468933ae67124161c083f91`  
		Last Modified: Tue, 12 Jul 2022 22:38:40 GMT  
		Size: 112.9 MB (112933066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce0b392544f2bb46540e64338d384bdea04f6d9ce9281014b8994a8805d0442`  
		Last Modified: Tue, 12 Jul 2022 22:38:25 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; mips64le

```console
$ docker pull golang@sha256:39e6e0fbc0fbbd73f221e62afa89e3533413dc08929cf0127db5d6d3f0af26bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.9 MB (279867238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e62639e8746b4956d579a2d8242cf0a4cedbc7740dc0c636a838c8132dc9a6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:55 GMT
ADD file:e97021cb9347cc6233316e4e1f31dc6728791c819d5c4f472c2e9009df33ed64 in / 
# Thu, 23 Jun 2022 01:10:58 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:00:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 02:00:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 02:02:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 25 Jun 2022 01:08:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jun 2022 01:08:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 25 Jun 2022 01:33:28 GMT
ENV GOLANG_VERSION=1.18.3
# Sat, 25 Jun 2022 01:44:59 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Sat, 25 Jun 2022 01:45:07 GMT
ENV GOPATH=/go
# Sat, 25 Jun 2022 01:45:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 25 Jun 2022 01:45:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 25 Jun 2022 01:45:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c69f93f35e40f60566a2c787b9d7a1e4ae3c026d480bd089de24eaaa432ffab6`  
		Last Modified: Thu, 23 Jun 2022 01:21:04 GMT  
		Size: 49.1 MB (49073169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8064d03bf4d62d6d286faab208b26248a41ff122c53e3a1cc34d98fff9698faa`  
		Last Modified: Thu, 23 Jun 2022 02:23:21 GMT  
		Size: 7.3 MB (7272853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11d44e638ac6c53724b0eefa08dde59c4fe2c7cb51801bb214ab56c4f8634a5`  
		Last Modified: Thu, 23 Jun 2022 02:23:22 GMT  
		Size: 9.8 MB (9800300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0c8148d6586ab0843c3316210a98b1355a7b90e58c7f09e81feee93e27bcd0`  
		Last Modified: Thu, 23 Jun 2022 02:24:08 GMT  
		Size: 50.9 MB (50862080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31596c76bed9facd68d30e0115c18026928a0c0ab694bb5212f70b2643a44d6`  
		Last Modified: Sat, 25 Jun 2022 02:10:41 GMT  
		Size: 54.5 MB (54494426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe22636fa86334e30e3896f9a7309694de250caf256f346d36ff22f06dce66e6`  
		Last Modified: Sat, 25 Jun 2022 02:14:03 GMT  
		Size: 108.4 MB (108364284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77ff70af1fdfab726ff86807c89a63794a174e5801e0a2208f568dc00eacd8a`  
		Last Modified: Sat, 25 Jun 2022 02:12:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; ppc64le

```console
$ docker pull golang@sha256:df9de3080c7ab45e816beda37b3080e71cb89e8229f4e7820c4237572bd596b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313286455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e592bb3990113ba8d32fae987bea31a1d593532ca3e3be9e3b5dcc10afc4483`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:51 GMT
ADD file:651dca0ba404ba6a560fe25a63054deb11b1aec0fc51ebd145c915e1b97fd834 in / 
# Thu, 23 Jun 2022 02:02:58 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:03:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 04:04:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 09:40:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 09:40:09 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jun 2022 09:42:27 GMT
ENV GOLANG_VERSION=1.18.3
# Fri, 24 Jun 2022 09:42:52 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Fri, 24 Jun 2022 09:43:00 GMT
ENV GOPATH=/go
# Fri, 24 Jun 2022 09:43:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jun 2022 09:43:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 24 Jun 2022 09:43:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb2f047b2d097aaf3e5da7de371063fbf729a1c3fd6ab1cee82d13f03254370`  
		Last Modified: Thu, 23 Jun 2022 02:16:23 GMT  
		Size: 54.2 MB (54177078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d902fbcc2ecb85d4ab4d36e29235eb6b978f4a3035968d4ea028626e38c71a4`  
		Last Modified: Thu, 23 Jun 2022 04:57:40 GMT  
		Size: 8.3 MB (8293484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f29aa6ed276658001fa6bd75c44868b4af4f56471e72abed20dab06f448352`  
		Last Modified: Thu, 23 Jun 2022 04:57:40 GMT  
		Size: 10.7 MB (10727747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140247e5e0a857ee6f2c5ce1b0cd1438933ec15284502dcd566ce57f45a406e8`  
		Last Modified: Thu, 23 Jun 2022 04:58:04 GMT  
		Size: 57.5 MB (57457818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f0d4ffdd04810894789224461a746faba71c3c73baf175a0c3296d07cc6a41`  
		Last Modified: Fri, 24 Jun 2022 09:48:49 GMT  
		Size: 73.7 MB (73708757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bccc9f7e66bc9dd9847db30689c8ed590c92c5972eab9d90193bda3d4a744`  
		Last Modified: Fri, 24 Jun 2022 09:50:10 GMT  
		Size: 108.9 MB (108921415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d99841a2c94607e7e46d3f5441859a2d5e3651b7d7f90b5c5365effa652621a`  
		Last Modified: Fri, 24 Jun 2022 09:49:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; s390x

```console
$ docker pull golang@sha256:21f56ffddf5402591a0f31a3eb26fa58973f769886e6691e45dfee3a60096632
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.2 MB (286201501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8590fe7b43a3bff6e6ebcb0dc3136a1d4d86257827c4c00f67a2c1629e834f4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:44:12 GMT
ADD file:b8babeb1255f220a475b65f77c9d786d49eda80433cab5dc00c944dc05d31c77 in / 
# Tue, 12 Jul 2022 00:44:18 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:42:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:42:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 21:26:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 21:26:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 21:30:13 GMT
ENV GOLANG_VERSION=1.18.3
# Tue, 12 Jul 2022 21:30:40 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 12 Jul 2022 21:30:56 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 21:30:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 21:30:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 21:30:59 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:99ceea1856d0a41d4fd9ea8821ed7e159ce3cc53839fdbed273f1a57f5d9f5b1`  
		Last Modified: Tue, 12 Jul 2022 00:53:59 GMT  
		Size: 49.0 MB (49006967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d39886922611614df255183efa3a602bc91f0072b4e1466a96123ed6a04fde`  
		Last Modified: Tue, 12 Jul 2022 02:54:32 GMT  
		Size: 7.4 MB (7424030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980866729827122d1363e7eeff83efd6aaf40f570e59520d17f45f371606fd3a`  
		Last Modified: Tue, 12 Jul 2022 02:54:32 GMT  
		Size: 9.9 MB (9884925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777c967a6f06f6c0185ac55b09d58fa88079c4e7614928ef9e63ba1df5e4eea9`  
		Last Modified: Tue, 12 Jul 2022 02:54:48 GMT  
		Size: 51.4 MB (51383024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c73ed0e97ef07fd54fab211db4d6a094632476d7b729d5cbb774c7e0f72a20d`  
		Last Modified: Tue, 12 Jul 2022 21:36:16 GMT  
		Size: 56.9 MB (56895690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afc11d3eb19bc887277870cf5fa1100b8a076ac678977e5175253ca561e91ec`  
		Last Modified: Tue, 12 Jul 2022 21:37:36 GMT  
		Size: 111.6 MB (111606709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029037790d0d5601c500f37a4a91acdb33a195ba6c22768d5829cc8f4f85aa94`  
		Last Modified: Tue, 12 Jul 2022 21:37:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
