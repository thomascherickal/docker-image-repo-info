## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:3d3fa240ad1c3ec849d9631e7fbbc729efd735608cab6c514873a3e72fb9cc8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:old-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:c836eca99d41b0fac888807069e2034e9fad902606e5bf6828f0257a0ffa4a0a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.0 MB (57981453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b2e847b262d83e7d67482e0c722043c9ec53e72b0bcf97d96e9cb55fabd802a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 01:09:58 GMT
ENV VARNISH_SIZE=100M
# Sat, 28 Aug 2021 01:10:56 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder
# Sat, 28 Aug 2021 01:10:57 GMT
WORKDIR /etc/varnish
# Sat, 28 Aug 2021 01:10:57 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:10:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 28 Aug 2021 01:10:57 GMT
EXPOSE 80 8443
# Sat, 28 Aug 2021 01:10:57 GMT
CMD []
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73307381f737dcaf50f2a1caf7ecf1bd52ea5d82ac93ebf6b45a793f3250724e`  
		Last Modified: Sat, 28 Aug 2021 01:11:37 GMT  
		Size: 55.2 MB (55166300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e441d0b5149e7dcac33cd5a25d927a5d4aa87a124eac5a1e480286f1035079d5`  
		Last Modified: Sat, 28 Aug 2021 01:11:28 GMT  
		Size: 707.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:b928dbc3d1a010d1d178699979edc9ee736c27dcb3f672574a474ee0ffcfbf67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.8 MB (43821929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3a72c77a04a37463c07f919e5462dab6e94daee21b2b756bc4a4e263201a36`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 03:06:44 GMT
ENV VARNISH_SIZE=100M
# Sat, 28 Aug 2021 03:08:08 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder
# Sat, 28 Aug 2021 03:08:09 GMT
WORKDIR /etc/varnish
# Sat, 28 Aug 2021 03:08:10 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 28 Aug 2021 03:08:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 28 Aug 2021 03:08:11 GMT
EXPOSE 80 8443
# Sat, 28 Aug 2021 03:08:11 GMT
CMD []
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bedc0c14ff50315cd8efd7019e665c1614e1f551ef9fb5c79a36ec3d035eb9d`  
		Last Modified: Sat, 28 Aug 2021 03:09:55 GMT  
		Size: 41.4 MB (41390805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7dbda0db270fb20034aae850a0208cdd35084a2936bde0d637b00898138105`  
		Last Modified: Sat, 28 Aug 2021 03:09:34 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:dcad603946fbdbde3f8091aeadfec59a32593886d2a3677e06ec153999602c0a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50731999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de07c78a7db786b0259191592ee3f133fe14e82e3771b98a2d89ae86740d7a04`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:02:27 GMT
ENV VARNISH_SIZE=100M
# Fri, 12 Nov 2021 18:07:12 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder
# Fri, 12 Nov 2021 18:07:12 GMT
WORKDIR /etc/varnish
# Fri, 12 Nov 2021 18:07:14 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:07:14 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 12 Nov 2021 18:07:15 GMT
EXPOSE 80 8443
# Fri, 12 Nov 2021 18:07:16 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaeddc4ee611ed5f3b3af99a1d64e8a9fe9ac65234c10ae76b8f87c7408ee2c`  
		Last Modified: Fri, 12 Nov 2021 18:12:02 GMT  
		Size: 48.0 MB (48013591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27eb513dedceb393ae14a219dcc10e6ba648d1a3235cffeef2ba2fc580f7733e`  
		Last Modified: Fri, 12 Nov 2021 18:11:55 GMT  
		Size: 708.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; 386

```console
$ docker pull varnish@sha256:6cd7f5496daf8d5cee94d23598c0ca332ec68a0cdc177bc9709b499ceeb281a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58198355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4b96991872090e8a8b3365cb68ba0faacaa135080273c8f4c96827c4e83a85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:27:36 GMT
ENV VARNISH_SIZE=100M
# Fri, 12 Nov 2021 20:31:59 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder
# Fri, 12 Nov 2021 20:31:59 GMT
WORKDIR /etc/varnish
# Fri, 12 Nov 2021 20:32:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:32:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 12 Nov 2021 20:32:01 GMT
EXPOSE 80 8443
# Fri, 12 Nov 2021 20:32:01 GMT
CMD []
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2418aa38a4d46c393e749f3b79218139cf03e08ee533488eef7a184ba3c4b0`  
		Last Modified: Fri, 12 Nov 2021 20:39:20 GMT  
		Size: 55.4 MB (55366703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eafccd51cc8016d5729ab976a08c451c8129732ca52bd56dad9a9d33029d19`  
		Last Modified: Fri, 12 Nov 2021 20:39:03 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:6acae0005f713fdebb0f8978979ddaa9710c703bf78ca8a1346362537261beac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47827216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a98ef55c0208b4c19e62c8aaca8f48f0e40cb2a27a2f48965304e018e62e72d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:39:41 GMT
ENV VARNISH_SIZE=100M
# Fri, 27 Aug 2021 21:40:57 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder
# Fri, 27 Aug 2021 21:41:05 GMT
WORKDIR /etc/varnish
# Fri, 27 Aug 2021 21:41:14 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:41:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 27 Aug 2021 21:41:28 GMT
EXPOSE 80 8443
# Fri, 27 Aug 2021 21:41:32 GMT
CMD []
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1cce8ddb158771014efb6bfda04a9e011ec4eca09dd63aa238dfcf1745e95`  
		Last Modified: Fri, 27 Aug 2021 21:42:36 GMT  
		Size: 45.0 MB (45014227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a30231e814f5d55431f1d2070b9a122bd255affd874c0dcf0827584ab4b155`  
		Last Modified: Fri, 27 Aug 2021 21:42:28 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:fcc4bca2790bf7ba56c26d5b5118596cd41f74644ea85441859745432fc73e1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46361978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6882dde469444e5fb43eaa831dcc307116623b9d2084b5d35519f728dd85e722`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 18:51:05 GMT
ENV VARNISH_SIZE=100M
# Fri, 27 Aug 2021 18:52:13 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder
# Fri, 27 Aug 2021 18:52:16 GMT
WORKDIR /etc/varnish
# Fri, 27 Aug 2021 18:52:16 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 27 Aug 2021 18:52:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 27 Aug 2021 18:52:17 GMT
EXPOSE 80 8443
# Fri, 27 Aug 2021 18:52:18 GMT
CMD []
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfb6ce7ffb175da94d141b4c6a2b77e8bfd9556fd37f1ef7ce3e2fcf659b63f`  
		Last Modified: Fri, 27 Aug 2021 18:53:08 GMT  
		Size: 43.8 MB (43757809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c267bd4c5f2946f3abee446ee4bd8473ddfb8d4c009f45fd510ab9152426702`  
		Last Modified: Fri, 27 Aug 2021 18:53:02 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
