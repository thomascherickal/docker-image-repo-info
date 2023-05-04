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
$ docker pull fluentd@sha256:0857028e8c231a9e04cdbab63d267350b780e5ffe27fc76cf9ca6fccc8e5d3e5
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
$ docker pull fluentd@sha256:c78365bc41ba48fb29f0221cd51d14a0a35604b522e4eba78240505d6c69a567
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101777439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c28ce6e6b605cea23e4ad5e035bcdd213a29a17e08c7b325ef95f32c1a3a93f4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:55:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:55:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 Apr 2023 09:55:24 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 10:05:33 GMT
ENV RUBY_MAJOR=3.1
# Wed, 12 Apr 2023 10:05:33 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 12 Apr 2023 10:05:33 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 12 Apr 2023 10:07:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 Apr 2023 10:07:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 Apr 2023 10:07:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 Apr 2023 10:07:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 10:07:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 12 Apr 2023 10:07:52 GMT
CMD ["irb"]
# Wed, 12 Apr 2023 23:01:06 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 12 Apr 2023 23:01:06 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 12 Apr 2023 23:01:06 GMT
ENV TINI_VERSION=0.18.0
# Wed, 12 Apr 2023 23:03:40 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 12 Apr 2023 23:03:41 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 12 Apr 2023 23:03:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 12 Apr 2023 23:03:41 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 12 Apr 2023 23:03:41 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 12 Apr 2023 23:03:42 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 12 Apr 2023 23:03:42 GMT
EXPOSE 24224 5140
# Wed, 12 Apr 2023 23:03:42 GMT
USER fluent
# Wed, 12 Apr 2023 23:03:42 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 12 Apr 2023 23:03:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2fbe3024787ee0b5651c377951f0aff1534b0cbe4e41dd25ab9c325c6402ec`  
		Last Modified: Wed, 12 Apr 2023 10:29:24 GMT  
		Size: 10.0 MB (10023454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b802f9abaf6bdf8e0c5a412a397a7c3db547b16838f0c9b9a22ed551b4784902`  
		Last Modified: Wed, 12 Apr 2023 10:29:22 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1020e00a94134fdba7c731728703eab411d92f43aeb9efdd879f2d36f87e21b5`  
		Last Modified: Wed, 12 Apr 2023 10:30:35 GMT  
		Size: 32.6 MB (32626044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c1f3e08b96c58904bdbb588b2143fa9f605c9c544a8028eaec2c650b248ae2`  
		Last Modified: Wed, 12 Apr 2023 10:30:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826f0352070bc55185698a26d65efe86e7f950300d0e91966e7ebca4c5c39b10`  
		Last Modified: Wed, 12 Apr 2023 23:03:55 GMT  
		Size: 27.7 MB (27706637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ced47b3e81b086157d80e4c3004adb25ca9d64d242914d4784be74022b5a6e`  
		Last Modified: Wed, 12 Apr 2023 23:03:51 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c58ce379f3827f18ed20468918053fa03e8e669e3c40bf96e8b0130f9b5fc5`  
		Last Modified: Wed, 12 Apr 2023 23:03:51 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bfdce9b13094a77193566103e4a181627a1c29c2d0786ead9bbab6f278ed49`  
		Last Modified: Wed, 12 Apr 2023 23:03:51 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:b98960aa32dfbee234a4a7acde918aeb9b89b7f75261cd4662523354d7d7bfb4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95248159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f02612fb5b6be9e528cc9feff67639b1385ab8a36173a0c431f8bd25b2b619ba`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 02 May 2023 22:48:53 GMT
ADD file:ca82c0d9094c1022a00b5f2157a02e1a9032aafc357a41c76c6b60bd74d25395 in / 
# Tue, 02 May 2023 22:48:53 GMT
CMD ["bash"]
# Wed, 03 May 2023 11:47:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 11:47:12 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 11:47:12 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 11:51:46 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 11:51:46 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 11:51:46 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 11:53:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 11:53:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 11:53:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 11:53:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 11:53:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 11:53:59 GMT
CMD ["irb"]
# Wed, 03 May 2023 14:08:16 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 03 May 2023 14:08:17 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 03 May 2023 14:08:17 GMT
ENV TINI_VERSION=0.18.0
# Wed, 03 May 2023 14:11:06 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 03 May 2023 14:11:07 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 03 May 2023 14:11:08 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 03 May 2023 14:11:08 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 03 May 2023 14:11:08 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 03 May 2023 14:11:08 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 03 May 2023 14:11:08 GMT
EXPOSE 24224 5140
# Wed, 03 May 2023 14:11:08 GMT
USER fluent
# Wed, 03 May 2023 14:11:09 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 03 May 2023 14:11:09 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:eb6ee5d3f82142e70aca665cea92048b1a46ff1aa5c5be47a04c27a471470c07`  
		Last Modified: Tue, 02 May 2023 22:51:25 GMT  
		Size: 28.9 MB (28903418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2520c96d75b8bbb8ca7b74094ff4ee8c41cf536df6bac998b01db4bd0935efe6`  
		Last Modified: Wed, 03 May 2023 12:03:22 GMT  
		Size: 8.6 MB (8634343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cb808d1e8f9d1f674dfe2463dc61ac8964cca0d926c771ef50a5b0d9a35ecb`  
		Last Modified: Wed, 03 May 2023 12:03:20 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4531177c93e28b694e7e317d2f2890bac6f942f7dee94878d6282471111f82f`  
		Last Modified: Wed, 03 May 2023 12:04:00 GMT  
		Size: 31.2 MB (31165955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfa7d2bcae37a40150f43a34637125411cf26751d3b7f0b59fea5bf3e03df1d`  
		Last Modified: Wed, 03 May 2023 12:03:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938a5dae69174beda90aa040f2985923b797e93fe1154694ba8485330c78475`  
		Last Modified: Wed, 03 May 2023 14:11:32 GMT  
		Size: 26.5 MB (26541369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab801154e33e362bb496df247355b272159f0a6e1f2b78803fc3f8930552bb78`  
		Last Modified: Wed, 03 May 2023 14:11:28 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505cd328058ae3f8aa615786d19c45fadc5f47d1030efe9742aa7d9d889eed51`  
		Last Modified: Wed, 03 May 2023 14:11:28 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0a09a6e328c7420072a0bce665de785c05078e85e1dfc25a29becd30ae8902`  
		Last Modified: Wed, 03 May 2023 14:11:28 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:4361ed56776d09dd7a4092fb97965c800689221b261f50008a13e62c987c745c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92142372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccb44afa17114880c0dc6b64e282e19abf4950536f258974daac3ce52baa95f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:39:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:39:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 Apr 2023 08:39:09 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:45:16 GMT
ENV RUBY_MAJOR=3.1
# Wed, 12 Apr 2023 08:45:16 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 12 Apr 2023 08:45:16 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 12 Apr 2023 08:47:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 Apr 2023 08:47:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 Apr 2023 08:47:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 Apr 2023 08:47:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:47:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 12 Apr 2023 08:47:50 GMT
CMD ["irb"]
# Wed, 12 Apr 2023 13:09:36 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 12 Apr 2023 13:09:36 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 12 Apr 2023 13:09:36 GMT
ENV TINI_VERSION=0.18.0
# Wed, 12 Apr 2023 13:12:10 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 12 Apr 2023 13:12:10 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 12 Apr 2023 13:12:11 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 12 Apr 2023 13:12:11 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 12 Apr 2023 13:12:11 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 12 Apr 2023 13:12:11 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 12 Apr 2023 13:12:11 GMT
EXPOSE 24224 5140
# Wed, 12 Apr 2023 13:12:11 GMT
USER fluent
# Wed, 12 Apr 2023 13:12:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 12 Apr 2023 13:12:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8514fc23d4c73c13fd5ee2eb64a764c5515d8964471685f56615da4543f0a92b`  
		Last Modified: Wed, 12 Apr 2023 09:05:49 GMT  
		Size: 8.1 MB (8145607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb6ef727048c9f77dd67911dc81de044d385f57265057bc5f21d684adcb3a4d`  
		Last Modified: Wed, 12 Apr 2023 09:05:46 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a32b51f5034d8b0e5303a0353824bedc686415da5b456bb691d954354eb814c`  
		Last Modified: Wed, 12 Apr 2023 09:06:40 GMT  
		Size: 31.0 MB (31035005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff330fddb9130e13fc8c5f1f3138ad95e5275c35b7975665723107a59030c506`  
		Last Modified: Wed, 12 Apr 2023 09:06:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d7b790502c1a875ef0442f51995912abea26297d82cbee2e00d099413e4700`  
		Last Modified: Wed, 12 Apr 2023 13:12:22 GMT  
		Size: 26.4 MB (26378919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbbc1a994af01f44669f34c5bf4f04faaaa5712b4259e34618c309337b940e8`  
		Last Modified: Wed, 12 Apr 2023 13:12:18 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92aa098f4701b7c3033ba6b0765ad3032a88e2350770a11af648949b527cc648`  
		Last Modified: Wed, 12 Apr 2023 13:12:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081ed5b00340296cfe023bc6b75456eabfaa152ce4d68b75e0261e5ab518a4b8`  
		Last Modified: Wed, 12 Apr 2023 13:12:18 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:193b699e259bb67fb8b2c0a0e90f5f5f7f8bec89b2f3788fe5e9cabeb3ef4604
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.7 MB (98745088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1191f22c59dfc31a502ef10396421cbdf7e1c48980ddd3c5e90f749757e4852`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 11:33:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 11:33:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 11:33:36 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 11:41:46 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 11:41:46 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 11:41:46 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 11:43:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 11:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 11:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 11:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 11:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 11:43:29 GMT
CMD ["irb"]
# Thu, 04 May 2023 03:56:11 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 04 May 2023 03:56:11 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Thu, 04 May 2023 03:56:11 GMT
ENV TINI_VERSION=0.18.0
# Thu, 04 May 2023 03:58:25 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 04 May 2023 03:58:26 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 04 May 2023 03:58:26 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 04 May 2023 03:58:26 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 04 May 2023 03:58:26 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 04 May 2023 03:58:26 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 04 May 2023 03:58:26 GMT
EXPOSE 24224 5140
# Thu, 04 May 2023 03:58:26 GMT
USER fluent
# Thu, 04 May 2023 03:58:26 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 04 May 2023 03:58:27 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c1531f71db6b0a18949b875d88c4e89771d1f342242ace07be465eaf823657`  
		Last Modified: Wed, 03 May 2023 12:00:18 GMT  
		Size: 9.2 MB (9243388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09062a3cd32c5e4b240a84c6d1b7286f252e13dd31c44688b8ef1fc66feb47ed`  
		Last Modified: Wed, 03 May 2023 12:00:15 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae0e0c21b62b4bd50e21055fb4282e3349a1877e660140f5ad2406a00e97f1f`  
		Last Modified: Wed, 03 May 2023 12:01:25 GMT  
		Size: 32.0 MB (31987241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13e53e9b73e036c9fdcc00931455984a0c2e31e51db93a901bd0fed695001f4`  
		Last Modified: Wed, 03 May 2023 12:01:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9623e92837e74a9da5c231eb0411020f385fca5eae7f931a438f344572488613`  
		Last Modified: Thu, 04 May 2023 03:58:43 GMT  
		Size: 27.5 MB (27458644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c73e35f194da853ede827b97c7ed911245b886567cd93aed37fd95c35fe8c0a`  
		Last Modified: Thu, 04 May 2023 03:58:39 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08194971e693d63e1b0314a090fcd1622e538515d4aaff3a3c6e17894ef8091b`  
		Last Modified: Thu, 04 May 2023 03:58:39 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef78c37541cdb76218f52ec857122eea42d5917e2469477371ded26f5ae17dce`  
		Last Modified: Thu, 04 May 2023 03:58:39 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:17ecb9aaff2e484d1f881062ff520b87b5412537f630257f8ddd2952627ccf9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102162439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed9f88683523d403f68b9f1ac3ec731d6c388b55be62bd099aa9a060b977212`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 21:04:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 21:04:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 Apr 2023 21:04:19 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 21:18:57 GMT
ENV RUBY_MAJOR=3.1
# Wed, 12 Apr 2023 21:18:57 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 12 Apr 2023 21:18:57 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 12 Apr 2023 21:22:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 Apr 2023 21:22:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 Apr 2023 21:22:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 Apr 2023 21:22:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 21:22:31 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 12 Apr 2023 21:22:31 GMT
CMD ["irb"]
# Thu, 13 Apr 2023 02:03:13 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 13 Apr 2023 02:03:13 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Thu, 13 Apr 2023 02:03:13 GMT
ENV TINI_VERSION=0.18.0
# Thu, 13 Apr 2023 02:06:06 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 13 Apr 2023 02:06:06 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 13 Apr 2023 02:06:06 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 13 Apr 2023 02:06:07 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 13 Apr 2023 02:06:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 13 Apr 2023 02:06:07 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 13 Apr 2023 02:06:07 GMT
EXPOSE 24224 5140
# Thu, 13 Apr 2023 02:06:07 GMT
USER fluent
# Thu, 13 Apr 2023 02:06:07 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 13 Apr 2023 02:06:07 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60077e7efe1823a2226765bd93d5612c4e7a99c40714f215b8841aa5477a53bb`  
		Last Modified: Wed, 12 Apr 2023 21:54:14 GMT  
		Size: 12.0 MB (11998376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f1e21f32e7ff416da3c752b2243c00cbbadee4611a8a3f6ab741e35ce1e1af`  
		Last Modified: Wed, 12 Apr 2023 21:54:10 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca3a6daab667419f553c1768237ed42a2d404b109882b1d3e20987730a19662`  
		Last Modified: Wed, 12 Apr 2023 21:55:28 GMT  
		Size: 31.2 MB (31181414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474c0298a0437d904e38a00ed99c6fdd5a7bcd245d6f20d8edb400f3421ad28e`  
		Last Modified: Wed, 12 Apr 2023 21:55:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a2e3c115245d9d18f5b59f2a1b595d0a495f0d0c4cd68fa21b4459ff68f782`  
		Last Modified: Thu, 13 Apr 2023 02:06:32 GMT  
		Size: 26.6 MB (26580652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb965716931696b11adeb04d43faeeeef98cc345be619032dcd6321a106401e`  
		Last Modified: Thu, 13 Apr 2023 02:06:27 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7126861aedcfb3a54b43f7d866757ff2c513b7c1d426daa59c8355d4637ef3`  
		Last Modified: Thu, 13 Apr 2023 02:06:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1c53932ac682ca7f821a219c33651aaea67feb5dc2360e6f2651e5d2eb433`  
		Last Modified: Thu, 13 Apr 2023 02:06:27 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:f9222f81590f7d7a0552addd2549114c1f1c7aee899f0c5c3ab6932875376702
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106755351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8333361d803585f3f2bd74eec8423095a100b582e373b330617ea73d97c3271`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 10:07:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 10:07:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 Apr 2023 10:07:10 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 10:18:30 GMT
ENV RUBY_MAJOR=3.1
# Wed, 12 Apr 2023 10:18:31 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 12 Apr 2023 10:18:32 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 12 Apr 2023 10:24:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 Apr 2023 10:24:56 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 Apr 2023 10:24:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 Apr 2023 10:24:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 10:25:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 12 Apr 2023 10:25:01 GMT
CMD ["irb"]
# Wed, 12 Apr 2023 22:21:40 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 12 Apr 2023 22:21:40 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 12 Apr 2023 22:21:40 GMT
ENV TINI_VERSION=0.18.0
# Wed, 12 Apr 2023 22:27:02 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 12 Apr 2023 22:27:05 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 12 Apr 2023 22:27:05 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 12 Apr 2023 22:27:05 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 12 Apr 2023 22:27:05 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 12 Apr 2023 22:27:05 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 12 Apr 2023 22:27:06 GMT
EXPOSE 24224 5140
# Wed, 12 Apr 2023 22:27:06 GMT
USER fluent
# Wed, 12 Apr 2023 22:27:06 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 12 Apr 2023 22:27:07 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfef4410d6b30c54e94e1df3e005783acd06c399fe69162f53f9bc0174fc776a`  
		Last Modified: Wed, 12 Apr 2023 10:46:39 GMT  
		Size: 10.5 MB (10481155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006ee1ba09a3296b438146b07cc3aa1a44edffd72bcd8905863b8ff79f81a8af`  
		Last Modified: Wed, 12 Apr 2023 10:46:35 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5505e99f800248bbbb8699bcef1232e5d2622afefa5c2df65ebd1fe72d61e29`  
		Last Modified: Wed, 12 Apr 2023 10:47:28 GMT  
		Size: 32.8 MB (32791745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59709a6cc035e148b5d63e4f4c335a562136f42d75f41b925b9bb2420883a97a`  
		Last Modified: Wed, 12 Apr 2023 10:47:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9409b1e2470a5bf17966523e32195a636cb376af861ba3bcccd6c6282279744d`  
		Last Modified: Wed, 12 Apr 2023 22:27:35 GMT  
		Size: 28.2 MB (28187372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eeef518dd0514329af9135a2eb0e155d498dcd7fec7c55522aac95e442057f`  
		Last Modified: Wed, 12 Apr 2023 22:27:28 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cde0d5e9ccac265746c18b13b8501130b21ec690f383e7909dee237115e046`  
		Last Modified: Wed, 12 Apr 2023 22:27:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a958bef6c1e703b5f9b164858089d712f33def6d8aefee7625f91756850e202a`  
		Last Modified: Wed, 12 Apr 2023 22:27:28 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:ca3527ace052a112aeb277bdc6487823ec291cc1127a3fff721d461db34ebc8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98891136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:363c92ee7bb6c1083cc894b57f94f5e69ae5b358eb625faa59e71c48c7c07f99`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:17:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 Apr 2023 07:17:06 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 07:21:43 GMT
ENV RUBY_MAJOR=3.1
# Wed, 12 Apr 2023 07:21:43 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 12 Apr 2023 07:21:44 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 12 Apr 2023 07:23:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 Apr 2023 07:24:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 Apr 2023 07:24:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 Apr 2023 07:24:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 07:24:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 12 Apr 2023 07:24:02 GMT
CMD ["irb"]
# Wed, 12 Apr 2023 14:03:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 12 Apr 2023 14:03:43 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 12 Apr 2023 14:03:43 GMT
ENV TINI_VERSION=0.18.0
# Wed, 12 Apr 2023 14:07:05 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 12 Apr 2023 14:07:09 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 12 Apr 2023 14:07:09 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 12 Apr 2023 14:07:09 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 12 Apr 2023 14:07:09 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 12 Apr 2023 14:07:10 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 12 Apr 2023 14:07:10 GMT
EXPOSE 24224 5140
# Wed, 12 Apr 2023 14:07:10 GMT
USER fluent
# Wed, 12 Apr 2023 14:07:10 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 12 Apr 2023 14:07:10 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee6698129be61e3b65320708e5b2c53483a49f3f996c87c93a3a290c8735bc4`  
		Last Modified: Wed, 12 Apr 2023 07:33:55 GMT  
		Size: 8.9 MB (8863585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6749b3515b44e03271a5bffd87d4da5aa83e886ed0736b4093feab7e588cc52`  
		Last Modified: Wed, 12 Apr 2023 07:33:53 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fef0d02ed6898d23f179e3bcd4e115b587ce451fb2c4f7ff78119916e6c3ca`  
		Last Modified: Wed, 12 Apr 2023 07:34:22 GMT  
		Size: 32.4 MB (32445191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b7f5f281e9640200dd2f9d23f5ad1491335f20f80a9a772a6f047f8e946a57`  
		Last Modified: Wed, 12 Apr 2023 07:34:20 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea8db7f375af1f9a6baacc675d725203c421b6f36af3e8d9cd9c373d8a2382`  
		Last Modified: Wed, 12 Apr 2023 14:07:32 GMT  
		Size: 27.9 MB (27926123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45037e6e0080f7b52f4040ecd6bf24b4edfb7a4967e4eb302a55fd1ee4ad9114`  
		Last Modified: Wed, 12 Apr 2023 14:07:28 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d634c1f580fa6ec64f5a58ba2dc97f217a8b4b6ae31121bb081a71a2aeaf5ba2`  
		Last Modified: Wed, 12 Apr 2023 14:07:28 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2664e304654c66ba6e91b0c504afa293cfbb883642ffc3b73565cd055856f87e`  
		Last Modified: Wed, 12 Apr 2023 14:07:28 GMT  
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
$ docker pull fluentd@sha256:0857028e8c231a9e04cdbab63d267350b780e5ffe27fc76cf9ca6fccc8e5d3e5
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
$ docker pull fluentd@sha256:c78365bc41ba48fb29f0221cd51d14a0a35604b522e4eba78240505d6c69a567
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101777439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c28ce6e6b605cea23e4ad5e035bcdd213a29a17e08c7b325ef95f32c1a3a93f4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:55:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:55:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 Apr 2023 09:55:24 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 10:05:33 GMT
ENV RUBY_MAJOR=3.1
# Wed, 12 Apr 2023 10:05:33 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 12 Apr 2023 10:05:33 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 12 Apr 2023 10:07:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 Apr 2023 10:07:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 Apr 2023 10:07:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 Apr 2023 10:07:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 10:07:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 12 Apr 2023 10:07:52 GMT
CMD ["irb"]
# Wed, 12 Apr 2023 23:01:06 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 12 Apr 2023 23:01:06 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 12 Apr 2023 23:01:06 GMT
ENV TINI_VERSION=0.18.0
# Wed, 12 Apr 2023 23:03:40 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 12 Apr 2023 23:03:41 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 12 Apr 2023 23:03:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 12 Apr 2023 23:03:41 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 12 Apr 2023 23:03:41 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 12 Apr 2023 23:03:42 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 12 Apr 2023 23:03:42 GMT
EXPOSE 24224 5140
# Wed, 12 Apr 2023 23:03:42 GMT
USER fluent
# Wed, 12 Apr 2023 23:03:42 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 12 Apr 2023 23:03:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2fbe3024787ee0b5651c377951f0aff1534b0cbe4e41dd25ab9c325c6402ec`  
		Last Modified: Wed, 12 Apr 2023 10:29:24 GMT  
		Size: 10.0 MB (10023454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b802f9abaf6bdf8e0c5a412a397a7c3db547b16838f0c9b9a22ed551b4784902`  
		Last Modified: Wed, 12 Apr 2023 10:29:22 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1020e00a94134fdba7c731728703eab411d92f43aeb9efdd879f2d36f87e21b5`  
		Last Modified: Wed, 12 Apr 2023 10:30:35 GMT  
		Size: 32.6 MB (32626044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c1f3e08b96c58904bdbb588b2143fa9f605c9c544a8028eaec2c650b248ae2`  
		Last Modified: Wed, 12 Apr 2023 10:30:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826f0352070bc55185698a26d65efe86e7f950300d0e91966e7ebca4c5c39b10`  
		Last Modified: Wed, 12 Apr 2023 23:03:55 GMT  
		Size: 27.7 MB (27706637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ced47b3e81b086157d80e4c3004adb25ca9d64d242914d4784be74022b5a6e`  
		Last Modified: Wed, 12 Apr 2023 23:03:51 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c58ce379f3827f18ed20468918053fa03e8e669e3c40bf96e8b0130f9b5fc5`  
		Last Modified: Wed, 12 Apr 2023 23:03:51 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bfdce9b13094a77193566103e4a181627a1c29c2d0786ead9bbab6f278ed49`  
		Last Modified: Wed, 12 Apr 2023 23:03:51 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:b98960aa32dfbee234a4a7acde918aeb9b89b7f75261cd4662523354d7d7bfb4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95248159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f02612fb5b6be9e528cc9feff67639b1385ab8a36173a0c431f8bd25b2b619ba`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 02 May 2023 22:48:53 GMT
ADD file:ca82c0d9094c1022a00b5f2157a02e1a9032aafc357a41c76c6b60bd74d25395 in / 
# Tue, 02 May 2023 22:48:53 GMT
CMD ["bash"]
# Wed, 03 May 2023 11:47:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 11:47:12 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 11:47:12 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 11:51:46 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 11:51:46 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 11:51:46 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 11:53:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 11:53:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 11:53:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 11:53:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 11:53:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 11:53:59 GMT
CMD ["irb"]
# Wed, 03 May 2023 14:08:16 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 03 May 2023 14:08:17 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 03 May 2023 14:08:17 GMT
ENV TINI_VERSION=0.18.0
# Wed, 03 May 2023 14:11:06 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 03 May 2023 14:11:07 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 03 May 2023 14:11:08 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 03 May 2023 14:11:08 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 03 May 2023 14:11:08 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 03 May 2023 14:11:08 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 03 May 2023 14:11:08 GMT
EXPOSE 24224 5140
# Wed, 03 May 2023 14:11:08 GMT
USER fluent
# Wed, 03 May 2023 14:11:09 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 03 May 2023 14:11:09 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:eb6ee5d3f82142e70aca665cea92048b1a46ff1aa5c5be47a04c27a471470c07`  
		Last Modified: Tue, 02 May 2023 22:51:25 GMT  
		Size: 28.9 MB (28903418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2520c96d75b8bbb8ca7b74094ff4ee8c41cf536df6bac998b01db4bd0935efe6`  
		Last Modified: Wed, 03 May 2023 12:03:22 GMT  
		Size: 8.6 MB (8634343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cb808d1e8f9d1f674dfe2463dc61ac8964cca0d926c771ef50a5b0d9a35ecb`  
		Last Modified: Wed, 03 May 2023 12:03:20 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4531177c93e28b694e7e317d2f2890bac6f942f7dee94878d6282471111f82f`  
		Last Modified: Wed, 03 May 2023 12:04:00 GMT  
		Size: 31.2 MB (31165955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfa7d2bcae37a40150f43a34637125411cf26751d3b7f0b59fea5bf3e03df1d`  
		Last Modified: Wed, 03 May 2023 12:03:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a938a5dae69174beda90aa040f2985923b797e93fe1154694ba8485330c78475`  
		Last Modified: Wed, 03 May 2023 14:11:32 GMT  
		Size: 26.5 MB (26541369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab801154e33e362bb496df247355b272159f0a6e1f2b78803fc3f8930552bb78`  
		Last Modified: Wed, 03 May 2023 14:11:28 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505cd328058ae3f8aa615786d19c45fadc5f47d1030efe9742aa7d9d889eed51`  
		Last Modified: Wed, 03 May 2023 14:11:28 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0a09a6e328c7420072a0bce665de785c05078e85e1dfc25a29becd30ae8902`  
		Last Modified: Wed, 03 May 2023 14:11:28 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:4361ed56776d09dd7a4092fb97965c800689221b261f50008a13e62c987c745c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92142372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccb44afa17114880c0dc6b64e282e19abf4950536f258974daac3ce52baa95f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:39:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:39:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 Apr 2023 08:39:09 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:45:16 GMT
ENV RUBY_MAJOR=3.1
# Wed, 12 Apr 2023 08:45:16 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 12 Apr 2023 08:45:16 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 12 Apr 2023 08:47:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 Apr 2023 08:47:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 Apr 2023 08:47:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 Apr 2023 08:47:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:47:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 12 Apr 2023 08:47:50 GMT
CMD ["irb"]
# Wed, 12 Apr 2023 13:09:36 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 12 Apr 2023 13:09:36 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 12 Apr 2023 13:09:36 GMT
ENV TINI_VERSION=0.18.0
# Wed, 12 Apr 2023 13:12:10 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 12 Apr 2023 13:12:10 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 12 Apr 2023 13:12:11 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 12 Apr 2023 13:12:11 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 12 Apr 2023 13:12:11 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 12 Apr 2023 13:12:11 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 12 Apr 2023 13:12:11 GMT
EXPOSE 24224 5140
# Wed, 12 Apr 2023 13:12:11 GMT
USER fluent
# Wed, 12 Apr 2023 13:12:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 12 Apr 2023 13:12:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8514fc23d4c73c13fd5ee2eb64a764c5515d8964471685f56615da4543f0a92b`  
		Last Modified: Wed, 12 Apr 2023 09:05:49 GMT  
		Size: 8.1 MB (8145607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb6ef727048c9f77dd67911dc81de044d385f57265057bc5f21d684adcb3a4d`  
		Last Modified: Wed, 12 Apr 2023 09:05:46 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a32b51f5034d8b0e5303a0353824bedc686415da5b456bb691d954354eb814c`  
		Last Modified: Wed, 12 Apr 2023 09:06:40 GMT  
		Size: 31.0 MB (31035005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff330fddb9130e13fc8c5f1f3138ad95e5275c35b7975665723107a59030c506`  
		Last Modified: Wed, 12 Apr 2023 09:06:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d7b790502c1a875ef0442f51995912abea26297d82cbee2e00d099413e4700`  
		Last Modified: Wed, 12 Apr 2023 13:12:22 GMT  
		Size: 26.4 MB (26378919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbbc1a994af01f44669f34c5bf4f04faaaa5712b4259e34618c309337b940e8`  
		Last Modified: Wed, 12 Apr 2023 13:12:18 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92aa098f4701b7c3033ba6b0765ad3032a88e2350770a11af648949b527cc648`  
		Last Modified: Wed, 12 Apr 2023 13:12:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081ed5b00340296cfe023bc6b75456eabfaa152ce4d68b75e0261e5ab518a4b8`  
		Last Modified: Wed, 12 Apr 2023 13:12:18 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:193b699e259bb67fb8b2c0a0e90f5f5f7f8bec89b2f3788fe5e9cabeb3ef4604
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.7 MB (98745088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1191f22c59dfc31a502ef10396421cbdf7e1c48980ddd3c5e90f749757e4852`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 11:33:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 11:33:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 11:33:36 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 11:41:46 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 11:41:46 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 11:41:46 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 11:43:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 11:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 11:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 11:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 11:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 11:43:29 GMT
CMD ["irb"]
# Thu, 04 May 2023 03:56:11 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 04 May 2023 03:56:11 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Thu, 04 May 2023 03:56:11 GMT
ENV TINI_VERSION=0.18.0
# Thu, 04 May 2023 03:58:25 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 04 May 2023 03:58:26 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 04 May 2023 03:58:26 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 04 May 2023 03:58:26 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 04 May 2023 03:58:26 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 04 May 2023 03:58:26 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 04 May 2023 03:58:26 GMT
EXPOSE 24224 5140
# Thu, 04 May 2023 03:58:26 GMT
USER fluent
# Thu, 04 May 2023 03:58:26 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 04 May 2023 03:58:27 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c1531f71db6b0a18949b875d88c4e89771d1f342242ace07be465eaf823657`  
		Last Modified: Wed, 03 May 2023 12:00:18 GMT  
		Size: 9.2 MB (9243388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09062a3cd32c5e4b240a84c6d1b7286f252e13dd31c44688b8ef1fc66feb47ed`  
		Last Modified: Wed, 03 May 2023 12:00:15 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae0e0c21b62b4bd50e21055fb4282e3349a1877e660140f5ad2406a00e97f1f`  
		Last Modified: Wed, 03 May 2023 12:01:25 GMT  
		Size: 32.0 MB (31987241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13e53e9b73e036c9fdcc00931455984a0c2e31e51db93a901bd0fed695001f4`  
		Last Modified: Wed, 03 May 2023 12:01:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9623e92837e74a9da5c231eb0411020f385fca5eae7f931a438f344572488613`  
		Last Modified: Thu, 04 May 2023 03:58:43 GMT  
		Size: 27.5 MB (27458644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c73e35f194da853ede827b97c7ed911245b886567cd93aed37fd95c35fe8c0a`  
		Last Modified: Thu, 04 May 2023 03:58:39 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08194971e693d63e1b0314a090fcd1622e538515d4aaff3a3c6e17894ef8091b`  
		Last Modified: Thu, 04 May 2023 03:58:39 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef78c37541cdb76218f52ec857122eea42d5917e2469477371ded26f5ae17dce`  
		Last Modified: Thu, 04 May 2023 03:58:39 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:17ecb9aaff2e484d1f881062ff520b87b5412537f630257f8ddd2952627ccf9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102162439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed9f88683523d403f68b9f1ac3ec731d6c388b55be62bd099aa9a060b977212`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 21:04:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 21:04:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 Apr 2023 21:04:19 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 21:18:57 GMT
ENV RUBY_MAJOR=3.1
# Wed, 12 Apr 2023 21:18:57 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 12 Apr 2023 21:18:57 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 12 Apr 2023 21:22:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 Apr 2023 21:22:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 Apr 2023 21:22:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 Apr 2023 21:22:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 21:22:31 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 12 Apr 2023 21:22:31 GMT
CMD ["irb"]
# Thu, 13 Apr 2023 02:03:13 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 13 Apr 2023 02:03:13 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Thu, 13 Apr 2023 02:03:13 GMT
ENV TINI_VERSION=0.18.0
# Thu, 13 Apr 2023 02:06:06 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 13 Apr 2023 02:06:06 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 13 Apr 2023 02:06:06 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 13 Apr 2023 02:06:07 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 13 Apr 2023 02:06:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 13 Apr 2023 02:06:07 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 13 Apr 2023 02:06:07 GMT
EXPOSE 24224 5140
# Thu, 13 Apr 2023 02:06:07 GMT
USER fluent
# Thu, 13 Apr 2023 02:06:07 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 13 Apr 2023 02:06:07 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60077e7efe1823a2226765bd93d5612c4e7a99c40714f215b8841aa5477a53bb`  
		Last Modified: Wed, 12 Apr 2023 21:54:14 GMT  
		Size: 12.0 MB (11998376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f1e21f32e7ff416da3c752b2243c00cbbadee4611a8a3f6ab741e35ce1e1af`  
		Last Modified: Wed, 12 Apr 2023 21:54:10 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca3a6daab667419f553c1768237ed42a2d404b109882b1d3e20987730a19662`  
		Last Modified: Wed, 12 Apr 2023 21:55:28 GMT  
		Size: 31.2 MB (31181414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474c0298a0437d904e38a00ed99c6fdd5a7bcd245d6f20d8edb400f3421ad28e`  
		Last Modified: Wed, 12 Apr 2023 21:55:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a2e3c115245d9d18f5b59f2a1b595d0a495f0d0c4cd68fa21b4459ff68f782`  
		Last Modified: Thu, 13 Apr 2023 02:06:32 GMT  
		Size: 26.6 MB (26580652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb965716931696b11adeb04d43faeeeef98cc345be619032dcd6321a106401e`  
		Last Modified: Thu, 13 Apr 2023 02:06:27 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7126861aedcfb3a54b43f7d866757ff2c513b7c1d426daa59c8355d4637ef3`  
		Last Modified: Thu, 13 Apr 2023 02:06:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1c53932ac682ca7f821a219c33651aaea67feb5dc2360e6f2651e5d2eb433`  
		Last Modified: Thu, 13 Apr 2023 02:06:27 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:f9222f81590f7d7a0552addd2549114c1f1c7aee899f0c5c3ab6932875376702
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106755351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8333361d803585f3f2bd74eec8423095a100b582e373b330617ea73d97c3271`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 10:07:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 10:07:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 Apr 2023 10:07:10 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 10:18:30 GMT
ENV RUBY_MAJOR=3.1
# Wed, 12 Apr 2023 10:18:31 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 12 Apr 2023 10:18:32 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 12 Apr 2023 10:24:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 Apr 2023 10:24:56 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 Apr 2023 10:24:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 Apr 2023 10:24:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 10:25:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 12 Apr 2023 10:25:01 GMT
CMD ["irb"]
# Wed, 12 Apr 2023 22:21:40 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 12 Apr 2023 22:21:40 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 12 Apr 2023 22:21:40 GMT
ENV TINI_VERSION=0.18.0
# Wed, 12 Apr 2023 22:27:02 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 12 Apr 2023 22:27:05 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 12 Apr 2023 22:27:05 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 12 Apr 2023 22:27:05 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 12 Apr 2023 22:27:05 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 12 Apr 2023 22:27:05 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 12 Apr 2023 22:27:06 GMT
EXPOSE 24224 5140
# Wed, 12 Apr 2023 22:27:06 GMT
USER fluent
# Wed, 12 Apr 2023 22:27:06 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 12 Apr 2023 22:27:07 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfef4410d6b30c54e94e1df3e005783acd06c399fe69162f53f9bc0174fc776a`  
		Last Modified: Wed, 12 Apr 2023 10:46:39 GMT  
		Size: 10.5 MB (10481155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006ee1ba09a3296b438146b07cc3aa1a44edffd72bcd8905863b8ff79f81a8af`  
		Last Modified: Wed, 12 Apr 2023 10:46:35 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5505e99f800248bbbb8699bcef1232e5d2622afefa5c2df65ebd1fe72d61e29`  
		Last Modified: Wed, 12 Apr 2023 10:47:28 GMT  
		Size: 32.8 MB (32791745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59709a6cc035e148b5d63e4f4c335a562136f42d75f41b925b9bb2420883a97a`  
		Last Modified: Wed, 12 Apr 2023 10:47:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9409b1e2470a5bf17966523e32195a636cb376af861ba3bcccd6c6282279744d`  
		Last Modified: Wed, 12 Apr 2023 22:27:35 GMT  
		Size: 28.2 MB (28187372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eeef518dd0514329af9135a2eb0e155d498dcd7fec7c55522aac95e442057f`  
		Last Modified: Wed, 12 Apr 2023 22:27:28 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cde0d5e9ccac265746c18b13b8501130b21ec690f383e7909dee237115e046`  
		Last Modified: Wed, 12 Apr 2023 22:27:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a958bef6c1e703b5f9b164858089d712f33def6d8aefee7625f91756850e202a`  
		Last Modified: Wed, 12 Apr 2023 22:27:28 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.0-debian-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:ca3527ace052a112aeb277bdc6487823ec291cc1127a3fff721d461db34ebc8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98891136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:363c92ee7bb6c1083cc894b57f94f5e69ae5b358eb625faa59e71c48c7c07f99`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:17:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 Apr 2023 07:17:06 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 07:21:43 GMT
ENV RUBY_MAJOR=3.1
# Wed, 12 Apr 2023 07:21:43 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 12 Apr 2023 07:21:44 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 12 Apr 2023 07:23:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 Apr 2023 07:24:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 Apr 2023 07:24:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 Apr 2023 07:24:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 07:24:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 12 Apr 2023 07:24:02 GMT
CMD ["irb"]
# Wed, 12 Apr 2023 14:03:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 12 Apr 2023 14:03:43 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 12 Apr 2023 14:03:43 GMT
ENV TINI_VERSION=0.18.0
# Wed, 12 Apr 2023 14:07:05 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 12 Apr 2023 14:07:09 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 12 Apr 2023 14:07:09 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 12 Apr 2023 14:07:09 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 12 Apr 2023 14:07:09 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 12 Apr 2023 14:07:10 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 12 Apr 2023 14:07:10 GMT
EXPOSE 24224 5140
# Wed, 12 Apr 2023 14:07:10 GMT
USER fluent
# Wed, 12 Apr 2023 14:07:10 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 12 Apr 2023 14:07:10 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee6698129be61e3b65320708e5b2c53483a49f3f996c87c93a3a290c8735bc4`  
		Last Modified: Wed, 12 Apr 2023 07:33:55 GMT  
		Size: 8.9 MB (8863585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6749b3515b44e03271a5bffd87d4da5aa83e886ed0736b4093feab7e588cc52`  
		Last Modified: Wed, 12 Apr 2023 07:33:53 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fef0d02ed6898d23f179e3bcd4e115b587ce451fb2c4f7ff78119916e6c3ca`  
		Last Modified: Wed, 12 Apr 2023 07:34:22 GMT  
		Size: 32.4 MB (32445191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b7f5f281e9640200dd2f9d23f5ad1491335f20f80a9a772a6f047f8e946a57`  
		Last Modified: Wed, 12 Apr 2023 07:34:20 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea8db7f375af1f9a6baacc675d725203c421b6f36af3e8d9cd9c373d8a2382`  
		Last Modified: Wed, 12 Apr 2023 14:07:32 GMT  
		Size: 27.9 MB (27926123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45037e6e0080f7b52f4040ecd6bf24b4edfb7a4967e4eb302a55fd1ee4ad9114`  
		Last Modified: Wed, 12 Apr 2023 14:07:28 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d634c1f580fa6ec64f5a58ba2dc97f217a8b4b6ae31121bb081a71a2aeaf5ba2`  
		Last Modified: Wed, 12 Apr 2023 14:07:28 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2664e304654c66ba6e91b0c504afa293cfbb883642ffc3b73565cd055856f87e`  
		Last Modified: Wed, 12 Apr 2023 14:07:28 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
