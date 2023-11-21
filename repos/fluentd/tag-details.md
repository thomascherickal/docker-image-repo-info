<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.16-1`](#fluentdv116-1)
-	[`fluentd:v1.16-debian-1`](#fluentdv116-debian-1)
-	[`fluentd:v1.16.2-1.1`](#fluentdv1162-11)
-	[`fluentd:v1.16.2-debian-1.1`](#fluentdv1162-debian-11)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:346358e90c07ef9a6b9fad03489f867cb5dc75a00b3106ff410f6c513379fb75
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
$ docker pull fluentd@sha256:75bfe9553d8eaf41b853feea165a34a0ebcbe16913678f59da28bf1e67f0b914
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25156753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5753cb15f75469b9c70d6caf78efb15ac5262723e1384512538b8ed8602cc58`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:55:55 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:55:55 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:56:48 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:56:49 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:56:49 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:56:49 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:56:49 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:56:49 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:56:49 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:56:49 GMT
USER fluent
# Sat, 21 Oct 2023 00:56:49 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:56:50 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8376758d7f65ec25ea223ef7bbafc5f26e793c3bdcafc8dc00773e671afd2e79`  
		Last Modified: Sat, 21 Oct 2023 00:57:05 GMT  
		Size: 21.8 MB (21775931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc4563dcb0c96767d1176a0f296533198190b7de7ce870b687cc2b26eb9307b`  
		Last Modified: Sat, 21 Oct 2023 00:57:02 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84aaef6731a67021e310e6ee61efdd50d535063cd745b58537b5d6be1b403fd5`  
		Last Modified: Sat, 21 Oct 2023 00:57:02 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb379e120ea943cd6686bd302e2852c6de2e6ad4df759a3fa01267f493b103`  
		Last Modified: Sat, 21 Oct 2023 00:57:02 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:3f2213b3ceb36bd178b3b9c9da6605c0256bea34aa720753ce22fb98a9d175ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23848320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa175d111a15eaebd49daa0be452360294ac5c6951a5f289f9d98e2db825c9a3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:20:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:20:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:21:16 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:21:17 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:21:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:21:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:21:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:21:17 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:21:17 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:21:17 GMT
USER fluent
# Sat, 21 Oct 2023 00:21:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:21:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6272f5aba2d83ca3cb0da9b8b8ea413c4405314184d890c9f45ec6ce7bea5b2c`  
		Last Modified: Sat, 21 Oct 2023 00:21:40 GMT  
		Size: 20.7 MB (20733652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acffb79d5a5cdc39102cfbb99f6964b1acbcb76a9161b9ba2b5d51d36a630cee`  
		Last Modified: Sat, 21 Oct 2023 00:21:37 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7fbc6130e444eb89d15b84ab466005aa2df1d603163787a827420db07a5d2e`  
		Last Modified: Sat, 21 Oct 2023 00:21:37 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381df3c8eabfef21742251b70c22a41ac7ea8a9de052debdbbad3795b6ecaf35`  
		Last Modified: Sat, 21 Oct 2023 00:21:37 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:06b726c6f3eefae9ce8fa10746eee66af26fb9852c1881ad286af276cbd102d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24630185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44dfb8e93fecfed45462613ac7f31978908f5ba8ece4ae3d75f327eb79e87ec6`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:54:45 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:54:45 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:55:33 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:55:33 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:55:34 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:55:34 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:55:34 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:55:34 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:55:34 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:55:34 GMT
USER fluent
# Sat, 21 Oct 2023 00:55:34 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:55:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1ec00e7593c94a73645d5a23538f5a0ef272148c631fb2180c364c09dc4378`  
		Last Modified: Sat, 21 Oct 2023 00:55:54 GMT  
		Size: 21.4 MB (21369678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b25585882671ccef4c985197c364aa727f0e1d8b6fc53413ed04a6c0826196d`  
		Last Modified: Sat, 21 Oct 2023 00:55:52 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7b079d03420368b92ebded355718f1a1118f9d739dbfcec2ea73fbf2d91f7d`  
		Last Modified: Sat, 21 Oct 2023 00:55:52 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38769e98bf3af23f79f56d9a58e37a428bb84a00114581b22f85626b9d1e7f2`  
		Last Modified: Sat, 21 Oct 2023 00:55:52 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; 386

```console
$ docker pull fluentd@sha256:18747edca75cbd0a32946c24e0f96ff179fbc13d20ca08482c6d438ad67fb370
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24437983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0ad11bd392e421c8a344cb4ab2eac725292e368cfd3a5c9b586c85bea6a2fb`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:00:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 01:00:43 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 01:01:57 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 01:01:58 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 01:01:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 01:01:58 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 01:01:58 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 01:01:58 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 01:01:58 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 01:01:58 GMT
USER fluent
# Sat, 21 Oct 2023 01:01:58 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 01:01:58 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c98d2d26330aab1341d9ddf5b6d79700d19d8b73621e9bf914723d50eb849a4`  
		Last Modified: Sat, 21 Oct 2023 01:02:19 GMT  
		Size: 21.0 MB (21021988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f39745c5bc83005ffcd79ea3b41adf1712966c62cb9b70a1047342f7627512`  
		Last Modified: Sat, 21 Oct 2023 01:02:15 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61cf065a210c6cdcd8ed51190aa394ed32e605032d5b2d6f9d2d2c921c33bdc`  
		Last Modified: Sat, 21 Oct 2023 01:02:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865efaef1fc67ff9272e0e15d5e27e1730fc0840dae0f145d36c712c19e75dd`  
		Last Modified: Sat, 21 Oct 2023 01:02:15 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:fcb88239c453c4794e186f1701278990a9a737a91b111d7016ef412e91504c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (25011791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b032d1755278e0e612139b445d1ce18ac2150233a9611c9c22ddd4c491cbfacf`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:30:06 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:30:07 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:31:12 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:31:15 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:31:15 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:31:15 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:31:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:31:15 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:31:15 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:31:16 GMT
USER fluent
# Sat, 21 Oct 2023 00:31:16 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:31:16 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbaa2e7f2ea58633b56edda9091ecefa81b8723b7600ce62e5a39da5ffde0f5d`  
		Last Modified: Sat, 21 Oct 2023 00:31:42 GMT  
		Size: 21.6 MB (21618224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daa6ac791df9bca62f53fc841f9b484ebccf3fbbcf52d5cd060477810d7d5b3`  
		Last Modified: Sat, 21 Oct 2023 00:31:39 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4b29672e745496aefa33c93cf65970f072a929fcf9dedc79fda14be98d1342`  
		Last Modified: Sat, 21 Oct 2023 00:31:39 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27f22f12605d3ad806c396c1504a5250ece58cb31d941069ba7425e10d2aae3`  
		Last Modified: Sat, 21 Oct 2023 00:31:39 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:608392169a76d3014e4a408b267bcbb42299b4387a1a92931e79ea65925ac5a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24380635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b094b31e746efa26b3a4b87c04f0c9e51a35d907c1e6f7aa50b1210344df02f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:24:28 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:24:28 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:25:15 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:25:17 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:25:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:25:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:25:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:25:17 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:25:18 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:25:18 GMT
USER fluent
# Sat, 21 Oct 2023 00:25:18 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:25:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313f13302b63aa1e26193c6c3029779f7cf6f9ccfec22267447622329ce2a32`  
		Last Modified: Sat, 21 Oct 2023 00:25:45 GMT  
		Size: 21.2 MB (21202449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d2ca75c30b0833bdbde8dc16d21aefa64e3e7325eff69992cb0ed9ae0135b7`  
		Last Modified: Sat, 21 Oct 2023 00:25:42 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f093efb15da3945df260d185c12c8ad81e19e4cc074ec941fa1b8c66ca8ff34d`  
		Last Modified: Sat, 21 Oct 2023 00:25:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5b744f7972624e9dc72a074aff76bae61e6e0ce6280fffcad2fdda27b1d757`  
		Last Modified: Sat, 21 Oct 2023 00:25:42 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16-1`

```console
$ docker pull fluentd@sha256:346358e90c07ef9a6b9fad03489f867cb5dc75a00b3106ff410f6c513379fb75
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
$ docker pull fluentd@sha256:75bfe9553d8eaf41b853feea165a34a0ebcbe16913678f59da28bf1e67f0b914
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25156753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5753cb15f75469b9c70d6caf78efb15ac5262723e1384512538b8ed8602cc58`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:55:55 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:55:55 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:56:48 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:56:49 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:56:49 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:56:49 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:56:49 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:56:49 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:56:49 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:56:49 GMT
USER fluent
# Sat, 21 Oct 2023 00:56:49 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:56:50 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8376758d7f65ec25ea223ef7bbafc5f26e793c3bdcafc8dc00773e671afd2e79`  
		Last Modified: Sat, 21 Oct 2023 00:57:05 GMT  
		Size: 21.8 MB (21775931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc4563dcb0c96767d1176a0f296533198190b7de7ce870b687cc2b26eb9307b`  
		Last Modified: Sat, 21 Oct 2023 00:57:02 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84aaef6731a67021e310e6ee61efdd50d535063cd745b58537b5d6be1b403fd5`  
		Last Modified: Sat, 21 Oct 2023 00:57:02 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb379e120ea943cd6686bd302e2852c6de2e6ad4df759a3fa01267f493b103`  
		Last Modified: Sat, 21 Oct 2023 00:57:02 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:3f2213b3ceb36bd178b3b9c9da6605c0256bea34aa720753ce22fb98a9d175ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23848320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa175d111a15eaebd49daa0be452360294ac5c6951a5f289f9d98e2db825c9a3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:20:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:20:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:21:16 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:21:17 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:21:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:21:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:21:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:21:17 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:21:17 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:21:17 GMT
USER fluent
# Sat, 21 Oct 2023 00:21:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:21:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6272f5aba2d83ca3cb0da9b8b8ea413c4405314184d890c9f45ec6ce7bea5b2c`  
		Last Modified: Sat, 21 Oct 2023 00:21:40 GMT  
		Size: 20.7 MB (20733652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acffb79d5a5cdc39102cfbb99f6964b1acbcb76a9161b9ba2b5d51d36a630cee`  
		Last Modified: Sat, 21 Oct 2023 00:21:37 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7fbc6130e444eb89d15b84ab466005aa2df1d603163787a827420db07a5d2e`  
		Last Modified: Sat, 21 Oct 2023 00:21:37 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381df3c8eabfef21742251b70c22a41ac7ea8a9de052debdbbad3795b6ecaf35`  
		Last Modified: Sat, 21 Oct 2023 00:21:37 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:06b726c6f3eefae9ce8fa10746eee66af26fb9852c1881ad286af276cbd102d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24630185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44dfb8e93fecfed45462613ac7f31978908f5ba8ece4ae3d75f327eb79e87ec6`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:54:45 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:54:45 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:55:33 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:55:33 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:55:34 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:55:34 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:55:34 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:55:34 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:55:34 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:55:34 GMT
USER fluent
# Sat, 21 Oct 2023 00:55:34 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:55:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1ec00e7593c94a73645d5a23538f5a0ef272148c631fb2180c364c09dc4378`  
		Last Modified: Sat, 21 Oct 2023 00:55:54 GMT  
		Size: 21.4 MB (21369678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b25585882671ccef4c985197c364aa727f0e1d8b6fc53413ed04a6c0826196d`  
		Last Modified: Sat, 21 Oct 2023 00:55:52 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7b079d03420368b92ebded355718f1a1118f9d739dbfcec2ea73fbf2d91f7d`  
		Last Modified: Sat, 21 Oct 2023 00:55:52 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38769e98bf3af23f79f56d9a58e37a428bb84a00114581b22f85626b9d1e7f2`  
		Last Modified: Sat, 21 Oct 2023 00:55:52 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; 386

```console
$ docker pull fluentd@sha256:18747edca75cbd0a32946c24e0f96ff179fbc13d20ca08482c6d438ad67fb370
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24437983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0ad11bd392e421c8a344cb4ab2eac725292e368cfd3a5c9b586c85bea6a2fb`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:00:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 01:00:43 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 01:01:57 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 01:01:58 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 01:01:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 01:01:58 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 01:01:58 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 01:01:58 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 01:01:58 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 01:01:58 GMT
USER fluent
# Sat, 21 Oct 2023 01:01:58 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 01:01:58 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c98d2d26330aab1341d9ddf5b6d79700d19d8b73621e9bf914723d50eb849a4`  
		Last Modified: Sat, 21 Oct 2023 01:02:19 GMT  
		Size: 21.0 MB (21021988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f39745c5bc83005ffcd79ea3b41adf1712966c62cb9b70a1047342f7627512`  
		Last Modified: Sat, 21 Oct 2023 01:02:15 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61cf065a210c6cdcd8ed51190aa394ed32e605032d5b2d6f9d2d2c921c33bdc`  
		Last Modified: Sat, 21 Oct 2023 01:02:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865efaef1fc67ff9272e0e15d5e27e1730fc0840dae0f145d36c712c19e75dd`  
		Last Modified: Sat, 21 Oct 2023 01:02:15 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:fcb88239c453c4794e186f1701278990a9a737a91b111d7016ef412e91504c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (25011791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b032d1755278e0e612139b445d1ce18ac2150233a9611c9c22ddd4c491cbfacf`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:30:06 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:30:07 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:31:12 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:31:15 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:31:15 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:31:15 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:31:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:31:15 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:31:15 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:31:16 GMT
USER fluent
# Sat, 21 Oct 2023 00:31:16 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:31:16 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbaa2e7f2ea58633b56edda9091ecefa81b8723b7600ce62e5a39da5ffde0f5d`  
		Last Modified: Sat, 21 Oct 2023 00:31:42 GMT  
		Size: 21.6 MB (21618224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daa6ac791df9bca62f53fc841f9b484ebccf3fbbcf52d5cd060477810d7d5b3`  
		Last Modified: Sat, 21 Oct 2023 00:31:39 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4b29672e745496aefa33c93cf65970f072a929fcf9dedc79fda14be98d1342`  
		Last Modified: Sat, 21 Oct 2023 00:31:39 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27f22f12605d3ad806c396c1504a5250ece58cb31d941069ba7425e10d2aae3`  
		Last Modified: Sat, 21 Oct 2023 00:31:39 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; s390x

```console
$ docker pull fluentd@sha256:608392169a76d3014e4a408b267bcbb42299b4387a1a92931e79ea65925ac5a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24380635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b094b31e746efa26b3a4b87c04f0c9e51a35d907c1e6f7aa50b1210344df02f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:24:28 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:24:28 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:25:15 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:25:17 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:25:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:25:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:25:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:25:17 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:25:18 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:25:18 GMT
USER fluent
# Sat, 21 Oct 2023 00:25:18 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:25:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313f13302b63aa1e26193c6c3029779f7cf6f9ccfec22267447622329ce2a32`  
		Last Modified: Sat, 21 Oct 2023 00:25:45 GMT  
		Size: 21.2 MB (21202449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d2ca75c30b0833bdbde8dc16d21aefa64e3e7325eff69992cb0ed9ae0135b7`  
		Last Modified: Sat, 21 Oct 2023 00:25:42 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f093efb15da3945df260d185c12c8ad81e19e4cc074ec941fa1b8c66ca8ff34d`  
		Last Modified: Sat, 21 Oct 2023 00:25:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5b744f7972624e9dc72a074aff76bae61e6e0ce6280fffcad2fdda27b1d757`  
		Last Modified: Sat, 21 Oct 2023 00:25:42 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16-debian-1`

```console
$ docker pull fluentd@sha256:177d5718d2a95cba7f7bfa09c2ad684216405bf7742f4522a91904ce7cca17a0
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
$ docker pull fluentd@sha256:b2e067b81f6760f4950fc0a38c87e08e8bc6c3f29a77e7254df79b3f0e4d48a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101942055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23de4c5e1fdc61aabf81a30468da9a7d35270175920d21e42d7b3317ba1a3ea5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 15:18:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 15:18:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Nov 2023 15:18:23 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 15:41:06 GMT
ENV RUBY_MAJOR=3.1
# Wed, 01 Nov 2023 15:41:06 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 01 Nov 2023 15:41:07 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 01 Nov 2023 15:43:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Nov 2023 15:43:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Nov 2023 15:43:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Nov 2023 15:43:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:43:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 01 Nov 2023 15:43:25 GMT
CMD ["irb"]
# Wed, 01 Nov 2023 22:52:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 01 Nov 2023 22:52:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 01 Nov 2023 22:52:10 GMT
ENV TINI_VERSION=0.18.0
# Wed, 01 Nov 2023 22:54:44 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 01 Nov 2023 22:54:45 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 01 Nov 2023 22:54:45 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 01 Nov 2023 22:54:45 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 01 Nov 2023 22:54:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 01 Nov 2023 22:54:45 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 01 Nov 2023 22:54:46 GMT
EXPOSE 24224 5140
# Wed, 01 Nov 2023 22:54:46 GMT
USER fluent
# Wed, 01 Nov 2023 22:54:46 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 01 Nov 2023 22:54:46 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69341098b2f234c853f6ae6ceb2be1816adb67a16d8843cb047a63325fe29a0c`  
		Last Modified: Wed, 01 Nov 2023 15:54:07 GMT  
		Size: 10.0 MB (10021771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b896e7d9a30baf37fad41181a45fece23dadec02936e16200b245819f56dd20`  
		Last Modified: Wed, 01 Nov 2023 15:54:05 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c2aef4794f0df599ddb75459cc12c5fc13e3ed9e05207bd3a4e088ca29d37`  
		Last Modified: Wed, 01 Nov 2023 15:56:40 GMT  
		Size: 32.6 MB (32626521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc381e7e0828635a3041c2c0989aebce36afa41a479118107fe9bead80d99486`  
		Last Modified: Wed, 01 Nov 2023 15:56:37 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be3011a54a05f417a65849cab7dbfd3ea8c5768ad0a6973a272639f3e84fa8a`  
		Last Modified: Wed, 01 Nov 2023 22:55:01 GMT  
		Size: 27.9 MB (27872769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a2463eea66f31090b6f7cd13a9a1cb333099ac3c6c29c80718eea9984c4518`  
		Last Modified: Wed, 01 Nov 2023 22:54:57 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237fedb38023431e2d5274feea0a695a597294f7313b23dedbb17bd081bead0f`  
		Last Modified: Wed, 01 Nov 2023 22:54:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f554862fb4e4a2d79885366bafcbb0fd67ff25bec2867236f62f0520468f4b`  
		Last Modified: Wed, 01 Nov 2023 22:54:57 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:627fa4cb1db78d37fa1938282af8f1930b14a5dd8666f2f27788db127aba7acf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.4 MB (95427791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d807e00bdf0e036aec63d78fd7e9cff46e3a6df2feff484fceded2b2473b104`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:09 GMT
ADD file:f7d1d017cc4e588f213f4536967b8d58c50b8602fb8a10b786856c35a843f31e in / 
# Tue, 21 Nov 2023 05:01:09 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:27:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:27:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 05:27:24 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:38:36 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 05:38:36 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 05:38:36 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 05:40:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 05:40:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 05:40:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 05:40:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 05:40:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 05:40:47 GMT
CMD ["irb"]
# Tue, 21 Nov 2023 16:11:35 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Nov 2023 16:11:35 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 21 Nov 2023 16:11:35 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Nov 2023 16:14:26 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 21 Nov 2023 16:14:26 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Nov 2023 16:14:26 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Nov 2023 16:14:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Nov 2023 16:14:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Nov 2023 16:14:27 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Nov 2023 16:14:27 GMT
EXPOSE 24224 5140
# Tue, 21 Nov 2023 16:14:27 GMT
USER fluent
# Tue, 21 Nov 2023 16:14:27 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Nov 2023 16:14:27 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:d051266714ac5508b442ebbe5911d353bfacddc64f657eeba14a993cced96358`  
		Last Modified: Tue, 21 Nov 2023 05:04:38 GMT  
		Size: 28.9 MB (28921267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec3e2f4ed70f7a6ff62ff15d04822a0dfe972559db93385e2dc8dba05ecb06c`  
		Last Modified: Tue, 21 Nov 2023 05:44:29 GMT  
		Size: 8.6 MB (8634953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbde3702c4b0c15a573b9e7b9c2f87492bad117b7b3c21abd06f5b0f913bdc0`  
		Last Modified: Tue, 21 Nov 2023 05:44:28 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffda89f4ed0e1b94a1fa5862d204c222ae50142552208dc1faa75ff8764c267f`  
		Last Modified: Tue, 21 Nov 2023 05:45:42 GMT  
		Size: 31.2 MB (31166744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14897c4d9cf59fdf6b4be859a107cf3ad20eb2b701011ec5560cb2b54cf399fd`  
		Last Modified: Tue, 21 Nov 2023 05:45:39 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac5b6ce352208b3705bc898ba0d5a987899be48c66554950eb17fcd36767fec`  
		Last Modified: Tue, 21 Nov 2023 16:14:54 GMT  
		Size: 26.7 MB (26701759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2233d7a633e377d238fbc529c3f547c7a4cab4249de5bffe387cb3844f37ca3`  
		Last Modified: Tue, 21 Nov 2023 16:14:49 GMT  
		Size: 1.8 KB (1829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d815726563d183099212915a008e0b36c273b99398f4a249ea5d6a06e5545f5`  
		Last Modified: Tue, 21 Nov 2023 16:14:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2f8b2ca4fa7cd659c07b18329a0e7a383d309932ba977539e80207d610041e`  
		Last Modified: Tue, 21 Nov 2023 16:14:49 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:7f7b83cf352f792f20296950870c3d6736807fb4f83e6f3c63ef9c3c7d0396cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92300695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3590143f467428e2aa2fcf4b183dc86ba10265ced87c079e7ee0377a1862c26`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:04 GMT
ADD file:c4afced274aaa80ab3018b368ed739c1c55e49b41e9637ac44d63e61344fe865 in / 
# Tue, 21 Nov 2023 03:58:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:50:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:50:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 07:50:49 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 08:01:23 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 08:01:23 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 08:01:23 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 08:03:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 08:03:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 08:03:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 08:03:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 08:03:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 08:03:26 GMT
CMD ["irb"]
# Tue, 21 Nov 2023 16:56:48 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Nov 2023 16:56:48 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 21 Nov 2023 16:56:49 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Nov 2023 16:59:38 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 21 Nov 2023 16:59:39 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Nov 2023 16:59:39 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Nov 2023 16:59:39 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Nov 2023 16:59:39 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Nov 2023 16:59:39 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Nov 2023 16:59:39 GMT
EXPOSE 24224 5140
# Tue, 21 Nov 2023 16:59:39 GMT
USER fluent
# Tue, 21 Nov 2023 16:59:39 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Nov 2023 16:59:39 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6dc4ed5513793308b8e30b08e03f97fa54025c3d3f3172c6edccb1dbbc7ff139`  
		Last Modified: Tue, 21 Nov 2023 04:02:35 GMT  
		Size: 26.6 MB (26579014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7011811be080b3ec10eb390c78eb1b81bde867946f61686c1898bb89ef4ee30b`  
		Last Modified: Tue, 21 Nov 2023 08:09:21 GMT  
		Size: 8.1 MB (8143369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17046219f223403a42245317d506cf41d8598ff0e6b724a2f8fd5741a21c82a2`  
		Last Modified: Tue, 21 Nov 2023 08:09:19 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5591c39c82e62aeff5d31f2933194de53fe4c581cea0f7a2c7207a2c4a840e71`  
		Last Modified: Tue, 21 Nov 2023 08:10:45 GMT  
		Size: 31.0 MB (31036973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7879eec1d2c94304558aadea4ff39a09268082325bd71f59c3d23d372fdb2cc4`  
		Last Modified: Tue, 21 Nov 2023 08:10:41 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399c1b0ccf3e0bd69000f6771cb5b723e499b66e529f3600a189d31976964fa2`  
		Last Modified: Tue, 21 Nov 2023 17:00:08 GMT  
		Size: 26.5 MB (26538267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33698d354abd7b4a606d86a1409365a7c72d7464ba2d82df5cbdca9512b524cc`  
		Last Modified: Tue, 21 Nov 2023 17:00:02 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb600fde28ceedb4c4571a1679638f569b40b4f6a3c3b5e7b0d3dba7b583dd7`  
		Last Modified: Tue, 21 Nov 2023 17:00:02 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6035164ee840277fad9d17f1b64172c7eb16e967482197480c4880cd1f8ecb05`  
		Last Modified: Tue, 21 Nov 2023 17:00:02 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:509c9052f9fb4660c8e68331f86aab256e217e5cb0127d22a1473cbef5175082
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98934364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85dc721f714d97f36dc0d34cb49a7813ff36a7215f548108d27abe76220abdc9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:12:34 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Nov 2023 01:12:34 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 01:24:11 GMT
ENV RUBY_MAJOR=3.1
# Wed, 01 Nov 2023 01:24:11 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 01 Nov 2023 01:24:11 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 01 Nov 2023 01:26:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Nov 2023 01:26:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Nov 2023 01:26:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Nov 2023 01:26:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 01:26:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 01 Nov 2023 01:26:02 GMT
CMD ["irb"]
# Wed, 01 Nov 2023 13:59:02 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 01 Nov 2023 13:59:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 01 Nov 2023 13:59:02 GMT
ENV TINI_VERSION=0.18.0
# Wed, 01 Nov 2023 14:01:16 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 01 Nov 2023 14:01:17 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 01 Nov 2023 14:01:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 01 Nov 2023 14:01:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 01 Nov 2023 14:01:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 01 Nov 2023 14:01:17 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 01 Nov 2023 14:01:17 GMT
EXPOSE 24224 5140
# Wed, 01 Nov 2023 14:01:17 GMT
USER fluent
# Wed, 01 Nov 2023 14:01:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 01 Nov 2023 14:01:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e462567f43d59c23b0eeb4e4f7b82571e47c354df7e4ce7de9e98da5838427`  
		Last Modified: Wed, 01 Nov 2023 01:31:30 GMT  
		Size: 9.2 MB (9242851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe47b2ecbd3b294423b603b2d3c184238f3076d09e3c5d639120da2526cd4e`  
		Last Modified: Wed, 01 Nov 2023 01:31:28 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473cfae5a9f89c141d5bc191b180701efb9113ff46d9fbed596094d3da07e5d`  
		Last Modified: Wed, 01 Nov 2023 01:32:51 GMT  
		Size: 32.0 MB (31988455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971677043ef7aa65bbc6a16685398b198fd4101c3d61d4711a9bf14606fc4cce`  
		Last Modified: Wed, 01 Nov 2023 01:32:49 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7f02e1d532df4bca2953c04d0ddedacc324586a444f27d5b3463919f572917`  
		Last Modified: Wed, 01 Nov 2023 14:01:36 GMT  
		Size: 27.6 MB (27636077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a29c9527f300b844e5cbb27e1df2cfaf82d35d28300b090847d74e0694444d3`  
		Last Modified: Wed, 01 Nov 2023 14:01:33 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf246382aadd4413c4929ecad7107e1b7dd36c40b77aa84c5881809892fde67`  
		Last Modified: Wed, 01 Nov 2023 14:01:33 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef724aeee7820ff673da71093183f2cdc8005fdcfbfe0434921dbb57d758d447`  
		Last Modified: Wed, 01 Nov 2023 14:01:33 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:1b90d4210ba010bec00916928d3d810edf309a5b01cdc600614c0d0d7567f17f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102334274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb470b63b836375077495e3658759ed489f36527a270372e920aef72c002a32`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:18 GMT
ADD file:67f223c9c48e525a23fb110e4c105d7128dcac0c10f32c38f98ea84a21d2bd00 in / 
# Wed, 01 Nov 2023 00:39:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 07:26:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 07:26:26 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Nov 2023 07:26:26 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 07:44:32 GMT
ENV RUBY_MAJOR=3.1
# Wed, 01 Nov 2023 07:44:32 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 01 Nov 2023 07:44:32 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 01 Nov 2023 07:48:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Nov 2023 07:48:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Nov 2023 07:48:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Nov 2023 07:48:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 07:48:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 01 Nov 2023 07:48:11 GMT
CMD ["irb"]
# Wed, 01 Nov 2023 17:59:29 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 01 Nov 2023 17:59:29 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 01 Nov 2023 17:59:30 GMT
ENV TINI_VERSION=0.18.0
# Wed, 01 Nov 2023 18:02:46 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 01 Nov 2023 18:02:47 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 01 Nov 2023 18:02:47 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 01 Nov 2023 18:02:48 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 01 Nov 2023 18:02:48 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 01 Nov 2023 18:02:48 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 01 Nov 2023 18:02:48 GMT
EXPOSE 24224 5140
# Wed, 01 Nov 2023 18:02:48 GMT
USER fluent
# Wed, 01 Nov 2023 18:02:48 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 01 Nov 2023 18:02:48 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:bc6810e8fe9346a3caaff984163b789d12b6964a15a2029e384143ca19fef5ad`  
		Last Modified: Wed, 01 Nov 2023 00:44:14 GMT  
		Size: 32.4 MB (32402692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc8aa5a6299b233d98530a3f363070aa9c8f7f9a97abc58fd95ea8690eeef97`  
		Last Modified: Wed, 01 Nov 2023 07:57:12 GMT  
		Size: 12.0 MB (11996809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496d766fea70213207993851140a6e94f29fed693349286945419b5432965cb0`  
		Last Modified: Wed, 01 Nov 2023 07:57:08 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2971d177aa536a3a2de54348bb58284c087a060257020d13464ffe73bbe14c33`  
		Last Modified: Wed, 01 Nov 2023 07:58:34 GMT  
		Size: 31.2 MB (31182893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f341a335c62cc8acff733dc87930d39908c138d2a88ef42e3f52d223e457c0fc`  
		Last Modified: Wed, 01 Nov 2023 07:58:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9608f4575c81263f72734c54d07c163325dcac6611ecec8ec61aea76e37d9db3`  
		Last Modified: Wed, 01 Nov 2023 18:03:07 GMT  
		Size: 26.7 MB (26748813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef226dc2a9a6e233c739d7f837db466b8bee233b1a8a2f7ddf47b5748bed6549`  
		Last Modified: Wed, 01 Nov 2023 18:03:03 GMT  
		Size: 1.8 KB (1829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ed15b7756a556fd407ff838a3ac35d07c693bd2699a49c8d8e8f762b4a6a8c`  
		Last Modified: Wed, 01 Nov 2023 18:03:02 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f781a8149295f3c6445eb1045a0ad37fd821f99f197068241f86c6638a902bbd`  
		Last Modified: Wed, 01 Nov 2023 18:03:02 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:c02c07a536231c0b06db401ea95b928ed627f13ee8659d0ac6046378f6d62676
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106927598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9024386dba7616b8b60269f340716383167b903f5e95ec766d8f825c3c6cbb6`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:09 GMT
ADD file:a935b2993c62bfb1ade6ba0ffcf1f955422f6f76c63a723877d4bca5bb2aff7b in / 
# Wed, 01 Nov 2023 00:22:11 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 10:59:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 10:59:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Nov 2023 10:59:19 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 11:24:43 GMT
ENV RUBY_MAJOR=3.1
# Wed, 01 Nov 2023 11:24:43 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 01 Nov 2023 11:24:44 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 01 Nov 2023 11:27:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Nov 2023 11:27:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Nov 2023 11:27:48 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Nov 2023 11:27:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:27:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 01 Nov 2023 11:27:50 GMT
CMD ["irb"]
# Wed, 01 Nov 2023 15:18:20 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 01 Nov 2023 15:18:21 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 01 Nov 2023 15:18:22 GMT
ENV TINI_VERSION=0.18.0
# Wed, 01 Nov 2023 15:22:13 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 01 Nov 2023 15:22:19 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 01 Nov 2023 15:22:19 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 01 Nov 2023 15:22:19 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 01 Nov 2023 15:22:20 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 01 Nov 2023 15:22:20 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 01 Nov 2023 15:22:21 GMT
EXPOSE 24224 5140
# Wed, 01 Nov 2023 15:22:22 GMT
USER fluent
# Wed, 01 Nov 2023 15:22:22 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 01 Nov 2023 15:22:23 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c4a0eee30f72e7c0e9938500fbc7f30b5eb02d04d49bfe7f18a17af1a6d82f81`  
		Last Modified: Wed, 01 Nov 2023 00:26:59 GMT  
		Size: 35.3 MB (35293810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b58acf1d61173c3cc9dda53894435722c4fd61ccc1e81914ae7ddc825a90bd`  
		Last Modified: Wed, 01 Nov 2023 11:34:58 GMT  
		Size: 10.5 MB (10481955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae2ef73f1aa5f82d22eb60d7f771a7d42b28e24b06db27cf9257cf88def03be`  
		Last Modified: Wed, 01 Nov 2023 11:34:56 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37adaedb1254458869a324d073177243c47b8055299e381d4a6e159d107b70fd`  
		Last Modified: Wed, 01 Nov 2023 11:37:35 GMT  
		Size: 32.8 MB (32792213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b28562bceb5b1862b8f522b979515c2a33db8ab7af1c9be556ed7f231e0390`  
		Last Modified: Wed, 01 Nov 2023 11:37:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71d04b15dbb00998222272f9699870318e21986f2dca83afa20399539996e7a`  
		Last Modified: Wed, 01 Nov 2023 15:22:42 GMT  
		Size: 28.4 MB (28356539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b318b883b4fa46650001ee2add72a1d21d30613880d9496942446b0a89660f`  
		Last Modified: Wed, 01 Nov 2023 15:22:37 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e309cf77c98c046724607620b1b28421d28ae46b9213065c6cc2f7dd05c0a9`  
		Last Modified: Wed, 01 Nov 2023 15:22:38 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e59c3732ca98b4ce07e46ab8a9e905ffd600d71f34d5359f5a287153b708796`  
		Last Modified: Wed, 01 Nov 2023 15:22:37 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:75be0555a9e822037deb83584229b03ef7a06712c29bf0a5334fb3efbfe73e4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99069771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afcfed271ac2872262c4a8509a058cdce3ec6d87dbd606a0452076fad8b3c6b5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:18:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:18:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 15:18:50 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 15:39:25 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 15:39:25 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 15:39:26 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 15:41:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 15:41:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 15:41:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 15:41:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 15:41:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 15:41:50 GMT
CMD ["irb"]
# Tue, 21 Nov 2023 18:41:19 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Nov 2023 18:41:19 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 21 Nov 2023 18:41:19 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Nov 2023 18:43:25 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 21 Nov 2023 18:43:29 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Nov 2023 18:43:29 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Nov 2023 18:43:29 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Nov 2023 18:43:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Nov 2023 18:43:29 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Nov 2023 18:43:30 GMT
EXPOSE 24224 5140
# Tue, 21 Nov 2023 18:43:30 GMT
USER fluent
# Tue, 21 Nov 2023 18:43:30 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Nov 2023 18:43:30 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8dbfedb102f36df242183cfa3ddba1ff955b33e45a768d3325c37d0db970404`  
		Last Modified: Tue, 21 Nov 2023 15:47:40 GMT  
		Size: 8.9 MB (8863507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6cf84657c67ba483a43312118db12b738b36e57aef922a1590c3488435150a`  
		Last Modified: Tue, 21 Nov 2023 15:47:39 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942b813fc845050bc509cc088a3f4de68d7b318d69fd88c5e748532a28798c7c`  
		Last Modified: Tue, 21 Nov 2023 15:49:23 GMT  
		Size: 32.4 MB (32445768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3e1ac1137a5279ae95d6907deace80b73d54fc9723e4f697f8faf625d52cd`  
		Last Modified: Tue, 21 Nov 2023 15:49:19 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f1e540ef9231f30a0baa5120424f4de8533a87c27832f6c14b5deb06833818`  
		Last Modified: Tue, 21 Nov 2023 18:43:54 GMT  
		Size: 28.1 MB (28100475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d36491869991335fe9e89f4b121e39b016526e08c7e2b1d043437bdb5a7410`  
		Last Modified: Tue, 21 Nov 2023 18:43:50 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642f8438de05b18fd897d7edcb85f64cbbb63034af7ca8458f22730f3e91626`  
		Last Modified: Tue, 21 Nov 2023 18:43:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ff12f33bcdb2b48faca62ddd0be37182dabd561716bc85100bdd77080ae595`  
		Last Modified: Tue, 21 Nov 2023 18:43:50 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16.2-1.1`

```console
$ docker pull fluentd@sha256:346358e90c07ef9a6b9fad03489f867cb5dc75a00b3106ff410f6c513379fb75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.16.2-1.1` - linux; amd64

```console
$ docker pull fluentd@sha256:75bfe9553d8eaf41b853feea165a34a0ebcbe16913678f59da28bf1e67f0b914
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25156753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5753cb15f75469b9c70d6caf78efb15ac5262723e1384512538b8ed8602cc58`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:55:55 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:55:55 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:56:48 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:56:49 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:56:49 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:56:49 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:56:49 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:56:49 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:56:49 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:56:49 GMT
USER fluent
# Sat, 21 Oct 2023 00:56:49 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:56:50 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8376758d7f65ec25ea223ef7bbafc5f26e793c3bdcafc8dc00773e671afd2e79`  
		Last Modified: Sat, 21 Oct 2023 00:57:05 GMT  
		Size: 21.8 MB (21775931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc4563dcb0c96767d1176a0f296533198190b7de7ce870b687cc2b26eb9307b`  
		Last Modified: Sat, 21 Oct 2023 00:57:02 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84aaef6731a67021e310e6ee61efdd50d535063cd745b58537b5d6be1b403fd5`  
		Last Modified: Sat, 21 Oct 2023 00:57:02 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb379e120ea943cd6686bd302e2852c6de2e6ad4df759a3fa01267f493b103`  
		Last Modified: Sat, 21 Oct 2023 00:57:02 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:3f2213b3ceb36bd178b3b9c9da6605c0256bea34aa720753ce22fb98a9d175ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23848320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa175d111a15eaebd49daa0be452360294ac5c6951a5f289f9d98e2db825c9a3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:20:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:20:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:21:16 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:21:17 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:21:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:21:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:21:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:21:17 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:21:17 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:21:17 GMT
USER fluent
# Sat, 21 Oct 2023 00:21:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:21:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6272f5aba2d83ca3cb0da9b8b8ea413c4405314184d890c9f45ec6ce7bea5b2c`  
		Last Modified: Sat, 21 Oct 2023 00:21:40 GMT  
		Size: 20.7 MB (20733652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acffb79d5a5cdc39102cfbb99f6964b1acbcb76a9161b9ba2b5d51d36a630cee`  
		Last Modified: Sat, 21 Oct 2023 00:21:37 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7fbc6130e444eb89d15b84ab466005aa2df1d603163787a827420db07a5d2e`  
		Last Modified: Sat, 21 Oct 2023 00:21:37 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381df3c8eabfef21742251b70c22a41ac7ea8a9de052debdbbad3795b6ecaf35`  
		Last Modified: Sat, 21 Oct 2023 00:21:37 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:06b726c6f3eefae9ce8fa10746eee66af26fb9852c1881ad286af276cbd102d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24630185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44dfb8e93fecfed45462613ac7f31978908f5ba8ece4ae3d75f327eb79e87ec6`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:54:45 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:54:45 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:55:33 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:55:33 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:55:34 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:55:34 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:55:34 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:55:34 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:55:34 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:55:34 GMT
USER fluent
# Sat, 21 Oct 2023 00:55:34 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:55:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1ec00e7593c94a73645d5a23538f5a0ef272148c631fb2180c364c09dc4378`  
		Last Modified: Sat, 21 Oct 2023 00:55:54 GMT  
		Size: 21.4 MB (21369678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b25585882671ccef4c985197c364aa727f0e1d8b6fc53413ed04a6c0826196d`  
		Last Modified: Sat, 21 Oct 2023 00:55:52 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7b079d03420368b92ebded355718f1a1118f9d739dbfcec2ea73fbf2d91f7d`  
		Last Modified: Sat, 21 Oct 2023 00:55:52 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38769e98bf3af23f79f56d9a58e37a428bb84a00114581b22f85626b9d1e7f2`  
		Last Modified: Sat, 21 Oct 2023 00:55:52 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; 386

```console
$ docker pull fluentd@sha256:18747edca75cbd0a32946c24e0f96ff179fbc13d20ca08482c6d438ad67fb370
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24437983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0ad11bd392e421c8a344cb4ab2eac725292e368cfd3a5c9b586c85bea6a2fb`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:00:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 01:00:43 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 01:01:57 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 01:01:58 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 01:01:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 01:01:58 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 01:01:58 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 01:01:58 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 01:01:58 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 01:01:58 GMT
USER fluent
# Sat, 21 Oct 2023 01:01:58 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 01:01:58 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c98d2d26330aab1341d9ddf5b6d79700d19d8b73621e9bf914723d50eb849a4`  
		Last Modified: Sat, 21 Oct 2023 01:02:19 GMT  
		Size: 21.0 MB (21021988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f39745c5bc83005ffcd79ea3b41adf1712966c62cb9b70a1047342f7627512`  
		Last Modified: Sat, 21 Oct 2023 01:02:15 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61cf065a210c6cdcd8ed51190aa394ed32e605032d5b2d6f9d2d2c921c33bdc`  
		Last Modified: Sat, 21 Oct 2023 01:02:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865efaef1fc67ff9272e0e15d5e27e1730fc0840dae0f145d36c712c19e75dd`  
		Last Modified: Sat, 21 Oct 2023 01:02:15 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:fcb88239c453c4794e186f1701278990a9a737a91b111d7016ef412e91504c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (25011791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b032d1755278e0e612139b445d1ce18ac2150233a9611c9c22ddd4c491cbfacf`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:30:06 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:30:07 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:31:12 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:31:15 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:31:15 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:31:15 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:31:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:31:15 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:31:15 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:31:16 GMT
USER fluent
# Sat, 21 Oct 2023 00:31:16 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:31:16 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbaa2e7f2ea58633b56edda9091ecefa81b8723b7600ce62e5a39da5ffde0f5d`  
		Last Modified: Sat, 21 Oct 2023 00:31:42 GMT  
		Size: 21.6 MB (21618224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daa6ac791df9bca62f53fc841f9b484ebccf3fbbcf52d5cd060477810d7d5b3`  
		Last Modified: Sat, 21 Oct 2023 00:31:39 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4b29672e745496aefa33c93cf65970f072a929fcf9dedc79fda14be98d1342`  
		Last Modified: Sat, 21 Oct 2023 00:31:39 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27f22f12605d3ad806c396c1504a5250ece58cb31d941069ba7425e10d2aae3`  
		Last Modified: Sat, 21 Oct 2023 00:31:39 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; s390x

```console
$ docker pull fluentd@sha256:608392169a76d3014e4a408b267bcbb42299b4387a1a92931e79ea65925ac5a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24380635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b094b31e746efa26b3a4b87c04f0c9e51a35d907c1e6f7aa50b1210344df02f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:24:28 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 21 Oct 2023 00:24:28 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Sat, 21 Oct 2023 00:25:15 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Sat, 21 Oct 2023 00:25:17 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 21 Oct 2023 00:25:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 21 Oct 2023 00:25:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 21 Oct 2023 00:25:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 21 Oct 2023 00:25:17 GMT
ENV LD_PRELOAD=
# Sat, 21 Oct 2023 00:25:18 GMT
EXPOSE 24224 5140
# Sat, 21 Oct 2023 00:25:18 GMT
USER fluent
# Sat, 21 Oct 2023 00:25:18 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 00:25:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b313f13302b63aa1e26193c6c3029779f7cf6f9ccfec22267447622329ce2a32`  
		Last Modified: Sat, 21 Oct 2023 00:25:45 GMT  
		Size: 21.2 MB (21202449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d2ca75c30b0833bdbde8dc16d21aefa64e3e7325eff69992cb0ed9ae0135b7`  
		Last Modified: Sat, 21 Oct 2023 00:25:42 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f093efb15da3945df260d185c12c8ad81e19e4cc074ec941fa1b8c66ca8ff34d`  
		Last Modified: Sat, 21 Oct 2023 00:25:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5b744f7972624e9dc72a074aff76bae61e6e0ce6280fffcad2fdda27b1d757`  
		Last Modified: Sat, 21 Oct 2023 00:25:42 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16.2-debian-1.1`

```console
$ docker pull fluentd@sha256:177d5718d2a95cba7f7bfa09c2ad684216405bf7742f4522a91904ce7cca17a0
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

### `fluentd:v1.16.2-debian-1.1` - linux; amd64

```console
$ docker pull fluentd@sha256:b2e067b81f6760f4950fc0a38c87e08e8bc6c3f29a77e7254df79b3f0e4d48a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101942055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23de4c5e1fdc61aabf81a30468da9a7d35270175920d21e42d7b3317ba1a3ea5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 15:18:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 15:18:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Nov 2023 15:18:23 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 15:41:06 GMT
ENV RUBY_MAJOR=3.1
# Wed, 01 Nov 2023 15:41:06 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 01 Nov 2023 15:41:07 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 01 Nov 2023 15:43:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Nov 2023 15:43:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Nov 2023 15:43:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Nov 2023 15:43:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:43:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 01 Nov 2023 15:43:25 GMT
CMD ["irb"]
# Wed, 01 Nov 2023 22:52:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 01 Nov 2023 22:52:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 01 Nov 2023 22:52:10 GMT
ENV TINI_VERSION=0.18.0
# Wed, 01 Nov 2023 22:54:44 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 01 Nov 2023 22:54:45 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 01 Nov 2023 22:54:45 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 01 Nov 2023 22:54:45 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 01 Nov 2023 22:54:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 01 Nov 2023 22:54:45 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 01 Nov 2023 22:54:46 GMT
EXPOSE 24224 5140
# Wed, 01 Nov 2023 22:54:46 GMT
USER fluent
# Wed, 01 Nov 2023 22:54:46 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 01 Nov 2023 22:54:46 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69341098b2f234c853f6ae6ceb2be1816adb67a16d8843cb047a63325fe29a0c`  
		Last Modified: Wed, 01 Nov 2023 15:54:07 GMT  
		Size: 10.0 MB (10021771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b896e7d9a30baf37fad41181a45fece23dadec02936e16200b245819f56dd20`  
		Last Modified: Wed, 01 Nov 2023 15:54:05 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c2aef4794f0df599ddb75459cc12c5fc13e3ed9e05207bd3a4e088ca29d37`  
		Last Modified: Wed, 01 Nov 2023 15:56:40 GMT  
		Size: 32.6 MB (32626521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc381e7e0828635a3041c2c0989aebce36afa41a479118107fe9bead80d99486`  
		Last Modified: Wed, 01 Nov 2023 15:56:37 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be3011a54a05f417a65849cab7dbfd3ea8c5768ad0a6973a272639f3e84fa8a`  
		Last Modified: Wed, 01 Nov 2023 22:55:01 GMT  
		Size: 27.9 MB (27872769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a2463eea66f31090b6f7cd13a9a1cb333099ac3c6c29c80718eea9984c4518`  
		Last Modified: Wed, 01 Nov 2023 22:54:57 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237fedb38023431e2d5274feea0a695a597294f7313b23dedbb17bd081bead0f`  
		Last Modified: Wed, 01 Nov 2023 22:54:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f554862fb4e4a2d79885366bafcbb0fd67ff25bec2867236f62f0520468f4b`  
		Last Modified: Wed, 01 Nov 2023 22:54:57 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:627fa4cb1db78d37fa1938282af8f1930b14a5dd8666f2f27788db127aba7acf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.4 MB (95427791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d807e00bdf0e036aec63d78fd7e9cff46e3a6df2feff484fceded2b2473b104`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:09 GMT
ADD file:f7d1d017cc4e588f213f4536967b8d58c50b8602fb8a10b786856c35a843f31e in / 
# Tue, 21 Nov 2023 05:01:09 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:27:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:27:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 05:27:24 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:38:36 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 05:38:36 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 05:38:36 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 05:40:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 05:40:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 05:40:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 05:40:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 05:40:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 05:40:47 GMT
CMD ["irb"]
# Tue, 21 Nov 2023 16:11:35 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Nov 2023 16:11:35 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 21 Nov 2023 16:11:35 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Nov 2023 16:14:26 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 21 Nov 2023 16:14:26 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Nov 2023 16:14:26 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Nov 2023 16:14:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Nov 2023 16:14:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Nov 2023 16:14:27 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Nov 2023 16:14:27 GMT
EXPOSE 24224 5140
# Tue, 21 Nov 2023 16:14:27 GMT
USER fluent
# Tue, 21 Nov 2023 16:14:27 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Nov 2023 16:14:27 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:d051266714ac5508b442ebbe5911d353bfacddc64f657eeba14a993cced96358`  
		Last Modified: Tue, 21 Nov 2023 05:04:38 GMT  
		Size: 28.9 MB (28921267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec3e2f4ed70f7a6ff62ff15d04822a0dfe972559db93385e2dc8dba05ecb06c`  
		Last Modified: Tue, 21 Nov 2023 05:44:29 GMT  
		Size: 8.6 MB (8634953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbde3702c4b0c15a573b9e7b9c2f87492bad117b7b3c21abd06f5b0f913bdc0`  
		Last Modified: Tue, 21 Nov 2023 05:44:28 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffda89f4ed0e1b94a1fa5862d204c222ae50142552208dc1faa75ff8764c267f`  
		Last Modified: Tue, 21 Nov 2023 05:45:42 GMT  
		Size: 31.2 MB (31166744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14897c4d9cf59fdf6b4be859a107cf3ad20eb2b701011ec5560cb2b54cf399fd`  
		Last Modified: Tue, 21 Nov 2023 05:45:39 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac5b6ce352208b3705bc898ba0d5a987899be48c66554950eb17fcd36767fec`  
		Last Modified: Tue, 21 Nov 2023 16:14:54 GMT  
		Size: 26.7 MB (26701759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2233d7a633e377d238fbc529c3f547c7a4cab4249de5bffe387cb3844f37ca3`  
		Last Modified: Tue, 21 Nov 2023 16:14:49 GMT  
		Size: 1.8 KB (1829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d815726563d183099212915a008e0b36c273b99398f4a249ea5d6a06e5545f5`  
		Last Modified: Tue, 21 Nov 2023 16:14:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2f8b2ca4fa7cd659c07b18329a0e7a383d309932ba977539e80207d610041e`  
		Last Modified: Tue, 21 Nov 2023 16:14:49 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:7f7b83cf352f792f20296950870c3d6736807fb4f83e6f3c63ef9c3c7d0396cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92300695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3590143f467428e2aa2fcf4b183dc86ba10265ced87c079e7ee0377a1862c26`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:04 GMT
ADD file:c4afced274aaa80ab3018b368ed739c1c55e49b41e9637ac44d63e61344fe865 in / 
# Tue, 21 Nov 2023 03:58:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:50:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:50:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 07:50:49 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 08:01:23 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 08:01:23 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 08:01:23 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 08:03:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 08:03:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 08:03:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 08:03:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 08:03:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 08:03:26 GMT
CMD ["irb"]
# Tue, 21 Nov 2023 16:56:48 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Nov 2023 16:56:48 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 21 Nov 2023 16:56:49 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Nov 2023 16:59:38 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 21 Nov 2023 16:59:39 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Nov 2023 16:59:39 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Nov 2023 16:59:39 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Nov 2023 16:59:39 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Nov 2023 16:59:39 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Nov 2023 16:59:39 GMT
EXPOSE 24224 5140
# Tue, 21 Nov 2023 16:59:39 GMT
USER fluent
# Tue, 21 Nov 2023 16:59:39 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Nov 2023 16:59:39 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6dc4ed5513793308b8e30b08e03f97fa54025c3d3f3172c6edccb1dbbc7ff139`  
		Last Modified: Tue, 21 Nov 2023 04:02:35 GMT  
		Size: 26.6 MB (26579014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7011811be080b3ec10eb390c78eb1b81bde867946f61686c1898bb89ef4ee30b`  
		Last Modified: Tue, 21 Nov 2023 08:09:21 GMT  
		Size: 8.1 MB (8143369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17046219f223403a42245317d506cf41d8598ff0e6b724a2f8fd5741a21c82a2`  
		Last Modified: Tue, 21 Nov 2023 08:09:19 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5591c39c82e62aeff5d31f2933194de53fe4c581cea0f7a2c7207a2c4a840e71`  
		Last Modified: Tue, 21 Nov 2023 08:10:45 GMT  
		Size: 31.0 MB (31036973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7879eec1d2c94304558aadea4ff39a09268082325bd71f59c3d23d372fdb2cc4`  
		Last Modified: Tue, 21 Nov 2023 08:10:41 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399c1b0ccf3e0bd69000f6771cb5b723e499b66e529f3600a189d31976964fa2`  
		Last Modified: Tue, 21 Nov 2023 17:00:08 GMT  
		Size: 26.5 MB (26538267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33698d354abd7b4a606d86a1409365a7c72d7464ba2d82df5cbdca9512b524cc`  
		Last Modified: Tue, 21 Nov 2023 17:00:02 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb600fde28ceedb4c4571a1679638f569b40b4f6a3c3b5e7b0d3dba7b583dd7`  
		Last Modified: Tue, 21 Nov 2023 17:00:02 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6035164ee840277fad9d17f1b64172c7eb16e967482197480c4880cd1f8ecb05`  
		Last Modified: Tue, 21 Nov 2023 17:00:02 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:509c9052f9fb4660c8e68331f86aab256e217e5cb0127d22a1473cbef5175082
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98934364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85dc721f714d97f36dc0d34cb49a7813ff36a7215f548108d27abe76220abdc9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:12:34 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Nov 2023 01:12:34 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 01:24:11 GMT
ENV RUBY_MAJOR=3.1
# Wed, 01 Nov 2023 01:24:11 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 01 Nov 2023 01:24:11 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 01 Nov 2023 01:26:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Nov 2023 01:26:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Nov 2023 01:26:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Nov 2023 01:26:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 01:26:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 01 Nov 2023 01:26:02 GMT
CMD ["irb"]
# Wed, 01 Nov 2023 13:59:02 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 01 Nov 2023 13:59:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 01 Nov 2023 13:59:02 GMT
ENV TINI_VERSION=0.18.0
# Wed, 01 Nov 2023 14:01:16 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 01 Nov 2023 14:01:17 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 01 Nov 2023 14:01:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 01 Nov 2023 14:01:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 01 Nov 2023 14:01:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 01 Nov 2023 14:01:17 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 01 Nov 2023 14:01:17 GMT
EXPOSE 24224 5140
# Wed, 01 Nov 2023 14:01:17 GMT
USER fluent
# Wed, 01 Nov 2023 14:01:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 01 Nov 2023 14:01:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e462567f43d59c23b0eeb4e4f7b82571e47c354df7e4ce7de9e98da5838427`  
		Last Modified: Wed, 01 Nov 2023 01:31:30 GMT  
		Size: 9.2 MB (9242851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe47b2ecbd3b294423b603b2d3c184238f3076d09e3c5d639120da2526cd4e`  
		Last Modified: Wed, 01 Nov 2023 01:31:28 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473cfae5a9f89c141d5bc191b180701efb9113ff46d9fbed596094d3da07e5d`  
		Last Modified: Wed, 01 Nov 2023 01:32:51 GMT  
		Size: 32.0 MB (31988455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971677043ef7aa65bbc6a16685398b198fd4101c3d61d4711a9bf14606fc4cce`  
		Last Modified: Wed, 01 Nov 2023 01:32:49 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7f02e1d532df4bca2953c04d0ddedacc324586a444f27d5b3463919f572917`  
		Last Modified: Wed, 01 Nov 2023 14:01:36 GMT  
		Size: 27.6 MB (27636077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a29c9527f300b844e5cbb27e1df2cfaf82d35d28300b090847d74e0694444d3`  
		Last Modified: Wed, 01 Nov 2023 14:01:33 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf246382aadd4413c4929ecad7107e1b7dd36c40b77aa84c5881809892fde67`  
		Last Modified: Wed, 01 Nov 2023 14:01:33 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef724aeee7820ff673da71093183f2cdc8005fdcfbfe0434921dbb57d758d447`  
		Last Modified: Wed, 01 Nov 2023 14:01:33 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; 386

```console
$ docker pull fluentd@sha256:1b90d4210ba010bec00916928d3d810edf309a5b01cdc600614c0d0d7567f17f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102334274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb470b63b836375077495e3658759ed489f36527a270372e920aef72c002a32`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:18 GMT
ADD file:67f223c9c48e525a23fb110e4c105d7128dcac0c10f32c38f98ea84a21d2bd00 in / 
# Wed, 01 Nov 2023 00:39:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 07:26:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 07:26:26 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Nov 2023 07:26:26 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 07:44:32 GMT
ENV RUBY_MAJOR=3.1
# Wed, 01 Nov 2023 07:44:32 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 01 Nov 2023 07:44:32 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 01 Nov 2023 07:48:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Nov 2023 07:48:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Nov 2023 07:48:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Nov 2023 07:48:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 07:48:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 01 Nov 2023 07:48:11 GMT
CMD ["irb"]
# Wed, 01 Nov 2023 17:59:29 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 01 Nov 2023 17:59:29 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 01 Nov 2023 17:59:30 GMT
ENV TINI_VERSION=0.18.0
# Wed, 01 Nov 2023 18:02:46 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 01 Nov 2023 18:02:47 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 01 Nov 2023 18:02:47 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 01 Nov 2023 18:02:48 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 01 Nov 2023 18:02:48 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 01 Nov 2023 18:02:48 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 01 Nov 2023 18:02:48 GMT
EXPOSE 24224 5140
# Wed, 01 Nov 2023 18:02:48 GMT
USER fluent
# Wed, 01 Nov 2023 18:02:48 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 01 Nov 2023 18:02:48 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:bc6810e8fe9346a3caaff984163b789d12b6964a15a2029e384143ca19fef5ad`  
		Last Modified: Wed, 01 Nov 2023 00:44:14 GMT  
		Size: 32.4 MB (32402692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc8aa5a6299b233d98530a3f363070aa9c8f7f9a97abc58fd95ea8690eeef97`  
		Last Modified: Wed, 01 Nov 2023 07:57:12 GMT  
		Size: 12.0 MB (11996809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496d766fea70213207993851140a6e94f29fed693349286945419b5432965cb0`  
		Last Modified: Wed, 01 Nov 2023 07:57:08 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2971d177aa536a3a2de54348bb58284c087a060257020d13464ffe73bbe14c33`  
		Last Modified: Wed, 01 Nov 2023 07:58:34 GMT  
		Size: 31.2 MB (31182893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f341a335c62cc8acff733dc87930d39908c138d2a88ef42e3f52d223e457c0fc`  
		Last Modified: Wed, 01 Nov 2023 07:58:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9608f4575c81263f72734c54d07c163325dcac6611ecec8ec61aea76e37d9db3`  
		Last Modified: Wed, 01 Nov 2023 18:03:07 GMT  
		Size: 26.7 MB (26748813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef226dc2a9a6e233c739d7f837db466b8bee233b1a8a2f7ddf47b5748bed6549`  
		Last Modified: Wed, 01 Nov 2023 18:03:03 GMT  
		Size: 1.8 KB (1829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ed15b7756a556fd407ff838a3ac35d07c693bd2699a49c8d8e8f762b4a6a8c`  
		Last Modified: Wed, 01 Nov 2023 18:03:02 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f781a8149295f3c6445eb1045a0ad37fd821f99f197068241f86c6638a902bbd`  
		Last Modified: Wed, 01 Nov 2023 18:03:02 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:c02c07a536231c0b06db401ea95b928ed627f13ee8659d0ac6046378f6d62676
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106927598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9024386dba7616b8b60269f340716383167b903f5e95ec766d8f825c3c6cbb6`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:09 GMT
ADD file:a935b2993c62bfb1ade6ba0ffcf1f955422f6f76c63a723877d4bca5bb2aff7b in / 
# Wed, 01 Nov 2023 00:22:11 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 10:59:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 10:59:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Nov 2023 10:59:19 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 11:24:43 GMT
ENV RUBY_MAJOR=3.1
# Wed, 01 Nov 2023 11:24:43 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 01 Nov 2023 11:24:44 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 01 Nov 2023 11:27:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Nov 2023 11:27:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Nov 2023 11:27:48 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Nov 2023 11:27:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:27:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 01 Nov 2023 11:27:50 GMT
CMD ["irb"]
# Wed, 01 Nov 2023 15:18:20 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 01 Nov 2023 15:18:21 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 01 Nov 2023 15:18:22 GMT
ENV TINI_VERSION=0.18.0
# Wed, 01 Nov 2023 15:22:13 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 01 Nov 2023 15:22:19 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 01 Nov 2023 15:22:19 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 01 Nov 2023 15:22:19 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 01 Nov 2023 15:22:20 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 01 Nov 2023 15:22:20 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 01 Nov 2023 15:22:21 GMT
EXPOSE 24224 5140
# Wed, 01 Nov 2023 15:22:22 GMT
USER fluent
# Wed, 01 Nov 2023 15:22:22 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 01 Nov 2023 15:22:23 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c4a0eee30f72e7c0e9938500fbc7f30b5eb02d04d49bfe7f18a17af1a6d82f81`  
		Last Modified: Wed, 01 Nov 2023 00:26:59 GMT  
		Size: 35.3 MB (35293810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b58acf1d61173c3cc9dda53894435722c4fd61ccc1e81914ae7ddc825a90bd`  
		Last Modified: Wed, 01 Nov 2023 11:34:58 GMT  
		Size: 10.5 MB (10481955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae2ef73f1aa5f82d22eb60d7f771a7d42b28e24b06db27cf9257cf88def03be`  
		Last Modified: Wed, 01 Nov 2023 11:34:56 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37adaedb1254458869a324d073177243c47b8055299e381d4a6e159d107b70fd`  
		Last Modified: Wed, 01 Nov 2023 11:37:35 GMT  
		Size: 32.8 MB (32792213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b28562bceb5b1862b8f522b979515c2a33db8ab7af1c9be556ed7f231e0390`  
		Last Modified: Wed, 01 Nov 2023 11:37:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71d04b15dbb00998222272f9699870318e21986f2dca83afa20399539996e7a`  
		Last Modified: Wed, 01 Nov 2023 15:22:42 GMT  
		Size: 28.4 MB (28356539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b318b883b4fa46650001ee2add72a1d21d30613880d9496942446b0a89660f`  
		Last Modified: Wed, 01 Nov 2023 15:22:37 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e309cf77c98c046724607620b1b28421d28ae46b9213065c6cc2f7dd05c0a9`  
		Last Modified: Wed, 01 Nov 2023 15:22:38 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e59c3732ca98b4ce07e46ab8a9e905ffd600d71f34d5359f5a287153b708796`  
		Last Modified: Wed, 01 Nov 2023 15:22:37 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; s390x

```console
$ docker pull fluentd@sha256:75be0555a9e822037deb83584229b03ef7a06712c29bf0a5334fb3efbfe73e4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99069771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afcfed271ac2872262c4a8509a058cdce3ec6d87dbd606a0452076fad8b3c6b5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:18:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:18:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 15:18:50 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 15:39:25 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 15:39:25 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 15:39:26 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 15:41:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 15:41:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 15:41:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 15:41:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 15:41:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 15:41:50 GMT
CMD ["irb"]
# Tue, 21 Nov 2023 18:41:19 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Nov 2023 18:41:19 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 21 Nov 2023 18:41:19 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Nov 2023 18:43:25 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 21 Nov 2023 18:43:29 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Nov 2023 18:43:29 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Nov 2023 18:43:29 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Nov 2023 18:43:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Nov 2023 18:43:29 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Nov 2023 18:43:30 GMT
EXPOSE 24224 5140
# Tue, 21 Nov 2023 18:43:30 GMT
USER fluent
# Tue, 21 Nov 2023 18:43:30 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Nov 2023 18:43:30 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8dbfedb102f36df242183cfa3ddba1ff955b33e45a768d3325c37d0db970404`  
		Last Modified: Tue, 21 Nov 2023 15:47:40 GMT  
		Size: 8.9 MB (8863507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6cf84657c67ba483a43312118db12b738b36e57aef922a1590c3488435150a`  
		Last Modified: Tue, 21 Nov 2023 15:47:39 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942b813fc845050bc509cc088a3f4de68d7b318d69fd88c5e748532a28798c7c`  
		Last Modified: Tue, 21 Nov 2023 15:49:23 GMT  
		Size: 32.4 MB (32445768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3e1ac1137a5279ae95d6907deace80b73d54fc9723e4f697f8faf625d52cd`  
		Last Modified: Tue, 21 Nov 2023 15:49:19 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f1e540ef9231f30a0baa5120424f4de8533a87c27832f6c14b5deb06833818`  
		Last Modified: Tue, 21 Nov 2023 18:43:54 GMT  
		Size: 28.1 MB (28100475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d36491869991335fe9e89f4b121e39b016526e08c7e2b1d043437bdb5a7410`  
		Last Modified: Tue, 21 Nov 2023 18:43:50 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642f8438de05b18fd897d7edcb85f64cbbb63034af7ca8458f22730f3e91626`  
		Last Modified: Tue, 21 Nov 2023 18:43:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ff12f33bcdb2b48faca62ddd0be37182dabd561716bc85100bdd77080ae595`  
		Last Modified: Tue, 21 Nov 2023 18:43:50 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
