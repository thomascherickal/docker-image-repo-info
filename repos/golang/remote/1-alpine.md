## `golang:1-alpine`

```console
$ docker pull golang@sha256:d4b1380a9b98367e32cd83620e1f1f2016a2b75481cc3fd258cee183f6404d53
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

### `golang:1-alpine` - linux; amd64

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

### `golang:1-alpine` - linux; arm variant v6

```console
$ docker pull golang@sha256:5c15d81085053c9df4a6a6dd43a3f113968b48c614a08c2af255763fdbac3920
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105444746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f230ec408748d46a95ba4586e406bb216bc584d4661c59a1874da1cce5c00377`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:19:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:19:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 01:19:30 GMT
ENV GOLANG_VERSION=1.15.6
# Thu, 17 Dec 2020 01:22:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 17 Dec 2020 01:22:08 GMT
ENV GOPATH=/go
# Thu, 17 Dec 2020 01:22:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 01:22:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Dec 2020 01:22:12 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec13a9d7ac84771eb7bc7617ba663afac7b1d2653e88d9bcdb8bccf6582b80aa`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 281.0 KB (280973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9257d191bf96f32644fd965aa6a4ff717d858165485be44d9b4ab2f88819120`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d83b8425d453629ec206e00b38ebffac69551fc3dcf106ac85bbbbc9ce87f3d`  
		Last Modified: Thu, 17 Dec 2020 01:30:15 GMT  
		Size: 102.6 MB (102559301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a435cb896ff93a5be68d37c052dc45f4362c886b64ca61312fbaa06a89f926f`  
		Last Modified: Thu, 17 Dec 2020 01:29:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; arm variant v7

```console
$ docker pull golang@sha256:e946774905f6b72f01471355260c23ce41950544d5ef0eb1027b13742aab0b21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e1ff3cc9639dea3a51e98aa3d3b9e44eaccc8cf712c62c65ecfb2d42ff24a1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:33 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:25:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:25:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 01:25:39 GMT
ENV GOLANG_VERSION=1.15.6
# Thu, 17 Dec 2020 01:28:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 17 Dec 2020 01:28:14 GMT
ENV GOPATH=/go
# Thu, 17 Dec 2020 01:28:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 01:28:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Dec 2020 01:28:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0ca5f7e7e39c37c9f0a26160a742edda20ab73836336395e0b0aeded33776`  
		Last Modified: Thu, 17 Dec 2020 01:34:49 GMT  
		Size: 280.1 KB (280060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6490e713d90e3419a99e20463b25f536cd4a3aa5b97dc06f62e6dbdc4f826435`  
		Last Modified: Thu, 17 Dec 2020 01:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceaa45986b4eb3f29644518c0b38cb449c6f1a2da26887ce51ae55155cbe9e87`  
		Last Modified: Thu, 17 Dec 2020 01:35:19 GMT  
		Size: 102.4 MB (102359943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441a2cf812c9d0c6e2e90e786e796a9534eb4efeb477b879fcbad2f65210ba65`  
		Last Modified: Thu, 17 Dec 2020 01:34:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:20c2e95307cf27e1192679317ba8aa80fc686fe47cceb20b11ff28f6f1d59e08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105006982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad8b9783386381558175c5dab439f8b0bd25cdeacf36989d1aee7aa0352e0154`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:41:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 04:41:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 04:41:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 04:41:50 GMT
ENV GOLANG_VERSION=1.15.6
# Thu, 17 Dec 2020 04:44:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 17 Dec 2020 04:44:06 GMT
ENV GOPATH=/go
# Thu, 17 Dec 2020 04:44:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 04:44:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Dec 2020 04:44:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e1f0424fba9fa0ae1558cf9537def9b5de2873566d5ef8564ba0f4a4e99fc6`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 281.2 KB (281214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e458f4c6c667cc63829508308a9735d0586f4f55eff2b6c07236536557461e0`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4e3c46f4b2da2c30b588abbdbc1c965ca45dec57c46ac7ff7667276354f41c`  
		Last Modified: Thu, 17 Dec 2020 04:51:29 GMT  
		Size: 102.0 MB (102016410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577341a4c2b5003d7ac897786268733201eca320790b7918e0575462f29ca0df`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; 386

```console
$ docker pull golang@sha256:00967cc62fe598f62aec4b63c9f53f1de00f838384ab39e18ea02e5d2853e5ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.4 MB (108360956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33756cc7eba6bdd4b534c3df15fb6b49a5986ffc0913eaffecb5cf6c3649fbbe`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:07:15 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 02:07:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 02:07:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 02:07:16 GMT
ENV GOLANG_VERSION=1.15.6
# Thu, 17 Dec 2020 02:11:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 17 Dec 2020 02:11:25 GMT
ENV GOPATH=/go
# Thu, 17 Dec 2020 02:11:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 02:11:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Dec 2020 02:11:26 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40840432391b9874ed7a9993a624f9f0a51b79928c8c8b9fe7e847802e39bb9e`  
		Last Modified: Thu, 17 Dec 2020 02:21:49 GMT  
		Size: 281.3 KB (281318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcd07ee69985a1d4a6d371a2c38b73690408d26fa31258f2301df6973fa4035`  
		Last Modified: Thu, 17 Dec 2020 02:21:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251ededb54386bbd5ba9d5a6e879ea564658eaf91e58a6fe8277aa7519c11bff`  
		Last Modified: Thu, 17 Dec 2020 02:22:19 GMT  
		Size: 105.3 MB (105285229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333c9cc3aff50eeecfa4769a06f4d9ba188f4bdc83f6750b693c3905429c40a5`  
		Last Modified: Thu, 17 Dec 2020 02:21:50 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; ppc64le

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

### `golang:1-alpine` - linux; s390x

```console
$ docker pull golang@sha256:33e3373af0eb9e4eda183f5f7c8c8397b50bcdf99a88df1a971f203df7ba4e47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.7 MB (108674002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93d15df85f01b697801f8171373b0aacbe72840276df5994700ad14c062ec69d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:33:00 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:33:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:33:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 01:33:03 GMT
ENV GOLANG_VERSION=1.15.6
# Thu, 17 Dec 2020 01:34:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 17 Dec 2020 01:35:07 GMT
ENV GOPATH=/go
# Thu, 17 Dec 2020 01:35:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 01:35:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Dec 2020 01:35:09 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a14f4067d7797fd5cfb87803df1ad2a3d7625d0b843e97d16cb7603123a7`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 281.3 KB (281328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7c9b3bde5c297668741ef40758508b43d424457fdbd8fcf1feb93e32b22f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b885e078d779a906a017db70793772d08bfd1c09e050ad172577c0fab7b96784`  
		Last Modified: Thu, 17 Dec 2020 01:41:32 GMT  
		Size: 105.8 MB (105825345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e0301d931c4c8c59aa0d28c7d3e1f9d2393f0dcf388736ac58ae013b1cb61`  
		Last Modified: Thu, 17 Dec 2020 01:41:20 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
