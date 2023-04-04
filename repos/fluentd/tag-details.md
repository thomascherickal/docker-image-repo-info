<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.16-1`](#fluentdv116-1)
-	[`fluentd:v1.16-debian-1`](#fluentdv116-debian-1)
-	[`fluentd:v1.16.0-1.0`](#fluentdv1160-10)
-	[`fluentd:v1.16.0-debian-1.0`](#fluentdv1160-debian-10)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:23b2ae4235bf29886c5837dc1b0077c2cec83dc83a3f487eb87a76fe466bad5f
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
$ docker pull fluentd@sha256:001d2a51a850037c96ed3ac4fa78cbcbd1221839de5da38b6634c6e9eba86a51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 MB (24349962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880b3c4874df382cf8694342ff89e648274603b841bd70352f48306bedbbc493`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Mon, 03 Apr 2023 23:27:58 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Mon, 03 Apr 2023 23:27:59 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Mon, 03 Apr 2023 23:28:47 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Mon, 03 Apr 2023 23:28:50 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Mon, 03 Apr 2023 23:28:50 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Mon, 03 Apr 2023 23:28:50 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Mon, 03 Apr 2023 23:28:50 GMT
ENV FLUENTD_CONF=fluent.conf
# Mon, 03 Apr 2023 23:28:50 GMT
ENV LD_PRELOAD=
# Mon, 03 Apr 2023 23:28:51 GMT
EXPOSE 24224 5140
# Mon, 03 Apr 2023 23:28:51 GMT
USER fluent
# Mon, 03 Apr 2023 23:28:51 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Mon, 03 Apr 2023 23:28:51 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ac5bd72fbffa874e5d0fe209c6a1b307198f205b8e4d5ec8f020526670649`  
		Last Modified: Mon, 03 Apr 2023 23:31:22 GMT  
		Size: 21.2 MB (21172560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a476a1392375893899c9adccc09d5de446342c3b3679c6b7d59b94001ec262d4`  
		Last Modified: Mon, 03 Apr 2023 23:31:20 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2cd03bd7b304700dfc5d69e003ba9fe11e67c6277731736c718afd73aa4fa54`  
		Last Modified: Mon, 03 Apr 2023 23:31:20 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4921fcfe9790dd687de7cfeeb8e67b1cc300da3276d37aa99171ecfbc47b6e`  
		Last Modified: Mon, 03 Apr 2023 23:31:19 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16-1`

```console
$ docker pull fluentd@sha256:23b2ae4235bf29886c5837dc1b0077c2cec83dc83a3f487eb87a76fe466bad5f
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
$ docker pull fluentd@sha256:001d2a51a850037c96ed3ac4fa78cbcbd1221839de5da38b6634c6e9eba86a51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 MB (24349962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880b3c4874df382cf8694342ff89e648274603b841bd70352f48306bedbbc493`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Mon, 03 Apr 2023 23:27:58 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Mon, 03 Apr 2023 23:27:59 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Mon, 03 Apr 2023 23:28:47 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Mon, 03 Apr 2023 23:28:50 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Mon, 03 Apr 2023 23:28:50 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Mon, 03 Apr 2023 23:28:50 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Mon, 03 Apr 2023 23:28:50 GMT
ENV FLUENTD_CONF=fluent.conf
# Mon, 03 Apr 2023 23:28:50 GMT
ENV LD_PRELOAD=
# Mon, 03 Apr 2023 23:28:51 GMT
EXPOSE 24224 5140
# Mon, 03 Apr 2023 23:28:51 GMT
USER fluent
# Mon, 03 Apr 2023 23:28:51 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Mon, 03 Apr 2023 23:28:51 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ac5bd72fbffa874e5d0fe209c6a1b307198f205b8e4d5ec8f020526670649`  
		Last Modified: Mon, 03 Apr 2023 23:31:22 GMT  
		Size: 21.2 MB (21172560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a476a1392375893899c9adccc09d5de446342c3b3679c6b7d59b94001ec262d4`  
		Last Modified: Mon, 03 Apr 2023 23:31:20 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2cd03bd7b304700dfc5d69e003ba9fe11e67c6277731736c718afd73aa4fa54`  
		Last Modified: Mon, 03 Apr 2023 23:31:20 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4921fcfe9790dd687de7cfeeb8e67b1cc300da3276d37aa99171ecfbc47b6e`  
		Last Modified: Mon, 03 Apr 2023 23:31:19 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16-debian-1`

```console
$ docker pull fluentd@sha256:eda3a731a5b481a6a2575d970b13e149b5628dd0ba7e3efe6d32ded5688cca87
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
$ docker pull fluentd@sha256:c12cd975bf1d0568ac8d720d606048f7ec60b4d0473b3da010a5d7d43f769c60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101770763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43979cb0f9d95d16dce1def736679ca71ed498ddb50748bbc9e8210006675401`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 16:05:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 16:05:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 16:05:39 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 16:16:21 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:39:16 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:39:16 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:41:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:41:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:41:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:41:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:41:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:41:30 GMT
CMD ["irb"]
# Tue, 04 Apr 2023 00:22:08 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:22:08 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:22:08 GMT
ENV TINI_VERSION=0.18.0
# Tue, 04 Apr 2023 00:24:43 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:24:44 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:24:44 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:24:44 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:24:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:24:45 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 04 Apr 2023 00:24:45 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:24:45 GMT
USER fluent
# Tue, 04 Apr 2023 00:24:45 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:24:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b6c5e514e1b14fbdb31cb290dc9e714aab2152526b6807ebca5713c53cfa19`  
		Last Modified: Thu, 23 Mar 2023 16:39:55 GMT  
		Size: 10.0 MB (10023421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77fe2302da079bdc4425a38a2e8615bb9a8a19e32bd72f7d7b0b63e1831e069`  
		Last Modified: Thu, 23 Mar 2023 16:39:53 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d577fe9d8654459652bd7c69262c163ce9567c0231b5630b07ee163a73d442`  
		Last Modified: Thu, 30 Mar 2023 20:13:30 GMT  
		Size: 32.6 MB (32626154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5876e5aba0df9cbc0a632a0b86ba7972a39abb70f4bc7c98960ee470e91a82e9`  
		Last Modified: Thu, 30 Mar 2023 20:13:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed4813af1aeb4b12e2b555a3feb76c928b20075f48503177c806a8115f1d950`  
		Last Modified: Tue, 04 Apr 2023 00:25:25 GMT  
		Size: 27.7 MB (27706700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfde4897c00ce06ef4de3b267e0233d857271679a0a29ceee7fe1c5e38df994`  
		Last Modified: Tue, 04 Apr 2023 00:25:20 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07b4a64a5f37eb059c05ad7e4a294c4a641688ec6ccc9e933b3c16c5bc4967e`  
		Last Modified: Tue, 04 Apr 2023 00:25:20 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e341681ac673d148b468ebfe6c2e83fae29c359ac1aa4c29a901c77846e13e1f`  
		Last Modified: Tue, 04 Apr 2023 00:25:20 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:942fbb6ef96523333a78f5ab305c24efb3486c972067774ccb43b2deae8485af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95261905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f8ddc2c445ca2b4020d5202e9eeae14120c9c4007817d7c656d4a1e01ae85c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:44 GMT
ADD file:7595c7bfa6b3741f57a3ec7790e3108bb526244e52bb4a54548b8b5541e66616 in / 
# Thu, 23 Mar 2023 00:48:44 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:42:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 06:42:50 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 06:47:41 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:00:30 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:00:30 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:02:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:02:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:02:38 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:02:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:02:39 GMT
CMD ["irb"]
# Mon, 03 Apr 2023 23:12:15 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Mon, 03 Apr 2023 23:12:15 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Mon, 03 Apr 2023 23:12:15 GMT
ENV TINI_VERSION=0.18.0
# Mon, 03 Apr 2023 23:15:06 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Mon, 03 Apr 2023 23:15:06 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Mon, 03 Apr 2023 23:15:06 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Mon, 03 Apr 2023 23:15:07 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Mon, 03 Apr 2023 23:15:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Mon, 03 Apr 2023 23:15:07 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Mon, 03 Apr 2023 23:15:07 GMT
EXPOSE 24224 5140
# Mon, 03 Apr 2023 23:15:07 GMT
USER fluent
# Mon, 03 Apr 2023 23:15:07 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Mon, 03 Apr 2023 23:15:07 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b83d345710cdef1626d1940689dd3160e5ce3e4f63b3154cf612c52b704baa66`  
		Last Modified: Thu, 23 Mar 2023 02:22:00 GMT  
		Size: 28.9 MB (28915852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01823b006e73c4ea0cff9c35ae3dce62fc987febd01d0a092b8ac2815d5246b1`  
		Last Modified: Fri, 24 Mar 2023 23:27:15 GMT  
		Size: 8.6 MB (8635898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dbe6acaf6962399719d4c660823c56b892af485f4e2596b748c9cd0724b9c1`  
		Last Modified: Fri, 24 Mar 2023 23:27:12 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e78b20864ab83fc7e0329e406a79ade96d4f76e5b7d02518a761d09109c878a`  
		Last Modified: Thu, 30 Mar 2023 20:49:57 GMT  
		Size: 31.2 MB (31165835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6bd7652282f7fef67562600ec96645d6f69afd7148bd96fcf2338f14fda129`  
		Last Modified: Thu, 30 Mar 2023 20:49:54 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa72e0fb53c78f2bb5e28287e2564cc778a9cc3f108f60194d953d88cca93cf`  
		Last Modified: Tue, 04 Apr 2023 00:19:44 GMT  
		Size: 26.5 MB (26541244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a040e51f0d0904dc704461487f6d32a29eec953099246b328f21677ca24a4ee1`  
		Last Modified: Tue, 04 Apr 2023 00:19:40 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f970057ef53b3683906d0d7b950d6f5dd92fea0d834c0f7cdac37bea6d07606a`  
		Last Modified: Tue, 04 Apr 2023 00:19:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f608622e1770272b304b55a84eb3224200c9e19a6a80dff37b166e0eb61433b4`  
		Last Modified: Tue, 04 Apr 2023 00:19:39 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:60c1734ae51123c14ff3da6e1fce46b158c06e60c65e03b73312c02cc3e4a5f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92139379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c609296458d778df892df7fbed5920e6601c82eb3a2a37cbeb1ed5b03a709fdd`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:01:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:01:47 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 12:01:47 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 12:06:43 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:26:43 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:26:43 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:28:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:28:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:28:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:28:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:28:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:28:43 GMT
CMD ["irb"]
# Tue, 04 Apr 2023 01:28:30 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 01:28:30 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 01:28:30 GMT
ENV TINI_VERSION=0.18.0
# Tue, 04 Apr 2023 01:31:06 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 01:31:07 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 01:31:07 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 01:31:07 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 01:31:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 01:31:07 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 04 Apr 2023 01:31:07 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 01:31:08 GMT
USER fluent
# Tue, 04 Apr 2023 01:31:08 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 01:31:08 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8df912a289c6207563585bbdbcecbaf882532ee37701510780368dfc169edb`  
		Last Modified: Thu, 23 Mar 2023 12:19:16 GMT  
		Size: 8.1 MB (8145357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b732e8aacf04397c43f20b96535748cf9ff21c9d2cc823cd5ea73fb474a709`  
		Last Modified: Thu, 23 Mar 2023 12:19:14 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fa8fbb1b2b516dd2cf9e958ff8359901abc9c9f15fc83caae2a1432d18bd7d`  
		Last Modified: Thu, 30 Mar 2023 19:58:56 GMT  
		Size: 31.0 MB (31034262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed24e2ec6f169ac053b414ad28defa6f70dcc2d1cfd8d6f952a37e41d5068f94`  
		Last Modified: Thu, 30 Mar 2023 19:58:53 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709b88800c4ec9091cd0a81d713314069a2dfd8a64f2de17d88847a29e21f0b2`  
		Last Modified: Tue, 04 Apr 2023 01:32:02 GMT  
		Size: 26.4 MB (26379351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fabbe7d96726c30c69f4cfb84b225d311cc18eff3696ac74c6abb1f1d4873e9`  
		Last Modified: Tue, 04 Apr 2023 01:31:58 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6966fda14b69edd56aa16cf55261b12e2d248ef2d39a02436bee9fa47565b01e`  
		Last Modified: Tue, 04 Apr 2023 01:31:58 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d5829bb78c5a9743af48b9eeddaa0a4b2cea71f62104d7330475b429a75328`  
		Last Modified: Tue, 04 Apr 2023 01:31:59 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:a377a0a9cc406874e2542d59f0b021dbd2e52e0805f0aef76c5dfe38ed1af1a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.8 MB (98756545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b979d9f2b3ba0a2bde4fff7b8f3c106cb4dd310ba3ffb2c071374c041ce2c14c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:13:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 06:13:20 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 06:18:02 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:00:46 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:00:46 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:02:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:02:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:02:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:02:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:02:31 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:02:31 GMT
CMD ["irb"]
# Tue, 04 Apr 2023 00:33:25 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:33:25 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:33:25 GMT
ENV TINI_VERSION=0.18.0
# Tue, 04 Apr 2023 00:35:44 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:35:45 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:35:45 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:35:45 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:35:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:35:45 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 04 Apr 2023 00:35:45 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:35:45 GMT
USER fluent
# Tue, 04 Apr 2023 00:35:45 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:35:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a96a7aa954e0123803b20ac7f00cac949799f3311a00e4d7e3d3a695602041`  
		Last Modified: Thu, 23 Mar 2023 06:29:04 GMT  
		Size: 9.2 MB (9244609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a759fe3d4385aa21faa3a8c109a649c866edf763ba19bf9a83fcfbc81b5f83b`  
		Last Modified: Thu, 23 Mar 2023 06:29:03 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6718b4e09290a25827867abd642ad608ccd7a34e173092e5223e77f9d3a9ac`  
		Last Modified: Thu, 30 Mar 2023 19:28:00 GMT  
		Size: 32.0 MB (31987334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c375fb3304543819eb8392761158cd0c170fd870675038686f75c467036c05b`  
		Last Modified: Thu, 30 Mar 2023 19:27:58 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d742b5fbdf8e142a74ea6592c3605a090c720cd592ffba7006b7f51602dfda`  
		Last Modified: Tue, 04 Apr 2023 00:36:10 GMT  
		Size: 27.5 MB (27458811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a793531fadb9d0f0f03c822e8f1bb9da777bd8985aaf6151e7d56675a5f08d6a`  
		Last Modified: Tue, 04 Apr 2023 00:36:07 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cd6cff1da66f216dc1453c489497482a0718bdc9c56a66cdb11586e8d95992`  
		Last Modified: Tue, 04 Apr 2023 00:36:07 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b370bea279a69d8dd9b3fbb7c002a3b7a625912d902702fb0cc5642503948a`  
		Last Modified: Tue, 04 Apr 2023 00:36:07 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:16f27f9c7ad25a1c61e09938ffb4693a15817151360c40298717a6e92bf4357c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102159216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60cfa8383ced1d7112d6a449c9418e7c6a20e63e8fbf0388688bae43eaf9a028`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 19:56:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 19:56:26 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 19:56:27 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 20:10:20 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:04:23 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:04:23 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:07:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:07:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:07:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:07:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:07:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:07:51 GMT
CMD ["irb"]
# Tue, 04 Apr 2023 01:18:03 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 01:18:03 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 01:18:03 GMT
ENV TINI_VERSION=0.18.0
# Tue, 04 Apr 2023 01:20:55 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 01:20:56 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 01:20:56 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 01:20:56 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 01:20:56 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 01:20:56 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 04 Apr 2023 01:20:56 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 01:20:56 GMT
USER fluent
# Tue, 04 Apr 2023 01:20:56 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 01:20:57 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d164c2aa0d7283d0965068628d0acc27d38828e4403ad6735e3e5de808aa56d5`  
		Last Modified: Thu, 23 Mar 2023 20:45:00 GMT  
		Size: 12.0 MB (11998249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71f1e847ad5979318ce0c7d87e0899270ffb40d5dfb0b567f77c7d15dcf7177`  
		Last Modified: Thu, 23 Mar 2023 20:44:56 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6cd82fce682a1616d3a4ebe32da0969bb8f348a51004a01d3bddbb3ef91c16`  
		Last Modified: Thu, 30 Mar 2023 19:56:53 GMT  
		Size: 31.2 MB (31181071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d512d5a12e945ce9774e806dd7c07817f8d9ffe4346b7b2f745f2f8591677ff`  
		Last Modified: Thu, 30 Mar 2023 19:56:49 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fabc343d57028c870edc2c9ba37b8840ac34b6a40b0509a60c5bb4c2b8e57cb`  
		Last Modified: Tue, 04 Apr 2023 01:21:36 GMT  
		Size: 26.6 MB (26580545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbdaf1833816399fca88916fc01a4462ec9ab2313c7f8482059913c6d30f507`  
		Last Modified: Tue, 04 Apr 2023 01:21:31 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb32f8a7225d8f6e0d3a15c580e81d3877074fc56da4c76619ce8e68548317`  
		Last Modified: Tue, 04 Apr 2023 01:21:31 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c86302e190e0c658ba6038ef724be029687b61ca6de1c89e020800d8a2ea46`  
		Last Modified: Tue, 04 Apr 2023 01:21:31 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:6943b0c1eb48f170ba1a3f802a6a4f35f8a1e00460f234840982a6d58f8e5804
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106750429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d9bd806d9b6e26dcfd8ca76d8804ee31bdbb241b30057201d7c2b5c267090fa`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 15:51:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 15:51:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 15:51:48 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 15:59:37 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:34:08 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:34:08 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:37:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:37:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:37:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:37:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:37:57 GMT
CMD ["irb"]
# Tue, 04 Apr 2023 00:43:25 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:43:26 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:43:27 GMT
ENV TINI_VERSION=0.18.0
# Tue, 04 Apr 2023 00:49:37 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:49:42 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:49:43 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:49:43 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:49:44 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:49:44 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 04 Apr 2023 00:49:45 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:49:45 GMT
USER fluent
# Tue, 04 Apr 2023 00:49:45 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:49:46 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c068db9fac31f9b975b8b7e2f824bb1269b0b90875799e39dc34d2c11f6b59`  
		Last Modified: Thu, 23 Mar 2023 16:19:23 GMT  
		Size: 10.5 MB (10480889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b18b6f3a2a8e37b2f1a89fc1c7efdf9e4b3f06d9cd433edd35634e7ebe98dd`  
		Last Modified: Thu, 23 Mar 2023 16:19:19 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78273869b448509a48eed0c4616ff76a8af908920d5a6d177e26a7b72fb0b9cf`  
		Last Modified: Thu, 30 Mar 2023 20:06:41 GMT  
		Size: 32.8 MB (32791346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43630b1859e57542fa5c5ac0d7c59a8b775eaa1349d1982ba1d8d239dd0a4d7`  
		Last Modified: Thu, 30 Mar 2023 20:06:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c3a15d1c5c8879aa5b94dda6cd5c2393ade68b107095ef8d89b6868e3db34e`  
		Last Modified: Tue, 04 Apr 2023 00:50:24 GMT  
		Size: 28.2 MB (28187056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e329846174e34740cc31a05d048d0947a585fe7cd27a77527d29bea3316813c5`  
		Last Modified: Tue, 04 Apr 2023 00:50:17 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f946b6e9c0942f1687d2b8c88f4e0c9f140fe3d52e6f12be2eef75b128b6801e`  
		Last Modified: Tue, 04 Apr 2023 00:50:17 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e6d587f00178203b56e77a3518b747cb97a9cce5348f24c83ca97b13dc6944`  
		Last Modified: Tue, 04 Apr 2023 00:50:17 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:61575f83c479d25cf7821001a2cfa66038bf1cd8709eb94ba4dfbdcac71ecec2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98884414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10db35df468c33fe5092a52e4899849c285514a2a80b0759f64e3dc3e0e336e1`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 11:04:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:04:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 11:04:28 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 11:08:50 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 18:53:15 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 18:53:15 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 18:55:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 18:55:13 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 18:55:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 18:55:13 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 18:55:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 18:55:13 GMT
CMD ["irb"]
# Mon, 03 Apr 2023 23:28:56 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Mon, 03 Apr 2023 23:28:56 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Mon, 03 Apr 2023 23:28:56 GMT
ENV TINI_VERSION=0.18.0
# Mon, 03 Apr 2023 23:31:01 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Mon, 03 Apr 2023 23:31:03 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Mon, 03 Apr 2023 23:31:03 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Mon, 03 Apr 2023 23:31:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Mon, 03 Apr 2023 23:31:03 GMT
ENV FLUENTD_CONF=fluent.conf
# Mon, 03 Apr 2023 23:31:03 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Mon, 03 Apr 2023 23:31:03 GMT
EXPOSE 24224 5140
# Mon, 03 Apr 2023 23:31:03 GMT
USER fluent
# Mon, 03 Apr 2023 23:31:03 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Mon, 03 Apr 2023 23:31:03 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b9af96d3e722e82f7629031b0987250947fbdb2a8206dccca92c1619fb8929`  
		Last Modified: Thu, 23 Mar 2023 11:19:23 GMT  
		Size: 8.9 MB (8863610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59a5c6470be792bccee1395851606bf8f724f17e1ff5739ef9263875df729f`  
		Last Modified: Thu, 23 Mar 2023 11:19:22 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad59dd1de97cd6a2c8d0f9521202d9e34c41b19728220deed1369b77dd87be66`  
		Last Modified: Thu, 30 Mar 2023 19:12:10 GMT  
		Size: 32.4 MB (32445106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4f01f7bb1614c319af053459a9cd260edc96aac21be2d49e0651aca0727dcc`  
		Last Modified: Thu, 30 Mar 2023 19:12:08 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4947e4d6ca83043a92e5549f2fee48c32fd03d7b0448c52203b178ee1df59e`  
		Last Modified: Mon, 03 Apr 2023 23:31:31 GMT  
		Size: 27.9 MB (27925787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350890baf78ab1d5caeac50183b0564d3eb0220e574f9a8a9dd8aeced4513d31`  
		Last Modified: Mon, 03 Apr 2023 23:31:28 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8decf9537301401dc59e52fd3ad9523f9315b2659c57225acf452b1d4643c8`  
		Last Modified: Mon, 03 Apr 2023 23:31:28 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5bf28f08285199ee9856ee7b66725de48925a0e36411555f33fb3f5f9de3a0`  
		Last Modified: Mon, 03 Apr 2023 23:31:28 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16.0-1.0`

```console
$ docker pull fluentd@sha256:23b2ae4235bf29886c5837dc1b0077c2cec83dc83a3f487eb87a76fe466bad5f
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
$ docker pull fluentd@sha256:001d2a51a850037c96ed3ac4fa78cbcbd1221839de5da38b6634c6e9eba86a51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 MB (24349962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880b3c4874df382cf8694342ff89e648274603b841bd70352f48306bedbbc493`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Mon, 03 Apr 2023 23:27:58 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Mon, 03 Apr 2023 23:27:59 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Mon, 03 Apr 2023 23:28:47 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Mon, 03 Apr 2023 23:28:50 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Mon, 03 Apr 2023 23:28:50 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Mon, 03 Apr 2023 23:28:50 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Mon, 03 Apr 2023 23:28:50 GMT
ENV FLUENTD_CONF=fluent.conf
# Mon, 03 Apr 2023 23:28:50 GMT
ENV LD_PRELOAD=
# Mon, 03 Apr 2023 23:28:51 GMT
EXPOSE 24224 5140
# Mon, 03 Apr 2023 23:28:51 GMT
USER fluent
# Mon, 03 Apr 2023 23:28:51 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Mon, 03 Apr 2023 23:28:51 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60ac5bd72fbffa874e5d0fe209c6a1b307198f205b8e4d5ec8f020526670649`  
		Last Modified: Mon, 03 Apr 2023 23:31:22 GMT  
		Size: 21.2 MB (21172560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a476a1392375893899c9adccc09d5de446342c3b3679c6b7d59b94001ec262d4`  
		Last Modified: Mon, 03 Apr 2023 23:31:20 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2cd03bd7b304700dfc5d69e003ba9fe11e67c6277731736c718afd73aa4fa54`  
		Last Modified: Mon, 03 Apr 2023 23:31:20 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4921fcfe9790dd687de7cfeeb8e67b1cc300da3276d37aa99171ecfbc47b6e`  
		Last Modified: Mon, 03 Apr 2023 23:31:19 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16.0-debian-1.0`

```console
$ docker pull fluentd@sha256:eda3a731a5b481a6a2575d970b13e149b5628dd0ba7e3efe6d32ded5688cca87
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
$ docker pull fluentd@sha256:c12cd975bf1d0568ac8d720d606048f7ec60b4d0473b3da010a5d7d43f769c60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101770763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43979cb0f9d95d16dce1def736679ca71ed498ddb50748bbc9e8210006675401`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 16:05:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 16:05:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 16:05:39 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 16:16:21 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:39:16 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:39:16 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:41:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:41:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:41:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:41:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:41:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:41:30 GMT
CMD ["irb"]
# Tue, 04 Apr 2023 00:22:08 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:22:08 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:22:08 GMT
ENV TINI_VERSION=0.18.0
# Tue, 04 Apr 2023 00:24:43 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:24:44 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:24:44 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:24:44 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:24:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:24:45 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 04 Apr 2023 00:24:45 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:24:45 GMT
USER fluent
# Tue, 04 Apr 2023 00:24:45 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:24:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b6c5e514e1b14fbdb31cb290dc9e714aab2152526b6807ebca5713c53cfa19`  
		Last Modified: Thu, 23 Mar 2023 16:39:55 GMT  
		Size: 10.0 MB (10023421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77fe2302da079bdc4425a38a2e8615bb9a8a19e32bd72f7d7b0b63e1831e069`  
		Last Modified: Thu, 23 Mar 2023 16:39:53 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d577fe9d8654459652bd7c69262c163ce9567c0231b5630b07ee163a73d442`  
		Last Modified: Thu, 30 Mar 2023 20:13:30 GMT  
		Size: 32.6 MB (32626154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5876e5aba0df9cbc0a632a0b86ba7972a39abb70f4bc7c98960ee470e91a82e9`  
		Last Modified: Thu, 30 Mar 2023 20:13:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed4813af1aeb4b12e2b555a3feb76c928b20075f48503177c806a8115f1d950`  
		Last Modified: Tue, 04 Apr 2023 00:25:25 GMT  
		Size: 27.7 MB (27706700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfde4897c00ce06ef4de3b267e0233d857271679a0a29ceee7fe1c5e38df994`  
		Last Modified: Tue, 04 Apr 2023 00:25:20 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07b4a64a5f37eb059c05ad7e4a294c4a641688ec6ccc9e933b3c16c5bc4967e`  
		Last Modified: Tue, 04 Apr 2023 00:25:20 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e341681ac673d148b468ebfe6c2e83fae29c359ac1aa4c29a901c77846e13e1f`  
		Last Modified: Tue, 04 Apr 2023 00:25:20 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:942fbb6ef96523333a78f5ab305c24efb3486c972067774ccb43b2deae8485af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95261905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f8ddc2c445ca2b4020d5202e9eeae14120c9c4007817d7c656d4a1e01ae85c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:44 GMT
ADD file:7595c7bfa6b3741f57a3ec7790e3108bb526244e52bb4a54548b8b5541e66616 in / 
# Thu, 23 Mar 2023 00:48:44 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:42:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 06:42:50 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 06:47:41 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:00:30 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:00:30 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:02:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:02:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:02:38 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:02:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:02:39 GMT
CMD ["irb"]
# Mon, 03 Apr 2023 23:12:15 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Mon, 03 Apr 2023 23:12:15 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Mon, 03 Apr 2023 23:12:15 GMT
ENV TINI_VERSION=0.18.0
# Mon, 03 Apr 2023 23:15:06 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Mon, 03 Apr 2023 23:15:06 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Mon, 03 Apr 2023 23:15:06 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Mon, 03 Apr 2023 23:15:07 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Mon, 03 Apr 2023 23:15:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Mon, 03 Apr 2023 23:15:07 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Mon, 03 Apr 2023 23:15:07 GMT
EXPOSE 24224 5140
# Mon, 03 Apr 2023 23:15:07 GMT
USER fluent
# Mon, 03 Apr 2023 23:15:07 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Mon, 03 Apr 2023 23:15:07 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b83d345710cdef1626d1940689dd3160e5ce3e4f63b3154cf612c52b704baa66`  
		Last Modified: Thu, 23 Mar 2023 02:22:00 GMT  
		Size: 28.9 MB (28915852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01823b006e73c4ea0cff9c35ae3dce62fc987febd01d0a092b8ac2815d5246b1`  
		Last Modified: Fri, 24 Mar 2023 23:27:15 GMT  
		Size: 8.6 MB (8635898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dbe6acaf6962399719d4c660823c56b892af485f4e2596b748c9cd0724b9c1`  
		Last Modified: Fri, 24 Mar 2023 23:27:12 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e78b20864ab83fc7e0329e406a79ade96d4f76e5b7d02518a761d09109c878a`  
		Last Modified: Thu, 30 Mar 2023 20:49:57 GMT  
		Size: 31.2 MB (31165835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6bd7652282f7fef67562600ec96645d6f69afd7148bd96fcf2338f14fda129`  
		Last Modified: Thu, 30 Mar 2023 20:49:54 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa72e0fb53c78f2bb5e28287e2564cc778a9cc3f108f60194d953d88cca93cf`  
		Last Modified: Tue, 04 Apr 2023 00:19:44 GMT  
		Size: 26.5 MB (26541244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a040e51f0d0904dc704461487f6d32a29eec953099246b328f21677ca24a4ee1`  
		Last Modified: Tue, 04 Apr 2023 00:19:40 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f970057ef53b3683906d0d7b950d6f5dd92fea0d834c0f7cdac37bea6d07606a`  
		Last Modified: Tue, 04 Apr 2023 00:19:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f608622e1770272b304b55a84eb3224200c9e19a6a80dff37b166e0eb61433b4`  
		Last Modified: Tue, 04 Apr 2023 00:19:39 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:60c1734ae51123c14ff3da6e1fce46b158c06e60c65e03b73312c02cc3e4a5f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92139379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c609296458d778df892df7fbed5920e6601c82eb3a2a37cbeb1ed5b03a709fdd`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:01:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:01:47 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 12:01:47 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 12:06:43 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:26:43 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:26:43 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:28:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:28:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:28:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:28:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:28:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:28:43 GMT
CMD ["irb"]
# Tue, 04 Apr 2023 01:28:30 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 01:28:30 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 01:28:30 GMT
ENV TINI_VERSION=0.18.0
# Tue, 04 Apr 2023 01:31:06 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 01:31:07 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 01:31:07 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 01:31:07 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 01:31:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 01:31:07 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 04 Apr 2023 01:31:07 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 01:31:08 GMT
USER fluent
# Tue, 04 Apr 2023 01:31:08 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 01:31:08 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8df912a289c6207563585bbdbcecbaf882532ee37701510780368dfc169edb`  
		Last Modified: Thu, 23 Mar 2023 12:19:16 GMT  
		Size: 8.1 MB (8145357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b732e8aacf04397c43f20b96535748cf9ff21c9d2cc823cd5ea73fb474a709`  
		Last Modified: Thu, 23 Mar 2023 12:19:14 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fa8fbb1b2b516dd2cf9e958ff8359901abc9c9f15fc83caae2a1432d18bd7d`  
		Last Modified: Thu, 30 Mar 2023 19:58:56 GMT  
		Size: 31.0 MB (31034262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed24e2ec6f169ac053b414ad28defa6f70dcc2d1cfd8d6f952a37e41d5068f94`  
		Last Modified: Thu, 30 Mar 2023 19:58:53 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709b88800c4ec9091cd0a81d713314069a2dfd8a64f2de17d88847a29e21f0b2`  
		Last Modified: Tue, 04 Apr 2023 01:32:02 GMT  
		Size: 26.4 MB (26379351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fabbe7d96726c30c69f4cfb84b225d311cc18eff3696ac74c6abb1f1d4873e9`  
		Last Modified: Tue, 04 Apr 2023 01:31:58 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6966fda14b69edd56aa16cf55261b12e2d248ef2d39a02436bee9fa47565b01e`  
		Last Modified: Tue, 04 Apr 2023 01:31:58 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d5829bb78c5a9743af48b9eeddaa0a4b2cea71f62104d7330475b429a75328`  
		Last Modified: Tue, 04 Apr 2023 01:31:59 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:a377a0a9cc406874e2542d59f0b021dbd2e52e0805f0aef76c5dfe38ed1af1a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.8 MB (98756545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b979d9f2b3ba0a2bde4fff7b8f3c106cb4dd310ba3ffb2c071374c041ce2c14c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:13:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 06:13:20 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 06:18:02 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:00:46 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:00:46 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:02:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:02:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:02:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:02:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:02:31 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:02:31 GMT
CMD ["irb"]
# Tue, 04 Apr 2023 00:33:25 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:33:25 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:33:25 GMT
ENV TINI_VERSION=0.18.0
# Tue, 04 Apr 2023 00:35:44 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:35:45 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:35:45 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:35:45 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:35:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:35:45 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 04 Apr 2023 00:35:45 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:35:45 GMT
USER fluent
# Tue, 04 Apr 2023 00:35:45 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:35:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a96a7aa954e0123803b20ac7f00cac949799f3311a00e4d7e3d3a695602041`  
		Last Modified: Thu, 23 Mar 2023 06:29:04 GMT  
		Size: 9.2 MB (9244609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a759fe3d4385aa21faa3a8c109a649c866edf763ba19bf9a83fcfbc81b5f83b`  
		Last Modified: Thu, 23 Mar 2023 06:29:03 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6718b4e09290a25827867abd642ad608ccd7a34e173092e5223e77f9d3a9ac`  
		Last Modified: Thu, 30 Mar 2023 19:28:00 GMT  
		Size: 32.0 MB (31987334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c375fb3304543819eb8392761158cd0c170fd870675038686f75c467036c05b`  
		Last Modified: Thu, 30 Mar 2023 19:27:58 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d742b5fbdf8e142a74ea6592c3605a090c720cd592ffba7006b7f51602dfda`  
		Last Modified: Tue, 04 Apr 2023 00:36:10 GMT  
		Size: 27.5 MB (27458811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a793531fadb9d0f0f03c822e8f1bb9da777bd8985aaf6151e7d56675a5f08d6a`  
		Last Modified: Tue, 04 Apr 2023 00:36:07 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cd6cff1da66f216dc1453c489497482a0718bdc9c56a66cdb11586e8d95992`  
		Last Modified: Tue, 04 Apr 2023 00:36:07 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b370bea279a69d8dd9b3fbb7c002a3b7a625912d902702fb0cc5642503948a`  
		Last Modified: Tue, 04 Apr 2023 00:36:07 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:16f27f9c7ad25a1c61e09938ffb4693a15817151360c40298717a6e92bf4357c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102159216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60cfa8383ced1d7112d6a449c9418e7c6a20e63e8fbf0388688bae43eaf9a028`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 19:56:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 19:56:26 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 19:56:27 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 20:10:20 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:04:23 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:04:23 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:07:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:07:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:07:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:07:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:07:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:07:51 GMT
CMD ["irb"]
# Tue, 04 Apr 2023 01:18:03 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 01:18:03 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 01:18:03 GMT
ENV TINI_VERSION=0.18.0
# Tue, 04 Apr 2023 01:20:55 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 01:20:56 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 01:20:56 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 01:20:56 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 01:20:56 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 01:20:56 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 04 Apr 2023 01:20:56 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 01:20:56 GMT
USER fluent
# Tue, 04 Apr 2023 01:20:56 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 01:20:57 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d164c2aa0d7283d0965068628d0acc27d38828e4403ad6735e3e5de808aa56d5`  
		Last Modified: Thu, 23 Mar 2023 20:45:00 GMT  
		Size: 12.0 MB (11998249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71f1e847ad5979318ce0c7d87e0899270ffb40d5dfb0b567f77c7d15dcf7177`  
		Last Modified: Thu, 23 Mar 2023 20:44:56 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6cd82fce682a1616d3a4ebe32da0969bb8f348a51004a01d3bddbb3ef91c16`  
		Last Modified: Thu, 30 Mar 2023 19:56:53 GMT  
		Size: 31.2 MB (31181071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d512d5a12e945ce9774e806dd7c07817f8d9ffe4346b7b2f745f2f8591677ff`  
		Last Modified: Thu, 30 Mar 2023 19:56:49 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fabc343d57028c870edc2c9ba37b8840ac34b6a40b0509a60c5bb4c2b8e57cb`  
		Last Modified: Tue, 04 Apr 2023 01:21:36 GMT  
		Size: 26.6 MB (26580545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbdaf1833816399fca88916fc01a4462ec9ab2313c7f8482059913c6d30f507`  
		Last Modified: Tue, 04 Apr 2023 01:21:31 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb32f8a7225d8f6e0d3a15c580e81d3877074fc56da4c76619ce8e68548317`  
		Last Modified: Tue, 04 Apr 2023 01:21:31 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c86302e190e0c658ba6038ef724be029687b61ca6de1c89e020800d8a2ea46`  
		Last Modified: Tue, 04 Apr 2023 01:21:31 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:6943b0c1eb48f170ba1a3f802a6a4f35f8a1e00460f234840982a6d58f8e5804
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106750429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d9bd806d9b6e26dcfd8ca76d8804ee31bdbb241b30057201d7c2b5c267090fa`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 15:51:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 15:51:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 15:51:48 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 15:59:37 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:34:08 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:34:08 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:37:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:37:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:37:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:37:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:37:57 GMT
CMD ["irb"]
# Tue, 04 Apr 2023 00:43:25 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 04 Apr 2023 00:43:26 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Tue, 04 Apr 2023 00:43:27 GMT
ENV TINI_VERSION=0.18.0
# Tue, 04 Apr 2023 00:49:37 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 04 Apr 2023 00:49:42 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 04 Apr 2023 00:49:43 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 04 Apr 2023 00:49:43 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 04 Apr 2023 00:49:44 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 04 Apr 2023 00:49:44 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 04 Apr 2023 00:49:45 GMT
EXPOSE 24224 5140
# Tue, 04 Apr 2023 00:49:45 GMT
USER fluent
# Tue, 04 Apr 2023 00:49:45 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 04 Apr 2023 00:49:46 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c068db9fac31f9b975b8b7e2f824bb1269b0b90875799e39dc34d2c11f6b59`  
		Last Modified: Thu, 23 Mar 2023 16:19:23 GMT  
		Size: 10.5 MB (10480889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b18b6f3a2a8e37b2f1a89fc1c7efdf9e4b3f06d9cd433edd35634e7ebe98dd`  
		Last Modified: Thu, 23 Mar 2023 16:19:19 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78273869b448509a48eed0c4616ff76a8af908920d5a6d177e26a7b72fb0b9cf`  
		Last Modified: Thu, 30 Mar 2023 20:06:41 GMT  
		Size: 32.8 MB (32791346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43630b1859e57542fa5c5ac0d7c59a8b775eaa1349d1982ba1d8d239dd0a4d7`  
		Last Modified: Thu, 30 Mar 2023 20:06:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c3a15d1c5c8879aa5b94dda6cd5c2393ade68b107095ef8d89b6868e3db34e`  
		Last Modified: Tue, 04 Apr 2023 00:50:24 GMT  
		Size: 28.2 MB (28187056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e329846174e34740cc31a05d048d0947a585fe7cd27a77527d29bea3316813c5`  
		Last Modified: Tue, 04 Apr 2023 00:50:17 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f946b6e9c0942f1687d2b8c88f4e0c9f140fe3d52e6f12be2eef75b128b6801e`  
		Last Modified: Tue, 04 Apr 2023 00:50:17 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e6d587f00178203b56e77a3518b747cb97a9cce5348f24c83ca97b13dc6944`  
		Last Modified: Tue, 04 Apr 2023 00:50:17 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:61575f83c479d25cf7821001a2cfa66038bf1cd8709eb94ba4dfbdcac71ecec2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98884414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10db35df468c33fe5092a52e4899849c285514a2a80b0759f64e3dc3e0e336e1`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 11:04:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:04:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Mar 2023 11:04:28 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 11:08:50 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 18:53:15 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 18:53:15 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 18:55:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 18:55:13 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 18:55:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 18:55:13 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 18:55:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 18:55:13 GMT
CMD ["irb"]
# Mon, 03 Apr 2023 23:28:56 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Mon, 03 Apr 2023 23:28:56 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Mon, 03 Apr 2023 23:28:56 GMT
ENV TINI_VERSION=0.18.0
# Mon, 03 Apr 2023 23:31:01 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Mon, 03 Apr 2023 23:31:03 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Mon, 03 Apr 2023 23:31:03 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Mon, 03 Apr 2023 23:31:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Mon, 03 Apr 2023 23:31:03 GMT
ENV FLUENTD_CONF=fluent.conf
# Mon, 03 Apr 2023 23:31:03 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Mon, 03 Apr 2023 23:31:03 GMT
EXPOSE 24224 5140
# Mon, 03 Apr 2023 23:31:03 GMT
USER fluent
# Mon, 03 Apr 2023 23:31:03 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Mon, 03 Apr 2023 23:31:03 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b9af96d3e722e82f7629031b0987250947fbdb2a8206dccca92c1619fb8929`  
		Last Modified: Thu, 23 Mar 2023 11:19:23 GMT  
		Size: 8.9 MB (8863610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59a5c6470be792bccee1395851606bf8f724f17e1ff5739ef9263875df729f`  
		Last Modified: Thu, 23 Mar 2023 11:19:22 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad59dd1de97cd6a2c8d0f9521202d9e34c41b19728220deed1369b77dd87be66`  
		Last Modified: Thu, 30 Mar 2023 19:12:10 GMT  
		Size: 32.4 MB (32445106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4f01f7bb1614c319af053459a9cd260edc96aac21be2d49e0651aca0727dcc`  
		Last Modified: Thu, 30 Mar 2023 19:12:08 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4947e4d6ca83043a92e5549f2fee48c32fd03d7b0448c52203b178ee1df59e`  
		Last Modified: Mon, 03 Apr 2023 23:31:31 GMT  
		Size: 27.9 MB (27925787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350890baf78ab1d5caeac50183b0564d3eb0220e574f9a8a9dd8aeced4513d31`  
		Last Modified: Mon, 03 Apr 2023 23:31:28 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8decf9537301401dc59e52fd3ad9523f9315b2659c57225acf452b1d4643c8`  
		Last Modified: Mon, 03 Apr 2023 23:31:28 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5bf28f08285199ee9856ee7b66725de48925a0e36411555f33fb3f5f9de3a0`  
		Last Modified: Mon, 03 Apr 2023 23:31:28 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
