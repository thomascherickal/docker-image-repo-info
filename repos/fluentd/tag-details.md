<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.16-1`](#fluentdv116-1)
-	[`fluentd:v1.16-debian-1`](#fluentdv116-debian-1)
-	[`fluentd:v1.16.0-1.0`](#fluentdv1160-10)
-	[`fluentd:v1.16.0-debian-1.0`](#fluentdv1160-debian-10)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:07b5c85e4e1fcc138f8b027e6bf5b5f213c413cef90f18d82d5163920780a2d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:latest` - linux; amd64

```console
$ docker pull fluentd@sha256:352d55d2078fbfc9a937d0363b5bbd534c8beb697a50e83bf22bf0a10aa2b3f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25140944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b8e09ecb2b9be644f07766135ac88f79f14da7d166ffb26973b1b4bc860841a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:21:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:21:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:22:02 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:22:03 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:22:03 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:22:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:22:03 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:22:03 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:22:04 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:22:04 GMT
USER fluent
# Tue, 04 Apr 2023 00:22:04 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:22:04 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa07d670c0f5933d60efc971af846c6ae888f4e23b0327e32b12994d37743654`  
		Last Modified: Tue, 04 Apr 2023 00:25:10 GMT  
		Size: 21.8 MB (21764169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f602c3750d1aecc6c4a586ef442a773b8f7760ba57e7f79264ed14cdf8d4ed`  
		Last Modified: Tue, 04 Apr 2023 00:25:07 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2498f159ecfc088f6f02d163dfb8b047290b30ac5fcd8311bc17afe8d824bd9a`  
		Last Modified: Tue, 04 Apr 2023 00:25:07 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0461207db4ddd97bbc8a0b68c25efcc5e97fd9f3f43ef59e42b8732b7365c492`  
		Last Modified: Tue, 04 Apr 2023 00:25:07 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:65d2a7a2677137edd41e9d5c64ff89acfc281743d7ef32412c813534067daa2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23810626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3c8433a0c3f42b76c1509792a291d63f86697031c4f1d8a3b5f7559d859cf7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:06:39 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:06:39 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:07:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:07:40 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:07:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:07:40 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:07:40 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:07:40 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:07:40 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:07:40 GMT
USER fluent
# Tue, 04 Apr 2023 00:07:40 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:07:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ba6d6f8ecfc29753c59b0ba643012ce6907ab381fb451d451a93c0c17012e6`  
		Last Modified: Tue, 04 Apr 2023 00:07:57 GMT  
		Size: 20.7 MB (20697612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf6c016ad72c78a88d7b7b26a7cf1d74fd021da7b18ad6459839400bb684668`  
		Last Modified: Tue, 04 Apr 2023 00:07:53 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63640f7ce6faef8e9f6a1c2363709bccc7380527b37269499ed9c29c0bba312`  
		Last Modified: Tue, 04 Apr 2023 00:07:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1774ae06f6540f8048b494472e2863501a9defbb42df777d641b26195c23f1`  
		Last Modified: Tue, 04 Apr 2023 00:07:53 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:bf838b9ced09ce9d892ecdf02d5ab79237747f87b71608ad612f255122fed97b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457e56584ffa420563004b6e6d532a222271b0f5a7e463616f31c3527370d232`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:32:28 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:32:28 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:33:16 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:33:16 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:33:16 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:33:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:33:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:33:17 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:33:17 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:33:17 GMT
USER fluent
# Tue, 04 Apr 2023 00:33:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:33:17 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bda3a270166f2a977c0884235cad5b8f021f8db56ea9b2c432cecf74329247`  
		Last Modified: Tue, 04 Apr 2023 00:35:57 GMT  
		Size: 21.3 MB (21342740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a16a4585660946e7720147d598a27d843c96abfa610a11201d6f8257800cc14`  
		Last Modified: Tue, 04 Apr 2023 00:35:55 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785af8e229db635092bdcbafbaf0b44b685a6074f64e0cda523b636f08538b39`  
		Last Modified: Tue, 04 Apr 2023 00:35:55 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b6783ed8e3a73fe1cb5dbcc5c8cc6248c5860c1cc4eb302f2107d3f78ab34`  
		Last Modified: Tue, 04 Apr 2023 00:35:55 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; 386

```console
$ docker pull fluentd@sha256:76b60221ded7a71376bb5b26e375615cc729d01cd0ff46c17465a4773534db1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24411093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cea1608e07e2659c0aca6e680315bc4e5c3508f9b3f8a5a7156a3aafca641eee`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 01:16:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 01:16:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 01:17:55 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 01:17:56 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 01:17:56 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 01:17:56 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 01:17:56 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 01:17:56 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 01:17:57 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 01:17:57 GMT
USER fluent
# Tue, 04 Apr 2023 01:17:57 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 01:17:57 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed08b8285ffd56e96393c2dff4fb2ce0a3c27a92394d54abf1c1716421e804`  
		Last Modified: Tue, 04 Apr 2023 01:21:21 GMT  
		Size: 21.0 MB (20996620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959325317237f318931715bd2bbd656167fabf07670987717972e64a0da60bad`  
		Last Modified: Tue, 04 Apr 2023 01:21:17 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa24e173dae39c3ecdd5bdbbc010db1cfcdee84d3a01c48a43e776cf6f798150`  
		Last Modified: Tue, 04 Apr 2023 01:21:17 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2429838a83f4ef0f0d1e7dad9771de9b7febd4ee886354d14035325fff0a958e`  
		Last Modified: Tue, 04 Apr 2023 01:21:17 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:01a35c95635804feaa927be6ddd8d50f27da355ffec4b0be26e632577dcc5f52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (24990680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f68fc5f2ab5d0b4cc08684d231004414d406a6428929fdf914b10bd9a271a59`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:41:15 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:41:17 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:43:10 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:43:13 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:43:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:43:14 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:43:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:43:15 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:43:16 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:43:17 GMT
USER fluent
# Tue, 04 Apr 2023 00:43:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:43:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e5d552a1c089c6d62019d6363c52cc538432e91dff873e1b88f559a5bc8d56`  
		Last Modified: Tue, 04 Apr 2023 00:50:04 GMT  
		Size: 21.6 MB (21597531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4846e34c153455ca303d93be3b6891184cdf81fdb542be2ddf33936434a18a`  
		Last Modified: Tue, 04 Apr 2023 00:49:58 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc4f08d35e6fa7282eb71c46f2a983dc42b8f3ac3b10f1dc5d8aad8fb8cc70f`  
		Last Modified: Tue, 04 Apr 2023 00:49:58 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27735545a7315c8e8a081426bd355599eb0a3828750063e75a4a6385655d61a`  
		Last Modified: Tue, 04 Apr 2023 00:49:58 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:de41a2a9ccf81ba76fcafddb31dba48fb8e46294d150fa18cdd3cbdd796cacf1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 MB (24345941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93a9225e2eb720e3696ed7db8406b7622174b761b5ffd91d252174b0a7f5ca63`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Fri, 05 May 2023 00:36:09 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 05 May 2023 00:36:09 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Fri, 05 May 2023 00:36:56 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 05 May 2023 00:36:58 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 05 May 2023 00:36:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 05 May 2023 00:36:58 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 05 May 2023 00:36:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 05 May 2023 00:36:59 GMT
ENV LD_PRELOAD=
# Fri, 05 May 2023 00:36:59 GMT
EXPOSE 24224 5140
# Fri, 05 May 2023 00:36:59 GMT
USER fluent
# Fri, 05 May 2023 00:36:59 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 05 May 2023 00:36:59 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dfcaf3da0dcc5db8c5ab1ecfbb8d021d0486173a5fe8813c727ac8cd06805e`  
		Last Modified: Fri, 05 May 2023 00:39:34 GMT  
		Size: 21.2 MB (21168543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0efbe4644268746c3e1eff581e0ccc2b2b689ff0a2cd774719c7faf5e08ccf`  
		Last Modified: Fri, 05 May 2023 00:39:31 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0020f048480ef88a5b12c1f92ec54ccd07a5257a66d36780e045ebca4efdae9d`  
		Last Modified: Fri, 05 May 2023 00:39:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a2a4da469cac674fce9f8503512acb9c265a5e72f69785a38f3dcd83bb8b84`  
		Last Modified: Fri, 05 May 2023 00:39:31 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16-1`

```console
$ docker pull fluentd@sha256:07b5c85e4e1fcc138f8b027e6bf5b5f213c413cef90f18d82d5163920780a2d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.16-1` - linux; amd64

```console
$ docker pull fluentd@sha256:352d55d2078fbfc9a937d0363b5bbd534c8beb697a50e83bf22bf0a10aa2b3f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25140944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b8e09ecb2b9be644f07766135ac88f79f14da7d166ffb26973b1b4bc860841a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:21:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:21:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:22:02 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:22:03 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:22:03 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:22:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:22:03 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:22:03 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:22:04 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:22:04 GMT
USER fluent
# Tue, 04 Apr 2023 00:22:04 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:22:04 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa07d670c0f5933d60efc971af846c6ae888f4e23b0327e32b12994d37743654`  
		Last Modified: Tue, 04 Apr 2023 00:25:10 GMT  
		Size: 21.8 MB (21764169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f602c3750d1aecc6c4a586ef442a773b8f7760ba57e7f79264ed14cdf8d4ed`  
		Last Modified: Tue, 04 Apr 2023 00:25:07 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2498f159ecfc088f6f02d163dfb8b047290b30ac5fcd8311bc17afe8d824bd9a`  
		Last Modified: Tue, 04 Apr 2023 00:25:07 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0461207db4ddd97bbc8a0b68c25efcc5e97fd9f3f43ef59e42b8732b7365c492`  
		Last Modified: Tue, 04 Apr 2023 00:25:07 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:65d2a7a2677137edd41e9d5c64ff89acfc281743d7ef32412c813534067daa2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23810626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3c8433a0c3f42b76c1509792a291d63f86697031c4f1d8a3b5f7559d859cf7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:06:39 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:06:39 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:07:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:07:40 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:07:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:07:40 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:07:40 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:07:40 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:07:40 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:07:40 GMT
USER fluent
# Tue, 04 Apr 2023 00:07:40 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:07:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ba6d6f8ecfc29753c59b0ba643012ce6907ab381fb451d451a93c0c17012e6`  
		Last Modified: Tue, 04 Apr 2023 00:07:57 GMT  
		Size: 20.7 MB (20697612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf6c016ad72c78a88d7b7b26a7cf1d74fd021da7b18ad6459839400bb684668`  
		Last Modified: Tue, 04 Apr 2023 00:07:53 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63640f7ce6faef8e9f6a1c2363709bccc7380527b37269499ed9c29c0bba312`  
		Last Modified: Tue, 04 Apr 2023 00:07:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1774ae06f6540f8048b494472e2863501a9defbb42df777d641b26195c23f1`  
		Last Modified: Tue, 04 Apr 2023 00:07:53 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:bf838b9ced09ce9d892ecdf02d5ab79237747f87b71608ad612f255122fed97b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457e56584ffa420563004b6e6d532a222271b0f5a7e463616f31c3527370d232`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:32:28 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:32:28 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:33:16 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:33:16 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:33:16 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:33:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:33:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:33:17 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:33:17 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:33:17 GMT
USER fluent
# Tue, 04 Apr 2023 00:33:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:33:17 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bda3a270166f2a977c0884235cad5b8f021f8db56ea9b2c432cecf74329247`  
		Last Modified: Tue, 04 Apr 2023 00:35:57 GMT  
		Size: 21.3 MB (21342740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a16a4585660946e7720147d598a27d843c96abfa610a11201d6f8257800cc14`  
		Last Modified: Tue, 04 Apr 2023 00:35:55 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785af8e229db635092bdcbafbaf0b44b685a6074f64e0cda523b636f08538b39`  
		Last Modified: Tue, 04 Apr 2023 00:35:55 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b6783ed8e3a73fe1cb5dbcc5c8cc6248c5860c1cc4eb302f2107d3f78ab34`  
		Last Modified: Tue, 04 Apr 2023 00:35:55 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; 386

```console
$ docker pull fluentd@sha256:76b60221ded7a71376bb5b26e375615cc729d01cd0ff46c17465a4773534db1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24411093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cea1608e07e2659c0aca6e680315bc4e5c3508f9b3f8a5a7156a3aafca641eee`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 01:16:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 01:16:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 01:17:55 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 01:17:56 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 01:17:56 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 01:17:56 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 01:17:56 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 01:17:56 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 01:17:57 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 01:17:57 GMT
USER fluent
# Tue, 04 Apr 2023 01:17:57 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 01:17:57 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed08b8285ffd56e96393c2dff4fb2ce0a3c27a92394d54abf1c1716421e804`  
		Last Modified: Tue, 04 Apr 2023 01:21:21 GMT  
		Size: 21.0 MB (20996620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959325317237f318931715bd2bbd656167fabf07670987717972e64a0da60bad`  
		Last Modified: Tue, 04 Apr 2023 01:21:17 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa24e173dae39c3ecdd5bdbbc010db1cfcdee84d3a01c48a43e776cf6f798150`  
		Last Modified: Tue, 04 Apr 2023 01:21:17 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2429838a83f4ef0f0d1e7dad9771de9b7febd4ee886354d14035325fff0a958e`  
		Last Modified: Tue, 04 Apr 2023 01:21:17 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:01a35c95635804feaa927be6ddd8d50f27da355ffec4b0be26e632577dcc5f52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (24990680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f68fc5f2ab5d0b4cc08684d231004414d406a6428929fdf914b10bd9a271a59`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:41:15 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:41:17 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:43:10 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:43:13 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:43:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:43:14 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:43:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:43:15 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:43:16 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:43:17 GMT
USER fluent
# Tue, 04 Apr 2023 00:43:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:43:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e5d552a1c089c6d62019d6363c52cc538432e91dff873e1b88f559a5bc8d56`  
		Last Modified: Tue, 04 Apr 2023 00:50:04 GMT  
		Size: 21.6 MB (21597531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4846e34c153455ca303d93be3b6891184cdf81fdb542be2ddf33936434a18a`  
		Last Modified: Tue, 04 Apr 2023 00:49:58 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc4f08d35e6fa7282eb71c46f2a983dc42b8f3ac3b10f1dc5d8aad8fb8cc70f`  
		Last Modified: Tue, 04 Apr 2023 00:49:58 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27735545a7315c8e8a081426bd355599eb0a3828750063e75a4a6385655d61a`  
		Last Modified: Tue, 04 Apr 2023 00:49:58 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; s390x

```console
$ docker pull fluentd@sha256:de41a2a9ccf81ba76fcafddb31dba48fb8e46294d150fa18cdd3cbdd796cacf1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 MB (24345941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93a9225e2eb720e3696ed7db8406b7622174b761b5ffd91d252174b0a7f5ca63`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Fri, 05 May 2023 00:36:09 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 05 May 2023 00:36:09 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Fri, 05 May 2023 00:36:56 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 05 May 2023 00:36:58 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 05 May 2023 00:36:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 05 May 2023 00:36:58 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 05 May 2023 00:36:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 05 May 2023 00:36:59 GMT
ENV LD_PRELOAD=
# Fri, 05 May 2023 00:36:59 GMT
EXPOSE 24224 5140
# Fri, 05 May 2023 00:36:59 GMT
USER fluent
# Fri, 05 May 2023 00:36:59 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 05 May 2023 00:36:59 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dfcaf3da0dcc5db8c5ab1ecfbb8d021d0486173a5fe8813c727ac8cd06805e`  
		Last Modified: Fri, 05 May 2023 00:39:34 GMT  
		Size: 21.2 MB (21168543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0efbe4644268746c3e1eff581e0ccc2b2b689ff0a2cd774719c7faf5e08ccf`  
		Last Modified: Fri, 05 May 2023 00:39:31 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0020f048480ef88a5b12c1f92ec54ccd07a5257a66d36780e045ebca4efdae9d`  
		Last Modified: Fri, 05 May 2023 00:39:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a2a4da469cac674fce9f8503512acb9c265a5e72f69785a38f3dcd83bb8b84`  
		Last Modified: Fri, 05 May 2023 00:39:31 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16-debian-1`

```console
$ docker pull fluentd@sha256:c0743231e9fcf61d2395a01d8bda7bca381b90453216cdf86c282f5a957ba5c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.16-debian-1` - linux; amd64

```console
$ docker pull fluentd@sha256:34798804af5d79350cad454af9f27dda2369e900c479d6987986a7cc5101cff5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101764787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee5d396ffe5f6dea71870bf918f87a30130ff1729b382aea2ff0e311860ecdf3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 11:28:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 11:28:53 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 11:28:53 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 11:49:26 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 11:49:26 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 11:49:26 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 11:51:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 11:51:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 11:51:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 11:51:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 11:51:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 11:51:42 GMT
CMD ["irb"]
# Tue, 23 May 2023 23:43:57 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 23:43:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 23:43:57 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 23:46:33 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 23:46:34 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 23:46:34 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 23:46:35 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 23:46:35 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 23:46:35 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 23:46:35 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 23:46:35 GMT
USER fluent
# Tue, 23 May 2023 23:46:35 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 23:46:35 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a1dfbc0e3c1cddb150865089039a9023dbac788fdf37a4f698b2a242393430`  
		Last Modified: Tue, 23 May 2023 12:05:53 GMT  
		Size: 10.0 MB (10023269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50db7b862053780f8046cd4090d0b17584a13013d7dce8ad4f404734fd1c902a`  
		Last Modified: Tue, 23 May 2023 12:05:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0cec51f183aef280729ae039fa4e76e7eb84c3eef57e59e073f51470ab6c8f`  
		Last Modified: Tue, 23 May 2023 12:08:13 GMT  
		Size: 32.6 MB (32626024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b934eff42c9311bb8b61df5e4cfdc6d3210b09e3b1cbd5dfea875ec41fddd033`  
		Last Modified: Tue, 23 May 2023 12:08:10 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e5b6e03ed07a5e851383b675b3e863b5bb8cf1032eb4c348a7ee0b8cbf9ce1`  
		Last Modified: Tue, 23 May 2023 23:47:01 GMT  
		Size: 27.7 MB (27708820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f378cfcc3cb686b089cd08f7ec8c1acc4664cf1eb836e091769da88cf30737f`  
		Last Modified: Tue, 23 May 2023 23:46:57 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa6a5baf0d72ab3054bd949c716387dc8c0cb115f29925dfe17b7b6bebe3df`  
		Last Modified: Tue, 23 May 2023 23:46:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3074318e81de9867f633281b8c19e19f618a08c6d7807d90ac881bfd132ca4cb`  
		Last Modified: Tue, 23 May 2023 23:46:57 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:63a2cd55488c0416aa72cee3153d084f85a4e87619a19c5d9ae2b417ed09b99f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95253139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40ea4a5e6c1bf2ff09459c744fdc5027a754681f609b198ab460ded663adc43a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 00:48:41 GMT
ADD file:868f634f5ddb80ed9e9c719ccaf5d564d96fe819f0b000ecc734311baf5da99b in / 
# Tue, 23 May 2023 00:48:42 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:43:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:43:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 07:43:58 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 07:53:32 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 07:53:32 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 07:53:32 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 07:56:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 07:56:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 07:56:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 07:56:00 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 07:56:01 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 07:56:01 GMT
CMD ["irb"]
# Tue, 23 May 2023 14:06:42 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 14:06:42 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 14:06:42 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 14:09:37 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 14:09:38 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 14:09:38 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 14:09:38 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 14:09:38 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 14:09:38 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 14:09:38 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 14:09:38 GMT
USER fluent
# Tue, 23 May 2023 14:09:38 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 14:09:38 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:812967ccba449e7a96044b2d48ffc62816b22eb17641844c4dfffbe3b3ec6f21`  
		Last Modified: Tue, 23 May 2023 00:51:19 GMT  
		Size: 28.9 MB (28903411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be04097d1ded9335b3db9447099711ba6b7e06110590c1dce452f7bfbde88a6b`  
		Last Modified: Tue, 23 May 2023 08:01:48 GMT  
		Size: 8.6 MB (8634451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22a934b77fc215fc18ccde8e1d1820798abb4b25ed01191b3bb3c4815f31168`  
		Last Modified: Tue, 23 May 2023 08:01:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e558fe7b0b7f0c483952f729a9b4538079f921461ee708c55b103cf7712078c2`  
		Last Modified: Tue, 23 May 2023 08:03:08 GMT  
		Size: 31.2 MB (31165902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09bd2353f05cb293e4149ffe41c6f17410af979ed625452c1d65ea76df4a388`  
		Last Modified: Tue, 23 May 2023 08:03:05 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3579ba85a1ea2ab414bbc750307485a987a0a31d9140c83e8a4049e7aae54981`  
		Last Modified: Tue, 23 May 2023 14:10:00 GMT  
		Size: 26.5 MB (26546298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64760944e08c577d65da8d66f3491bffb96e30c7f9161c0c64ef07dafc09577`  
		Last Modified: Tue, 23 May 2023 14:09:55 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a24442b206e924e60c0c853e69b3f4da5b0f0c7bddada10dc694e24e39f0c6`  
		Last Modified: Tue, 23 May 2023 14:09:55 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94632d40ef4f818499a20ad7ae500da0eace49dcc1d209c4b92d497490da9e60`  
		Last Modified: Tue, 23 May 2023 14:09:55 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:58af03c16b82949f0a46261c3d9deff04a9fb2fd827a03523a998f9cfc20dd07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92129948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9e3d97872d6a319f78d975f6b9ca01bb0dbea6e6575c4f0b4834c7c87def11`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:30:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:30:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 05:30:28 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 05:40:42 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 05:40:42 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 05:40:42 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 05:42:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 05:42:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 05:42:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 05:42:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 05:42:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 05:42:46 GMT
CMD ["irb"]
# Tue, 23 May 2023 11:21:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 11:21:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 11:21:54 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 11:24:45 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 11:24:45 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 11:24:45 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 11:24:46 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 11:24:46 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 11:24:46 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 11:24:46 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 11:24:46 GMT
USER fluent
# Tue, 23 May 2023 11:24:46 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 11:24:46 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb6a09bcc5c0984ecb3a04b714caca1098f621d70de5fb59d22fc016d46ffae`  
		Last Modified: Tue, 23 May 2023 05:50:53 GMT  
		Size: 8.1 MB (8143926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca2368c379d00172553a3637b0c56b1cdb714a97b92bb40f910b023e9ac82c3`  
		Last Modified: Tue, 23 May 2023 05:50:51 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78962edc36f5ff06f5957f41aec3bc1dafd3618cb6e13c99ec2b9d672ce2d46`  
		Last Modified: Tue, 23 May 2023 05:52:01 GMT  
		Size: 31.0 MB (31035229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5cd2c80a56fed84af20ba9be79ed5dac3e9a1b6e1836258be0c336c9a5d6c2`  
		Last Modified: Tue, 23 May 2023 05:51:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da01f5f14b76cd026a041d821586399ee1d001069ecee5d3b094ff4d3edeab11`  
		Last Modified: Tue, 23 May 2023 11:25:10 GMT  
		Size: 26.4 MB (26383084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c77433b38e451ecdd7e9b29de43727689fa84bca8f4dacc28b31cc6a86d3fb`  
		Last Modified: Tue, 23 May 2023 11:25:05 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997fc11b9f431e3b81cee260d095c9e0494c99d1346c1aa2d58f406637dcd08`  
		Last Modified: Tue, 23 May 2023 11:25:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b271058e601b3a5ac882e8f5feb99a66fd16e41a2cfe1d9048231084c202027`  
		Last Modified: Tue, 23 May 2023 11:25:05 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:8dd6b2dde2fd86cde3f161e972c179295c5b2fbdbe0aac1b27843650d6c0f8f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.7 MB (98742575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99424dea3591c74df4dfe8d8c0eee56d1f2f74dcaeb8fb5082ca80d74a3a64a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:17:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:17:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 06:17:13 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 06:33:27 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 06:33:27 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 06:33:27 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 06:35:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 06:35:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 06:35:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 06:35:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:35:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 06:35:17 GMT
CMD ["irb"]
# Tue, 23 May 2023 19:38:49 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 19:38:49 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 19:38:49 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 19:41:09 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 19:41:10 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 19:41:10 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 19:41:10 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 19:41:10 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 19:41:11 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 19:41:11 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 19:41:11 GMT
USER fluent
# Tue, 23 May 2023 19:41:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 19:41:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c44207aeb95c5c97b69601e7ecf6205b0018dc481f58c8d1c35c7e9f1ce3d6e`  
		Last Modified: Tue, 23 May 2023 06:46:42 GMT  
		Size: 9.2 MB (9243477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68b42fcab4b6e0ed16656636285da203ba16863eff8f005def15c873988b921`  
		Last Modified: Tue, 23 May 2023 06:46:41 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f6677e34939ef3d61f952f03eb1fd89bde1a1894e28bddeaa6bab4abcd7015`  
		Last Modified: Tue, 23 May 2023 06:48:53 GMT  
		Size: 32.0 MB (31987287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d18bebe0e6b2814ed86e3b712f39ca4b5fc012cb4753e109949603be9cfe78b`  
		Last Modified: Tue, 23 May 2023 06:48:51 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bc4d360fc0448da1de6b1d389ffe87a5440380e673469cbeaee92effa67c1e`  
		Last Modified: Tue, 23 May 2023 19:41:36 GMT  
		Size: 27.5 MB (27455976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fb3bef85d57b3b7fc3bf58c8ab88e60904d62a5075a1618ab6668e4694e1bc`  
		Last Modified: Tue, 23 May 2023 19:41:33 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98157824256abbfd44628fb3ba45aeb0f930b7c20ae756781a4b0240f05c802`  
		Last Modified: Tue, 23 May 2023 19:41:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65de085db6e9276f33e5df470cbbb4664e6493dccb70a7d434c08fea4e43125`  
		Last Modified: Tue, 23 May 2023 19:41:33 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:d9a49fa00e22b0b02e6554fea3bf2dce9cfd94570333040c7d3c9a0e1de85702
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102148831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb6733d8f9d1c7791d728734fd6250fb09415e834aaa1f0529988b8257e71c3a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:12:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:12:04 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 01:12:04 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 01:28:03 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 01:28:03 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 01:28:03 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 01:31:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 01:31:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 01:31:40 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 01:31:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:31:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 01:31:40 GMT
CMD ["irb"]
# Tue, 23 May 2023 20:03:34 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 20:03:34 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 20:03:34 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 20:06:31 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 20:06:32 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 20:06:32 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 20:06:32 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 20:06:32 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 20:06:32 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 20:06:32 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 20:06:32 GMT
USER fluent
# Tue, 23 May 2023 20:06:32 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 20:06:32 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e573e66fa2cd19b7052169187d24733be9d6d250dc8898046d0fea6cd049d`  
		Last Modified: Tue, 23 May 2023 01:43:19 GMT  
		Size: 12.0 MB (11997370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35afa18cbcba46f8516124b77bcc5ade8c55162dc60d023b4302c72e9cb40e08`  
		Last Modified: Tue, 23 May 2023 01:43:15 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35da886c11b3e44726a8d010f5314900641263fd2ee12d332bd3587940af7bb`  
		Last Modified: Tue, 23 May 2023 01:44:35 GMT  
		Size: 31.2 MB (31181783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8906d58f8e100a1cc314b06760b6084baa703ad4692de9f4421a955bca26d235`  
		Last Modified: Tue, 23 May 2023 01:44:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02699f810fccd7455168170e0f4e316ac6e4a600e5440319be02c45acc25ae48`  
		Last Modified: Tue, 23 May 2023 20:06:55 GMT  
		Size: 26.6 MB (26578433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b626fbc5cd4378136253cad9db380b06f5cb2572cdd57e2dbf071a8166357b09`  
		Last Modified: Tue, 23 May 2023 20:06:50 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d778ffbe1a34d2f0053abfe3e33a055f3952301dab1cd8e8281d20a1a2eff3d1`  
		Last Modified: Tue, 23 May 2023 20:06:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4da0f4b1f77486a59eaba18767fbccb83baab50337c5bed3eb73309018756c5`  
		Last Modified: Tue, 23 May 2023 20:06:50 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:3c24325053f32db3e85a1d6105e77459e247939442d4fd68f56e50e7df2131db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106748156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af62282a59b9815935eb5e0c85cdc13d73179b68796b1933d4d270e16c58b9c4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:23:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:23:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 02:23:32 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 02:40:17 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 02:40:18 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 02:40:18 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 02:44:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 02:44:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 02:44:20 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 02:44:20 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:44:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 02:44:22 GMT
CMD ["irb"]
# Tue, 23 May 2023 18:22:20 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 18:22:20 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 18:22:21 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 18:27:29 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 18:27:32 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 18:27:32 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 18:27:32 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 18:27:32 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 18:27:33 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 18:27:33 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 18:27:33 GMT
USER fluent
# Tue, 23 May 2023 18:27:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 18:27:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d38ba339ef6043fdfe3ddd5359c69fcf0314d3e805835066f25f5bdec81cbaa`  
		Last Modified: Tue, 23 May 2023 02:52:45 GMT  
		Size: 10.5 MB (10481258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6686de7ce20c5bf6829105ad713ada3bd60313789b594e248ffe5250dc1b159f`  
		Last Modified: Tue, 23 May 2023 02:52:42 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4951bfecfe434f2065bfa58d65d30fcd4683531c9458244fa962c03cc48cd61e`  
		Last Modified: Tue, 23 May 2023 02:54:21 GMT  
		Size: 32.8 MB (32791406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6822a4153fffa9635a3af305ce435ccee23f1029d7a694a724a74fd392835a95`  
		Last Modified: Tue, 23 May 2023 02:54:16 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71abde10f8f427c3aa332fb8212f0a26a02db5ac37458cc5a9ba0085644aa4c9`  
		Last Modified: Tue, 23 May 2023 18:28:00 GMT  
		Size: 28.2 MB (28191497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa549617805f59c555997200a428c14171b483b7a14983074b92d593038156ca`  
		Last Modified: Tue, 23 May 2023 18:27:53 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55be1358fafcaa95f4eaedea36011475dc6544349a637f879a9fd96586a5e5`  
		Last Modified: Tue, 23 May 2023 18:27:53 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e960237bd065aef85488dbfbf179b82c7415c294827b0dc9bf255d72859ad4b4`  
		Last Modified: Tue, 23 May 2023 18:27:53 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:280474dd7d723a6e0f3f613447ed6dc5d9a9a19c6191213159239b9692168005
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98885605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:412413267f439d94cc9e69a7cf29468703d666de437d6ac2b3c46b0858cc6b1f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:16:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:16:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 02:16:13 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 02:20:52 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 02:20:52 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 02:20:52 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 02:22:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 02:22:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 02:22:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 02:22:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:22:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 02:22:51 GMT
CMD ["irb"]
# Tue, 23 May 2023 07:34:18 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 07:34:18 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 07:34:19 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 07:36:34 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 07:36:42 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 07:36:42 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 07:36:42 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 07:36:43 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 07:36:43 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 07:36:44 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 07:36:44 GMT
USER fluent
# Tue, 23 May 2023 07:36:44 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 07:36:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389e5acb5f585dd7876222f795a0f8adb45bbb36dfee1707ad06ef3c32abe06a`  
		Last Modified: Tue, 23 May 2023 02:25:49 GMT  
		Size: 8.9 MB (8864321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f41881192359d6eae65c1dea80a1676401b472e6565797e2c8a05658dbfc19`  
		Last Modified: Tue, 23 May 2023 02:25:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024533d1e28fb42ceec653648bb53ba0eec8a926cca2b4c37f7b9b789b7af370`  
		Last Modified: Tue, 23 May 2023 02:26:18 GMT  
		Size: 32.4 MB (32444939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b5d84dde0b278d9f070f6f6be97cb4cd0dd9049cae6b5db6e105f3c27889b4`  
		Last Modified: Tue, 23 May 2023 02:26:15 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46cdab6f14951c66d27711ad392574c46660f5f49c9267fe884221e566afb3b`  
		Last Modified: Tue, 23 May 2023 07:37:05 GMT  
		Size: 27.9 MB (27931089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c787127535fef7623fff56414b4142dc7fd48019892f9b13bb318811bb59fb80`  
		Last Modified: Tue, 23 May 2023 07:37:01 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa09eece0a3b6c953dbbff800b217a3fea7d92bf76fee667b8e7975dd65167e`  
		Last Modified: Tue, 23 May 2023 07:37:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd69db2a81327365cce1daf3c24f1e16505dec378db47cff7c6cea2ad3b8950`  
		Last Modified: Tue, 23 May 2023 07:37:01 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16.0-1.0`

```console
$ docker pull fluentd@sha256:07b5c85e4e1fcc138f8b027e6bf5b5f213c413cef90f18d82d5163920780a2d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.16.0-1.0` - linux; amd64

```console
$ docker pull fluentd@sha256:352d55d2078fbfc9a937d0363b5bbd534c8beb697a50e83bf22bf0a10aa2b3f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25140944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b8e09ecb2b9be644f07766135ac88f79f14da7d166ffb26973b1b4bc860841a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:21:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:21:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:22:02 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:22:03 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:22:03 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:22:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:22:03 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:22:03 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:22:04 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:22:04 GMT
USER fluent
# Tue, 04 Apr 2023 00:22:04 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:22:04 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa07d670c0f5933d60efc971af846c6ae888f4e23b0327e32b12994d37743654`  
		Last Modified: Tue, 04 Apr 2023 00:25:10 GMT  
		Size: 21.8 MB (21764169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f602c3750d1aecc6c4a586ef442a773b8f7760ba57e7f79264ed14cdf8d4ed`  
		Last Modified: Tue, 04 Apr 2023 00:25:07 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2498f159ecfc088f6f02d163dfb8b047290b30ac5fcd8311bc17afe8d824bd9a`  
		Last Modified: Tue, 04 Apr 2023 00:25:07 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0461207db4ddd97bbc8a0b68c25efcc5e97fd9f3f43ef59e42b8732b7365c492`  
		Last Modified: Tue, 04 Apr 2023 00:25:07 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-1.0` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:65d2a7a2677137edd41e9d5c64ff89acfc281743d7ef32412c813534067daa2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23810626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3c8433a0c3f42b76c1509792a291d63f86697031c4f1d8a3b5f7559d859cf7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:06:39 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:06:39 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:07:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:07:40 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:07:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:07:40 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:07:40 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:07:40 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:07:40 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:07:40 GMT
USER fluent
# Tue, 04 Apr 2023 00:07:40 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:07:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ba6d6f8ecfc29753c59b0ba643012ce6907ab381fb451d451a93c0c17012e6`  
		Last Modified: Tue, 04 Apr 2023 00:07:57 GMT  
		Size: 20.7 MB (20697612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf6c016ad72c78a88d7b7b26a7cf1d74fd021da7b18ad6459839400bb684668`  
		Last Modified: Tue, 04 Apr 2023 00:07:53 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63640f7ce6faef8e9f6a1c2363709bccc7380527b37269499ed9c29c0bba312`  
		Last Modified: Tue, 04 Apr 2023 00:07:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1774ae06f6540f8048b494472e2863501a9defbb42df777d641b26195c23f1`  
		Last Modified: Tue, 04 Apr 2023 00:07:53 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:bf838b9ced09ce9d892ecdf02d5ab79237747f87b71608ad612f255122fed97b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457e56584ffa420563004b6e6d532a222271b0f5a7e463616f31c3527370d232`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:32:28 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:32:28 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:33:16 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:33:16 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:33:16 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:33:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:33:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:33:17 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:33:17 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:33:17 GMT
USER fluent
# Tue, 04 Apr 2023 00:33:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:33:17 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bda3a270166f2a977c0884235cad5b8f021f8db56ea9b2c432cecf74329247`  
		Last Modified: Tue, 04 Apr 2023 00:35:57 GMT  
		Size: 21.3 MB (21342740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a16a4585660946e7720147d598a27d843c96abfa610a11201d6f8257800cc14`  
		Last Modified: Tue, 04 Apr 2023 00:35:55 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785af8e229db635092bdcbafbaf0b44b685a6074f64e0cda523b636f08538b39`  
		Last Modified: Tue, 04 Apr 2023 00:35:55 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b6783ed8e3a73fe1cb5dbcc5c8cc6248c5860c1cc4eb302f2107d3f78ab34`  
		Last Modified: Tue, 04 Apr 2023 00:35:55 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:76b60221ded7a71376bb5b26e375615cc729d01cd0ff46c17465a4773534db1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24411093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cea1608e07e2659c0aca6e680315bc4e5c3508f9b3f8a5a7156a3aafca641eee`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 01:16:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 01:16:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 01:17:55 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 01:17:56 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 01:17:56 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 01:17:56 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 01:17:56 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 01:17:56 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 01:17:57 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 01:17:57 GMT
USER fluent
# Tue, 04 Apr 2023 01:17:57 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 01:17:57 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed08b8285ffd56e96393c2dff4fb2ce0a3c27a92394d54abf1c1716421e804`  
		Last Modified: Tue, 04 Apr 2023 01:21:21 GMT  
		Size: 21.0 MB (20996620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959325317237f318931715bd2bbd656167fabf07670987717972e64a0da60bad`  
		Last Modified: Tue, 04 Apr 2023 01:21:17 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa24e173dae39c3ecdd5bdbbc010db1cfcdee84d3a01c48a43e776cf6f798150`  
		Last Modified: Tue, 04 Apr 2023 01:21:17 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2429838a83f4ef0f0d1e7dad9771de9b7febd4ee886354d14035325fff0a958e`  
		Last Modified: Tue, 04 Apr 2023 01:21:17 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:01a35c95635804feaa927be6ddd8d50f27da355ffec4b0be26e632577dcc5f52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (24990680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f68fc5f2ab5d0b4cc08684d231004414d406a6428929fdf914b10bd9a271a59`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 00:41:15 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:41:17 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:43:10 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:43:13 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:43:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:43:14 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:43:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:43:15 GMT
ENV LD_PRELOAD=
# Tue, 04 Apr 2023 00:43:16 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:43:17 GMT
USER fluent
# Tue, 04 Apr 2023 00:43:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:43:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e5d552a1c089c6d62019d6363c52cc538432e91dff873e1b88f559a5bc8d56`  
		Last Modified: Tue, 04 Apr 2023 00:50:04 GMT  
		Size: 21.6 MB (21597531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4846e34c153455ca303d93be3b6891184cdf81fdb542be2ddf33936434a18a`  
		Last Modified: Tue, 04 Apr 2023 00:49:58 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc4f08d35e6fa7282eb71c46f2a983dc42b8f3ac3b10f1dc5d8aad8fb8cc70f`  
		Last Modified: Tue, 04 Apr 2023 00:49:58 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27735545a7315c8e8a081426bd355599eb0a3828750063e75a4a6385655d61a`  
		Last Modified: Tue, 04 Apr 2023 00:49:58 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:de41a2a9ccf81ba76fcafddb31dba48fb8e46294d150fa18cdd3cbdd796cacf1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 MB (24345941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93a9225e2eb720e3696ed7db8406b7622174b761b5ffd91d252174b0a7f5ca63`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Fri, 05 May 2023 00:36:09 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 05 May 2023 00:36:09 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Fri, 05 May 2023 00:36:56 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 05 May 2023 00:36:58 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 05 May 2023 00:36:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 05 May 2023 00:36:58 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 05 May 2023 00:36:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 05 May 2023 00:36:59 GMT
ENV LD_PRELOAD=
# Fri, 05 May 2023 00:36:59 GMT
EXPOSE 24224 5140
# Fri, 05 May 2023 00:36:59 GMT
USER fluent
# Fri, 05 May 2023 00:36:59 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 05 May 2023 00:36:59 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dfcaf3da0dcc5db8c5ab1ecfbb8d021d0486173a5fe8813c727ac8cd06805e`  
		Last Modified: Fri, 05 May 2023 00:39:34 GMT  
		Size: 21.2 MB (21168543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0efbe4644268746c3e1eff581e0ccc2b2b689ff0a2cd774719c7faf5e08ccf`  
		Last Modified: Fri, 05 May 2023 00:39:31 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0020f048480ef88a5b12c1f92ec54ccd07a5257a66d36780e045ebca4efdae9d`  
		Last Modified: Fri, 05 May 2023 00:39:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a2a4da469cac674fce9f8503512acb9c265a5e72f69785a38f3dcd83bb8b84`  
		Last Modified: Fri, 05 May 2023 00:39:31 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16.0-debian-1.0`

```console
$ docker pull fluentd@sha256:c0743231e9fcf61d2395a01d8bda7bca381b90453216cdf86c282f5a957ba5c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.16.0-debian-1.0` - linux; amd64

```console
$ docker pull fluentd@sha256:34798804af5d79350cad454af9f27dda2369e900c479d6987986a7cc5101cff5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101764787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee5d396ffe5f6dea71870bf918f87a30130ff1729b382aea2ff0e311860ecdf3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 11:28:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 11:28:53 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 11:28:53 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 11:49:26 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 11:49:26 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 11:49:26 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 11:51:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 11:51:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 11:51:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 11:51:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 11:51:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 11:51:42 GMT
CMD ["irb"]
# Tue, 23 May 2023 23:43:57 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 23:43:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 23:43:57 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 23:46:33 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 23:46:34 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 23:46:34 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 23:46:35 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 23:46:35 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 23:46:35 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 23:46:35 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 23:46:35 GMT
USER fluent
# Tue, 23 May 2023 23:46:35 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 23:46:35 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a1dfbc0e3c1cddb150865089039a9023dbac788fdf37a4f698b2a242393430`  
		Last Modified: Tue, 23 May 2023 12:05:53 GMT  
		Size: 10.0 MB (10023269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50db7b862053780f8046cd4090d0b17584a13013d7dce8ad4f404734fd1c902a`  
		Last Modified: Tue, 23 May 2023 12:05:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0cec51f183aef280729ae039fa4e76e7eb84c3eef57e59e073f51470ab6c8f`  
		Last Modified: Tue, 23 May 2023 12:08:13 GMT  
		Size: 32.6 MB (32626024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b934eff42c9311bb8b61df5e4cfdc6d3210b09e3b1cbd5dfea875ec41fddd033`  
		Last Modified: Tue, 23 May 2023 12:08:10 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e5b6e03ed07a5e851383b675b3e863b5bb8cf1032eb4c348a7ee0b8cbf9ce1`  
		Last Modified: Tue, 23 May 2023 23:47:01 GMT  
		Size: 27.7 MB (27708820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f378cfcc3cb686b089cd08f7ec8c1acc4664cf1eb836e091769da88cf30737f`  
		Last Modified: Tue, 23 May 2023 23:46:57 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa6a5baf0d72ab3054bd949c716387dc8c0cb115f29925dfe17b7b6bebe3df`  
		Last Modified: Tue, 23 May 2023 23:46:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3074318e81de9867f633281b8c19e19f618a08c6d7807d90ac881bfd132ca4cb`  
		Last Modified: Tue, 23 May 2023 23:46:57 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:63a2cd55488c0416aa72cee3153d084f85a4e87619a19c5d9ae2b417ed09b99f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95253139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40ea4a5e6c1bf2ff09459c744fdc5027a754681f609b198ab460ded663adc43a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 00:48:41 GMT
ADD file:868f634f5ddb80ed9e9c719ccaf5d564d96fe819f0b000ecc734311baf5da99b in / 
# Tue, 23 May 2023 00:48:42 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:43:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:43:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 07:43:58 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 07:53:32 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 07:53:32 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 07:53:32 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 07:56:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 07:56:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 07:56:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 07:56:00 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 07:56:01 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 07:56:01 GMT
CMD ["irb"]
# Tue, 23 May 2023 14:06:42 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 14:06:42 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 14:06:42 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 14:09:37 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 14:09:38 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 14:09:38 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 14:09:38 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 14:09:38 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 14:09:38 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 14:09:38 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 14:09:38 GMT
USER fluent
# Tue, 23 May 2023 14:09:38 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 14:09:38 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:812967ccba449e7a96044b2d48ffc62816b22eb17641844c4dfffbe3b3ec6f21`  
		Last Modified: Tue, 23 May 2023 00:51:19 GMT  
		Size: 28.9 MB (28903411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be04097d1ded9335b3db9447099711ba6b7e06110590c1dce452f7bfbde88a6b`  
		Last Modified: Tue, 23 May 2023 08:01:48 GMT  
		Size: 8.6 MB (8634451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22a934b77fc215fc18ccde8e1d1820798abb4b25ed01191b3bb3c4815f31168`  
		Last Modified: Tue, 23 May 2023 08:01:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e558fe7b0b7f0c483952f729a9b4538079f921461ee708c55b103cf7712078c2`  
		Last Modified: Tue, 23 May 2023 08:03:08 GMT  
		Size: 31.2 MB (31165902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09bd2353f05cb293e4149ffe41c6f17410af979ed625452c1d65ea76df4a388`  
		Last Modified: Tue, 23 May 2023 08:03:05 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3579ba85a1ea2ab414bbc750307485a987a0a31d9140c83e8a4049e7aae54981`  
		Last Modified: Tue, 23 May 2023 14:10:00 GMT  
		Size: 26.5 MB (26546298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64760944e08c577d65da8d66f3491bffb96e30c7f9161c0c64ef07dafc09577`  
		Last Modified: Tue, 23 May 2023 14:09:55 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a24442b206e924e60c0c853e69b3f4da5b0f0c7bddada10dc694e24e39f0c6`  
		Last Modified: Tue, 23 May 2023 14:09:55 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94632d40ef4f818499a20ad7ae500da0eace49dcc1d209c4b92d497490da9e60`  
		Last Modified: Tue, 23 May 2023 14:09:55 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:58af03c16b82949f0a46261c3d9deff04a9fb2fd827a03523a998f9cfc20dd07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92129948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9e3d97872d6a319f78d975f6b9ca01bb0dbea6e6575c4f0b4834c7c87def11`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:30:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:30:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 05:30:28 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 05:40:42 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 05:40:42 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 05:40:42 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 05:42:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 05:42:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 05:42:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 05:42:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 05:42:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 05:42:46 GMT
CMD ["irb"]
# Tue, 23 May 2023 11:21:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 11:21:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 11:21:54 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 11:24:45 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 11:24:45 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 11:24:45 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 11:24:46 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 11:24:46 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 11:24:46 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 11:24:46 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 11:24:46 GMT
USER fluent
# Tue, 23 May 2023 11:24:46 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 11:24:46 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb6a09bcc5c0984ecb3a04b714caca1098f621d70de5fb59d22fc016d46ffae`  
		Last Modified: Tue, 23 May 2023 05:50:53 GMT  
		Size: 8.1 MB (8143926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca2368c379d00172553a3637b0c56b1cdb714a97b92bb40f910b023e9ac82c3`  
		Last Modified: Tue, 23 May 2023 05:50:51 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78962edc36f5ff06f5957f41aec3bc1dafd3618cb6e13c99ec2b9d672ce2d46`  
		Last Modified: Tue, 23 May 2023 05:52:01 GMT  
		Size: 31.0 MB (31035229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5cd2c80a56fed84af20ba9be79ed5dac3e9a1b6e1836258be0c336c9a5d6c2`  
		Last Modified: Tue, 23 May 2023 05:51:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da01f5f14b76cd026a041d821586399ee1d001069ecee5d3b094ff4d3edeab11`  
		Last Modified: Tue, 23 May 2023 11:25:10 GMT  
		Size: 26.4 MB (26383084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c77433b38e451ecdd7e9b29de43727689fa84bca8f4dacc28b31cc6a86d3fb`  
		Last Modified: Tue, 23 May 2023 11:25:05 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997fc11b9f431e3b81cee260d095c9e0494c99d1346c1aa2d58f406637dcd08`  
		Last Modified: Tue, 23 May 2023 11:25:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b271058e601b3a5ac882e8f5feb99a66fd16e41a2cfe1d9048231084c202027`  
		Last Modified: Tue, 23 May 2023 11:25:05 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:8dd6b2dde2fd86cde3f161e972c179295c5b2fbdbe0aac1b27843650d6c0f8f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.7 MB (98742575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99424dea3591c74df4dfe8d8c0eee56d1f2f74dcaeb8fb5082ca80d74a3a64a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:17:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:17:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 06:17:13 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 06:33:27 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 06:33:27 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 06:33:27 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 06:35:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 06:35:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 06:35:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 06:35:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:35:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 06:35:17 GMT
CMD ["irb"]
# Tue, 23 May 2023 19:38:49 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 19:38:49 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 19:38:49 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 19:41:09 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 19:41:10 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 19:41:10 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 19:41:10 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 19:41:10 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 19:41:11 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 19:41:11 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 19:41:11 GMT
USER fluent
# Tue, 23 May 2023 19:41:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 19:41:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c44207aeb95c5c97b69601e7ecf6205b0018dc481f58c8d1c35c7e9f1ce3d6e`  
		Last Modified: Tue, 23 May 2023 06:46:42 GMT  
		Size: 9.2 MB (9243477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68b42fcab4b6e0ed16656636285da203ba16863eff8f005def15c873988b921`  
		Last Modified: Tue, 23 May 2023 06:46:41 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f6677e34939ef3d61f952f03eb1fd89bde1a1894e28bddeaa6bab4abcd7015`  
		Last Modified: Tue, 23 May 2023 06:48:53 GMT  
		Size: 32.0 MB (31987287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d18bebe0e6b2814ed86e3b712f39ca4b5fc012cb4753e109949603be9cfe78b`  
		Last Modified: Tue, 23 May 2023 06:48:51 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bc4d360fc0448da1de6b1d389ffe87a5440380e673469cbeaee92effa67c1e`  
		Last Modified: Tue, 23 May 2023 19:41:36 GMT  
		Size: 27.5 MB (27455976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fb3bef85d57b3b7fc3bf58c8ab88e60904d62a5075a1618ab6668e4694e1bc`  
		Last Modified: Tue, 23 May 2023 19:41:33 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98157824256abbfd44628fb3ba45aeb0f930b7c20ae756781a4b0240f05c802`  
		Last Modified: Tue, 23 May 2023 19:41:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65de085db6e9276f33e5df470cbbb4664e6493dccb70a7d434c08fea4e43125`  
		Last Modified: Tue, 23 May 2023 19:41:33 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:d9a49fa00e22b0b02e6554fea3bf2dce9cfd94570333040c7d3c9a0e1de85702
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102148831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb6733d8f9d1c7791d728734fd6250fb09415e834aaa1f0529988b8257e71c3a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:12:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:12:04 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 01:12:04 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 01:28:03 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 01:28:03 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 01:28:03 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 01:31:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 01:31:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 01:31:40 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 01:31:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:31:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 01:31:40 GMT
CMD ["irb"]
# Tue, 23 May 2023 20:03:34 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 20:03:34 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 20:03:34 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 20:06:31 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 20:06:32 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 20:06:32 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 20:06:32 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 20:06:32 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 20:06:32 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 20:06:32 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 20:06:32 GMT
USER fluent
# Tue, 23 May 2023 20:06:32 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 20:06:32 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e573e66fa2cd19b7052169187d24733be9d6d250dc8898046d0fea6cd049d`  
		Last Modified: Tue, 23 May 2023 01:43:19 GMT  
		Size: 12.0 MB (11997370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35afa18cbcba46f8516124b77bcc5ade8c55162dc60d023b4302c72e9cb40e08`  
		Last Modified: Tue, 23 May 2023 01:43:15 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35da886c11b3e44726a8d010f5314900641263fd2ee12d332bd3587940af7bb`  
		Last Modified: Tue, 23 May 2023 01:44:35 GMT  
		Size: 31.2 MB (31181783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8906d58f8e100a1cc314b06760b6084baa703ad4692de9f4421a955bca26d235`  
		Last Modified: Tue, 23 May 2023 01:44:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02699f810fccd7455168170e0f4e316ac6e4a600e5440319be02c45acc25ae48`  
		Last Modified: Tue, 23 May 2023 20:06:55 GMT  
		Size: 26.6 MB (26578433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b626fbc5cd4378136253cad9db380b06f5cb2572cdd57e2dbf071a8166357b09`  
		Last Modified: Tue, 23 May 2023 20:06:50 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d778ffbe1a34d2f0053abfe3e33a055f3952301dab1cd8e8281d20a1a2eff3d1`  
		Last Modified: Tue, 23 May 2023 20:06:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4da0f4b1f77486a59eaba18767fbccb83baab50337c5bed3eb73309018756c5`  
		Last Modified: Tue, 23 May 2023 20:06:50 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:3c24325053f32db3e85a1d6105e77459e247939442d4fd68f56e50e7df2131db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106748156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af62282a59b9815935eb5e0c85cdc13d73179b68796b1933d4d270e16c58b9c4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:23:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:23:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 02:23:32 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 02:40:17 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 02:40:18 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 02:40:18 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 02:44:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 02:44:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 02:44:20 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 02:44:20 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:44:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 02:44:22 GMT
CMD ["irb"]
# Tue, 23 May 2023 18:22:20 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 18:22:20 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 18:22:21 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 18:27:29 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 18:27:32 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 18:27:32 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 18:27:32 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 18:27:32 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 18:27:33 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 18:27:33 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 18:27:33 GMT
USER fluent
# Tue, 23 May 2023 18:27:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 18:27:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d38ba339ef6043fdfe3ddd5359c69fcf0314d3e805835066f25f5bdec81cbaa`  
		Last Modified: Tue, 23 May 2023 02:52:45 GMT  
		Size: 10.5 MB (10481258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6686de7ce20c5bf6829105ad713ada3bd60313789b594e248ffe5250dc1b159f`  
		Last Modified: Tue, 23 May 2023 02:52:42 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4951bfecfe434f2065bfa58d65d30fcd4683531c9458244fa962c03cc48cd61e`  
		Last Modified: Tue, 23 May 2023 02:54:21 GMT  
		Size: 32.8 MB (32791406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6822a4153fffa9635a3af305ce435ccee23f1029d7a694a724a74fd392835a95`  
		Last Modified: Tue, 23 May 2023 02:54:16 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71abde10f8f427c3aa332fb8212f0a26a02db5ac37458cc5a9ba0085644aa4c9`  
		Last Modified: Tue, 23 May 2023 18:28:00 GMT  
		Size: 28.2 MB (28191497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa549617805f59c555997200a428c14171b483b7a14983074b92d593038156ca`  
		Last Modified: Tue, 23 May 2023 18:27:53 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55be1358fafcaa95f4eaedea36011475dc6544349a637f879a9fd96586a5e5`  
		Last Modified: Tue, 23 May 2023 18:27:53 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e960237bd065aef85488dbfbf179b82c7415c294827b0dc9bf255d72859ad4b4`  
		Last Modified: Tue, 23 May 2023 18:27:53 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:280474dd7d723a6e0f3f613447ed6dc5d9a9a19c6191213159239b9692168005
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98885605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:412413267f439d94cc9e69a7cf29468703d666de437d6ac2b3c46b0858cc6b1f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:16:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:16:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 02:16:13 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 02:20:52 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 May 2023 02:20:52 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 23 May 2023 02:20:52 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 23 May 2023 02:22:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 02:22:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 02:22:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 02:22:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:22:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 02:22:51 GMT
CMD ["irb"]
# Tue, 23 May 2023 07:34:18 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 May 2023 07:34:18 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 23 May 2023 07:34:19 GMT
ENV TINI_VERSION=0.18.0
# Tue, 23 May 2023 07:36:34 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 23 May 2023 07:36:42 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 May 2023 07:36:42 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 May 2023 07:36:42 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 23 May 2023 07:36:43 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 May 2023 07:36:43 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 23 May 2023 07:36:44 GMT
EXPOSE 24224 5140
# Tue, 23 May 2023 07:36:44 GMT
USER fluent
# Tue, 23 May 2023 07:36:44 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 May 2023 07:36:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389e5acb5f585dd7876222f795a0f8adb45bbb36dfee1707ad06ef3c32abe06a`  
		Last Modified: Tue, 23 May 2023 02:25:49 GMT  
		Size: 8.9 MB (8864321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f41881192359d6eae65c1dea80a1676401b472e6565797e2c8a05658dbfc19`  
		Last Modified: Tue, 23 May 2023 02:25:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024533d1e28fb42ceec653648bb53ba0eec8a926cca2b4c37f7b9b789b7af370`  
		Last Modified: Tue, 23 May 2023 02:26:18 GMT  
		Size: 32.4 MB (32444939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b5d84dde0b278d9f070f6f6be97cb4cd0dd9049cae6b5db6e105f3c27889b4`  
		Last Modified: Tue, 23 May 2023 02:26:15 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46cdab6f14951c66d27711ad392574c46660f5f49c9267fe884221e566afb3b`  
		Last Modified: Tue, 23 May 2023 07:37:05 GMT  
		Size: 27.9 MB (27931089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c787127535fef7623fff56414b4142dc7fd48019892f9b13bb318811bb59fb80`  
		Last Modified: Tue, 23 May 2023 07:37:01 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa09eece0a3b6c953dbbff800b217a3fea7d92bf76fee667b8e7975dd65167e`  
		Last Modified: Tue, 23 May 2023 07:37:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd69db2a81327365cce1daf3c24f1e16505dec378db47cff7c6cea2ad3b8950`  
		Last Modified: Tue, 23 May 2023 07:37:01 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
