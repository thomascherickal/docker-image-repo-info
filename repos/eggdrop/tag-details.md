<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.8`](#eggdrop18)
-	[`eggdrop:1.8.4`](#eggdrop184)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.8`

```console
$ docker pull eggdrop@sha256:bf954c76a6b22bafa5a1152045e8320cec873b0adf46bfb885db6bd81d6a4ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:1.8` - linux; amd64

```console
$ docker pull eggdrop@sha256:dc3eb82740c517c499ab8a0e0e6029d31a1355132e054984cd9c9da42631d8c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8786443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da52c01e299f093296afc165d5f00b03e59207ddae8c434f7496b67c1292dce6`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:01:51 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 23 Mar 2020 22:01:52 GMT
RUN adduser -S eggdrop
# Mon, 23 Mar 2020 22:01:54 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 23 Mar 2020 22:03:53 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 23 Mar 2020 22:05:14 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 23 Mar 2020 22:05:15 GMT
ENV NICK=
# Mon, 23 Mar 2020 22:05:15 GMT
ENV SERVER=
# Mon, 23 Mar 2020 22:05:16 GMT
ENV LISTEN=3333
# Mon, 23 Mar 2020 22:05:16 GMT
ENV OWNER=
# Mon, 23 Mar 2020 22:05:16 GMT
ENV USERFILE=eggdrop.user
# Mon, 23 Mar 2020 22:05:17 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 23 Mar 2020 22:05:17 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 23 Mar 2020 22:05:18 GMT
EXPOSE 3333
# Mon, 23 Mar 2020 22:05:18 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Mon, 23 Mar 2020 22:05:19 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 23 Mar 2020 22:05:19 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 23 Mar 2020 22:05:19 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90ac254f3b2092e08d0d1a27fade104236143c7429ad4bfd7a17858c302031`  
		Last Modified: Mon, 23 Mar 2020 22:05:43 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7989bd96822c15f6ae1d0789c29950de5717ef922d3f3f8e284011e9e169c4`  
		Last Modified: Mon, 23 Mar 2020 22:05:41 GMT  
		Size: 9.6 KB (9581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7689126dd51138dc04d8f316f2219b9bb5588d4f9a6b7fb9d19fe9917cfa76e`  
		Last Modified: Mon, 23 Mar 2020 22:05:48 GMT  
		Size: 2.7 MB (2684248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63278b54642d69450022162c6395d8b02367c5b0cc0745d295e8e4165b196c`  
		Last Modified: Mon, 23 Mar 2020 22:05:48 GMT  
		Size: 3.3 MB (3285542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef178bab7af5fea90f56fd61a8ee49c76fb93729d8d4deb48bf776213dc02c1e`  
		Last Modified: Mon, 23 Mar 2020 22:05:47 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb097a7c2750f9c97142d213394ada805c5e33cba328e781699e8303c560664`  
		Last Modified: Mon, 23 Mar 2020 22:05:47 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.8.4`

```console
$ docker pull eggdrop@sha256:bf954c76a6b22bafa5a1152045e8320cec873b0adf46bfb885db6bd81d6a4ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:1.8.4` - linux; amd64

```console
$ docker pull eggdrop@sha256:dc3eb82740c517c499ab8a0e0e6029d31a1355132e054984cd9c9da42631d8c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8786443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da52c01e299f093296afc165d5f00b03e59207ddae8c434f7496b67c1292dce6`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:01:51 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 23 Mar 2020 22:01:52 GMT
RUN adduser -S eggdrop
# Mon, 23 Mar 2020 22:01:54 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 23 Mar 2020 22:03:53 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 23 Mar 2020 22:05:14 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 23 Mar 2020 22:05:15 GMT
ENV NICK=
# Mon, 23 Mar 2020 22:05:15 GMT
ENV SERVER=
# Mon, 23 Mar 2020 22:05:16 GMT
ENV LISTEN=3333
# Mon, 23 Mar 2020 22:05:16 GMT
ENV OWNER=
# Mon, 23 Mar 2020 22:05:16 GMT
ENV USERFILE=eggdrop.user
# Mon, 23 Mar 2020 22:05:17 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 23 Mar 2020 22:05:17 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 23 Mar 2020 22:05:18 GMT
EXPOSE 3333
# Mon, 23 Mar 2020 22:05:18 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Mon, 23 Mar 2020 22:05:19 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 23 Mar 2020 22:05:19 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 23 Mar 2020 22:05:19 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90ac254f3b2092e08d0d1a27fade104236143c7429ad4bfd7a17858c302031`  
		Last Modified: Mon, 23 Mar 2020 22:05:43 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7989bd96822c15f6ae1d0789c29950de5717ef922d3f3f8e284011e9e169c4`  
		Last Modified: Mon, 23 Mar 2020 22:05:41 GMT  
		Size: 9.6 KB (9581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7689126dd51138dc04d8f316f2219b9bb5588d4f9a6b7fb9d19fe9917cfa76e`  
		Last Modified: Mon, 23 Mar 2020 22:05:48 GMT  
		Size: 2.7 MB (2684248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63278b54642d69450022162c6395d8b02367c5b0cc0745d295e8e4165b196c`  
		Last Modified: Mon, 23 Mar 2020 22:05:48 GMT  
		Size: 3.3 MB (3285542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef178bab7af5fea90f56fd61a8ee49c76fb93729d8d4deb48bf776213dc02c1e`  
		Last Modified: Mon, 23 Mar 2020 22:05:47 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb097a7c2750f9c97142d213394ada805c5e33cba328e781699e8303c560664`  
		Last Modified: Mon, 23 Mar 2020 22:05:47 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:2f7afb7baa6fec36c7b2a07f98d310260a90ea884b2cc8f47e999fbcec721a31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:7fc7146740ac23e356324f06c9d6002e06de60bf22cc4224a1d473b1e382faf5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13161878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a4ededa2642b05e7e4f04aefbab25030c5a3d703400cbfb15e11ea0ef12f9f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:01:51 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 23 Mar 2020 22:01:52 GMT
RUN adduser -S eggdrop
# Mon, 23 Mar 2020 22:01:54 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 23 Mar 2020 22:01:55 GMT
ENV EGGDROP_SHA256=12f560ad31e27f1ad631964f6d4ca43e97de6b11c35d4b733a44d21216d83bb4
# Mon, 23 Mar 2020 22:01:55 GMT
ENV EGGDROP_COMMIT=7a490c534fd53af99cbf33a85d907785e9156629
# Mon, 23 Mar 2020 22:01:58 GMT
RUN apk --update add --no-cache tcl bash openssl
# Mon, 23 Mar 2020 22:03:40 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 23 Mar 2020 22:03:41 GMT
ENV NICK=
# Mon, 23 Mar 2020 22:03:41 GMT
ENV SERVER=
# Mon, 23 Mar 2020 22:03:41 GMT
ENV LISTEN=3333
# Mon, 23 Mar 2020 22:03:42 GMT
ENV OWNER=
# Mon, 23 Mar 2020 22:03:42 GMT
ENV USERFILE=eggdrop.user
# Mon, 23 Mar 2020 22:03:42 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 23 Mar 2020 22:03:43 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 23 Mar 2020 22:03:43 GMT
EXPOSE 3333
# Mon, 23 Mar 2020 22:03:44 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Mon, 23 Mar 2020 22:03:44 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 23 Mar 2020 22:03:45 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 23 Mar 2020 22:03:45 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90ac254f3b2092e08d0d1a27fade104236143c7429ad4bfd7a17858c302031`  
		Last Modified: Mon, 23 Mar 2020 22:05:43 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7989bd96822c15f6ae1d0789c29950de5717ef922d3f3f8e284011e9e169c4`  
		Last Modified: Mon, 23 Mar 2020 22:05:41 GMT  
		Size: 9.6 KB (9581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c6f695262d96126f5d8ace179315acdee7e373a1758730524daad3dc571e81`  
		Last Modified: Mon, 23 Mar 2020 22:05:42 GMT  
		Size: 2.7 MB (2684257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660b0b8f894961a00dd343f973f8e3e029cf6cf07e6008a1ab3b99939369b623`  
		Last Modified: Mon, 23 Mar 2020 22:05:43 GMT  
		Size: 7.7 MB (7660959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaeb4a05350a979e38a4258d792a75fbf628d49449be1c3786a6839c4a647f91`  
		Last Modified: Mon, 23 Mar 2020 22:05:41 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbdfc077c3e48e443051bfe7f83a6d15187d16766b62278f09cdb63b71a8dac`  
		Last Modified: Mon, 23 Mar 2020 22:05:41 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:66b70820b405a82c2be740969af6e10e6acda0dcd663f53d38189df4fdbba93c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.8 MB (12845127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb459cffc9df6a6ffa5858548420eccbb14b254d2b8bc988e69d57244d7d0796`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:36:48 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 23 Apr 2020 17:36:52 GMT
RUN adduser -S eggdrop
# Thu, 23 Apr 2020 17:36:54 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 23 Apr 2020 17:36:55 GMT
ENV EGGDROP_SHA256=12f560ad31e27f1ad631964f6d4ca43e97de6b11c35d4b733a44d21216d83bb4
# Thu, 23 Apr 2020 17:36:56 GMT
ENV EGGDROP_COMMIT=7a490c534fd53af99cbf33a85d907785e9156629
# Thu, 23 Apr 2020 17:37:03 GMT
RUN apk --update add --no-cache tcl bash openssl
# Thu, 23 Apr 2020 17:39:04 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 23 Apr 2020 17:39:05 GMT
ENV NICK=
# Thu, 23 Apr 2020 17:39:06 GMT
ENV SERVER=
# Thu, 23 Apr 2020 17:39:07 GMT
ENV LISTEN=3333
# Thu, 23 Apr 2020 17:39:08 GMT
ENV OWNER=
# Thu, 23 Apr 2020 17:39:08 GMT
ENV USERFILE=eggdrop.user
# Thu, 23 Apr 2020 17:39:09 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 23 Apr 2020 17:39:10 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 23 Apr 2020 17:39:10 GMT
EXPOSE 3333
# Thu, 23 Apr 2020 17:39:11 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Thu, 23 Apr 2020 17:39:12 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 23 Apr 2020 17:39:12 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 23 Apr 2020 17:39:13 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f412a5980f526ade995939566f7c342b9adb4c13754922fed8d1798066f9eed`  
		Last Modified: Thu, 23 Apr 2020 17:39:27 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f404049eca1aec0b894cf78c6e968dd2065753284309b55be17f3291c31ad065`  
		Last Modified: Thu, 23 Apr 2020 17:39:24 GMT  
		Size: 9.4 KB (9390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59742158857b1dd535ac41399f7d4394181e53384e9d232920dbd3ea76141c65`  
		Last Modified: Thu, 23 Apr 2020 17:39:25 GMT  
		Size: 2.6 MB (2608162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576b568885b56ef30dc69ec15ad3d84230b828a17b49595a616e12d97f400426`  
		Last Modified: Thu, 23 Apr 2020 17:39:26 GMT  
		Size: 7.6 MB (7603793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0bec210903ad7e7f55610ab22068f322a6c530668ca880b62d975730bbb974`  
		Last Modified: Thu, 23 Apr 2020 17:39:24 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7c734405bebe7061ba5895931c94d0119a538922bfbcc62024ee7abbf21d18`  
		Last Modified: Thu, 23 Apr 2020 17:39:25 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:19a062e171c430e18c2a7da18883cf282d3e108eae061846151d45a97cfd3dd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13146560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b8ac75e27f10a19f9bff9cb474c66e5a4805b942e266343c5788130edef9a42`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:02:28 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 24 Apr 2020 09:02:31 GMT
RUN adduser -S eggdrop
# Fri, 24 Apr 2020 09:02:34 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 24 Apr 2020 09:02:35 GMT
ENV EGGDROP_SHA256=12f560ad31e27f1ad631964f6d4ca43e97de6b11c35d4b733a44d21216d83bb4
# Fri, 24 Apr 2020 09:02:35 GMT
ENV EGGDROP_COMMIT=7a490c534fd53af99cbf33a85d907785e9156629
# Fri, 24 Apr 2020 09:02:38 GMT
RUN apk --update add --no-cache tcl bash openssl
# Fri, 24 Apr 2020 09:04:30 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 24 Apr 2020 09:04:31 GMT
ENV NICK=
# Fri, 24 Apr 2020 09:04:32 GMT
ENV SERVER=
# Fri, 24 Apr 2020 09:04:32 GMT
ENV LISTEN=3333
# Fri, 24 Apr 2020 09:04:33 GMT
ENV OWNER=
# Fri, 24 Apr 2020 09:04:33 GMT
ENV USERFILE=eggdrop.user
# Fri, 24 Apr 2020 09:04:34 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 24 Apr 2020 09:04:35 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 24 Apr 2020 09:04:36 GMT
EXPOSE 3333
# Fri, 24 Apr 2020 09:04:37 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Fri, 24 Apr 2020 09:04:38 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 24 Apr 2020 09:04:39 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 24 Apr 2020 09:04:39 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848a8db5818fe5b735a8e3706dd1ae7043eb3b468306058c8c416fb4770df991`  
		Last Modified: Fri, 24 Apr 2020 09:04:52 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdba78ca0222af81b132121091d817259b1a4e7a7e98379b4dcaec6e64d10a2c`  
		Last Modified: Fri, 24 Apr 2020 09:04:50 GMT  
		Size: 9.5 KB (9514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d804560281d0dbf23c7bd23fa98458db91bbb6c693869808003103582b786277`  
		Last Modified: Fri, 24 Apr 2020 09:04:50 GMT  
		Size: 2.7 MB (2724583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0d48b96a09a7cc968ef409bcf0fe7df290dacce554c7adeca8970a6fb2d11e`  
		Last Modified: Fri, 24 Apr 2020 09:04:52 GMT  
		Size: 7.7 MB (7684186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ea6bfe9c0fbe7c00d411793600eb08805f9f1d89cb82641264cfaded8e6019`  
		Last Modified: Fri, 24 Apr 2020 09:04:50 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d84b56e50f3ffabf6814288073063d35609fe6535cd83947fa39d9456727f2d`  
		Last Modified: Fri, 24 Apr 2020 09:04:50 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:bf954c76a6b22bafa5a1152045e8320cec873b0adf46bfb885db6bd81d6a4ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:dc3eb82740c517c499ab8a0e0e6029d31a1355132e054984cd9c9da42631d8c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8786443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da52c01e299f093296afc165d5f00b03e59207ddae8c434f7496b67c1292dce6`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:01:51 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 23 Mar 2020 22:01:52 GMT
RUN adduser -S eggdrop
# Mon, 23 Mar 2020 22:01:54 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 23 Mar 2020 22:03:53 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 23 Mar 2020 22:05:14 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 23 Mar 2020 22:05:15 GMT
ENV NICK=
# Mon, 23 Mar 2020 22:05:15 GMT
ENV SERVER=
# Mon, 23 Mar 2020 22:05:16 GMT
ENV LISTEN=3333
# Mon, 23 Mar 2020 22:05:16 GMT
ENV OWNER=
# Mon, 23 Mar 2020 22:05:16 GMT
ENV USERFILE=eggdrop.user
# Mon, 23 Mar 2020 22:05:17 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 23 Mar 2020 22:05:17 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 23 Mar 2020 22:05:18 GMT
EXPOSE 3333
# Mon, 23 Mar 2020 22:05:18 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Mon, 23 Mar 2020 22:05:19 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 23 Mar 2020 22:05:19 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 23 Mar 2020 22:05:19 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90ac254f3b2092e08d0d1a27fade104236143c7429ad4bfd7a17858c302031`  
		Last Modified: Mon, 23 Mar 2020 22:05:43 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7989bd96822c15f6ae1d0789c29950de5717ef922d3f3f8e284011e9e169c4`  
		Last Modified: Mon, 23 Mar 2020 22:05:41 GMT  
		Size: 9.6 KB (9581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7689126dd51138dc04d8f316f2219b9bb5588d4f9a6b7fb9d19fe9917cfa76e`  
		Last Modified: Mon, 23 Mar 2020 22:05:48 GMT  
		Size: 2.7 MB (2684248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63278b54642d69450022162c6395d8b02367c5b0cc0745d295e8e4165b196c`  
		Last Modified: Mon, 23 Mar 2020 22:05:48 GMT  
		Size: 3.3 MB (3285542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef178bab7af5fea90f56fd61a8ee49c76fb93729d8d4deb48bf776213dc02c1e`  
		Last Modified: Mon, 23 Mar 2020 22:05:47 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb097a7c2750f9c97142d213394ada805c5e33cba328e781699e8303c560664`  
		Last Modified: Mon, 23 Mar 2020 22:05:47 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:bf954c76a6b22bafa5a1152045e8320cec873b0adf46bfb885db6bd81d6a4ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:dc3eb82740c517c499ab8a0e0e6029d31a1355132e054984cd9c9da42631d8c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8786443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da52c01e299f093296afc165d5f00b03e59207ddae8c434f7496b67c1292dce6`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:01:51 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 23 Mar 2020 22:01:52 GMT
RUN adduser -S eggdrop
# Mon, 23 Mar 2020 22:01:54 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 23 Mar 2020 22:03:53 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 23 Mar 2020 22:05:14 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 23 Mar 2020 22:05:15 GMT
ENV NICK=
# Mon, 23 Mar 2020 22:05:15 GMT
ENV SERVER=
# Mon, 23 Mar 2020 22:05:16 GMT
ENV LISTEN=3333
# Mon, 23 Mar 2020 22:05:16 GMT
ENV OWNER=
# Mon, 23 Mar 2020 22:05:16 GMT
ENV USERFILE=eggdrop.user
# Mon, 23 Mar 2020 22:05:17 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 23 Mar 2020 22:05:17 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 23 Mar 2020 22:05:18 GMT
EXPOSE 3333
# Mon, 23 Mar 2020 22:05:18 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Mon, 23 Mar 2020 22:05:19 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 23 Mar 2020 22:05:19 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 23 Mar 2020 22:05:19 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90ac254f3b2092e08d0d1a27fade104236143c7429ad4bfd7a17858c302031`  
		Last Modified: Mon, 23 Mar 2020 22:05:43 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7989bd96822c15f6ae1d0789c29950de5717ef922d3f3f8e284011e9e169c4`  
		Last Modified: Mon, 23 Mar 2020 22:05:41 GMT  
		Size: 9.6 KB (9581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7689126dd51138dc04d8f316f2219b9bb5588d4f9a6b7fb9d19fe9917cfa76e`  
		Last Modified: Mon, 23 Mar 2020 22:05:48 GMT  
		Size: 2.7 MB (2684248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63278b54642d69450022162c6395d8b02367c5b0cc0745d295e8e4165b196c`  
		Last Modified: Mon, 23 Mar 2020 22:05:48 GMT  
		Size: 3.3 MB (3285542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef178bab7af5fea90f56fd61a8ee49c76fb93729d8d4deb48bf776213dc02c1e`  
		Last Modified: Mon, 23 Mar 2020 22:05:47 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb097a7c2750f9c97142d213394ada805c5e33cba328e781699e8303c560664`  
		Last Modified: Mon, 23 Mar 2020 22:05:47 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
