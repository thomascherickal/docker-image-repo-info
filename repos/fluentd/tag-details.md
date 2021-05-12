<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.9-1`](#fluentdv19-1)
-	[`fluentd:v1.9-debian-1`](#fluentdv19-debian-1)
-	[`fluentd:v1.9.1-1.0`](#fluentdv191-10)
-	[`fluentd:v1.9.1-debian-1.0`](#fluentdv191-debian-10)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:47c595013b00409fd52d7165773731c6a360cd610d513c665a04c2923d89fba8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:latest` - linux; amd64

```console
$ docker pull fluentd@sha256:3536d047aa7a961d8c826617282e8afa2075990c7e4be122a6501605ec5f3a8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15174420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b84547e9c6cfe8be39cc6870d9b942554d48005ecf5cd2ba4156a3a380fa53a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 11:38:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Mar 2021 11:38:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 13 Mar 2021 11:39:29 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 13 Mar 2021 11:39:30 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Mar 2021 11:39:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Mar 2021 11:39:31 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 13 Mar 2021 11:39:31 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Mar 2021 11:39:31 GMT
ENV LD_PRELOAD=
# Sat, 13 Mar 2021 11:39:31 GMT
EXPOSE 24224 5140
# Sat, 13 Mar 2021 11:39:31 GMT
USER fluent
# Sat, 13 Mar 2021 11:39:32 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Mar 2021 11:39:32 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9651430fd06f066ea7cd1dde55009fe606a5c9357f60d2c418363f4c8d3e29d6`  
		Last Modified: Sat, 13 Mar 2021 11:41:13 GMT  
		Size: 12.4 MB (12398794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1eccd3574cb406400b237809e45a86e63983263d1f67e8887c6e89d31ef835`  
		Last Modified: Sat, 13 Mar 2021 11:41:11 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd5db2e3e2d262b39a393666a8efc9edb577b63c8f3934f23e7f16425cd4cd`  
		Last Modified: Sat, 13 Mar 2021 11:41:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d18dcc36773b2d18dbe989da843efc8bee18a990bfd603d2a340174c3246af`  
		Last Modified: Sat, 13 Mar 2021 11:41:11 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:44f31c1936eb1fb832ffab84cf23b98d016b2646cae11aaec96aef5939cd17e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15976216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021add57c37363fa0e7aa9dd21f7a3fe33da8e7e72cb09d25d866ddb6f3fd259`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:39:49 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Apr 2020 17:39:50 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Thu, 23 Apr 2020 17:41:27 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Apr 2020 17:41:31 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Apr 2020 17:41:32 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Apr 2020 17:41:32 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Apr 2020 17:41:33 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Apr 2020 17:41:34 GMT
ENV LD_PRELOAD=
# Thu, 23 Apr 2020 17:41:34 GMT
EXPOSE 24224 5140
# Thu, 23 Apr 2020 17:41:35 GMT
USER fluent
# Thu, 23 Apr 2020 17:41:36 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Apr 2020 17:41:37 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d522b01371d30767392094a66b629aa2f6a1cfeeb82ae15eeb64f931a1fa4b`  
		Last Modified: Thu, 23 Apr 2020 17:42:00 GMT  
		Size: 13.4 MB (13425275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad32a34e355514cb68abd5ee8454fa9b8f13c30395d005fccaa99434a30406e`  
		Last Modified: Thu, 23 Apr 2020 17:41:55 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f703ee04ff8bd4f967972c80763171663ea5f1670044ebf18ff8273097c5c5`  
		Last Modified: Thu, 23 Apr 2020 17:41:55 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c24c5529dab1e5be1e7eec9c51d402281e9e72a5e13f9244a461073bca7241c`  
		Last Modified: Thu, 23 Apr 2020 17:41:55 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:9a3af653771a6a04c358f7c2a60b8bb57c64d3de5dd298c0d4657ceb35ea0f66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16449859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d62a0ca09e6cfbf89d9db9d526962faa229e3de5ec48e9ef934e8566431b4c9d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:05:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 24 Apr 2020 09:05:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Fri, 24 Apr 2020 09:06:41 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Fri, 24 Apr 2020 09:06:45 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 24 Apr 2020 09:06:46 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 24 Apr 2020 09:06:46 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Fri, 24 Apr 2020 09:06:47 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 24 Apr 2020 09:06:48 GMT
ENV LD_PRELOAD=
# Fri, 24 Apr 2020 09:06:48 GMT
EXPOSE 24224 5140
# Fri, 24 Apr 2020 09:06:49 GMT
USER fluent
# Fri, 24 Apr 2020 09:06:49 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 24 Apr 2020 09:06:50 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7c433500fac88cd265a112da6bb53517cca36634a766db54f966da1f64e6ae`  
		Last Modified: Fri, 24 Apr 2020 09:07:26 GMT  
		Size: 13.8 MB (13753176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcba662d9a25425bd9d1fd78c25999719742ab37190f21b0228c999766407978`  
		Last Modified: Fri, 24 Apr 2020 09:07:20 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a458dc4b98ef9ffa86fcd837c55416fd16fee3a6154a3e1f38011c7dad2a51`  
		Last Modified: Fri, 24 Apr 2020 09:07:20 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0293d533db263a29c969b1f2ca4ef1c0df2bbfe728041795f264b905641d6009`  
		Last Modified: Fri, 24 Apr 2020 09:07:20 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; 386

```console
$ docker pull fluentd@sha256:2674458e5ee30b6811a635b030e7a5c02f09a60ac2b526e9233ae520b9e52d36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15066972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6050199bd42bf9ce01c19ba5ea4ae473745e01fa2692be5d9603f3ab09958dc7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 04:51:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Mar 2021 04:51:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 13 Mar 2021 04:53:00 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 13 Mar 2021 04:53:03 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Mar 2021 04:53:04 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Mar 2021 04:53:04 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 13 Mar 2021 04:53:05 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Mar 2021 04:53:05 GMT
ENV LD_PRELOAD=
# Sat, 13 Mar 2021 04:53:05 GMT
EXPOSE 24224 5140
# Sat, 13 Mar 2021 04:53:06 GMT
USER fluent
# Sat, 13 Mar 2021 04:53:06 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Mar 2021 04:53:07 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a86c3883d026d251c0b98f179473179adc48ddd9931c34671ec927485c2b30`  
		Last Modified: Sat, 13 Mar 2021 04:56:41 GMT  
		Size: 12.3 MB (12295016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdff586ec846debe504cab0d5418aed7a757990f1c2e5535febd3c2434383f9`  
		Last Modified: Sat, 13 Mar 2021 04:56:36 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec361a5d42c106aff6fc935ed2b65a028307e9e2fee0160ec1d41376855b6969`  
		Last Modified: Sat, 13 Mar 2021 04:56:36 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1fe75d1dda1ff8c1442a52d915e50e76400a2c2499c166340a71e5c9953409`  
		Last Modified: Sat, 13 Mar 2021 04:56:36 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:624655b564b9a0d8aff2adb11bc4e4ab152cc6cddbb0f80dbec0ccc280a6c7e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16969348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9996e3889db7f499cb26285f39e7577a3572c8c83eefb66472ac0e3d67d6c9f7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 20:41:14 GMT
ADD file:2eaa074d9379f98d31cc4112997e1c1bb55b3871574af6aee576cf1c5ed99645 in / 
# Thu, 23 Apr 2020 20:41:16 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:52:12 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 24 Apr 2020 02:52:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Fri, 24 Apr 2020 02:53:15 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Fri, 24 Apr 2020 02:53:21 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 24 Apr 2020 02:53:21 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 24 Apr 2020 02:53:22 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Fri, 24 Apr 2020 02:53:24 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 24 Apr 2020 02:53:26 GMT
ENV LD_PRELOAD=
# Fri, 24 Apr 2020 02:53:27 GMT
EXPOSE 24224 5140
# Fri, 24 Apr 2020 02:53:29 GMT
USER fluent
# Fri, 24 Apr 2020 02:53:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 24 Apr 2020 02:53:33 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:16f2eaeeecc1446c304d41ae21441f168e376dc76733ec3a9f8f2d17119638a1`  
		Last Modified: Thu, 23 Apr 2020 20:41:57 GMT  
		Size: 2.8 MB (2787865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27df74a3decbbc71f688e8319c7055315cbba6b350b28324d4ad9c021ca50135`  
		Last Modified: Fri, 24 Apr 2020 02:54:03 GMT  
		Size: 14.2 MB (14179267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1465abcf9b778cb4d299d4fec3ccbd1b1284867a62dc8b6d6d59a7a195cc0203`  
		Last Modified: Fri, 24 Apr 2020 02:53:59 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b323e14271e2cf6ac4ee482e207353aa39585d4e58bf75475fe54e2a7f1fdb65`  
		Last Modified: Fri, 24 Apr 2020 02:53:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a13af9e734338dbe7adf7de4ab71210d13beaeed6a6fec5d7b9a7b4dff17131`  
		Last Modified: Fri, 24 Apr 2020 02:53:59 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:12f970948d5704cc42194be7cbfd8fe038e802f8fc2fb8f2169bf7c4c2c5eb5b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16441885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b6e3f25bb06297f8b35538b6b7a44d6c0ce04bfa379393397e3eef1c4c16e9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:19 GMT
ADD file:87357838aa76ab358b68ac6734871df2dacb0b5918d89a091836f0d33264f803 in / 
# Thu, 23 Apr 2020 17:51:20 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 19:59:44 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Apr 2020 19:59:44 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Thu, 23 Apr 2020 20:00:12 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Apr 2020 20:00:14 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Apr 2020 20:00:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Apr 2020 20:00:14 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Apr 2020 20:00:14 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Apr 2020 20:00:14 GMT
ENV LD_PRELOAD=
# Thu, 23 Apr 2020 20:00:15 GMT
EXPOSE 24224 5140
# Thu, 23 Apr 2020 20:00:15 GMT
USER fluent
# Thu, 23 Apr 2020 20:00:15 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Apr 2020 20:00:15 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1aff3887737eb15ee1a53e92e8c87162b9caac2281ecb01242da00d1a32f5a04`  
		Last Modified: Thu, 23 Apr 2020 17:51:52 GMT  
		Size: 2.6 MB (2550329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84a8d1f46d684e96854f17f7222edf696d71cf5cd842954e92f378e005dab17`  
		Last Modified: Thu, 23 Apr 2020 20:00:33 GMT  
		Size: 13.9 MB (13889338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52edf66127670c83c7f5a2aed5e38db5dca87e51eb8966174df5900dc2e0c9`  
		Last Modified: Thu, 23 Apr 2020 20:00:30 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec06b392ce74e92be850c3ddc84f05a6f54ed80e3920a6da6d4327a8d62b5137`  
		Last Modified: Thu, 23 Apr 2020 20:00:35 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d063c86f8d64af1ad29498f54a054870ec143617b700e0f374dd7a023214ef43`  
		Last Modified: Thu, 23 Apr 2020 20:00:35 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.9-1`

```console
$ docker pull fluentd@sha256:47c595013b00409fd52d7165773731c6a360cd610d513c665a04c2923d89fba8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.9-1` - linux; amd64

```console
$ docker pull fluentd@sha256:3536d047aa7a961d8c826617282e8afa2075990c7e4be122a6501605ec5f3a8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15174420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b84547e9c6cfe8be39cc6870d9b942554d48005ecf5cd2ba4156a3a380fa53a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 11:38:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Mar 2021 11:38:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 13 Mar 2021 11:39:29 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 13 Mar 2021 11:39:30 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Mar 2021 11:39:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Mar 2021 11:39:31 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 13 Mar 2021 11:39:31 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Mar 2021 11:39:31 GMT
ENV LD_PRELOAD=
# Sat, 13 Mar 2021 11:39:31 GMT
EXPOSE 24224 5140
# Sat, 13 Mar 2021 11:39:31 GMT
USER fluent
# Sat, 13 Mar 2021 11:39:32 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Mar 2021 11:39:32 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9651430fd06f066ea7cd1dde55009fe606a5c9357f60d2c418363f4c8d3e29d6`  
		Last Modified: Sat, 13 Mar 2021 11:41:13 GMT  
		Size: 12.4 MB (12398794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1eccd3574cb406400b237809e45a86e63983263d1f67e8887c6e89d31ef835`  
		Last Modified: Sat, 13 Mar 2021 11:41:11 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd5db2e3e2d262b39a393666a8efc9edb577b63c8f3934f23e7f16425cd4cd`  
		Last Modified: Sat, 13 Mar 2021 11:41:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d18dcc36773b2d18dbe989da843efc8bee18a990bfd603d2a340174c3246af`  
		Last Modified: Sat, 13 Mar 2021 11:41:11 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9-1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:44f31c1936eb1fb832ffab84cf23b98d016b2646cae11aaec96aef5939cd17e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15976216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021add57c37363fa0e7aa9dd21f7a3fe33da8e7e72cb09d25d866ddb6f3fd259`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:39:49 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Apr 2020 17:39:50 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Thu, 23 Apr 2020 17:41:27 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Apr 2020 17:41:31 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Apr 2020 17:41:32 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Apr 2020 17:41:32 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Apr 2020 17:41:33 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Apr 2020 17:41:34 GMT
ENV LD_PRELOAD=
# Thu, 23 Apr 2020 17:41:34 GMT
EXPOSE 24224 5140
# Thu, 23 Apr 2020 17:41:35 GMT
USER fluent
# Thu, 23 Apr 2020 17:41:36 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Apr 2020 17:41:37 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d522b01371d30767392094a66b629aa2f6a1cfeeb82ae15eeb64f931a1fa4b`  
		Last Modified: Thu, 23 Apr 2020 17:42:00 GMT  
		Size: 13.4 MB (13425275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad32a34e355514cb68abd5ee8454fa9b8f13c30395d005fccaa99434a30406e`  
		Last Modified: Thu, 23 Apr 2020 17:41:55 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f703ee04ff8bd4f967972c80763171663ea5f1670044ebf18ff8273097c5c5`  
		Last Modified: Thu, 23 Apr 2020 17:41:55 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c24c5529dab1e5be1e7eec9c51d402281e9e72a5e13f9244a461073bca7241c`  
		Last Modified: Thu, 23 Apr 2020 17:41:55 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:9a3af653771a6a04c358f7c2a60b8bb57c64d3de5dd298c0d4657ceb35ea0f66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16449859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d62a0ca09e6cfbf89d9db9d526962faa229e3de5ec48e9ef934e8566431b4c9d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:05:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 24 Apr 2020 09:05:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Fri, 24 Apr 2020 09:06:41 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Fri, 24 Apr 2020 09:06:45 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 24 Apr 2020 09:06:46 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 24 Apr 2020 09:06:46 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Fri, 24 Apr 2020 09:06:47 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 24 Apr 2020 09:06:48 GMT
ENV LD_PRELOAD=
# Fri, 24 Apr 2020 09:06:48 GMT
EXPOSE 24224 5140
# Fri, 24 Apr 2020 09:06:49 GMT
USER fluent
# Fri, 24 Apr 2020 09:06:49 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 24 Apr 2020 09:06:50 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7c433500fac88cd265a112da6bb53517cca36634a766db54f966da1f64e6ae`  
		Last Modified: Fri, 24 Apr 2020 09:07:26 GMT  
		Size: 13.8 MB (13753176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcba662d9a25425bd9d1fd78c25999719742ab37190f21b0228c999766407978`  
		Last Modified: Fri, 24 Apr 2020 09:07:20 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a458dc4b98ef9ffa86fcd837c55416fd16fee3a6154a3e1f38011c7dad2a51`  
		Last Modified: Fri, 24 Apr 2020 09:07:20 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0293d533db263a29c969b1f2ca4ef1c0df2bbfe728041795f264b905641d6009`  
		Last Modified: Fri, 24 Apr 2020 09:07:20 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9-1` - linux; 386

```console
$ docker pull fluentd@sha256:2674458e5ee30b6811a635b030e7a5c02f09a60ac2b526e9233ae520b9e52d36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15066972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6050199bd42bf9ce01c19ba5ea4ae473745e01fa2692be5d9603f3ab09958dc7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 04:51:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Mar 2021 04:51:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 13 Mar 2021 04:53:00 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 13 Mar 2021 04:53:03 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Mar 2021 04:53:04 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Mar 2021 04:53:04 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 13 Mar 2021 04:53:05 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Mar 2021 04:53:05 GMT
ENV LD_PRELOAD=
# Sat, 13 Mar 2021 04:53:05 GMT
EXPOSE 24224 5140
# Sat, 13 Mar 2021 04:53:06 GMT
USER fluent
# Sat, 13 Mar 2021 04:53:06 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Mar 2021 04:53:07 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a86c3883d026d251c0b98f179473179adc48ddd9931c34671ec927485c2b30`  
		Last Modified: Sat, 13 Mar 2021 04:56:41 GMT  
		Size: 12.3 MB (12295016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdff586ec846debe504cab0d5418aed7a757990f1c2e5535febd3c2434383f9`  
		Last Modified: Sat, 13 Mar 2021 04:56:36 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec361a5d42c106aff6fc935ed2b65a028307e9e2fee0160ec1d41376855b6969`  
		Last Modified: Sat, 13 Mar 2021 04:56:36 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1fe75d1dda1ff8c1442a52d915e50e76400a2c2499c166340a71e5c9953409`  
		Last Modified: Sat, 13 Mar 2021 04:56:36 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:624655b564b9a0d8aff2adb11bc4e4ab152cc6cddbb0f80dbec0ccc280a6c7e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16969348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9996e3889db7f499cb26285f39e7577a3572c8c83eefb66472ac0e3d67d6c9f7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 20:41:14 GMT
ADD file:2eaa074d9379f98d31cc4112997e1c1bb55b3871574af6aee576cf1c5ed99645 in / 
# Thu, 23 Apr 2020 20:41:16 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:52:12 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 24 Apr 2020 02:52:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Fri, 24 Apr 2020 02:53:15 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Fri, 24 Apr 2020 02:53:21 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 24 Apr 2020 02:53:21 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 24 Apr 2020 02:53:22 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Fri, 24 Apr 2020 02:53:24 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 24 Apr 2020 02:53:26 GMT
ENV LD_PRELOAD=
# Fri, 24 Apr 2020 02:53:27 GMT
EXPOSE 24224 5140
# Fri, 24 Apr 2020 02:53:29 GMT
USER fluent
# Fri, 24 Apr 2020 02:53:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 24 Apr 2020 02:53:33 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:16f2eaeeecc1446c304d41ae21441f168e376dc76733ec3a9f8f2d17119638a1`  
		Last Modified: Thu, 23 Apr 2020 20:41:57 GMT  
		Size: 2.8 MB (2787865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27df74a3decbbc71f688e8319c7055315cbba6b350b28324d4ad9c021ca50135`  
		Last Modified: Fri, 24 Apr 2020 02:54:03 GMT  
		Size: 14.2 MB (14179267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1465abcf9b778cb4d299d4fec3ccbd1b1284867a62dc8b6d6d59a7a195cc0203`  
		Last Modified: Fri, 24 Apr 2020 02:53:59 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b323e14271e2cf6ac4ee482e207353aa39585d4e58bf75475fe54e2a7f1fdb65`  
		Last Modified: Fri, 24 Apr 2020 02:53:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a13af9e734338dbe7adf7de4ab71210d13beaeed6a6fec5d7b9a7b4dff17131`  
		Last Modified: Fri, 24 Apr 2020 02:53:59 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9-1` - linux; s390x

```console
$ docker pull fluentd@sha256:12f970948d5704cc42194be7cbfd8fe038e802f8fc2fb8f2169bf7c4c2c5eb5b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16441885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b6e3f25bb06297f8b35538b6b7a44d6c0ce04bfa379393397e3eef1c4c16e9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:19 GMT
ADD file:87357838aa76ab358b68ac6734871df2dacb0b5918d89a091836f0d33264f803 in / 
# Thu, 23 Apr 2020 17:51:20 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 19:59:44 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Apr 2020 19:59:44 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Thu, 23 Apr 2020 20:00:12 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Apr 2020 20:00:14 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Apr 2020 20:00:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Apr 2020 20:00:14 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Apr 2020 20:00:14 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Apr 2020 20:00:14 GMT
ENV LD_PRELOAD=
# Thu, 23 Apr 2020 20:00:15 GMT
EXPOSE 24224 5140
# Thu, 23 Apr 2020 20:00:15 GMT
USER fluent
# Thu, 23 Apr 2020 20:00:15 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Apr 2020 20:00:15 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1aff3887737eb15ee1a53e92e8c87162b9caac2281ecb01242da00d1a32f5a04`  
		Last Modified: Thu, 23 Apr 2020 17:51:52 GMT  
		Size: 2.6 MB (2550329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84a8d1f46d684e96854f17f7222edf696d71cf5cd842954e92f378e005dab17`  
		Last Modified: Thu, 23 Apr 2020 20:00:33 GMT  
		Size: 13.9 MB (13889338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52edf66127670c83c7f5a2aed5e38db5dca87e51eb8966174df5900dc2e0c9`  
		Last Modified: Thu, 23 Apr 2020 20:00:30 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec06b392ce74e92be850c3ddc84f05a6f54ed80e3920a6da6d4327a8d62b5137`  
		Last Modified: Thu, 23 Apr 2020 20:00:35 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d063c86f8d64af1ad29498f54a054870ec143617b700e0f374dd7a023214ef43`  
		Last Modified: Thu, 23 Apr 2020 20:00:35 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.9-debian-1`

```console
$ docker pull fluentd@sha256:aabb22577d9f8b7752a85ab0019a78f6d8e7ea2cffb69b646e7f1b423c8f053c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.9-debian-1` - linux; amd64

```console
$ docker pull fluentd@sha256:252da65de6465d0add2906b1687269ba7edf1fb510811507bce09a60c0381f38
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82493451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69ea641f7940f8a6ad3bef97a31463ea1255b1603e1ee37486cdfdc4d98cc0ec`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 18:49:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:49:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:49:04 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:53:53 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 11 Apr 2021 06:53:53 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sun, 11 Apr 2021 06:53:53 GMT
ENV TINI_VERSION=0.18.0
# Sun, 11 Apr 2021 06:55:05 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 11 Apr 2021 06:55:06 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 11 Apr 2021 06:55:07 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 11 Apr 2021 06:55:07 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 11 Apr 2021 06:55:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 11 Apr 2021 06:55:07 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 11 Apr 2021 06:55:07 GMT
EXPOSE 24224 5140
# Sun, 11 Apr 2021 06:55:07 GMT
USER fluent
# Sun, 11 Apr 2021 06:55:08 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 11 Apr 2021 06:55:08 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451af66bced958304be82120827542b55bd2229f2e83c5a058a441fa74254828`  
		Last Modified: Sat, 10 Apr 2021 19:10:36 GMT  
		Size: 21.5 MB (21467370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3264de8e4173291cbec86320f1fe2733ffcdc3ff53cfa7c0d3238e334b79dea`  
		Last Modified: Sat, 10 Apr 2021 19:10:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f112accd4f78deefda257913b04cde0a37df82ac2d22321d7b9e3e0a1fad44f9`  
		Last Modified: Sun, 11 Apr 2021 06:55:35 GMT  
		Size: 21.3 MB (21321334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c187eda5e9fa5dcc2b79f1378157a285315472df354493334defe33e508356`  
		Last Modified: Sun, 11 Apr 2021 06:55:32 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc82756b1be22095f405aa9e758dd71424e1033fd10ba535fc716d4dc426286`  
		Last Modified: Sun, 11 Apr 2021 06:55:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63675e64ab7fae4cf4e0fc5637b6429fdcc3ae067f979cd8ada813fe4c9dcb`  
		Last Modified: Sun, 11 Apr 2021 06:55:32 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:84afb53ffc4f4ddd57698dcb9ec356e3fbdbef288f3a02cafd71ab14161c370d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76427847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc3dd148b0b5c3d5f32fe1d3b8c07649d5664c438c8dbeb7ec6a534e3517e5e`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:27:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 07:27:10 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 07:42:11 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 07:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 07:45:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 07:45:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 07:45:55 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 17:32:57 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 10 Apr 2021 17:32:58 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 10 Apr 2021 17:32:59 GMT
ENV TINI_VERSION=0.18.0
# Sat, 10 Apr 2021 17:36:05 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 10 Apr 2021 17:36:09 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 10 Apr 2021 17:36:11 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 10 Apr 2021 17:36:11 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 10 Apr 2021 17:36:12 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 10 Apr 2021 17:36:13 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 10 Apr 2021 17:36:14 GMT
EXPOSE 24224 5140
# Sat, 10 Apr 2021 17:36:15 GMT
USER fluent
# Sat, 10 Apr 2021 17:36:15 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 10 Apr 2021 17:36:16 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8fc93885ff1edc1fec20b799c1c02e672d75d967815f7a98ffe7cb94969e2`  
		Last Modified: Sat, 10 Apr 2021 08:11:28 GMT  
		Size: 10.3 MB (10345305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfdecedfe5bd31f7499d5973d09b2665408cca73a9e1f83fea87d261763e6a`  
		Last Modified: Sat, 10 Apr 2021 08:11:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64f63c1e0d3af67924d2d3ef5636ed70900748b90fffc5bf4e748a38ef7d125`  
		Last Modified: Sat, 10 Apr 2021 08:12:41 GMT  
		Size: 20.7 MB (20732839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9ef980b82778a927138ed4192338fea82cdb79fe3d25e26ac958cc5dc33d62`  
		Last Modified: Sat, 10 Apr 2021 08:12:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2be6a3e99897bfd8c8b0031cdca1954ee20743702502780d2bddc483248e9f5`  
		Last Modified: Sat, 10 Apr 2021 17:36:45 GMT  
		Size: 20.5 MB (20473445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448f85071b171ec5a492b293fe248da108943b0d54e52333d93fc8b294d80608`  
		Last Modified: Sat, 10 Apr 2021 17:36:39 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7873e0b58f6016208e2f37cd0b8c984f219f2c53b140300380522a20bb0fc3b7`  
		Last Modified: Sat, 10 Apr 2021 17:36:39 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5182351736a7c8610417ae03f6776a1b7a01e977abc3fd33c58a68c11ffb0b64`  
		Last Modified: Sat, 10 Apr 2021 17:36:39 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:4bb4f27f160486872fa2538880cc99f0aa14389ace3139be5e3bc18129aaeb68
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73630876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28c30b78c53b091a8bbd464260d9386ee3a8a2679f24245f599a913f2c6122c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:21:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:21:36 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:49:54 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:49:56 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:49:57 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:53:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:53:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:53:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:53:49 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:32:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 11 Apr 2021 04:32:55 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sun, 11 Apr 2021 04:32:56 GMT
ENV TINI_VERSION=0.18.0
# Sun, 11 Apr 2021 04:35:31 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 11 Apr 2021 04:35:35 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 11 Apr 2021 04:35:36 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 11 Apr 2021 04:35:37 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 11 Apr 2021 04:35:38 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 11 Apr 2021 04:35:39 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 11 Apr 2021 04:35:40 GMT
EXPOSE 24224 5140
# Sun, 11 Apr 2021 04:35:41 GMT
USER fluent
# Sun, 11 Apr 2021 04:35:43 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 11 Apr 2021 04:35:43 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32a96003e74381aa8f941ca04050bac2ef44601573854f0c1f244c3a9e17d01`  
		Last Modified: Sat, 10 Apr 2021 17:18:43 GMT  
		Size: 9.9 MB (9872091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdc0d94d9639f64cb041cc65c24a66a9861b8c0ffba33a6eaa17b08d4b7ee1f`  
		Last Modified: Sat, 10 Apr 2021 17:18:36 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae68a3a282a83d0e6da8b00595a45c9fb467b44e46970f00dee3a849e860c81c`  
		Last Modified: Sat, 10 Apr 2021 17:20:12 GMT  
		Size: 20.6 MB (20643582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b299ede54fe617996860ca241d888ae39341d21408e0f7e892ef71dea23ee3`  
		Last Modified: Sat, 10 Apr 2021 17:20:08 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3f682e0e6022db47dfeb5b7d897e2f3d580b1e7021e9ad1580a9faa0ab583`  
		Last Modified: Sun, 11 Apr 2021 04:36:11 GMT  
		Size: 20.4 MB (20372337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a704c2bf4c8c30966924977ffe9778becb7758b4eb14fddb0204d6fe3b6a3c2c`  
		Last Modified: Sun, 11 Apr 2021 04:36:04 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05406b34f11f9cdc4835efbb64c2fd4bafed9ca9584825817acb361653fbc3c7`  
		Last Modified: Sun, 11 Apr 2021 04:36:04 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8417551944365350329ba4ae26dd356821095e2b824303f916582606838b66f`  
		Last Modified: Sun, 11 Apr 2021 04:36:04 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:5fd0d33b8e8909a75e325c318a9a9752e0407eeee3114e2862f71d97c98e5d04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.8 MB (79803809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ced8b947914367b50ac138327136a1fa99a75241f9975b91f8ea4a37071473`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:05:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:20:43 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:20:49 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:20:50 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:24:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:24:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:24:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:24:38 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:32:13 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 11 Apr 2021 04:32:13 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sun, 11 Apr 2021 04:32:14 GMT
ENV TINI_VERSION=0.18.0
# Sun, 11 Apr 2021 04:34:52 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 11 Apr 2021 04:34:56 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 11 Apr 2021 04:34:57 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 11 Apr 2021 04:34:58 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 11 Apr 2021 04:34:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 11 Apr 2021 04:34:59 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 11 Apr 2021 04:35:00 GMT
EXPOSE 24224 5140
# Sun, 11 Apr 2021 04:35:01 GMT
USER fluent
# Sun, 11 Apr 2021 04:35:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 11 Apr 2021 04:35:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d289ca2f3e2b5ab2015b85f9cc2daf060bc66943eb934d2c4bdabcbae6031b1`  
		Last Modified: Sat, 10 Apr 2021 16:48:38 GMT  
		Size: 11.3 MB (11262944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbc8b87c2241a1b73e9420a04309883e1c2157144321db6bef67d5ca1f651d`  
		Last Modified: Sat, 10 Apr 2021 16:48:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805a70932a287839e4483317925d47a504efbbe434fde5824ef4192898e352e2`  
		Last Modified: Sat, 10 Apr 2021 16:50:01 GMT  
		Size: 21.3 MB (21308477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f9a34f968a2b1af6ba62fe49a0831f817c21182613ab38a0633bf356c0cf23`  
		Last Modified: Sat, 10 Apr 2021 16:49:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d99e980b501f019e415420ab51f5dde877aa6e1dc914df5ba7657f6c142023`  
		Last Modified: Sun, 11 Apr 2021 04:35:33 GMT  
		Size: 21.3 MB (21324731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3f963a8c65f1f3ec7b3f26021522236d463e5422fd9a3b3acf21f56bb3f567`  
		Last Modified: Sun, 11 Apr 2021 04:35:27 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f491fa2569dc588e07277e6e4638ae6ad12241dd9118c01991af77ae428074ca`  
		Last Modified: Sun, 11 Apr 2021 04:35:27 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819b4d94209c9a036a49cc9eb1cc7423deeabe1d77e48fa3b75a377339258157`  
		Last Modified: Sun, 11 Apr 2021 04:35:27 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:c3ffe31335efd6e71343fc9abfc312d2ab9612e9f42f2ad6648af6fc702688be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.4 MB (86433699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c225a0de9f1e33c331be92ca420735ff1e2a4a440a19abac791ee2848be7decc`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:38:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 02:38:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:52:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:52:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:52:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:52:19 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 16:10:17 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 10 Apr 2021 16:10:17 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 10 Apr 2021 16:10:18 GMT
ENV TINI_VERSION=0.18.0
# Sat, 10 Apr 2021 16:11:45 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 10 Apr 2021 16:11:46 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 10 Apr 2021 16:11:46 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 10 Apr 2021 16:11:47 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 10 Apr 2021 16:11:47 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 10 Apr 2021 16:11:47 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 10 Apr 2021 16:11:47 GMT
EXPOSE 24224 5140
# Sat, 10 Apr 2021 16:11:48 GMT
USER fluent
# Sat, 10 Apr 2021 16:11:48 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 10 Apr 2021 16:11:48 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0fd260b5f4b604c9bfbc66ee8946e4667087566a076e75b234faaf8363fb9`  
		Last Modified: Sat, 10 Apr 2021 03:11:07 GMT  
		Size: 17.2 MB (17227278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f03815f2ae14591c00fdb7535113d4355263d840a9c34469ae708aea2e74966`  
		Last Modified: Sat, 10 Apr 2021 03:11:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4207aa5aba20825c04fb847653d3cf6d5011040c7f7b8147ce0824ebda58d682`  
		Last Modified: Sat, 10 Apr 2021 03:13:02 GMT  
		Size: 20.9 MB (20909318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a5e3665a3fdb3774edce1b87e369d385982d95b3f12169b947249c7ecb6566`  
		Last Modified: Sat, 10 Apr 2021 03:12:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443cf6115e286b2a34e51a03f2a10dc72c1d582b179767c2bde39e687652d8af`  
		Last Modified: Sat, 10 Apr 2021 16:12:24 GMT  
		Size: 20.5 MB (20505060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fff9d00b311196c3cfb9d474ad570de2fd0ee345bdb420be8f8bdbafb16deaf`  
		Last Modified: Sat, 10 Apr 2021 16:12:18 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecffac34d8a11cf95ca4f69948654a5b3d4ec06c4233e7dd712c2504224b0e8`  
		Last Modified: Sat, 10 Apr 2021 16:12:21 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a131b5d668c368b0885e184e0b768ff1cafcf8c377b1409f5a0b85ddc775d3c`  
		Last Modified: Sat, 10 Apr 2021 16:12:18 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:d7599186b090bbb5b5a0b79439733a88be5acdc0791bb57e60d9b333145b1f74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87135137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dae7eea3d204c4a71a9ecf2e9997a48fe6c5bb1421ba7448dc758329f6096e3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:26:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:26:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 May 2021 02:27:04 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 02:51:24 GMT
ENV RUBY_MAJOR=2.6
# Wed, 12 May 2021 02:51:28 GMT
ENV RUBY_VERSION=2.6.7
# Wed, 12 May 2021 02:51:33 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Wed, 12 May 2021 02:57:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 May 2021 02:57:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 May 2021 02:57:54 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 May 2021 02:57:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 02:58:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 12 May 2021 02:58:17 GMT
CMD ["irb"]
# Wed, 12 May 2021 17:50:55 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 12 May 2021 17:51:01 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Wed, 12 May 2021 17:51:04 GMT
ENV TINI_VERSION=0.18.0
# Wed, 12 May 2021 17:58:10 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 12 May 2021 17:58:27 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 12 May 2021 17:58:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 12 May 2021 17:58:32 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 12 May 2021 17:58:37 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 12 May 2021 17:58:41 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 12 May 2021 17:58:44 GMT
EXPOSE 24224 5140
# Wed, 12 May 2021 17:58:50 GMT
USER fluent
# Wed, 12 May 2021 17:58:54 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 12 May 2021 17:58:59 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dedade3f88269f1f91f5426a0fb429daefc141cb8b32080fddaae850bd454250`  
		Last Modified: Wed, 12 May 2021 03:11:04 GMT  
		Size: 12.7 MB (12704293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c15720eb44eea8269dc8063acd05c6b8085923a743e08789d38b00520a25a8a`  
		Last Modified: Wed, 12 May 2021 03:11:01 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d03da1d7f522bb04a2b2efa68dc4449e5bb95bfc21df66e14c032f1fd4070a`  
		Last Modified: Wed, 12 May 2021 03:12:05 GMT  
		Size: 22.0 MB (21984764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5ed180da0bc643bcacbef2061e6592c859f0267c6ca464f4c34ebe885385a9`  
		Last Modified: Wed, 12 May 2021 03:12:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a23be0ae2c6c81f4bf837cbfbada1afba212f29bd8207e4e7c4134b488a42aa`  
		Last Modified: Wed, 12 May 2021 17:59:24 GMT  
		Size: 21.9 MB (21890609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a48d564b6050df9d6483b8b6571c75b6344e0408362eb3e1bdb390e5e1b631`  
		Last Modified: Wed, 12 May 2021 17:59:19 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1745720f40c1506d02fcbcd88042bbf7d9f260c73c9d5904cf6d4405a31596`  
		Last Modified: Wed, 12 May 2021 17:59:19 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c9185df3c370bc60ce6427e4bfb83807823d0cfbaf5219d2070f59f57c0f5e`  
		Last Modified: Wed, 12 May 2021 17:59:19 GMT  
		Size: 443.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:767479648eff52ee448fd940debc465b11e484d210867db1d76dbb677ddc8283
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79671206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835381118660e9662829bf95a4831f6cf748e1936a6679f4693a4edd40067135`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:51:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 01:51:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:17:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:17:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:17:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:17:20 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 12:28:01 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 10 Apr 2021 12:28:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 10 Apr 2021 12:28:03 GMT
ENV TINI_VERSION=0.18.0
# Sat, 10 Apr 2021 12:30:25 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 10 Apr 2021 12:30:30 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 10 Apr 2021 12:30:31 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 10 Apr 2021 12:30:31 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 10 Apr 2021 12:30:32 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 10 Apr 2021 12:30:33 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 10 Apr 2021 12:30:33 GMT
EXPOSE 24224 5140
# Sat, 10 Apr 2021 12:30:34 GMT
USER fluent
# Sat, 10 Apr 2021 12:30:34 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 10 Apr 2021 12:30:35 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1e1850cea86d76ca69c7e014fa38730a01b6a7a6e1957745093b641be6947`  
		Last Modified: Sat, 10 Apr 2021 02:22:13 GMT  
		Size: 10.8 MB (10814272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5f18b62b368568a1040cba71445a611715e0c1d813045988453b628a8cec6`  
		Last Modified: Sat, 10 Apr 2021 02:22:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f085c8813292ca999ce489985962c48c430c2055b5e583be1f6f4e0dfd5353`  
		Last Modified: Sat, 10 Apr 2021 02:22:58 GMT  
		Size: 21.6 MB (21618739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea955664e86a3a2fc2a4765705d82563887aaa4c51dd1b6de0ad1d783561ee90`  
		Last Modified: Sat, 10 Apr 2021 02:22:56 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfac4078672b0b6e4aaa4ff0e50e5b57279f5288e42315c2f5238e65b96e6bd`  
		Last Modified: Sat, 10 Apr 2021 12:31:06 GMT  
		Size: 21.5 MB (21481324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074e72eb6a367bc21c484140c50930d582687818392d254924ddb2223fcf51c1`  
		Last Modified: Sat, 10 Apr 2021 12:31:03 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f6cc9f6426fb62e324e912ac2232e40fa10be75a00e2524e15709f2f3d5dc8`  
		Last Modified: Sat, 10 Apr 2021 12:31:05 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2053299b0553931e2773ad6d80c3eaa4640b6ce0e155d1f97378c35ca427ba17`  
		Last Modified: Sat, 10 Apr 2021 12:31:06 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.9.1-1.0`

```console
$ docker pull fluentd@sha256:47c595013b00409fd52d7165773731c6a360cd610d513c665a04c2923d89fba8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.9.1-1.0` - linux; amd64

```console
$ docker pull fluentd@sha256:3536d047aa7a961d8c826617282e8afa2075990c7e4be122a6501605ec5f3a8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15174420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b84547e9c6cfe8be39cc6870d9b942554d48005ecf5cd2ba4156a3a380fa53a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 11:38:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Mar 2021 11:38:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 13 Mar 2021 11:39:29 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 13 Mar 2021 11:39:30 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Mar 2021 11:39:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Mar 2021 11:39:31 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 13 Mar 2021 11:39:31 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Mar 2021 11:39:31 GMT
ENV LD_PRELOAD=
# Sat, 13 Mar 2021 11:39:31 GMT
EXPOSE 24224 5140
# Sat, 13 Mar 2021 11:39:31 GMT
USER fluent
# Sat, 13 Mar 2021 11:39:32 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Mar 2021 11:39:32 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9651430fd06f066ea7cd1dde55009fe606a5c9357f60d2c418363f4c8d3e29d6`  
		Last Modified: Sat, 13 Mar 2021 11:41:13 GMT  
		Size: 12.4 MB (12398794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1eccd3574cb406400b237809e45a86e63983263d1f67e8887c6e89d31ef835`  
		Last Modified: Sat, 13 Mar 2021 11:41:11 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd5db2e3e2d262b39a393666a8efc9edb577b63c8f3934f23e7f16425cd4cd`  
		Last Modified: Sat, 13 Mar 2021 11:41:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d18dcc36773b2d18dbe989da843efc8bee18a990bfd603d2a340174c3246af`  
		Last Modified: Sat, 13 Mar 2021 11:41:11 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9.1-1.0` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:44f31c1936eb1fb832ffab84cf23b98d016b2646cae11aaec96aef5939cd17e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15976216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021add57c37363fa0e7aa9dd21f7a3fe33da8e7e72cb09d25d866ddb6f3fd259`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:39:49 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Apr 2020 17:39:50 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Thu, 23 Apr 2020 17:41:27 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Apr 2020 17:41:31 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Apr 2020 17:41:32 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Apr 2020 17:41:32 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Apr 2020 17:41:33 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Apr 2020 17:41:34 GMT
ENV LD_PRELOAD=
# Thu, 23 Apr 2020 17:41:34 GMT
EXPOSE 24224 5140
# Thu, 23 Apr 2020 17:41:35 GMT
USER fluent
# Thu, 23 Apr 2020 17:41:36 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Apr 2020 17:41:37 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d522b01371d30767392094a66b629aa2f6a1cfeeb82ae15eeb64f931a1fa4b`  
		Last Modified: Thu, 23 Apr 2020 17:42:00 GMT  
		Size: 13.4 MB (13425275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad32a34e355514cb68abd5ee8454fa9b8f13c30395d005fccaa99434a30406e`  
		Last Modified: Thu, 23 Apr 2020 17:41:55 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f703ee04ff8bd4f967972c80763171663ea5f1670044ebf18ff8273097c5c5`  
		Last Modified: Thu, 23 Apr 2020 17:41:55 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c24c5529dab1e5be1e7eec9c51d402281e9e72a5e13f9244a461073bca7241c`  
		Last Modified: Thu, 23 Apr 2020 17:41:55 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9.1-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:9a3af653771a6a04c358f7c2a60b8bb57c64d3de5dd298c0d4657ceb35ea0f66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16449859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d62a0ca09e6cfbf89d9db9d526962faa229e3de5ec48e9ef934e8566431b4c9d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:05:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 24 Apr 2020 09:05:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Fri, 24 Apr 2020 09:06:41 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Fri, 24 Apr 2020 09:06:45 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 24 Apr 2020 09:06:46 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 24 Apr 2020 09:06:46 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Fri, 24 Apr 2020 09:06:47 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 24 Apr 2020 09:06:48 GMT
ENV LD_PRELOAD=
# Fri, 24 Apr 2020 09:06:48 GMT
EXPOSE 24224 5140
# Fri, 24 Apr 2020 09:06:49 GMT
USER fluent
# Fri, 24 Apr 2020 09:06:49 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 24 Apr 2020 09:06:50 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7c433500fac88cd265a112da6bb53517cca36634a766db54f966da1f64e6ae`  
		Last Modified: Fri, 24 Apr 2020 09:07:26 GMT  
		Size: 13.8 MB (13753176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcba662d9a25425bd9d1fd78c25999719742ab37190f21b0228c999766407978`  
		Last Modified: Fri, 24 Apr 2020 09:07:20 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a458dc4b98ef9ffa86fcd837c55416fd16fee3a6154a3e1f38011c7dad2a51`  
		Last Modified: Fri, 24 Apr 2020 09:07:20 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0293d533db263a29c969b1f2ca4ef1c0df2bbfe728041795f264b905641d6009`  
		Last Modified: Fri, 24 Apr 2020 09:07:20 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9.1-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:2674458e5ee30b6811a635b030e7a5c02f09a60ac2b526e9233ae520b9e52d36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15066972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6050199bd42bf9ce01c19ba5ea4ae473745e01fa2692be5d9603f3ab09958dc7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 04:51:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Mar 2021 04:51:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 13 Mar 2021 04:53:00 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 13 Mar 2021 04:53:03 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Mar 2021 04:53:04 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Mar 2021 04:53:04 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 13 Mar 2021 04:53:05 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Mar 2021 04:53:05 GMT
ENV LD_PRELOAD=
# Sat, 13 Mar 2021 04:53:05 GMT
EXPOSE 24224 5140
# Sat, 13 Mar 2021 04:53:06 GMT
USER fluent
# Sat, 13 Mar 2021 04:53:06 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Mar 2021 04:53:07 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a86c3883d026d251c0b98f179473179adc48ddd9931c34671ec927485c2b30`  
		Last Modified: Sat, 13 Mar 2021 04:56:41 GMT  
		Size: 12.3 MB (12295016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdff586ec846debe504cab0d5418aed7a757990f1c2e5535febd3c2434383f9`  
		Last Modified: Sat, 13 Mar 2021 04:56:36 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec361a5d42c106aff6fc935ed2b65a028307e9e2fee0160ec1d41376855b6969`  
		Last Modified: Sat, 13 Mar 2021 04:56:36 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1fe75d1dda1ff8c1442a52d915e50e76400a2c2499c166340a71e5c9953409`  
		Last Modified: Sat, 13 Mar 2021 04:56:36 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9.1-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:624655b564b9a0d8aff2adb11bc4e4ab152cc6cddbb0f80dbec0ccc280a6c7e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16969348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9996e3889db7f499cb26285f39e7577a3572c8c83eefb66472ac0e3d67d6c9f7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 20:41:14 GMT
ADD file:2eaa074d9379f98d31cc4112997e1c1bb55b3871574af6aee576cf1c5ed99645 in / 
# Thu, 23 Apr 2020 20:41:16 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:52:12 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 24 Apr 2020 02:52:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Fri, 24 Apr 2020 02:53:15 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Fri, 24 Apr 2020 02:53:21 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 24 Apr 2020 02:53:21 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 24 Apr 2020 02:53:22 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Fri, 24 Apr 2020 02:53:24 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 24 Apr 2020 02:53:26 GMT
ENV LD_PRELOAD=
# Fri, 24 Apr 2020 02:53:27 GMT
EXPOSE 24224 5140
# Fri, 24 Apr 2020 02:53:29 GMT
USER fluent
# Fri, 24 Apr 2020 02:53:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 24 Apr 2020 02:53:33 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:16f2eaeeecc1446c304d41ae21441f168e376dc76733ec3a9f8f2d17119638a1`  
		Last Modified: Thu, 23 Apr 2020 20:41:57 GMT  
		Size: 2.8 MB (2787865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27df74a3decbbc71f688e8319c7055315cbba6b350b28324d4ad9c021ca50135`  
		Last Modified: Fri, 24 Apr 2020 02:54:03 GMT  
		Size: 14.2 MB (14179267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1465abcf9b778cb4d299d4fec3ccbd1b1284867a62dc8b6d6d59a7a195cc0203`  
		Last Modified: Fri, 24 Apr 2020 02:53:59 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b323e14271e2cf6ac4ee482e207353aa39585d4e58bf75475fe54e2a7f1fdb65`  
		Last Modified: Fri, 24 Apr 2020 02:53:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a13af9e734338dbe7adf7de4ab71210d13beaeed6a6fec5d7b9a7b4dff17131`  
		Last Modified: Fri, 24 Apr 2020 02:53:59 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9.1-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:12f970948d5704cc42194be7cbfd8fe038e802f8fc2fb8f2169bf7c4c2c5eb5b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16441885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b6e3f25bb06297f8b35538b6b7a44d6c0ce04bfa379393397e3eef1c4c16e9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:19 GMT
ADD file:87357838aa76ab358b68ac6734871df2dacb0b5918d89a091836f0d33264f803 in / 
# Thu, 23 Apr 2020 17:51:20 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 19:59:44 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Apr 2020 19:59:44 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Thu, 23 Apr 2020 20:00:12 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Apr 2020 20:00:14 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Apr 2020 20:00:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Apr 2020 20:00:14 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Apr 2020 20:00:14 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Apr 2020 20:00:14 GMT
ENV LD_PRELOAD=
# Thu, 23 Apr 2020 20:00:15 GMT
EXPOSE 24224 5140
# Thu, 23 Apr 2020 20:00:15 GMT
USER fluent
# Thu, 23 Apr 2020 20:00:15 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Apr 2020 20:00:15 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1aff3887737eb15ee1a53e92e8c87162b9caac2281ecb01242da00d1a32f5a04`  
		Last Modified: Thu, 23 Apr 2020 17:51:52 GMT  
		Size: 2.6 MB (2550329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84a8d1f46d684e96854f17f7222edf696d71cf5cd842954e92f378e005dab17`  
		Last Modified: Thu, 23 Apr 2020 20:00:33 GMT  
		Size: 13.9 MB (13889338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52edf66127670c83c7f5a2aed5e38db5dca87e51eb8966174df5900dc2e0c9`  
		Last Modified: Thu, 23 Apr 2020 20:00:30 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec06b392ce74e92be850c3ddc84f05a6f54ed80e3920a6da6d4327a8d62b5137`  
		Last Modified: Thu, 23 Apr 2020 20:00:35 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d063c86f8d64af1ad29498f54a054870ec143617b700e0f374dd7a023214ef43`  
		Last Modified: Thu, 23 Apr 2020 20:00:35 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.9.1-debian-1.0`

```console
$ docker pull fluentd@sha256:aabb22577d9f8b7752a85ab0019a78f6d8e7ea2cffb69b646e7f1b423c8f053c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.9.1-debian-1.0` - linux; amd64

```console
$ docker pull fluentd@sha256:252da65de6465d0add2906b1687269ba7edf1fb510811507bce09a60c0381f38
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82493451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69ea641f7940f8a6ad3bef97a31463ea1255b1603e1ee37486cdfdc4d98cc0ec`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 18:49:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:49:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:49:04 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:53:53 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 11 Apr 2021 06:53:53 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sun, 11 Apr 2021 06:53:53 GMT
ENV TINI_VERSION=0.18.0
# Sun, 11 Apr 2021 06:55:05 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 11 Apr 2021 06:55:06 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 11 Apr 2021 06:55:07 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 11 Apr 2021 06:55:07 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 11 Apr 2021 06:55:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 11 Apr 2021 06:55:07 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 11 Apr 2021 06:55:07 GMT
EXPOSE 24224 5140
# Sun, 11 Apr 2021 06:55:07 GMT
USER fluent
# Sun, 11 Apr 2021 06:55:08 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 11 Apr 2021 06:55:08 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451af66bced958304be82120827542b55bd2229f2e83c5a058a441fa74254828`  
		Last Modified: Sat, 10 Apr 2021 19:10:36 GMT  
		Size: 21.5 MB (21467370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3264de8e4173291cbec86320f1fe2733ffcdc3ff53cfa7c0d3238e334b79dea`  
		Last Modified: Sat, 10 Apr 2021 19:10:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f112accd4f78deefda257913b04cde0a37df82ac2d22321d7b9e3e0a1fad44f9`  
		Last Modified: Sun, 11 Apr 2021 06:55:35 GMT  
		Size: 21.3 MB (21321334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c187eda5e9fa5dcc2b79f1378157a285315472df354493334defe33e508356`  
		Last Modified: Sun, 11 Apr 2021 06:55:32 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc82756b1be22095f405aa9e758dd71424e1033fd10ba535fc716d4dc426286`  
		Last Modified: Sun, 11 Apr 2021 06:55:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef63675e64ab7fae4cf4e0fc5637b6429fdcc3ae067f979cd8ada813fe4c9dcb`  
		Last Modified: Sun, 11 Apr 2021 06:55:32 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9.1-debian-1.0` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:84afb53ffc4f4ddd57698dcb9ec356e3fbdbef288f3a02cafd71ab14161c370d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76427847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc3dd148b0b5c3d5f32fe1d3b8c07649d5664c438c8dbeb7ec6a534e3517e5e`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:27:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 07:27:10 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 07:42:11 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 07:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 07:45:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 07:45:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 07:45:55 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 17:32:57 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 10 Apr 2021 17:32:58 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 10 Apr 2021 17:32:59 GMT
ENV TINI_VERSION=0.18.0
# Sat, 10 Apr 2021 17:36:05 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 10 Apr 2021 17:36:09 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 10 Apr 2021 17:36:11 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 10 Apr 2021 17:36:11 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 10 Apr 2021 17:36:12 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 10 Apr 2021 17:36:13 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 10 Apr 2021 17:36:14 GMT
EXPOSE 24224 5140
# Sat, 10 Apr 2021 17:36:15 GMT
USER fluent
# Sat, 10 Apr 2021 17:36:15 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 10 Apr 2021 17:36:16 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8fc93885ff1edc1fec20b799c1c02e672d75d967815f7a98ffe7cb94969e2`  
		Last Modified: Sat, 10 Apr 2021 08:11:28 GMT  
		Size: 10.3 MB (10345305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfdecedfe5bd31f7499d5973d09b2665408cca73a9e1f83fea87d261763e6a`  
		Last Modified: Sat, 10 Apr 2021 08:11:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64f63c1e0d3af67924d2d3ef5636ed70900748b90fffc5bf4e748a38ef7d125`  
		Last Modified: Sat, 10 Apr 2021 08:12:41 GMT  
		Size: 20.7 MB (20732839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9ef980b82778a927138ed4192338fea82cdb79fe3d25e26ac958cc5dc33d62`  
		Last Modified: Sat, 10 Apr 2021 08:12:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2be6a3e99897bfd8c8b0031cdca1954ee20743702502780d2bddc483248e9f5`  
		Last Modified: Sat, 10 Apr 2021 17:36:45 GMT  
		Size: 20.5 MB (20473445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448f85071b171ec5a492b293fe248da108943b0d54e52333d93fc8b294d80608`  
		Last Modified: Sat, 10 Apr 2021 17:36:39 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7873e0b58f6016208e2f37cd0b8c984f219f2c53b140300380522a20bb0fc3b7`  
		Last Modified: Sat, 10 Apr 2021 17:36:39 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5182351736a7c8610417ae03f6776a1b7a01e977abc3fd33c58a68c11ffb0b64`  
		Last Modified: Sat, 10 Apr 2021 17:36:39 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9.1-debian-1.0` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:4bb4f27f160486872fa2538880cc99f0aa14389ace3139be5e3bc18129aaeb68
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73630876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28c30b78c53b091a8bbd464260d9386ee3a8a2679f24245f599a913f2c6122c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:21:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:21:36 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:49:54 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:49:56 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:49:57 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:53:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:53:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:53:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:53:49 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:32:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 11 Apr 2021 04:32:55 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sun, 11 Apr 2021 04:32:56 GMT
ENV TINI_VERSION=0.18.0
# Sun, 11 Apr 2021 04:35:31 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 11 Apr 2021 04:35:35 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 11 Apr 2021 04:35:36 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 11 Apr 2021 04:35:37 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 11 Apr 2021 04:35:38 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 11 Apr 2021 04:35:39 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 11 Apr 2021 04:35:40 GMT
EXPOSE 24224 5140
# Sun, 11 Apr 2021 04:35:41 GMT
USER fluent
# Sun, 11 Apr 2021 04:35:43 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 11 Apr 2021 04:35:43 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32a96003e74381aa8f941ca04050bac2ef44601573854f0c1f244c3a9e17d01`  
		Last Modified: Sat, 10 Apr 2021 17:18:43 GMT  
		Size: 9.9 MB (9872091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdc0d94d9639f64cb041cc65c24a66a9861b8c0ffba33a6eaa17b08d4b7ee1f`  
		Last Modified: Sat, 10 Apr 2021 17:18:36 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae68a3a282a83d0e6da8b00595a45c9fb467b44e46970f00dee3a849e860c81c`  
		Last Modified: Sat, 10 Apr 2021 17:20:12 GMT  
		Size: 20.6 MB (20643582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b299ede54fe617996860ca241d888ae39341d21408e0f7e892ef71dea23ee3`  
		Last Modified: Sat, 10 Apr 2021 17:20:08 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3f682e0e6022db47dfeb5b7d897e2f3d580b1e7021e9ad1580a9faa0ab583`  
		Last Modified: Sun, 11 Apr 2021 04:36:11 GMT  
		Size: 20.4 MB (20372337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a704c2bf4c8c30966924977ffe9778becb7758b4eb14fddb0204d6fe3b6a3c2c`  
		Last Modified: Sun, 11 Apr 2021 04:36:04 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05406b34f11f9cdc4835efbb64c2fd4bafed9ca9584825817acb361653fbc3c7`  
		Last Modified: Sun, 11 Apr 2021 04:36:04 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8417551944365350329ba4ae26dd356821095e2b824303f916582606838b66f`  
		Last Modified: Sun, 11 Apr 2021 04:36:04 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9.1-debian-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:5fd0d33b8e8909a75e325c318a9a9752e0407eeee3114e2862f71d97c98e5d04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.8 MB (79803809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ced8b947914367b50ac138327136a1fa99a75241f9975b91f8ea4a37071473`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:05:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:20:43 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:20:49 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:20:50 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:24:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:24:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:24:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:24:38 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:32:13 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 11 Apr 2021 04:32:13 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sun, 11 Apr 2021 04:32:14 GMT
ENV TINI_VERSION=0.18.0
# Sun, 11 Apr 2021 04:34:52 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 11 Apr 2021 04:34:56 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 11 Apr 2021 04:34:57 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 11 Apr 2021 04:34:58 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 11 Apr 2021 04:34:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 11 Apr 2021 04:34:59 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 11 Apr 2021 04:35:00 GMT
EXPOSE 24224 5140
# Sun, 11 Apr 2021 04:35:01 GMT
USER fluent
# Sun, 11 Apr 2021 04:35:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 11 Apr 2021 04:35:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d289ca2f3e2b5ab2015b85f9cc2daf060bc66943eb934d2c4bdabcbae6031b1`  
		Last Modified: Sat, 10 Apr 2021 16:48:38 GMT  
		Size: 11.3 MB (11262944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbc8b87c2241a1b73e9420a04309883e1c2157144321db6bef67d5ca1f651d`  
		Last Modified: Sat, 10 Apr 2021 16:48:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805a70932a287839e4483317925d47a504efbbe434fde5824ef4192898e352e2`  
		Last Modified: Sat, 10 Apr 2021 16:50:01 GMT  
		Size: 21.3 MB (21308477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f9a34f968a2b1af6ba62fe49a0831f817c21182613ab38a0633bf356c0cf23`  
		Last Modified: Sat, 10 Apr 2021 16:49:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d99e980b501f019e415420ab51f5dde877aa6e1dc914df5ba7657f6c142023`  
		Last Modified: Sun, 11 Apr 2021 04:35:33 GMT  
		Size: 21.3 MB (21324731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3f963a8c65f1f3ec7b3f26021522236d463e5422fd9a3b3acf21f56bb3f567`  
		Last Modified: Sun, 11 Apr 2021 04:35:27 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f491fa2569dc588e07277e6e4638ae6ad12241dd9118c01991af77ae428074ca`  
		Last Modified: Sun, 11 Apr 2021 04:35:27 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819b4d94209c9a036a49cc9eb1cc7423deeabe1d77e48fa3b75a377339258157`  
		Last Modified: Sun, 11 Apr 2021 04:35:27 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9.1-debian-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:c3ffe31335efd6e71343fc9abfc312d2ab9612e9f42f2ad6648af6fc702688be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.4 MB (86433699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c225a0de9f1e33c331be92ca420735ff1e2a4a440a19abac791ee2848be7decc`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:38:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 02:38:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:52:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:52:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:52:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:52:19 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 16:10:17 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 10 Apr 2021 16:10:17 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 10 Apr 2021 16:10:18 GMT
ENV TINI_VERSION=0.18.0
# Sat, 10 Apr 2021 16:11:45 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 10 Apr 2021 16:11:46 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 10 Apr 2021 16:11:46 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 10 Apr 2021 16:11:47 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 10 Apr 2021 16:11:47 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 10 Apr 2021 16:11:47 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 10 Apr 2021 16:11:47 GMT
EXPOSE 24224 5140
# Sat, 10 Apr 2021 16:11:48 GMT
USER fluent
# Sat, 10 Apr 2021 16:11:48 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 10 Apr 2021 16:11:48 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0fd260b5f4b604c9bfbc66ee8946e4667087566a076e75b234faaf8363fb9`  
		Last Modified: Sat, 10 Apr 2021 03:11:07 GMT  
		Size: 17.2 MB (17227278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f03815f2ae14591c00fdb7535113d4355263d840a9c34469ae708aea2e74966`  
		Last Modified: Sat, 10 Apr 2021 03:11:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4207aa5aba20825c04fb847653d3cf6d5011040c7f7b8147ce0824ebda58d682`  
		Last Modified: Sat, 10 Apr 2021 03:13:02 GMT  
		Size: 20.9 MB (20909318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a5e3665a3fdb3774edce1b87e369d385982d95b3f12169b947249c7ecb6566`  
		Last Modified: Sat, 10 Apr 2021 03:12:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443cf6115e286b2a34e51a03f2a10dc72c1d582b179767c2bde39e687652d8af`  
		Last Modified: Sat, 10 Apr 2021 16:12:24 GMT  
		Size: 20.5 MB (20505060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fff9d00b311196c3cfb9d474ad570de2fd0ee345bdb420be8f8bdbafb16deaf`  
		Last Modified: Sat, 10 Apr 2021 16:12:18 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecffac34d8a11cf95ca4f69948654a5b3d4ec06c4233e7dd712c2504224b0e8`  
		Last Modified: Sat, 10 Apr 2021 16:12:21 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a131b5d668c368b0885e184e0b768ff1cafcf8c377b1409f5a0b85ddc775d3c`  
		Last Modified: Sat, 10 Apr 2021 16:12:18 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9.1-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:d7599186b090bbb5b5a0b79439733a88be5acdc0791bb57e60d9b333145b1f74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87135137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dae7eea3d204c4a71a9ecf2e9997a48fe6c5bb1421ba7448dc758329f6096e3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:26:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:26:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 May 2021 02:27:04 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 02:51:24 GMT
ENV RUBY_MAJOR=2.6
# Wed, 12 May 2021 02:51:28 GMT
ENV RUBY_VERSION=2.6.7
# Wed, 12 May 2021 02:51:33 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Wed, 12 May 2021 02:57:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 May 2021 02:57:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 May 2021 02:57:54 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 May 2021 02:57:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 02:58:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 12 May 2021 02:58:17 GMT
CMD ["irb"]
# Wed, 12 May 2021 17:50:55 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 12 May 2021 17:51:01 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Wed, 12 May 2021 17:51:04 GMT
ENV TINI_VERSION=0.18.0
# Wed, 12 May 2021 17:58:10 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 12 May 2021 17:58:27 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 12 May 2021 17:58:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 12 May 2021 17:58:32 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 12 May 2021 17:58:37 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 12 May 2021 17:58:41 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 12 May 2021 17:58:44 GMT
EXPOSE 24224 5140
# Wed, 12 May 2021 17:58:50 GMT
USER fluent
# Wed, 12 May 2021 17:58:54 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 12 May 2021 17:58:59 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dedade3f88269f1f91f5426a0fb429daefc141cb8b32080fddaae850bd454250`  
		Last Modified: Wed, 12 May 2021 03:11:04 GMT  
		Size: 12.7 MB (12704293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c15720eb44eea8269dc8063acd05c6b8085923a743e08789d38b00520a25a8a`  
		Last Modified: Wed, 12 May 2021 03:11:01 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d03da1d7f522bb04a2b2efa68dc4449e5bb95bfc21df66e14c032f1fd4070a`  
		Last Modified: Wed, 12 May 2021 03:12:05 GMT  
		Size: 22.0 MB (21984764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5ed180da0bc643bcacbef2061e6592c859f0267c6ca464f4c34ebe885385a9`  
		Last Modified: Wed, 12 May 2021 03:12:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a23be0ae2c6c81f4bf837cbfbada1afba212f29bd8207e4e7c4134b488a42aa`  
		Last Modified: Wed, 12 May 2021 17:59:24 GMT  
		Size: 21.9 MB (21890609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a48d564b6050df9d6483b8b6571c75b6344e0408362eb3e1bdb390e5e1b631`  
		Last Modified: Wed, 12 May 2021 17:59:19 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1745720f40c1506d02fcbcd88042bbf7d9f260c73c9d5904cf6d4405a31596`  
		Last Modified: Wed, 12 May 2021 17:59:19 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c9185df3c370bc60ce6427e4bfb83807823d0cfbaf5219d2070f59f57c0f5e`  
		Last Modified: Wed, 12 May 2021 17:59:19 GMT  
		Size: 443.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.9.1-debian-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:767479648eff52ee448fd940debc465b11e484d210867db1d76dbb677ddc8283
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79671206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835381118660e9662829bf95a4831f6cf748e1936a6679f4693a4edd40067135`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:51:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 01:51:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:17:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:17:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:17:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:17:20 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 12:28:01 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 10 Apr 2021 12:28:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.9.1
# Sat, 10 Apr 2021 12:28:03 GMT
ENV TINI_VERSION=0.18.0
# Sat, 10 Apr 2021 12:30:25 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.3.0  && gem install async-http -v 0.50.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.9.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sat, 10 Apr 2021 12:30:30 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 10 Apr 2021 12:30:31 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 10 Apr 2021 12:30:31 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sat, 10 Apr 2021 12:30:32 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 10 Apr 2021 12:30:33 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 10 Apr 2021 12:30:33 GMT
EXPOSE 24224 5140
# Sat, 10 Apr 2021 12:30:34 GMT
USER fluent
# Sat, 10 Apr 2021 12:30:34 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 10 Apr 2021 12:30:35 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1e1850cea86d76ca69c7e014fa38730a01b6a7a6e1957745093b641be6947`  
		Last Modified: Sat, 10 Apr 2021 02:22:13 GMT  
		Size: 10.8 MB (10814272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5f18b62b368568a1040cba71445a611715e0c1d813045988453b628a8cec6`  
		Last Modified: Sat, 10 Apr 2021 02:22:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f085c8813292ca999ce489985962c48c430c2055b5e583be1f6f4e0dfd5353`  
		Last Modified: Sat, 10 Apr 2021 02:22:58 GMT  
		Size: 21.6 MB (21618739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea955664e86a3a2fc2a4765705d82563887aaa4c51dd1b6de0ad1d783561ee90`  
		Last Modified: Sat, 10 Apr 2021 02:22:56 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfac4078672b0b6e4aaa4ff0e50e5b57279f5288e42315c2f5238e65b96e6bd`  
		Last Modified: Sat, 10 Apr 2021 12:31:06 GMT  
		Size: 21.5 MB (21481324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074e72eb6a367bc21c484140c50930d582687818392d254924ddb2223fcf51c1`  
		Last Modified: Sat, 10 Apr 2021 12:31:03 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f6cc9f6426fb62e324e912ac2232e40fa10be75a00e2524e15709f2f3d5dc8`  
		Last Modified: Sat, 10 Apr 2021 12:31:05 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2053299b0553931e2773ad6d80c3eaa4640b6ce0e155d1f97378c35ca427ba17`  
		Last Modified: Sat, 10 Apr 2021 12:31:06 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
