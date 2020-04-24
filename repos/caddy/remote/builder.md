## `caddy:builder`

```console
$ docker pull caddy@sha256:58dfd4e3cbef7b0b1048ef1f8713058b456434f0b5b0af49ace170a00bca62b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:486d86fe70265203228afb9b9e6e7934019090c6686da9a9fb98579931a05778
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322863984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33fd06ca5bdeb1a36375ba63a93a06401045ebb7a6154830e973a6de5949242b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:02:02 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 23 Mar 2020 23:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Apr 2020 23:06:10 GMT
ENV GOLANG_VERSION=1.14.2
# Wed, 08 Apr 2020 23:11:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 08 Apr 2020 23:11:13 GMT
ENV GOPATH=/go
# Wed, 08 Apr 2020 23:11:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Apr 2020 23:11:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Apr 2020 23:11:16 GMT
WORKDIR /go
# Mon, 13 Apr 2020 23:43:21 GMT
WORKDIR /src
# Mon, 13 Apr 2020 23:43:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 13 Apr 2020 23:43:24 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:27 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 13 Apr 2020 23:43:27 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 13 Apr 2020 23:43:57 GMT
RUN go get -d ./...
# Mon, 13 Apr 2020 23:43:59 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 13 Apr 2020 23:43:59 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c732a2540651eb09faab95b03b3b5928ab23e096fae0006bdc2abf9e0cb5bfb4`  
		Last Modified: Mon, 23 Mar 2020 23:13:03 GMT  
		Size: 301.3 KB (301283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2225181d6bcfb7877529a7257ff207cb14e52831420f770cbc2187031b6228`  
		Last Modified: Mon, 23 Mar 2020 23:13:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdfa13e5b48c976ba308826b27a4978c2ffe6833efcfcfc0bd40dbf25e88455`  
		Last Modified: Wed, 08 Apr 2020 23:26:23 GMT  
		Size: 132.0 MB (132012220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c48a539365d2d572e18de4a42ab11b02d9870a17bf1f65160d7fcbbd0423263`  
		Last Modified: Wed, 08 Apr 2020 23:25:47 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947fdad36c6d1e2fd7b618aa1a49dfabaa1ff9d6fb85a195e2437c2b9ac78142`  
		Last Modified: Mon, 13 Apr 2020 23:44:26 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a199e6b2236a218d72efd03fc1fa0971c00c87439722e1a40269b7edfd910b79`  
		Last Modified: Mon, 13 Apr 2020 23:44:28 GMT  
		Size: 8.2 MB (8155831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732862f7439776bbe7cc313ed1e10454506f168429234c0daea17d6c48a9692`  
		Last Modified: Mon, 13 Apr 2020 23:44:26 GMT  
		Size: 2.7 MB (2744273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54fb1573600e831b250c83cb9dc699bab8aa12040568d9ee542fb8d09c1d99`  
		Last Modified: Mon, 13 Apr 2020 23:45:02 GMT  
		Size: 176.8 MB (176846093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e336ec02e20348f57d1ef8151ecfcd216777f5489f01b29164883ec496bcbb`  
		Last Modified: Mon, 13 Apr 2020 23:44:25 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6f8a2da1c847ae8cd10d1f3e37ad75cc0ba17c5e9b4f7e68fdd3b7cffb5482`  
		Last Modified: Mon, 13 Apr 2020 23:44:25 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c9e71494cec26fe243c54231ae6fe4612a24fba7642b2782a2003bd4ac925f77
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.3 MB (318301249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8b7f3bccf28346106c5d13d871e3b568057fec490d1f94bb04447e57ff90fd2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:43:41 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 17:43:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:43:45 GMT
ENV GOLANG_VERSION=1.14.2
# Thu, 23 Apr 2020 17:49:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 23 Apr 2020 17:49:50 GMT
ENV GOPATH=/go
# Thu, 23 Apr 2020 17:49:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 17:49:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 23 Apr 2020 17:49:53 GMT
WORKDIR /go
# Fri, 24 Apr 2020 00:01:08 GMT
WORKDIR /src
# Fri, 24 Apr 2020 00:01:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 24 Apr 2020 00:01:22 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Fri, 24 Apr 2020 00:01:47 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 24 Apr 2020 00:01:52 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 24 Apr 2020 00:04:31 GMT
RUN go get -d ./...
# Fri, 24 Apr 2020 00:04:38 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Fri, 24 Apr 2020 00:04:46 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ace047eafbdd1d41e753db1fd1004be452f749a7de56a3d24b2614a64577f5`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 301.6 KB (301629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d0031acb1953f56f2c2592c1c5882b29aa828d45deccabbb9a1b5483090a43`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851f1e9e77f7c701487b8ba5a7a0c915267b412d298572641c41785cacdb0a87`  
		Last Modified: Thu, 23 Apr 2020 18:04:01 GMT  
		Size: 128.1 MB (128149566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8512d94a71aa9475406b77a5df2ea5a15483204ab412358643fbe90c4af6c63`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d515fa8cb76d9c64fedf8066a5d83b006a3f31d3f77bb6fda67c2e36668c18ab`  
		Last Modified: Fri, 24 Apr 2020 00:05:13 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14562a711f9706a0fb683480cf3849913e6b3f11d3599c62e4d1f9e831a46bf5`  
		Last Modified: Fri, 24 Apr 2020 00:05:12 GMT  
		Size: 7.8 MB (7794673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b172f9b87cc50b54dd1b3ec4a0a0d2e28b44b924e8f0602b2ba7a1a93987237d`  
		Last Modified: Fri, 24 Apr 2020 00:05:10 GMT  
		Size: 2.6 MB (2583752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbdcf6d6318b0e66c309c8d344563f2c4c5fada8a8764f7b513dbecd956170`  
		Last Modified: Fri, 24 Apr 2020 00:06:03 GMT  
		Size: 176.9 MB (176850568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb35003bc5bd2fabea9a8e09f2761c662d1ce95e5d3e829a07ea2b619b5e35e6`  
		Last Modified: Fri, 24 Apr 2020 00:05:11 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ba293916f1b61d0eee5c397f11e2e206ffaa0c54d17f2bfb328da7e6f09743`  
		Last Modified: Fri, 24 Apr 2020 00:05:10 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c6b2f1f5d52cfbabf244af757effe7b6ddc142acdb15ef5d8dc7452a9659b795
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.9 MB (316942094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:516ec248376a670b87153cbe61efb69b30615826ae2ec1ee48034a951a771e92`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:47:15 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 23 Mar 2020 23:47:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Apr 2020 23:11:43 GMT
ENV GOLANG_VERSION=1.14.2
# Wed, 08 Apr 2020 23:14:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 08 Apr 2020 23:14:23 GMT
ENV GOPATH=/go
# Wed, 08 Apr 2020 23:14:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Apr 2020 23:14:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Apr 2020 23:14:31 GMT
WORKDIR /go
# Tue, 14 Apr 2020 19:02:05 GMT
WORKDIR /src
# Tue, 14 Apr 2020 19:02:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 14 Apr 2020 19:02:10 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:02:15 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 14 Apr 2020 19:02:17 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 14 Apr 2020 19:03:31 GMT
RUN go get -d ./...
# Tue, 14 Apr 2020 19:03:39 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 14 Apr 2020 19:03:41 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0c66f8509bb56e1ead748baf3433dcad3c1fa170146d5d7d06506b9a80f367`  
		Last Modified: Mon, 23 Mar 2020 23:53:18 GMT  
		Size: 300.6 KB (300602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf5f16b98b20e6e4f07e24e93de1018e88310a49963dc147c370d360a02fdbb`  
		Last Modified: Mon, 23 Mar 2020 23:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a38fd97575c34aedd91676d7643f6dbf66a1bca83f7d010e631807b96dae74`  
		Last Modified: Wed, 08 Apr 2020 23:25:03 GMT  
		Size: 127.8 MB (127774109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61bd435de55167e1a5a8cbdd73838375b819c98df2c23be5991140c00cbfd9a`  
		Last Modified: Wed, 08 Apr 2020 23:24:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a743cd83ba00508dd353a743708e6e434e2f56a1abdc6f2156d953839d646a1`  
		Last Modified: Tue, 14 Apr 2020 19:04:09 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8928c849f33d759a505e159745da8960d19460b8735d7a08631ee817549c57d5`  
		Last Modified: Tue, 14 Apr 2020 19:04:11 GMT  
		Size: 7.0 MB (7010480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe4dbb3884a7fa0c551818da659e9c4d3f97f13eb6d53634655e97f9bd2f0d`  
		Last Modified: Tue, 14 Apr 2020 19:04:10 GMT  
		Size: 2.6 MB (2584042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb4bc7d74da5ae926bd30beea4c4abe59b6c0bb76705fb4f6b83391b591ecd7`  
		Last Modified: Tue, 14 Apr 2020 19:04:53 GMT  
		Size: 176.9 MB (176851243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fb3f4c0251d63ed371fb8a24333c2d9f9dada8830bad6af323550a4276f828`  
		Last Modified: Tue, 14 Apr 2020 19:04:09 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fcea70e4e7db2fed8fb230f66d27fc46446054a0cdc6f6a342235480e7a248`  
		Last Modified: Tue, 14 Apr 2020 19:04:07 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:75a990032363651bf7b39167b9e44e70cb8e6d4ae814545a2274a74005ce8660
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317221628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb140d2ac2499d88e26b91f2219f57edca78ae1597261d9799cb9519bf9f2e24`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:58:12 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 23 Mar 2020 22:58:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Apr 2020 23:11:00 GMT
ENV GOLANG_VERSION=1.14.2
# Wed, 08 Apr 2020 23:13:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 08 Apr 2020 23:13:19 GMT
ENV GOPATH=/go
# Wed, 08 Apr 2020 23:13:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Apr 2020 23:13:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Apr 2020 23:13:22 GMT
WORKDIR /go
# Tue, 14 Apr 2020 19:02:03 GMT
WORKDIR /src
# Tue, 14 Apr 2020 19:02:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 14 Apr 2020 19:02:08 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:02:12 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 14 Apr 2020 19:02:13 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 14 Apr 2020 19:03:13 GMT
RUN go get -d ./...
# Tue, 14 Apr 2020 19:03:15 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 14 Apr 2020 19:03:21 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d4106c43952870e20bfb808275012c22e6244af6eff1e916f446f7d338d0d`  
		Last Modified: Mon, 23 Mar 2020 23:03:34 GMT  
		Size: 301.8 KB (301778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f0a4e33d457336c22ac08eaec4609be330959ccdfefdb342be1045df4d26f0`  
		Last Modified: Mon, 23 Mar 2020 23:03:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44acbbdbf71f1d00fa6d0011bb10b82bef26b421a579bcf3a3491dced9f8233e`  
		Last Modified: Wed, 08 Apr 2020 23:21:31 GMT  
		Size: 126.4 MB (126405787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d054599df8f57e1578fdc2c554a9ac6124bf04f808dc623ef7f6548230fa3b5f`  
		Last Modified: Wed, 08 Apr 2020 23:20:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcee4e573bebbed33479e125fd8abf1f3debd0a7aee2137f55b67d9c38a79be`  
		Last Modified: Tue, 14 Apr 2020 19:03:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968260b321a071a55eb891faac5f738bc2c3340a7843fc9ebd092902475f6fb3`  
		Last Modified: Tue, 14 Apr 2020 19:03:59 GMT  
		Size: 8.4 MB (8353090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f7e47a5a4e440d1d8c40f1b42638e70ea0fbf9b5635f0145f58768993763d6`  
		Last Modified: Tue, 14 Apr 2020 19:03:57 GMT  
		Size: 2.6 MB (2584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e682841e5eb376ed223cc26d628878cb76d53d943e6f205310f7294f212717`  
		Last Modified: Tue, 14 Apr 2020 19:04:33 GMT  
		Size: 176.9 MB (176852681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffdb1a37f36e66ea176ba211db0396ddcf52e5c11bc8c335ad3814c1f091f33`  
		Last Modified: Tue, 14 Apr 2020 19:03:58 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d540e0414cc6a26d9aed38f141af756f0c60e88bb278d4807bda8d6b5939314`  
		Last Modified: Tue, 14 Apr 2020 19:03:57 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
