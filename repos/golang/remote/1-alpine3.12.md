## `golang:1-alpine3.12`

```console
$ docker pull golang@sha256:0825789cdfb612ca574a4f78d104e75cde41bc466d04dda7d9280099a0f77b93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1-alpine3.12` - linux; amd64

```console
$ docker pull golang@sha256:26530e208a08a6211b85fef395447e5b62d3f657f43856a30d65ee27d75ac778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109789959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa4324ee842a5a083df41ff179e1f706a15116fde07ae641efd035a62b717869`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:20:38 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:20:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:20:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:20:40 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 05:24:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:24:02 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:24:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:24:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:24:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bcff5d981b47d576e4ee185cfc784f975e2fb191f463b5c579fc5cf003f88d`  
		Last Modified: Fri, 11 Dec 2020 05:27:35 GMT  
		Size: 280.8 KB (280796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a343aaa7d2b207b798539017dfc6c3cb3f6043240b793f313c4439535b4855`  
		Last Modified: Fri, 11 Dec 2020 05:27:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2128e2ad96160c85ca6f26a5c5ca34b05d1358c90ab539d38e0365affc9a2e`  
		Last Modified: Fri, 11 Dec 2020 05:28:00 GMT  
		Size: 106.7 MB (106711940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3766394496033d48e3f79c602e0a29249ebcd72c6c50b4c4749717acc8734b5`  
		Last Modified: Fri, 11 Dec 2020 05:27:35 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; arm variant v6

```console
$ docker pull golang@sha256:5a0be74056d5029cff90f381246e39470ad2ad50ce73488fb977cc03a822a05b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105444268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cddd7eb14a03cabf0473ed7e5349b7ff7cb4eb1b9c5f536e436107337af62c1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:01:51 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:01:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:01:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:01:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 05:04:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:04:41 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:04:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:04:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:04:46 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7c54fb8a883364d44abe49903dc93546608e4be42299daf298ec0bf7d6774e`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 281.0 KB (280988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2330f20a2b2cb3bbef000f0a21e2e96505df7a101a96d9a3d64d6760512fb9`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d8c53a4ee3be371b79034d561557cf2baa089fea4ef82f543b6a5dbe1cad8`  
		Last Modified: Fri, 11 Dec 2020 05:09:10 GMT  
		Size: 102.6 MB (102560978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e48cebf375fe9c16f6944ab4921d5803644884d872978e5d553df5188bda1ad`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; arm variant v7

```console
$ docker pull golang@sha256:26170ab628b3726d18117d7395e5d57b728e6b2890d6859b627df603be9455bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105045671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6769f908f96921504e4a5209ff9e6089dfa309ac184a4b09a2419d851f315c70`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 04:21:20 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 04:21:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 04:21:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 04:21:24 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 04:23:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 04:23:45 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 04:23:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 04:23:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 04:23:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f7a33d13d3a67a15b0e6da476d45e9538e15c7b182b9e4e9b38443a1ca08cc`  
		Last Modified: Fri, 11 Dec 2020 04:27:44 GMT  
		Size: 280.1 KB (280075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a6430e76ae8f5ddbd80b7e0e9be11d8852ade60c6b8efb3b6170a3eaeb608e`  
		Last Modified: Fri, 11 Dec 2020 04:27:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20c052f7fc1598e403147f8bf3801b223ee426b6e13103d0c8e4896921fecf9`  
		Last Modified: Fri, 11 Dec 2020 04:28:16 GMT  
		Size: 102.4 MB (102359595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e6bb24a816c4542cb8cbe640b8727fd110a761d7e003da6eb3d55e50b6dd93`  
		Last Modified: Fri, 11 Dec 2020 04:27:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:9db7242849ab53455ff563ed2cd1f7b09f4ae52f66d46a0806d90473071b5784
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105004646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b69f12873ce72b43c6c9a13313bbcbb6f6c73d45e670da7cdca32f6f2eedf6bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:02:51 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:02:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:02:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:02:58 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 05:05:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:05:09 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:05:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:05:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:05:15 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5f482c3568cc90c6f20fb60dcbf6bb89a10c6f176ea45d8a2de645380e8a91`  
		Last Modified: Fri, 11 Dec 2020 05:08:51 GMT  
		Size: 281.2 KB (281217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bcf0ba98061cccf026504d0a60b6170a093072be2268ceb62bc7510b3ea930`  
		Last Modified: Fri, 11 Dec 2020 05:08:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f22952e8d798e70ca18175cfacf167025e3791afb0ad5fb65275551330e317`  
		Last Modified: Fri, 11 Dec 2020 05:09:16 GMT  
		Size: 102.0 MB (102016500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b710c8a110294899caff8d8083f104b8010653f5c8fd740b6d311582e8fdebd`  
		Last Modified: Fri, 11 Dec 2020 05:08:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; 386

```console
$ docker pull golang@sha256:58c9ba244a501a0b30eb103cdae94e8a0d1694421ec4310ddad7db16a40aa31d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.4 MB (108358235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d288049c4234f3017340be7e1dc4c49c0d03957fd1a402b69f3f2bf34889735b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:35:53 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 02:35:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:35:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 02:35:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 02:39:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 02:39:04 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 02:39:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 02:39:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 02:39:05 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4072a9f964a246083c34fad6d81c8f836286f31b1584a2577fa9baf2f75910b3`  
		Last Modified: Fri, 11 Dec 2020 02:43:08 GMT  
		Size: 281.3 KB (281306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064766f3f313546e30af55666fef23777b0fc7d2f20d6c64158085d093b3712d`  
		Last Modified: Fri, 11 Dec 2020 02:43:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70801b0873cb0f7151bd9bd328f6d1bf5cb2459850ca7aa5648d9d9c5d3e0d7a`  
		Last Modified: Fri, 11 Dec 2020 02:43:33 GMT  
		Size: 105.3 MB (105285148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce69570fdd71ece1b57ec5d28912be9ab89f1fc8e191d9cb303df7ad95a65d04`  
		Last Modified: Fri, 11 Dec 2020 02:43:09 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; ppc64le

```console
$ docker pull golang@sha256:ee373e860a2d21d6c0c7c75b2a7912dc8518e3d6ae8026c8bd0879f0195de458
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.8 MB (103785597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3bd73d4dc7f75b5bc0ee95006a4dd33f814721decb586320793fd349e98084e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 16:21:49 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 16:22:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 16:22:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:22:16 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 16:24:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 16:24:32 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 16:24:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:24:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 16:24:59 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b264b8b0b411987202a3e1ecfa44a4d6e0d7685fe6bab7db14eafaf71f17ede`  
		Last Modified: Fri, 11 Dec 2020 16:29:30 GMT  
		Size: 283.2 KB (283206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b66f48807f5cf40dd3fc1c828255b45f31af2afb6ef17a92dc765322276b9d`  
		Last Modified: Fri, 11 Dec 2020 16:29:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee10611cf535391a233e108cc0791e28bf5ae01fbfc7fb10ea87dafadb6064e0`  
		Last Modified: Fri, 11 Dec 2020 16:29:49 GMT  
		Size: 100.7 MB (100698657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a90ac851c3be7cb55e4131966ce03aac102b5c932b0c94c74035b7ab158793`  
		Last Modified: Fri, 11 Dec 2020 16:29:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; s390x

```console
$ docker pull golang@sha256:e0e6d3c824a5ae3a71f581888b32ca798503e61987cbcc20feb9843e1c84b9fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.7 MB (108672873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1acb5a5f0e47625a73d41f73928a804a4c8930b108281220707e7fa20869dd6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:30:08 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 03:30:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:30:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:30:11 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 03:31:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 03:32:05 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 03:32:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:32:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 03:32:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b8373ee2322550f964161dcc28f9d31ea197b1b06dc0b208d66814fd56c7c`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 281.3 KB (281326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7522c8c1c290acd48fd0576ff7b683af6c6810b571304e648801aa55ac3fc6d4`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7cf01ed0b10939a4565a6ba501d639022e8ae33a3601d3b154ea72128c3b3a`  
		Last Modified: Fri, 11 Dec 2020 03:35:23 GMT  
		Size: 105.8 MB (105825250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f330ba5036ee04e6172972318087882091d8b53b4936426ad450d1a0cfb514`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
