<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.14-1`](#fluentdv114-1)
-	[`fluentd:v1.14-debian-1`](#fluentdv114-debian-1)
-	[`fluentd:v1.14.0-1.0`](#fluentdv1140-10)
-	[`fluentd:v1.14.0-debian-1.0`](#fluentdv1140-debian-10)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:fd354af1da62b29ad3c3b8215cc9172ac6314a009292158b0055a977d3d1a799
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
$ docker pull fluentd@sha256:85a7cf3a926dd6ac0f9574e2398f6679a85dca66488d4079bbc5afe6ceaacdfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19110595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14524c6a22c2c89aa979fbae9187f5eef70e37e02664b56b0494a9dff209b686`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 00:27:53 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 00:27:53 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 00:29:08 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 00:29:09 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 00:29:09 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 00:29:10 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 00:29:10 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 00:29:10 GMT
ENV LD_PRELOAD=
# Sat, 19 Mar 2022 00:29:10 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 19 Mar 2022 00:29:10 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 00:29:11 GMT
USER fluent
# Sat, 19 Mar 2022 00:29:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 00:29:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6644cd2299ff4329647acf3ee8e556e739160eb644f3140c1d77d672f106edca`  
		Last Modified: Sat, 19 Mar 2022 00:32:40 GMT  
		Size: 16.3 MB (16291211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a0e99f864a939c91a3b504ddd1e055addd520397ed00749d496beee9063821`  
		Last Modified: Sat, 19 Mar 2022 00:32:37 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1329b03fafc23c578135dde919ed536650a3f9016668b3f3be55b6ce0a7bddc9`  
		Last Modified: Sat, 19 Mar 2022 00:32:37 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f493568ca2358618545d41cbc3b615c5a4f2acf556cf9c173ce651b3806f7b8`  
		Last Modified: Sat, 19 Mar 2022 00:32:37 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:e4fda859aa819f418607c8098260b824edab98c9dd4e5db0018b205423486e34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18392538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41d1b8773a47b107ae928101fe2f269cf4db25930a2355c0d42ff3f63ed5aad4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:19:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 17 Mar 2022 15:19:52 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 17 Mar 2022 15:21:56 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 17 Mar 2022 15:21:58 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 17 Mar 2022 15:21:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 17 Mar 2022 15:21:59 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 17 Mar 2022 15:21:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 17 Mar 2022 15:22:00 GMT
ENV LD_PRELOAD=
# Thu, 17 Mar 2022 15:22:00 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Thu, 17 Mar 2022 15:22:00 GMT
EXPOSE 24224 5140
# Thu, 17 Mar 2022 15:22:01 GMT
USER fluent
# Thu, 17 Mar 2022 15:22:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 17 Mar 2022 15:22:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7162e4502104fcb6b7003227f13340f7f2f50417bd95a1a89454e34e356f3bcd`  
		Last Modified: Thu, 17 Mar 2022 15:22:41 GMT  
		Size: 15.8 MB (15762408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ca6d3bb5a70d5243de9e35b1854f411679d66db2b3d3578bf3189ad8036306`  
		Last Modified: Thu, 17 Mar 2022 15:22:30 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b815522fc532f6fb085d4e75de7677e8033697bca03d2f82dca90481213b29`  
		Last Modified: Thu, 17 Mar 2022 15:22:30 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8eebc564eb2bd7478afb83d93af099f7a4732e7a462601ba70049ff987641a4`  
		Last Modified: Thu, 17 Mar 2022 15:22:30 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:e910670d92a778133bcf4c94e36668178273f1684214829ea81ebf26b13474d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18943945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91994bffff175ab1ea1e28434f6b78dd7343d770b96f08f23e239d60119e658`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:09:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 01:09:01 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 01:09:51 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 01:09:51 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 01:09:53 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 01:09:54 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 01:09:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 01:09:55 GMT
ENV LD_PRELOAD=
# Sat, 19 Mar 2022 01:09:56 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 19 Mar 2022 01:09:57 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 01:09:58 GMT
USER fluent
# Sat, 19 Mar 2022 01:09:59 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 01:10:00 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b16576518945a2eaa755fbc30c22597aaa148982baf8a1dfd694dfb5fb83b04`  
		Last Modified: Sat, 19 Mar 2022 01:12:55 GMT  
		Size: 16.2 MB (16222653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e650a4a5b7d0d11cc27483bc8dda61bf3a0236dc756ccef4d9a2ca2006e564`  
		Last Modified: Sat, 19 Mar 2022 01:12:52 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215c493bec56ccf55526488d336915a88c8016edd7fdbb282e120b161590e049`  
		Last Modified: Sat, 19 Mar 2022 01:12:52 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62f1bfa4d8384be6c79915a6c14a2709b484abe6f34af9cf493839c16efb9ee`  
		Last Modified: Sat, 19 Mar 2022 01:12:52 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; 386

```console
$ docker pull fluentd@sha256:6f24fb2531dc4c08c784033f02aa25f9c436dea61c36d7f70981a04c27a39c69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18622962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a4d97a7789c2de45b0d60e77478918a52789b32931edcd802f4f79a49f8912`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 16:34:42 GMT
ADD file:fbbd764c2b3ce734329c4dc8415d55b9cefc972125c5818e78698f7b894667da in / 
# Thu, 17 Mar 2022 16:34:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:36:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 17 Mar 2022 16:36:04 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 17 Mar 2022 16:37:00 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 17 Mar 2022 16:37:01 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 17 Mar 2022 16:37:01 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 17 Mar 2022 16:37:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 17 Mar 2022 16:37:01 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 17 Mar 2022 16:37:01 GMT
ENV LD_PRELOAD=
# Thu, 17 Mar 2022 16:37:01 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Thu, 17 Mar 2022 16:37:01 GMT
EXPOSE 24224 5140
# Thu, 17 Mar 2022 16:37:01 GMT
USER fluent
# Thu, 17 Mar 2022 16:37:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 17 Mar 2022 16:37:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4fcf0d6f8c0dc4a27651b1a8218d9febdd0bc510d8a2eb8474b17c87b284c5bd`  
		Last Modified: Thu, 17 Mar 2022 16:35:37 GMT  
		Size: 2.8 MB (2823620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5bf31a73f75790d59218e70a95944de87dc3ea7562e9c8caeb2898c6b50f5d`  
		Last Modified: Thu, 17 Mar 2022 16:37:35 GMT  
		Size: 15.8 MB (15797138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7a8ef36db1a7a21719acdab23a718ee6e85476bcc14c179320171964fe566`  
		Last Modified: Thu, 17 Mar 2022 16:37:32 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ae4545c2059a9e781a63b2af8676f51e165e6bf6c59a45d49c53997f04313`  
		Last Modified: Thu, 17 Mar 2022 16:37:32 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10575dfee2efac92f3ecc329cb1078b5cfb2990ac20c532c7e78444f79bb418f`  
		Last Modified: Thu, 17 Mar 2022 16:37:32 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:bf0e120dc92703bd2a52de94287f82a97c262164ae885b0d9d44bb3a2e6480cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19177525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c4f628e1f7b7a4b167dd5f832d4c639edbc6e58eda79ef64f176c600241ad8`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 18:19:00 GMT
ADD file:06587cebee2131b88da0944eb4be5128053d97f4d51a175881625be110548874 in / 
# Thu, 17 Mar 2022 18:19:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 23:10:46 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 17 Mar 2022 23:10:49 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 17 Mar 2022 23:12:11 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 17 Mar 2022 23:12:19 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 17 Mar 2022 23:12:20 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 17 Mar 2022 23:12:21 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 17 Mar 2022 23:12:24 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 17 Mar 2022 23:12:27 GMT
ENV LD_PRELOAD=
# Thu, 17 Mar 2022 23:12:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Thu, 17 Mar 2022 23:12:33 GMT
EXPOSE 24224 5140
# Thu, 17 Mar 2022 23:12:39 GMT
USER fluent
# Thu, 17 Mar 2022 23:12:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 17 Mar 2022 23:12:43 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9ba546239a73b7ff261e6813d8f1cf9e477de8825b6ae341227f315ea3a4cd51`  
		Last Modified: Thu, 17 Mar 2022 18:20:15 GMT  
		Size: 2.8 MB (2817924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891d2b4d19abb5b3d2fc74c43ee5c605524a6f365f86ca52b4c66e761a5bffdd`  
		Last Modified: Thu, 17 Mar 2022 23:13:17 GMT  
		Size: 16.4 MB (16357396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a0d9fac62ae0b8911e1de1b38f32f7a57699b17b1db3ebaa6b58f740f27850`  
		Last Modified: Thu, 17 Mar 2022 23:13:14 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0128d4a3b29ebe4f55475816da762444af03f822b54003bc63c1981eda92c4d0`  
		Last Modified: Thu, 17 Mar 2022 23:13:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b50af67a2823f45bbc7722c7c09b639478d6b36a92aa22c6b3920a1379cb808`  
		Last Modified: Thu, 17 Mar 2022 23:13:14 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:61993d0577d86b1cbd8fd038fbb3fc81fc1d87bbbebcb339974aa1a2cfec4db9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18807441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50d79707de39645031e57f48090fba44806670cc39585b0b7980198ccc470008`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 14:36:02 GMT
ADD file:cc3c2ea972c5b5d1135d0a82f5d1a6cc97fcc81f3006bb6c6b8580f1e9f4c238 in / 
# Thu, 17 Mar 2022 14:36:02 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 00:32:58 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 18 Mar 2022 00:32:58 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 18 Mar 2022 00:33:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 18 Mar 2022 00:33:40 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 18 Mar 2022 00:33:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 18 Mar 2022 00:33:41 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 18 Mar 2022 00:33:41 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 18 Mar 2022 00:33:41 GMT
ENV LD_PRELOAD=
# Fri, 18 Mar 2022 00:33:41 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 18 Mar 2022 00:33:41 GMT
EXPOSE 24224 5140
# Fri, 18 Mar 2022 00:33:41 GMT
USER fluent
# Fri, 18 Mar 2022 00:33:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 18 Mar 2022 00:33:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:3bb5875ccb136d6c7691dcf2927e52a66c831ce80fd5140d92e0a158400a4cfe`  
		Last Modified: Thu, 17 Mar 2022 14:36:53 GMT  
		Size: 2.6 MB (2606212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63aa3544cae7418c9813cee8b10188e8615768815e852f72707dcfb8540cca8`  
		Last Modified: Fri, 18 Mar 2022 00:36:08 GMT  
		Size: 16.2 MB (16199026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d5f444cc8717ced07f7ec85bd899af919e5c205e735d55c3d37384801241f`  
		Last Modified: Fri, 18 Mar 2022 00:36:07 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d8a6fb5d1349def3c489952403a43c43709ab247a2b8555646d700a515ef8d`  
		Last Modified: Fri, 18 Mar 2022 00:36:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56fce753c0aa58650cb432c407188afb53aeae214bef0be25cc94a96c04cffe`  
		Last Modified: Fri, 18 Mar 2022 00:36:06 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14-1`

```console
$ docker pull fluentd@sha256:fd354af1da62b29ad3c3b8215cc9172ac6314a009292158b0055a977d3d1a799
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.14-1` - linux; amd64

```console
$ docker pull fluentd@sha256:85a7cf3a926dd6ac0f9574e2398f6679a85dca66488d4079bbc5afe6ceaacdfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19110595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14524c6a22c2c89aa979fbae9187f5eef70e37e02664b56b0494a9dff209b686`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 00:27:53 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 00:27:53 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 00:29:08 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 00:29:09 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 00:29:09 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 00:29:10 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 00:29:10 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 00:29:10 GMT
ENV LD_PRELOAD=
# Sat, 19 Mar 2022 00:29:10 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 19 Mar 2022 00:29:10 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 00:29:11 GMT
USER fluent
# Sat, 19 Mar 2022 00:29:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 00:29:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6644cd2299ff4329647acf3ee8e556e739160eb644f3140c1d77d672f106edca`  
		Last Modified: Sat, 19 Mar 2022 00:32:40 GMT  
		Size: 16.3 MB (16291211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a0e99f864a939c91a3b504ddd1e055addd520397ed00749d496beee9063821`  
		Last Modified: Sat, 19 Mar 2022 00:32:37 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1329b03fafc23c578135dde919ed536650a3f9016668b3f3be55b6ce0a7bddc9`  
		Last Modified: Sat, 19 Mar 2022 00:32:37 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f493568ca2358618545d41cbc3b615c5a4f2acf556cf9c173ce651b3806f7b8`  
		Last Modified: Sat, 19 Mar 2022 00:32:37 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:e4fda859aa819f418607c8098260b824edab98c9dd4e5db0018b205423486e34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18392538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41d1b8773a47b107ae928101fe2f269cf4db25930a2355c0d42ff3f63ed5aad4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:19:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 17 Mar 2022 15:19:52 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 17 Mar 2022 15:21:56 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 17 Mar 2022 15:21:58 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 17 Mar 2022 15:21:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 17 Mar 2022 15:21:59 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 17 Mar 2022 15:21:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 17 Mar 2022 15:22:00 GMT
ENV LD_PRELOAD=
# Thu, 17 Mar 2022 15:22:00 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Thu, 17 Mar 2022 15:22:00 GMT
EXPOSE 24224 5140
# Thu, 17 Mar 2022 15:22:01 GMT
USER fluent
# Thu, 17 Mar 2022 15:22:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 17 Mar 2022 15:22:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7162e4502104fcb6b7003227f13340f7f2f50417bd95a1a89454e34e356f3bcd`  
		Last Modified: Thu, 17 Mar 2022 15:22:41 GMT  
		Size: 15.8 MB (15762408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ca6d3bb5a70d5243de9e35b1854f411679d66db2b3d3578bf3189ad8036306`  
		Last Modified: Thu, 17 Mar 2022 15:22:30 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b815522fc532f6fb085d4e75de7677e8033697bca03d2f82dca90481213b29`  
		Last Modified: Thu, 17 Mar 2022 15:22:30 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8eebc564eb2bd7478afb83d93af099f7a4732e7a462601ba70049ff987641a4`  
		Last Modified: Thu, 17 Mar 2022 15:22:30 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:e910670d92a778133bcf4c94e36668178273f1684214829ea81ebf26b13474d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18943945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91994bffff175ab1ea1e28434f6b78dd7343d770b96f08f23e239d60119e658`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:09:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 01:09:01 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 01:09:51 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 01:09:51 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 01:09:53 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 01:09:54 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 01:09:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 01:09:55 GMT
ENV LD_PRELOAD=
# Sat, 19 Mar 2022 01:09:56 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 19 Mar 2022 01:09:57 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 01:09:58 GMT
USER fluent
# Sat, 19 Mar 2022 01:09:59 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 01:10:00 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b16576518945a2eaa755fbc30c22597aaa148982baf8a1dfd694dfb5fb83b04`  
		Last Modified: Sat, 19 Mar 2022 01:12:55 GMT  
		Size: 16.2 MB (16222653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e650a4a5b7d0d11cc27483bc8dda61bf3a0236dc756ccef4d9a2ca2006e564`  
		Last Modified: Sat, 19 Mar 2022 01:12:52 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215c493bec56ccf55526488d336915a88c8016edd7fdbb282e120b161590e049`  
		Last Modified: Sat, 19 Mar 2022 01:12:52 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62f1bfa4d8384be6c79915a6c14a2709b484abe6f34af9cf493839c16efb9ee`  
		Last Modified: Sat, 19 Mar 2022 01:12:52 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; 386

```console
$ docker pull fluentd@sha256:6f24fb2531dc4c08c784033f02aa25f9c436dea61c36d7f70981a04c27a39c69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18622962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a4d97a7789c2de45b0d60e77478918a52789b32931edcd802f4f79a49f8912`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 16:34:42 GMT
ADD file:fbbd764c2b3ce734329c4dc8415d55b9cefc972125c5818e78698f7b894667da in / 
# Thu, 17 Mar 2022 16:34:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:36:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 17 Mar 2022 16:36:04 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 17 Mar 2022 16:37:00 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 17 Mar 2022 16:37:01 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 17 Mar 2022 16:37:01 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 17 Mar 2022 16:37:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 17 Mar 2022 16:37:01 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 17 Mar 2022 16:37:01 GMT
ENV LD_PRELOAD=
# Thu, 17 Mar 2022 16:37:01 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Thu, 17 Mar 2022 16:37:01 GMT
EXPOSE 24224 5140
# Thu, 17 Mar 2022 16:37:01 GMT
USER fluent
# Thu, 17 Mar 2022 16:37:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 17 Mar 2022 16:37:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4fcf0d6f8c0dc4a27651b1a8218d9febdd0bc510d8a2eb8474b17c87b284c5bd`  
		Last Modified: Thu, 17 Mar 2022 16:35:37 GMT  
		Size: 2.8 MB (2823620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5bf31a73f75790d59218e70a95944de87dc3ea7562e9c8caeb2898c6b50f5d`  
		Last Modified: Thu, 17 Mar 2022 16:37:35 GMT  
		Size: 15.8 MB (15797138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7a8ef36db1a7a21719acdab23a718ee6e85476bcc14c179320171964fe566`  
		Last Modified: Thu, 17 Mar 2022 16:37:32 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ae4545c2059a9e781a63b2af8676f51e165e6bf6c59a45d49c53997f04313`  
		Last Modified: Thu, 17 Mar 2022 16:37:32 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10575dfee2efac92f3ecc329cb1078b5cfb2990ac20c532c7e78444f79bb418f`  
		Last Modified: Thu, 17 Mar 2022 16:37:32 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:bf0e120dc92703bd2a52de94287f82a97c262164ae885b0d9d44bb3a2e6480cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19177525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c4f628e1f7b7a4b167dd5f832d4c639edbc6e58eda79ef64f176c600241ad8`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 18:19:00 GMT
ADD file:06587cebee2131b88da0944eb4be5128053d97f4d51a175881625be110548874 in / 
# Thu, 17 Mar 2022 18:19:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 23:10:46 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 17 Mar 2022 23:10:49 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 17 Mar 2022 23:12:11 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 17 Mar 2022 23:12:19 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 17 Mar 2022 23:12:20 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 17 Mar 2022 23:12:21 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 17 Mar 2022 23:12:24 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 17 Mar 2022 23:12:27 GMT
ENV LD_PRELOAD=
# Thu, 17 Mar 2022 23:12:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Thu, 17 Mar 2022 23:12:33 GMT
EXPOSE 24224 5140
# Thu, 17 Mar 2022 23:12:39 GMT
USER fluent
# Thu, 17 Mar 2022 23:12:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 17 Mar 2022 23:12:43 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9ba546239a73b7ff261e6813d8f1cf9e477de8825b6ae341227f315ea3a4cd51`  
		Last Modified: Thu, 17 Mar 2022 18:20:15 GMT  
		Size: 2.8 MB (2817924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891d2b4d19abb5b3d2fc74c43ee5c605524a6f365f86ca52b4c66e761a5bffdd`  
		Last Modified: Thu, 17 Mar 2022 23:13:17 GMT  
		Size: 16.4 MB (16357396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a0d9fac62ae0b8911e1de1b38f32f7a57699b17b1db3ebaa6b58f740f27850`  
		Last Modified: Thu, 17 Mar 2022 23:13:14 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0128d4a3b29ebe4f55475816da762444af03f822b54003bc63c1981eda92c4d0`  
		Last Modified: Thu, 17 Mar 2022 23:13:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b50af67a2823f45bbc7722c7c09b639478d6b36a92aa22c6b3920a1379cb808`  
		Last Modified: Thu, 17 Mar 2022 23:13:14 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; s390x

```console
$ docker pull fluentd@sha256:61993d0577d86b1cbd8fd038fbb3fc81fc1d87bbbebcb339974aa1a2cfec4db9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18807441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50d79707de39645031e57f48090fba44806670cc39585b0b7980198ccc470008`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 14:36:02 GMT
ADD file:cc3c2ea972c5b5d1135d0a82f5d1a6cc97fcc81f3006bb6c6b8580f1e9f4c238 in / 
# Thu, 17 Mar 2022 14:36:02 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 00:32:58 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 18 Mar 2022 00:32:58 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 18 Mar 2022 00:33:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 18 Mar 2022 00:33:40 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 18 Mar 2022 00:33:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 18 Mar 2022 00:33:41 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 18 Mar 2022 00:33:41 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 18 Mar 2022 00:33:41 GMT
ENV LD_PRELOAD=
# Fri, 18 Mar 2022 00:33:41 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 18 Mar 2022 00:33:41 GMT
EXPOSE 24224 5140
# Fri, 18 Mar 2022 00:33:41 GMT
USER fluent
# Fri, 18 Mar 2022 00:33:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 18 Mar 2022 00:33:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:3bb5875ccb136d6c7691dcf2927e52a66c831ce80fd5140d92e0a158400a4cfe`  
		Last Modified: Thu, 17 Mar 2022 14:36:53 GMT  
		Size: 2.6 MB (2606212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63aa3544cae7418c9813cee8b10188e8615768815e852f72707dcfb8540cca8`  
		Last Modified: Fri, 18 Mar 2022 00:36:08 GMT  
		Size: 16.2 MB (16199026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d5f444cc8717ced07f7ec85bd899af919e5c205e735d55c3d37384801241f`  
		Last Modified: Fri, 18 Mar 2022 00:36:07 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d8a6fb5d1349def3c489952403a43c43709ab247a2b8555646d700a515ef8d`  
		Last Modified: Fri, 18 Mar 2022 00:36:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56fce753c0aa58650cb432c407188afb53aeae214bef0be25cc94a96c04cffe`  
		Last Modified: Fri, 18 Mar 2022 00:36:06 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14-debian-1`

```console
$ docker pull fluentd@sha256:f9569ad07e89ae356af491d952804b2da6da23243cb921446c2fdd1f7d93ae15
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

### `fluentd:v1.14-debian-1` - linux; amd64

```console
$ docker pull fluentd@sha256:19704111ce24d89d45a14b4781e92d299861ae0053f03093f9271ef603abaeac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83265241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8567bad1c8085e3f6ddd58fe5754d7f8af8b104d7bdb1fccc3c1166e06a147b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 14:22:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 14:22:03 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 14:22:03 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 15:04:19 GMT
ENV RUBY_MAJOR=2.6
# Thu, 17 Mar 2022 15:04:19 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 17 Mar 2022 15:04:19 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 17 Mar 2022 15:07:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 15:07:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 15:07:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 15:07:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 15:07:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 15:07:53 GMT
CMD ["irb"]
# Sat, 19 Mar 2022 00:29:17 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 00:29:17 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 00:29:17 GMT
ENV TINI_VERSION=0.18.0
# Sat, 19 Mar 2022 00:32:10 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 00:32:11 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 00:32:12 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 00:32:12 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 00:32:12 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 00:32:12 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 19 Mar 2022 00:32:12 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 00:32:13 GMT
USER fluent
# Sat, 19 Mar 2022 00:32:13 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 00:32:13 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6926507f0c42f3a6c331883516b206192554825a66b3a50f810066c1ad462ab`  
		Last Modified: Thu, 17 Mar 2022 15:15:08 GMT  
		Size: 12.6 MB (12565221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313590c65c28ee93cfccdb8ac3e921c5d59907d6d12807c456aa3a7c5f8c0063`  
		Last Modified: Thu, 17 Mar 2022 15:15:05 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e053d243045b4f6ed7df71bf8746f3f53446be797fb847810da6676c43acb6ba`  
		Last Modified: Thu, 17 Mar 2022 15:18:16 GMT  
		Size: 21.5 MB (21499146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda74560c5216c0d63269e9ee8b25973cfbb9c31d0fc705b5311e74d31e7d0c7`  
		Last Modified: Thu, 17 Mar 2022 15:18:13 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd52317b42c718eb3ca3c23aac3182b84af13b0b5ee7ea9f0afaa0b07ec1d96`  
		Last Modified: Sat, 19 Mar 2022 00:32:58 GMT  
		Size: 22.0 MB (22043959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da20f040f6c64521aac7c44b7a80c12f7418991d052481eb28f115e28bc66ff2`  
		Last Modified: Sat, 19 Mar 2022 00:32:54 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd4cf9a45e6b88e631d51aabb173b7efdf627eee40609e7564340c6d7f1e48b`  
		Last Modified: Sat, 19 Mar 2022 00:32:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d062d3309027ee0211964be0b889ef980d8aff25d14a51a79915ec415dba3fdf`  
		Last Modified: Sat, 19 Mar 2022 00:32:53 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:3db9ae6ab0ec26366328eea8792f54c61638060ffc254f9df91b6cece885373c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77190331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dd4dae9b4e0ed6df610f5633302e2aefffafec097fafb0eeb98b394624d47e1`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 05:20:46 GMT
ADD file:4b7bce60b3e3455ba9b14c881ffa61187b9e56365fe4f275ee871e7c7e930fb9 in / 
# Thu, 17 Mar 2022 05:20:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:18:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:18:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 18:18:28 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 18:52:17 GMT
ENV RUBY_MAJOR=2.6
# Thu, 17 Mar 2022 18:52:17 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 17 Mar 2022 18:52:17 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 17 Mar 2022 18:57:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 18:57:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 18:57:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 18:57:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 18:57:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 18:57:04 GMT
CMD ["irb"]
# Fri, 18 Mar 2022 06:44:35 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 18 Mar 2022 06:44:35 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 18 Mar 2022 06:44:36 GMT
ENV TINI_VERSION=0.18.0
# Fri, 18 Mar 2022 06:48:23 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 18 Mar 2022 06:48:25 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 18 Mar 2022 06:48:25 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 18 Mar 2022 06:48:25 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 18 Mar 2022 06:48:26 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 18 Mar 2022 06:48:26 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 18 Mar 2022 06:48:27 GMT
EXPOSE 24224 5140
# Fri, 18 Mar 2022 06:48:27 GMT
USER fluent
# Fri, 18 Mar 2022 06:48:27 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 18 Mar 2022 06:48:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f193682138b0c37054cb843ef2155a75706f248a369d454bf6444833f120aefc`  
		Last Modified: Thu, 17 Mar 2022 05:36:29 GMT  
		Size: 24.9 MB (24886195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96710cd49a7971b2d375ed6a4e2b9b3c346ddd6eccddcf626a6a5952d4761371`  
		Last Modified: Thu, 17 Mar 2022 19:03:43 GMT  
		Size: 10.3 MB (10348954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea873326987bb8e6add742f0b299995920760d1a154732afb6605f8277c9268b`  
		Last Modified: Thu, 17 Mar 2022 19:03:37 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276ce2af224d310feb9f5da35024a81eb52b8461d367afabc86b0a9a0aff5279`  
		Last Modified: Thu, 17 Mar 2022 19:07:01 GMT  
		Size: 20.8 MB (20760669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43daaa31cb2e5f713c9f9528600d3b12e0710ded0430e8e8459d5df7b2c45c6d`  
		Last Modified: Thu, 17 Mar 2022 19:06:55 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068b2c583821bde0697cc28355b09c1fdd5afeb609789a9f0f0f3be506eca50d`  
		Last Modified: Fri, 18 Mar 2022 06:49:06 GMT  
		Size: 21.2 MB (21191439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7fd1b37d2a2c3e8b32391a45bbca60212587c64795deb46d1620834855d741`  
		Last Modified: Fri, 18 Mar 2022 06:48:53 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021b1b23f9798aa027b1bc35a36c30be781ddd86d7c2d4f6eb60ad9a1236b9f6`  
		Last Modified: Fri, 18 Mar 2022 06:48:53 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b1dd181b7f0e8acb30c0b33fe8da226fe9b2636f12d6b15d1af6582aeb28a9`  
		Last Modified: Fri, 18 Mar 2022 06:48:53 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:f904b1ae959c7954d8bd5643a4250bc85504f6620e5498b68105c3941354f5e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74379752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3463f2bd661dc679cfcf240e4391c32726b99a867b17b6eec08c191e2396406`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 09:32:07 GMT
ADD file:ca7a6b7c138de7fd85996719398396d0ed0f059d2e12b7f401cd460b64924e25 in / 
# Thu, 17 Mar 2022 09:32:08 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 12:41:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 12:41:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 18 Mar 2022 12:41:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 13:35:23 GMT
ENV RUBY_MAJOR=2.6
# Fri, 18 Mar 2022 13:35:23 GMT
ENV RUBY_VERSION=2.6.9
# Fri, 18 Mar 2022 13:35:24 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Fri, 18 Mar 2022 13:39:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 18 Mar 2022 13:39:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 18 Mar 2022 13:39:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 18 Mar 2022 13:39:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 13:39:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 18 Mar 2022 13:39:33 GMT
CMD ["irb"]
# Sun, 20 Mar 2022 09:09:13 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 20 Mar 2022 09:09:13 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sun, 20 Mar 2022 09:09:13 GMT
ENV TINI_VERSION=0.18.0
# Sun, 20 Mar 2022 09:12:44 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sun, 20 Mar 2022 09:12:46 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 20 Mar 2022 09:12:47 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 20 Mar 2022 09:12:47 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sun, 20 Mar 2022 09:12:48 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 20 Mar 2022 09:12:48 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 20 Mar 2022 09:12:48 GMT
EXPOSE 24224 5140
# Sun, 20 Mar 2022 09:12:49 GMT
USER fluent
# Sun, 20 Mar 2022 09:12:49 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 20 Mar 2022 09:12:50 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:0b8f06901fc5e8a29999e260b4ada4ee1cc4415e5c1a16fb7bb21cc2ac995f72`  
		Last Modified: Thu, 17 Mar 2022 09:48:01 GMT  
		Size: 22.8 MB (22754389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e124b65386fabaa7971619254cd2a043e78822adbf73cfa2c62da8c24234c5`  
		Last Modified: Fri, 18 Mar 2022 13:55:07 GMT  
		Size: 9.9 MB (9872973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5f8cac5fcdd0784685b4345eab21f5c830506856ea662bf8350910342a9879`  
		Last Modified: Fri, 18 Mar 2022 13:55:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a22cd6de0a91cbeda83286381b7663d16909fd6bcbf7cb585c36b74d328792`  
		Last Modified: Fri, 18 Mar 2022 14:01:38 GMT  
		Size: 20.7 MB (20672454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb84945ecd110d2d4af4eaa754a47177bf1fe86d9ebb79bdc603574c766bdf42`  
		Last Modified: Fri, 18 Mar 2022 14:01:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c33b15ce03f39f4681baa49a263b8cbe84b1a0f65e8a883056c99e9058df84`  
		Last Modified: Sun, 20 Mar 2022 09:13:27 GMT  
		Size: 21.1 MB (21076855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a42ff1f0f2f7adf14b8f4448ee045402e10950e44479de44207da88b59efdc`  
		Last Modified: Sun, 20 Mar 2022 09:13:14 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06b63d3bb55154ad9fbc8d8c93d648f5318155b0093a0b746417d730c2b6e62`  
		Last Modified: Sun, 20 Mar 2022 09:13:14 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ab1fdc8c85ae73c087789092f5a3b81dbf6053e2b6f14d6db39525342703b8`  
		Last Modified: Sun, 20 Mar 2022 09:13:14 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:29636a8080218de95dde668117a39869f9391ac4e4b62825584222af7ef3b9e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80137340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c913a0d5d56221cf4add568faaefa1143cb599778a7c122eb0fb28ce6762fdf`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:22 GMT
ADD file:1c7d8cedf5dc79c676acebde5252ecd3005088a9f29e5e6be547f659f41efb1f in / 
# Thu, 17 Mar 2022 03:22:22 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:14:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:14:05 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 20:14:06 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 20:42:06 GMT
ENV RUBY_MAJOR=2.6
# Thu, 17 Mar 2022 20:42:07 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 17 Mar 2022 20:42:08 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 17 Mar 2022 20:43:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 20:43:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 20:43:54 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 20:43:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 20:43:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 20:43:57 GMT
CMD ["irb"]
# Sat, 19 Mar 2022 01:10:13 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 01:10:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 01:10:15 GMT
ENV TINI_VERSION=0.18.0
# Sat, 19 Mar 2022 01:12:25 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 01:12:26 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 01:12:28 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 01:12:29 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 01:12:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 01:12:30 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 19 Mar 2022 01:12:31 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 01:12:32 GMT
USER fluent
# Sat, 19 Mar 2022 01:12:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 01:12:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c9277cac12165646c33f028489f2a5be3f70745382f4385cd9ed12fcc8cec183`  
		Last Modified: Thu, 17 Mar 2022 03:29:27 GMT  
		Size: 25.9 MB (25923233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba00919e9bc7af9af691a92dbfeef3ca40c29e924ff156b705f3d8168caf7f28`  
		Last Modified: Thu, 17 Mar 2022 20:51:59 GMT  
		Size: 11.3 MB (11261791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026504a0d60799aae9f35f23d7dbcaadfe16543f13e4f4ed3a811e62444a5151`  
		Last Modified: Thu, 17 Mar 2022 20:51:57 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a563dab2ef6f5725b78f1be860ffdf8d17ec19437ebde3c38028a2d3a41819c4`  
		Last Modified: Thu, 17 Mar 2022 20:56:21 GMT  
		Size: 21.1 MB (21124122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acba3b3cc2ff6d8b3fc5caf5f067e01ab6c067e42e0ba9e45f2e29024dda415f`  
		Last Modified: Thu, 17 Mar 2022 20:56:20 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf899d6e3eebc4a69a9bbd9b336c652d423c176c8c143ff0f94380a635b69dc`  
		Last Modified: Sat, 19 Mar 2022 01:13:12 GMT  
		Size: 21.8 MB (21825286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77aedd26ea26794103542ae1cdc310163ff0fa78d9087d059a894a8a0fcdce2`  
		Last Modified: Sat, 19 Mar 2022 01:13:09 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed5d47f74e05007554bb6dacae4b76321ebe03ce115a82aec11861760716c1b`  
		Last Modified: Sat, 19 Mar 2022 01:13:09 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b519482b8eb854ea5a6acae5f81b2505780475832bc7ab9716d1cfb4ca23e7a4`  
		Last Modified: Sat, 19 Mar 2022 01:13:09 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:c6654d0995f5529a1ee0c73574fa8e069c6c1b905ff56b49214c46dbdf6fd822
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87207527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e9205b484a18dcaff31eb4dcf0adcd501aa68bacabdf6d2699c97407c561c9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 08:16:28 GMT
ADD file:39b40ec7bd2f4e691b74f0287e43ab64ef32f99953e606d9e4b72d058659209c in / 
# Thu, 17 Mar 2022 08:16:29 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:12:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:12:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 20:12:02 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 21:13:32 GMT
ENV RUBY_MAJOR=2.6
# Thu, 17 Mar 2022 21:13:32 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 17 Mar 2022 21:13:32 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 17 Mar 2022 21:16:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 21:16:40 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 21:16:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 21:16:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 21:16:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 21:16:42 GMT
CMD ["irb"]
# Sat, 19 Mar 2022 03:17:31 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 03:17:31 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 03:17:31 GMT
ENV TINI_VERSION=0.18.0
# Sat, 19 Mar 2022 03:20:14 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 03:20:15 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 03:20:16 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 03:20:16 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 03:20:16 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 03:20:16 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 19 Mar 2022 03:20:16 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 03:20:17 GMT
USER fluent
# Sat, 19 Mar 2022 03:20:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 03:20:17 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:cef703cf0f3e19a7a5f8b305254c02563c8b07f5b842bb99741d3a2fd136e9f0`  
		Last Modified: Thu, 17 Mar 2022 08:24:59 GMT  
		Size: 27.8 MB (27804570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d1be88d2bd084f4a940d09972670c3fbe0c8ff5f6bd8902cf38d5218936b1a`  
		Last Modified: Thu, 17 Mar 2022 21:32:17 GMT  
		Size: 17.2 MB (17227109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaa7cd53192f660e18ef91319a055c5b3707261611a57b78727979d53ab6c12`  
		Last Modified: Thu, 17 Mar 2022 21:32:08 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145c5c16a3403918434c329c288afbe389e2bb96de28aada5bbdf5f40b4e8e45`  
		Last Modified: Thu, 17 Mar 2022 21:37:57 GMT  
		Size: 20.9 MB (20941789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad64dcea1035bb20c285a27b8c7e7c40f7f92accbccde17ef8101ff1bde2d8`  
		Last Modified: Thu, 17 Mar 2022 21:37:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c4ad77a25ad255cc29257cc074e5b3ef7fe868c9bd34a4716fbeb37ac2915b`  
		Last Modified: Sat, 19 Mar 2022 03:20:54 GMT  
		Size: 21.2 MB (21230979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96104ea9b08b62c8c998499cfb51a3e56aa5a8c7b9bec11f0a37e92b17c0daf1`  
		Last Modified: Sat, 19 Mar 2022 03:20:47 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9e48c5c45b15b3f1c04283388849874a40e70c651dc349d4b364d131690f26`  
		Last Modified: Sat, 19 Mar 2022 03:20:47 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e439f7c1adf49b9d5e045c414e29682ece7625a72f8fdbba816277ed9026d1f`  
		Last Modified: Sat, 19 Mar 2022 03:20:47 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:0b4bb8f3966d815a30a8bca6a7fb11ce0fb309fa31def741771c94fce72c34ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87911471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5656fc0bada313f656bc91d9adf09b22f1dca892dd4fb14c2914ba650477d9bb`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 11:19:08 GMT
ADD file:0af430b7759619d4d40ea316f823599879e4f3e0dfc8877bdee731020fb2620d in / 
# Thu, 17 Mar 2022 11:19:12 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:17:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:17:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 18 Mar 2022 09:17:56 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 11:05:30 GMT
ENV RUBY_MAJOR=2.6
# Fri, 18 Mar 2022 11:05:34 GMT
ENV RUBY_VERSION=2.6.9
# Fri, 18 Mar 2022 11:05:38 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Fri, 18 Mar 2022 11:13:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 18 Mar 2022 11:13:26 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 18 Mar 2022 11:13:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 18 Mar 2022 11:13:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 11:13:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 18 Mar 2022 11:13:40 GMT
CMD ["irb"]
# Sat, 19 Mar 2022 18:30:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 18:30:12 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 18:30:14 GMT
ENV TINI_VERSION=0.18.0
# Sat, 19 Mar 2022 18:35:01 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 18:35:13 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 18:35:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 18:35:15 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 18:35:16 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 18:35:18 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 19 Mar 2022 18:35:19 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 18:35:21 GMT
USER fluent
# Sat, 19 Mar 2022 18:35:23 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 18:35:26 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:303d92340e7868a8dc0fdad5d6c67a8a819a74a2bc47038b26339d5be6084bf4`  
		Last Modified: Thu, 17 Mar 2022 11:29:21 GMT  
		Size: 30.6 MB (30562350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f66151a771365bde67fd17be685cf1fdf64ec564de1ea1abd21857163d3fa1`  
		Last Modified: Fri, 18 Mar 2022 11:26:21 GMT  
		Size: 12.7 MB (12705799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8a13186fd38729296916af6473c01e211b70d1902e2a80bc6a07d483fc1299`  
		Last Modified: Fri, 18 Mar 2022 11:26:18 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea1311e913eb785a25b51326f66155d23ca19d8d39fc3198235e5a60a6ee1fa`  
		Last Modified: Fri, 18 Mar 2022 11:31:40 GMT  
		Size: 22.0 MB (22023538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6137c1e5318bf29cb971d297d077b165550a089e613b19261ae764f6345cf8a3`  
		Last Modified: Fri, 18 Mar 2022 11:31:37 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66fc3b375d01b37084effe219f7ba7a84a0949cf1eebc9dc849d23a27a7fd8c`  
		Last Modified: Sat, 19 Mar 2022 18:35:57 GMT  
		Size: 22.6 MB (22616699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d37d0dfb87e2ca2a2edd4acdbcc933de9fe98f98cd99f5c98c55a16794e63af`  
		Last Modified: Sat, 19 Mar 2022 18:35:53 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9eae5fc2113db7f125fbdf264974b9502f31bc6490cf1e9c1c4dafc34838831`  
		Last Modified: Sat, 19 Mar 2022 18:35:53 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e53b545c7e35959341a16ce01a764efe19ac0f40e75c052345990c23ed7ef`  
		Last Modified: Sat, 19 Mar 2022 18:35:53 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:3a90c942b177cb13756425e208acab692d97dbf43aad209ea6442092d002b365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80458771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf4fe7f6447b0debb6e1fb832c9354933900f15e603b99e0efb12cfabb4bfda9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 03:07:30 GMT
ADD file:4342e1d9db757e91953273ac7120c9d6004d38281f9cea830898b4f35ca43517 in / 
# Thu, 17 Mar 2022 03:07:32 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 15:49:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 15:49:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 15:49:57 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 16:14:13 GMT
ENV RUBY_MAJOR=2.6
# Thu, 17 Mar 2022 16:14:13 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 17 Mar 2022 16:14:13 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 17 Mar 2022 16:15:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 16:15:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 16:15:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 16:15:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 16:15:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 16:15:55 GMT
CMD ["irb"]
# Fri, 18 Mar 2022 00:33:48 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 18 Mar 2022 00:33:48 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 18 Mar 2022 00:33:49 GMT
ENV TINI_VERSION=0.18.0
# Fri, 18 Mar 2022 00:35:39 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 18 Mar 2022 00:35:43 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 18 Mar 2022 00:35:43 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 18 Mar 2022 00:35:43 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 18 Mar 2022 00:35:44 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 18 Mar 2022 00:35:44 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 18 Mar 2022 00:35:44 GMT
EXPOSE 24224 5140
# Fri, 18 Mar 2022 00:35:44 GMT
USER fluent
# Fri, 18 Mar 2022 00:35:44 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 18 Mar 2022 00:35:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6f8a08956872b0f67802da3a67e007322eb963a60e0dadd736077f3ece414e1f`  
		Last Modified: Thu, 17 Mar 2022 03:13:18 GMT  
		Size: 25.8 MB (25769076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9cef5c82f53c076a6b79c5df66e5aa85afd14eb4dfee12b48f9f24590f5787`  
		Last Modified: Thu, 17 Mar 2022 16:23:24 GMT  
		Size: 10.8 MB (10815376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d0a7487845abb7f24bbfa9fbfa7aa7ba2db74064de78c2e76a6d43cfa13400`  
		Last Modified: Thu, 17 Mar 2022 16:23:22 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702d01f5776fca30cdbaef386ecb99e95ca20dee02f34af3fed94fed7be0f2ec`  
		Last Modified: Thu, 17 Mar 2022 16:27:21 GMT  
		Size: 21.6 MB (21644656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d77a06b5cd31cc88689cceaef7cd57c02be52fe13b0d38812b774c6539b06c3`  
		Last Modified: Thu, 17 Mar 2022 16:27:19 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdec0ae49272d2bbb77c9403aba90515b89f9e2feceeefeedb9c4ca20eb5d0e8`  
		Last Modified: Fri, 18 Mar 2022 00:36:20 GMT  
		Size: 22.2 MB (22226575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beebf7abb9f7775a04208dbd334e979d2417387915102cbbc63cf64ffd4258f`  
		Last Modified: Fri, 18 Mar 2022 00:36:18 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da45a2d2559a73512e216762607fc94b2da86908de7e7f85c18dd3aeea5e5ea`  
		Last Modified: Fri, 18 Mar 2022 00:36:18 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc90b6341089328ac6b17480fa9f33202d719f1ec3f9dfe69400edec8c3e8a80`  
		Last Modified: Fri, 18 Mar 2022 00:36:18 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14.0-1.0`

```console
$ docker pull fluentd@sha256:fd354af1da62b29ad3c3b8215cc9172ac6314a009292158b0055a977d3d1a799
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.14.0-1.0` - linux; amd64

```console
$ docker pull fluentd@sha256:85a7cf3a926dd6ac0f9574e2398f6679a85dca66488d4079bbc5afe6ceaacdfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19110595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14524c6a22c2c89aa979fbae9187f5eef70e37e02664b56b0494a9dff209b686`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 00:27:53 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 00:27:53 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 00:29:08 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 00:29:09 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 00:29:09 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 00:29:10 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 00:29:10 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 00:29:10 GMT
ENV LD_PRELOAD=
# Sat, 19 Mar 2022 00:29:10 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 19 Mar 2022 00:29:10 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 00:29:11 GMT
USER fluent
# Sat, 19 Mar 2022 00:29:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 00:29:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6644cd2299ff4329647acf3ee8e556e739160eb644f3140c1d77d672f106edca`  
		Last Modified: Sat, 19 Mar 2022 00:32:40 GMT  
		Size: 16.3 MB (16291211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a0e99f864a939c91a3b504ddd1e055addd520397ed00749d496beee9063821`  
		Last Modified: Sat, 19 Mar 2022 00:32:37 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1329b03fafc23c578135dde919ed536650a3f9016668b3f3be55b6ce0a7bddc9`  
		Last Modified: Sat, 19 Mar 2022 00:32:37 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f493568ca2358618545d41cbc3b615c5a4f2acf556cf9c173ce651b3806f7b8`  
		Last Modified: Sat, 19 Mar 2022 00:32:37 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:e4fda859aa819f418607c8098260b824edab98c9dd4e5db0018b205423486e34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18392538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41d1b8773a47b107ae928101fe2f269cf4db25930a2355c0d42ff3f63ed5aad4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:19:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 17 Mar 2022 15:19:52 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 17 Mar 2022 15:21:56 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 17 Mar 2022 15:21:58 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 17 Mar 2022 15:21:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 17 Mar 2022 15:21:59 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 17 Mar 2022 15:21:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 17 Mar 2022 15:22:00 GMT
ENV LD_PRELOAD=
# Thu, 17 Mar 2022 15:22:00 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Thu, 17 Mar 2022 15:22:00 GMT
EXPOSE 24224 5140
# Thu, 17 Mar 2022 15:22:01 GMT
USER fluent
# Thu, 17 Mar 2022 15:22:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 17 Mar 2022 15:22:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7162e4502104fcb6b7003227f13340f7f2f50417bd95a1a89454e34e356f3bcd`  
		Last Modified: Thu, 17 Mar 2022 15:22:41 GMT  
		Size: 15.8 MB (15762408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ca6d3bb5a70d5243de9e35b1854f411679d66db2b3d3578bf3189ad8036306`  
		Last Modified: Thu, 17 Mar 2022 15:22:30 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b815522fc532f6fb085d4e75de7677e8033697bca03d2f82dca90481213b29`  
		Last Modified: Thu, 17 Mar 2022 15:22:30 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8eebc564eb2bd7478afb83d93af099f7a4732e7a462601ba70049ff987641a4`  
		Last Modified: Thu, 17 Mar 2022 15:22:30 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:e910670d92a778133bcf4c94e36668178273f1684214829ea81ebf26b13474d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18943945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91994bffff175ab1ea1e28434f6b78dd7343d770b96f08f23e239d60119e658`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:09:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 01:09:01 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 01:09:51 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 01:09:51 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 01:09:53 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 01:09:54 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 01:09:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 01:09:55 GMT
ENV LD_PRELOAD=
# Sat, 19 Mar 2022 01:09:56 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 19 Mar 2022 01:09:57 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 01:09:58 GMT
USER fluent
# Sat, 19 Mar 2022 01:09:59 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 01:10:00 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b16576518945a2eaa755fbc30c22597aaa148982baf8a1dfd694dfb5fb83b04`  
		Last Modified: Sat, 19 Mar 2022 01:12:55 GMT  
		Size: 16.2 MB (16222653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e650a4a5b7d0d11cc27483bc8dda61bf3a0236dc756ccef4d9a2ca2006e564`  
		Last Modified: Sat, 19 Mar 2022 01:12:52 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215c493bec56ccf55526488d336915a88c8016edd7fdbb282e120b161590e049`  
		Last Modified: Sat, 19 Mar 2022 01:12:52 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62f1bfa4d8384be6c79915a6c14a2709b484abe6f34af9cf493839c16efb9ee`  
		Last Modified: Sat, 19 Mar 2022 01:12:52 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:6f24fb2531dc4c08c784033f02aa25f9c436dea61c36d7f70981a04c27a39c69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18622962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a4d97a7789c2de45b0d60e77478918a52789b32931edcd802f4f79a49f8912`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 16:34:42 GMT
ADD file:fbbd764c2b3ce734329c4dc8415d55b9cefc972125c5818e78698f7b894667da in / 
# Thu, 17 Mar 2022 16:34:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:36:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 17 Mar 2022 16:36:04 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 17 Mar 2022 16:37:00 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 17 Mar 2022 16:37:01 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 17 Mar 2022 16:37:01 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 17 Mar 2022 16:37:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 17 Mar 2022 16:37:01 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 17 Mar 2022 16:37:01 GMT
ENV LD_PRELOAD=
# Thu, 17 Mar 2022 16:37:01 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Thu, 17 Mar 2022 16:37:01 GMT
EXPOSE 24224 5140
# Thu, 17 Mar 2022 16:37:01 GMT
USER fluent
# Thu, 17 Mar 2022 16:37:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 17 Mar 2022 16:37:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4fcf0d6f8c0dc4a27651b1a8218d9febdd0bc510d8a2eb8474b17c87b284c5bd`  
		Last Modified: Thu, 17 Mar 2022 16:35:37 GMT  
		Size: 2.8 MB (2823620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5bf31a73f75790d59218e70a95944de87dc3ea7562e9c8caeb2898c6b50f5d`  
		Last Modified: Thu, 17 Mar 2022 16:37:35 GMT  
		Size: 15.8 MB (15797138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7a8ef36db1a7a21719acdab23a718ee6e85476bcc14c179320171964fe566`  
		Last Modified: Thu, 17 Mar 2022 16:37:32 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ae4545c2059a9e781a63b2af8676f51e165e6bf6c59a45d49c53997f04313`  
		Last Modified: Thu, 17 Mar 2022 16:37:32 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10575dfee2efac92f3ecc329cb1078b5cfb2990ac20c532c7e78444f79bb418f`  
		Last Modified: Thu, 17 Mar 2022 16:37:32 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:bf0e120dc92703bd2a52de94287f82a97c262164ae885b0d9d44bb3a2e6480cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19177525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c4f628e1f7b7a4b167dd5f832d4c639edbc6e58eda79ef64f176c600241ad8`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 18:19:00 GMT
ADD file:06587cebee2131b88da0944eb4be5128053d97f4d51a175881625be110548874 in / 
# Thu, 17 Mar 2022 18:19:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 23:10:46 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 17 Mar 2022 23:10:49 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 17 Mar 2022 23:12:11 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 17 Mar 2022 23:12:19 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 17 Mar 2022 23:12:20 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 17 Mar 2022 23:12:21 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 17 Mar 2022 23:12:24 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 17 Mar 2022 23:12:27 GMT
ENV LD_PRELOAD=
# Thu, 17 Mar 2022 23:12:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Thu, 17 Mar 2022 23:12:33 GMT
EXPOSE 24224 5140
# Thu, 17 Mar 2022 23:12:39 GMT
USER fluent
# Thu, 17 Mar 2022 23:12:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 17 Mar 2022 23:12:43 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9ba546239a73b7ff261e6813d8f1cf9e477de8825b6ae341227f315ea3a4cd51`  
		Last Modified: Thu, 17 Mar 2022 18:20:15 GMT  
		Size: 2.8 MB (2817924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891d2b4d19abb5b3d2fc74c43ee5c605524a6f365f86ca52b4c66e761a5bffdd`  
		Last Modified: Thu, 17 Mar 2022 23:13:17 GMT  
		Size: 16.4 MB (16357396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a0d9fac62ae0b8911e1de1b38f32f7a57699b17b1db3ebaa6b58f740f27850`  
		Last Modified: Thu, 17 Mar 2022 23:13:14 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0128d4a3b29ebe4f55475816da762444af03f822b54003bc63c1981eda92c4d0`  
		Last Modified: Thu, 17 Mar 2022 23:13:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b50af67a2823f45bbc7722c7c09b639478d6b36a92aa22c6b3920a1379cb808`  
		Last Modified: Thu, 17 Mar 2022 23:13:14 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:61993d0577d86b1cbd8fd038fbb3fc81fc1d87bbbebcb339974aa1a2cfec4db9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18807441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50d79707de39645031e57f48090fba44806670cc39585b0b7980198ccc470008`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 14:36:02 GMT
ADD file:cc3c2ea972c5b5d1135d0a82f5d1a6cc97fcc81f3006bb6c6b8580f1e9f4c238 in / 
# Thu, 17 Mar 2022 14:36:02 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 00:32:58 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 18 Mar 2022 00:32:58 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 18 Mar 2022 00:33:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 18 Mar 2022 00:33:40 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 18 Mar 2022 00:33:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 18 Mar 2022 00:33:41 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 18 Mar 2022 00:33:41 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 18 Mar 2022 00:33:41 GMT
ENV LD_PRELOAD=
# Fri, 18 Mar 2022 00:33:41 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 18 Mar 2022 00:33:41 GMT
EXPOSE 24224 5140
# Fri, 18 Mar 2022 00:33:41 GMT
USER fluent
# Fri, 18 Mar 2022 00:33:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 18 Mar 2022 00:33:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:3bb5875ccb136d6c7691dcf2927e52a66c831ce80fd5140d92e0a158400a4cfe`  
		Last Modified: Thu, 17 Mar 2022 14:36:53 GMT  
		Size: 2.6 MB (2606212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63aa3544cae7418c9813cee8b10188e8615768815e852f72707dcfb8540cca8`  
		Last Modified: Fri, 18 Mar 2022 00:36:08 GMT  
		Size: 16.2 MB (16199026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d5f444cc8717ced07f7ec85bd899af919e5c205e735d55c3d37384801241f`  
		Last Modified: Fri, 18 Mar 2022 00:36:07 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d8a6fb5d1349def3c489952403a43c43709ab247a2b8555646d700a515ef8d`  
		Last Modified: Fri, 18 Mar 2022 00:36:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56fce753c0aa58650cb432c407188afb53aeae214bef0be25cc94a96c04cffe`  
		Last Modified: Fri, 18 Mar 2022 00:36:06 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14.0-debian-1.0`

```console
$ docker pull fluentd@sha256:f9569ad07e89ae356af491d952804b2da6da23243cb921446c2fdd1f7d93ae15
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

### `fluentd:v1.14.0-debian-1.0` - linux; amd64

```console
$ docker pull fluentd@sha256:19704111ce24d89d45a14b4781e92d299861ae0053f03093f9271ef603abaeac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83265241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8567bad1c8085e3f6ddd58fe5754d7f8af8b104d7bdb1fccc3c1166e06a147b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 14:22:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 14:22:03 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 14:22:03 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 15:04:19 GMT
ENV RUBY_MAJOR=2.6
# Thu, 17 Mar 2022 15:04:19 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 17 Mar 2022 15:04:19 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 17 Mar 2022 15:07:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 15:07:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 15:07:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 15:07:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 15:07:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 15:07:53 GMT
CMD ["irb"]
# Sat, 19 Mar 2022 00:29:17 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 00:29:17 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 00:29:17 GMT
ENV TINI_VERSION=0.18.0
# Sat, 19 Mar 2022 00:32:10 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 00:32:11 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 00:32:12 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 00:32:12 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 00:32:12 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 00:32:12 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 19 Mar 2022 00:32:12 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 00:32:13 GMT
USER fluent
# Sat, 19 Mar 2022 00:32:13 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 00:32:13 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6926507f0c42f3a6c331883516b206192554825a66b3a50f810066c1ad462ab`  
		Last Modified: Thu, 17 Mar 2022 15:15:08 GMT  
		Size: 12.6 MB (12565221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313590c65c28ee93cfccdb8ac3e921c5d59907d6d12807c456aa3a7c5f8c0063`  
		Last Modified: Thu, 17 Mar 2022 15:15:05 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e053d243045b4f6ed7df71bf8746f3f53446be797fb847810da6676c43acb6ba`  
		Last Modified: Thu, 17 Mar 2022 15:18:16 GMT  
		Size: 21.5 MB (21499146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda74560c5216c0d63269e9ee8b25973cfbb9c31d0fc705b5311e74d31e7d0c7`  
		Last Modified: Thu, 17 Mar 2022 15:18:13 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd52317b42c718eb3ca3c23aac3182b84af13b0b5ee7ea9f0afaa0b07ec1d96`  
		Last Modified: Sat, 19 Mar 2022 00:32:58 GMT  
		Size: 22.0 MB (22043959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da20f040f6c64521aac7c44b7a80c12f7418991d052481eb28f115e28bc66ff2`  
		Last Modified: Sat, 19 Mar 2022 00:32:54 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd4cf9a45e6b88e631d51aabb173b7efdf627eee40609e7564340c6d7f1e48b`  
		Last Modified: Sat, 19 Mar 2022 00:32:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d062d3309027ee0211964be0b889ef980d8aff25d14a51a79915ec415dba3fdf`  
		Last Modified: Sat, 19 Mar 2022 00:32:53 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:3db9ae6ab0ec26366328eea8792f54c61638060ffc254f9df91b6cece885373c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77190331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dd4dae9b4e0ed6df610f5633302e2aefffafec097fafb0eeb98b394624d47e1`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 05:20:46 GMT
ADD file:4b7bce60b3e3455ba9b14c881ffa61187b9e56365fe4f275ee871e7c7e930fb9 in / 
# Thu, 17 Mar 2022 05:20:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:18:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:18:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 18:18:28 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 18:52:17 GMT
ENV RUBY_MAJOR=2.6
# Thu, 17 Mar 2022 18:52:17 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 17 Mar 2022 18:52:17 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 17 Mar 2022 18:57:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 18:57:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 18:57:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 18:57:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 18:57:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 18:57:04 GMT
CMD ["irb"]
# Fri, 18 Mar 2022 06:44:35 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 18 Mar 2022 06:44:35 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 18 Mar 2022 06:44:36 GMT
ENV TINI_VERSION=0.18.0
# Fri, 18 Mar 2022 06:48:23 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 18 Mar 2022 06:48:25 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 18 Mar 2022 06:48:25 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 18 Mar 2022 06:48:25 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 18 Mar 2022 06:48:26 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 18 Mar 2022 06:48:26 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 18 Mar 2022 06:48:27 GMT
EXPOSE 24224 5140
# Fri, 18 Mar 2022 06:48:27 GMT
USER fluent
# Fri, 18 Mar 2022 06:48:27 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 18 Mar 2022 06:48:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f193682138b0c37054cb843ef2155a75706f248a369d454bf6444833f120aefc`  
		Last Modified: Thu, 17 Mar 2022 05:36:29 GMT  
		Size: 24.9 MB (24886195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96710cd49a7971b2d375ed6a4e2b9b3c346ddd6eccddcf626a6a5952d4761371`  
		Last Modified: Thu, 17 Mar 2022 19:03:43 GMT  
		Size: 10.3 MB (10348954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea873326987bb8e6add742f0b299995920760d1a154732afb6605f8277c9268b`  
		Last Modified: Thu, 17 Mar 2022 19:03:37 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276ce2af224d310feb9f5da35024a81eb52b8461d367afabc86b0a9a0aff5279`  
		Last Modified: Thu, 17 Mar 2022 19:07:01 GMT  
		Size: 20.8 MB (20760669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43daaa31cb2e5f713c9f9528600d3b12e0710ded0430e8e8459d5df7b2c45c6d`  
		Last Modified: Thu, 17 Mar 2022 19:06:55 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068b2c583821bde0697cc28355b09c1fdd5afeb609789a9f0f0f3be506eca50d`  
		Last Modified: Fri, 18 Mar 2022 06:49:06 GMT  
		Size: 21.2 MB (21191439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7fd1b37d2a2c3e8b32391a45bbca60212587c64795deb46d1620834855d741`  
		Last Modified: Fri, 18 Mar 2022 06:48:53 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021b1b23f9798aa027b1bc35a36c30be781ddd86d7c2d4f6eb60ad9a1236b9f6`  
		Last Modified: Fri, 18 Mar 2022 06:48:53 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b1dd181b7f0e8acb30c0b33fe8da226fe9b2636f12d6b15d1af6582aeb28a9`  
		Last Modified: Fri, 18 Mar 2022 06:48:53 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:f904b1ae959c7954d8bd5643a4250bc85504f6620e5498b68105c3941354f5e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74379752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3463f2bd661dc679cfcf240e4391c32726b99a867b17b6eec08c191e2396406`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 09:32:07 GMT
ADD file:ca7a6b7c138de7fd85996719398396d0ed0f059d2e12b7f401cd460b64924e25 in / 
# Thu, 17 Mar 2022 09:32:08 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 12:41:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 12:41:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 18 Mar 2022 12:41:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 13:35:23 GMT
ENV RUBY_MAJOR=2.6
# Fri, 18 Mar 2022 13:35:23 GMT
ENV RUBY_VERSION=2.6.9
# Fri, 18 Mar 2022 13:35:24 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Fri, 18 Mar 2022 13:39:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 18 Mar 2022 13:39:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 18 Mar 2022 13:39:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 18 Mar 2022 13:39:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 13:39:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 18 Mar 2022 13:39:33 GMT
CMD ["irb"]
# Sun, 20 Mar 2022 09:09:13 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 20 Mar 2022 09:09:13 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sun, 20 Mar 2022 09:09:13 GMT
ENV TINI_VERSION=0.18.0
# Sun, 20 Mar 2022 09:12:44 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sun, 20 Mar 2022 09:12:46 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 20 Mar 2022 09:12:47 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 20 Mar 2022 09:12:47 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sun, 20 Mar 2022 09:12:48 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 20 Mar 2022 09:12:48 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 20 Mar 2022 09:12:48 GMT
EXPOSE 24224 5140
# Sun, 20 Mar 2022 09:12:49 GMT
USER fluent
# Sun, 20 Mar 2022 09:12:49 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 20 Mar 2022 09:12:50 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:0b8f06901fc5e8a29999e260b4ada4ee1cc4415e5c1a16fb7bb21cc2ac995f72`  
		Last Modified: Thu, 17 Mar 2022 09:48:01 GMT  
		Size: 22.8 MB (22754389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e124b65386fabaa7971619254cd2a043e78822adbf73cfa2c62da8c24234c5`  
		Last Modified: Fri, 18 Mar 2022 13:55:07 GMT  
		Size: 9.9 MB (9872973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5f8cac5fcdd0784685b4345eab21f5c830506856ea662bf8350910342a9879`  
		Last Modified: Fri, 18 Mar 2022 13:55:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a22cd6de0a91cbeda83286381b7663d16909fd6bcbf7cb585c36b74d328792`  
		Last Modified: Fri, 18 Mar 2022 14:01:38 GMT  
		Size: 20.7 MB (20672454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb84945ecd110d2d4af4eaa754a47177bf1fe86d9ebb79bdc603574c766bdf42`  
		Last Modified: Fri, 18 Mar 2022 14:01:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c33b15ce03f39f4681baa49a263b8cbe84b1a0f65e8a883056c99e9058df84`  
		Last Modified: Sun, 20 Mar 2022 09:13:27 GMT  
		Size: 21.1 MB (21076855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a42ff1f0f2f7adf14b8f4448ee045402e10950e44479de44207da88b59efdc`  
		Last Modified: Sun, 20 Mar 2022 09:13:14 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06b63d3bb55154ad9fbc8d8c93d648f5318155b0093a0b746417d730c2b6e62`  
		Last Modified: Sun, 20 Mar 2022 09:13:14 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ab1fdc8c85ae73c087789092f5a3b81dbf6053e2b6f14d6db39525342703b8`  
		Last Modified: Sun, 20 Mar 2022 09:13:14 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:29636a8080218de95dde668117a39869f9391ac4e4b62825584222af7ef3b9e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80137340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c913a0d5d56221cf4add568faaefa1143cb599778a7c122eb0fb28ce6762fdf`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:22 GMT
ADD file:1c7d8cedf5dc79c676acebde5252ecd3005088a9f29e5e6be547f659f41efb1f in / 
# Thu, 17 Mar 2022 03:22:22 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:14:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:14:05 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 20:14:06 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 20:42:06 GMT
ENV RUBY_MAJOR=2.6
# Thu, 17 Mar 2022 20:42:07 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 17 Mar 2022 20:42:08 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 17 Mar 2022 20:43:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 20:43:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 20:43:54 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 20:43:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 20:43:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 20:43:57 GMT
CMD ["irb"]
# Sat, 19 Mar 2022 01:10:13 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 01:10:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 01:10:15 GMT
ENV TINI_VERSION=0.18.0
# Sat, 19 Mar 2022 01:12:25 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 01:12:26 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 01:12:28 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 01:12:29 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 01:12:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 01:12:30 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 19 Mar 2022 01:12:31 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 01:12:32 GMT
USER fluent
# Sat, 19 Mar 2022 01:12:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 01:12:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c9277cac12165646c33f028489f2a5be3f70745382f4385cd9ed12fcc8cec183`  
		Last Modified: Thu, 17 Mar 2022 03:29:27 GMT  
		Size: 25.9 MB (25923233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba00919e9bc7af9af691a92dbfeef3ca40c29e924ff156b705f3d8168caf7f28`  
		Last Modified: Thu, 17 Mar 2022 20:51:59 GMT  
		Size: 11.3 MB (11261791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026504a0d60799aae9f35f23d7dbcaadfe16543f13e4f4ed3a811e62444a5151`  
		Last Modified: Thu, 17 Mar 2022 20:51:57 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a563dab2ef6f5725b78f1be860ffdf8d17ec19437ebde3c38028a2d3a41819c4`  
		Last Modified: Thu, 17 Mar 2022 20:56:21 GMT  
		Size: 21.1 MB (21124122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acba3b3cc2ff6d8b3fc5caf5f067e01ab6c067e42e0ba9e45f2e29024dda415f`  
		Last Modified: Thu, 17 Mar 2022 20:56:20 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf899d6e3eebc4a69a9bbd9b336c652d423c176c8c143ff0f94380a635b69dc`  
		Last Modified: Sat, 19 Mar 2022 01:13:12 GMT  
		Size: 21.8 MB (21825286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77aedd26ea26794103542ae1cdc310163ff0fa78d9087d059a894a8a0fcdce2`  
		Last Modified: Sat, 19 Mar 2022 01:13:09 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed5d47f74e05007554bb6dacae4b76321ebe03ce115a82aec11861760716c1b`  
		Last Modified: Sat, 19 Mar 2022 01:13:09 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b519482b8eb854ea5a6acae5f81b2505780475832bc7ab9716d1cfb4ca23e7a4`  
		Last Modified: Sat, 19 Mar 2022 01:13:09 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:c6654d0995f5529a1ee0c73574fa8e069c6c1b905ff56b49214c46dbdf6fd822
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87207527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e9205b484a18dcaff31eb4dcf0adcd501aa68bacabdf6d2699c97407c561c9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 08:16:28 GMT
ADD file:39b40ec7bd2f4e691b74f0287e43ab64ef32f99953e606d9e4b72d058659209c in / 
# Thu, 17 Mar 2022 08:16:29 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:12:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:12:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 20:12:02 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 21:13:32 GMT
ENV RUBY_MAJOR=2.6
# Thu, 17 Mar 2022 21:13:32 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 17 Mar 2022 21:13:32 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 17 Mar 2022 21:16:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 21:16:40 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 21:16:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 21:16:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 21:16:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 21:16:42 GMT
CMD ["irb"]
# Sat, 19 Mar 2022 03:17:31 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 03:17:31 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 03:17:31 GMT
ENV TINI_VERSION=0.18.0
# Sat, 19 Mar 2022 03:20:14 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 03:20:15 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 03:20:16 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 03:20:16 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 03:20:16 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 03:20:16 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 19 Mar 2022 03:20:16 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 03:20:17 GMT
USER fluent
# Sat, 19 Mar 2022 03:20:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 03:20:17 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:cef703cf0f3e19a7a5f8b305254c02563c8b07f5b842bb99741d3a2fd136e9f0`  
		Last Modified: Thu, 17 Mar 2022 08:24:59 GMT  
		Size: 27.8 MB (27804570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d1be88d2bd084f4a940d09972670c3fbe0c8ff5f6bd8902cf38d5218936b1a`  
		Last Modified: Thu, 17 Mar 2022 21:32:17 GMT  
		Size: 17.2 MB (17227109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaa7cd53192f660e18ef91319a055c5b3707261611a57b78727979d53ab6c12`  
		Last Modified: Thu, 17 Mar 2022 21:32:08 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145c5c16a3403918434c329c288afbe389e2bb96de28aada5bbdf5f40b4e8e45`  
		Last Modified: Thu, 17 Mar 2022 21:37:57 GMT  
		Size: 20.9 MB (20941789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad64dcea1035bb20c285a27b8c7e7c40f7f92accbccde17ef8101ff1bde2d8`  
		Last Modified: Thu, 17 Mar 2022 21:37:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c4ad77a25ad255cc29257cc074e5b3ef7fe868c9bd34a4716fbeb37ac2915b`  
		Last Modified: Sat, 19 Mar 2022 03:20:54 GMT  
		Size: 21.2 MB (21230979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96104ea9b08b62c8c998499cfb51a3e56aa5a8c7b9bec11f0a37e92b17c0daf1`  
		Last Modified: Sat, 19 Mar 2022 03:20:47 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9e48c5c45b15b3f1c04283388849874a40e70c651dc349d4b364d131690f26`  
		Last Modified: Sat, 19 Mar 2022 03:20:47 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e439f7c1adf49b9d5e045c414e29682ece7625a72f8fdbba816277ed9026d1f`  
		Last Modified: Sat, 19 Mar 2022 03:20:47 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:0b4bb8f3966d815a30a8bca6a7fb11ce0fb309fa31def741771c94fce72c34ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87911471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5656fc0bada313f656bc91d9adf09b22f1dca892dd4fb14c2914ba650477d9bb`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 11:19:08 GMT
ADD file:0af430b7759619d4d40ea316f823599879e4f3e0dfc8877bdee731020fb2620d in / 
# Thu, 17 Mar 2022 11:19:12 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:17:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:17:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 18 Mar 2022 09:17:56 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 11:05:30 GMT
ENV RUBY_MAJOR=2.6
# Fri, 18 Mar 2022 11:05:34 GMT
ENV RUBY_VERSION=2.6.9
# Fri, 18 Mar 2022 11:05:38 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Fri, 18 Mar 2022 11:13:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 18 Mar 2022 11:13:26 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 18 Mar 2022 11:13:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 18 Mar 2022 11:13:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 11:13:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 18 Mar 2022 11:13:40 GMT
CMD ["irb"]
# Sat, 19 Mar 2022 18:30:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 19 Mar 2022 18:30:12 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 19 Mar 2022 18:30:14 GMT
ENV TINI_VERSION=0.18.0
# Sat, 19 Mar 2022 18:35:01 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 19 Mar 2022 18:35:13 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 19 Mar 2022 18:35:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 19 Mar 2022 18:35:15 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 19 Mar 2022 18:35:16 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 19 Mar 2022 18:35:18 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 19 Mar 2022 18:35:19 GMT
EXPOSE 24224 5140
# Sat, 19 Mar 2022 18:35:21 GMT
USER fluent
# Sat, 19 Mar 2022 18:35:23 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 19 Mar 2022 18:35:26 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:303d92340e7868a8dc0fdad5d6c67a8a819a74a2bc47038b26339d5be6084bf4`  
		Last Modified: Thu, 17 Mar 2022 11:29:21 GMT  
		Size: 30.6 MB (30562350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f66151a771365bde67fd17be685cf1fdf64ec564de1ea1abd21857163d3fa1`  
		Last Modified: Fri, 18 Mar 2022 11:26:21 GMT  
		Size: 12.7 MB (12705799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8a13186fd38729296916af6473c01e211b70d1902e2a80bc6a07d483fc1299`  
		Last Modified: Fri, 18 Mar 2022 11:26:18 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea1311e913eb785a25b51326f66155d23ca19d8d39fc3198235e5a60a6ee1fa`  
		Last Modified: Fri, 18 Mar 2022 11:31:40 GMT  
		Size: 22.0 MB (22023538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6137c1e5318bf29cb971d297d077b165550a089e613b19261ae764f6345cf8a3`  
		Last Modified: Fri, 18 Mar 2022 11:31:37 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66fc3b375d01b37084effe219f7ba7a84a0949cf1eebc9dc849d23a27a7fd8c`  
		Last Modified: Sat, 19 Mar 2022 18:35:57 GMT  
		Size: 22.6 MB (22616699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d37d0dfb87e2ca2a2edd4acdbcc933de9fe98f98cd99f5c98c55a16794e63af`  
		Last Modified: Sat, 19 Mar 2022 18:35:53 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9eae5fc2113db7f125fbdf264974b9502f31bc6490cf1e9c1c4dafc34838831`  
		Last Modified: Sat, 19 Mar 2022 18:35:53 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e53b545c7e35959341a16ce01a764efe19ac0f40e75c052345990c23ed7ef`  
		Last Modified: Sat, 19 Mar 2022 18:35:53 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:3a90c942b177cb13756425e208acab692d97dbf43aad209ea6442092d002b365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80458771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf4fe7f6447b0debb6e1fb832c9354933900f15e603b99e0efb12cfabb4bfda9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 17 Mar 2022 03:07:30 GMT
ADD file:4342e1d9db757e91953273ac7120c9d6004d38281f9cea830898b4f35ca43517 in / 
# Thu, 17 Mar 2022 03:07:32 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 15:49:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 15:49:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 15:49:57 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 16:14:13 GMT
ENV RUBY_MAJOR=2.6
# Thu, 17 Mar 2022 16:14:13 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 17 Mar 2022 16:14:13 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 17 Mar 2022 16:15:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 16:15:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 16:15:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 16:15:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 16:15:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 16:15:55 GMT
CMD ["irb"]
# Fri, 18 Mar 2022 00:33:48 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 18 Mar 2022 00:33:48 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 18 Mar 2022 00:33:49 GMT
ENV TINI_VERSION=0.18.0
# Fri, 18 Mar 2022 00:35:39 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 18 Mar 2022 00:35:43 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 18 Mar 2022 00:35:43 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 18 Mar 2022 00:35:43 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 18 Mar 2022 00:35:44 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 18 Mar 2022 00:35:44 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 18 Mar 2022 00:35:44 GMT
EXPOSE 24224 5140
# Fri, 18 Mar 2022 00:35:44 GMT
USER fluent
# Fri, 18 Mar 2022 00:35:44 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 18 Mar 2022 00:35:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6f8a08956872b0f67802da3a67e007322eb963a60e0dadd736077f3ece414e1f`  
		Last Modified: Thu, 17 Mar 2022 03:13:18 GMT  
		Size: 25.8 MB (25769076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9cef5c82f53c076a6b79c5df66e5aa85afd14eb4dfee12b48f9f24590f5787`  
		Last Modified: Thu, 17 Mar 2022 16:23:24 GMT  
		Size: 10.8 MB (10815376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d0a7487845abb7f24bbfa9fbfa7aa7ba2db74064de78c2e76a6d43cfa13400`  
		Last Modified: Thu, 17 Mar 2022 16:23:22 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702d01f5776fca30cdbaef386ecb99e95ca20dee02f34af3fed94fed7be0f2ec`  
		Last Modified: Thu, 17 Mar 2022 16:27:21 GMT  
		Size: 21.6 MB (21644656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d77a06b5cd31cc88689cceaef7cd57c02be52fe13b0d38812b774c6539b06c3`  
		Last Modified: Thu, 17 Mar 2022 16:27:19 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdec0ae49272d2bbb77c9403aba90515b89f9e2feceeefeedb9c4ca20eb5d0e8`  
		Last Modified: Fri, 18 Mar 2022 00:36:20 GMT  
		Size: 22.2 MB (22226575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beebf7abb9f7775a04208dbd334e979d2417387915102cbbc63cf64ffd4258f`  
		Last Modified: Fri, 18 Mar 2022 00:36:18 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da45a2d2559a73512e216762607fc94b2da86908de7e7f85c18dd3aeea5e5ea`  
		Last Modified: Fri, 18 Mar 2022 00:36:18 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc90b6341089328ac6b17480fa9f33202d719f1ec3f9dfe69400edec8c3e8a80`  
		Last Modified: Fri, 18 Mar 2022 00:36:18 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
