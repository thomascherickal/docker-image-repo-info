<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.16-1`](#fluentdv116-1)
-	[`fluentd:v1.16-debian-1`](#fluentdv116-debian-1)
-	[`fluentd:v1.16.2-1.1`](#fluentdv1162-11)
-	[`fluentd:v1.16.2-debian-1.1`](#fluentdv1162-debian-11)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:5e9ce2a4e1a44810532a79820fef177b1bf79f0f92e007cdb34ca9b008bd1c13
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
$ docker pull fluentd@sha256:a4e91af5c2c5b4fe94670babe10bd382044adaf166138e53f73851530010d8b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25121008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5996c1f199123fe8af5a3e0b28bedae745ec7fc70e8aed237f6e1132d4340161`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:58 GMT
ADD file:80331a5d882ac8a70763f4b19e06f2e04ea3dca34ae6d92810815b170b3c806c in / 
# Thu, 30 Nov 2023 23:22:59 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:44:46 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 03:44:46 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 03:45:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 03:45:40 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 03:45:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 03:45:40 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 03:45:41 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 03:45:41 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 03:45:41 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 03:45:41 GMT
USER fluent
# Fri, 01 Dec 2023 03:45:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 03:45:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1207c741d8c9b028d98c4006013f9de959da3c55f85b91ed5e4583438a0112ca`  
		Last Modified: Thu, 30 Nov 2023 23:23:40 GMT  
		Size: 3.4 MB (3379323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76a3a1fd0ad4aa159c3974eff3353b9ad001c91f4cac3ac65e05834caed10b7`  
		Last Modified: Fri, 01 Dec 2023 03:45:55 GMT  
		Size: 21.7 MB (21739472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8e0bba4418fc5273315d4eabd20aea23bb83da441bd3c1f7a5b04f585b960d`  
		Last Modified: Fri, 01 Dec 2023 03:45:52 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168ad43ac562c4427586f655da8ed8376f859908f88eade6ed6c996fff973b51`  
		Last Modified: Fri, 01 Dec 2023 03:45:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cb712fbbcfa599bd991a8e5da01ff98aa4861e6943c91634867a18bdd54cef`  
		Last Modified: Fri, 01 Dec 2023 03:45:52 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:afedc2a33faeede6659a9921c0eae9beace4bb0a33bce0ac3b607ed23d46bee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23850373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d66b3410458227ab22fb76f46cbeb6e9bdbd07b6098d1dd61ef1f82784d8711c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:21 GMT
ADD file:90d3bdc6a557ead63796de0110e2fda87e65aa091070cbae612dfb2126568253 in / 
# Thu, 30 Nov 2023 22:49:21 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:52:01 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 00:52:01 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 00:53:06 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 00:53:08 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 00:53:08 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 00:53:09 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 00:53:09 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 00:53:09 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 00:53:09 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 00:53:10 GMT
USER fluent
# Fri, 01 Dec 2023 00:53:10 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 00:53:10 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f0440ff44d712e5fc701b84856116589b428157893ac461b633b1ab30b627eed`  
		Last Modified: Thu, 30 Nov 2023 22:49:52 GMT  
		Size: 3.1 MB (3113003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a065954eac3dc28635864bddc60436f4fb0c0b750d5b35de23b537576578b709`  
		Last Modified: Fri, 01 Dec 2023 00:53:33 GMT  
		Size: 20.7 MB (20735155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d1449c20b5b2fbf9dd9829f7492493ed5a2921c2477f633a87a9c66981fb91`  
		Last Modified: Fri, 01 Dec 2023 00:53:30 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57af02e674f92ad4845d7bdbd01f1f1f90cb50d8bef7a44ba2f409db0a2b89e1`  
		Last Modified: Fri, 01 Dec 2023 00:53:30 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e61f3299bc61397e27afa65898b9a506230f29195bb7ec589dac633e08aa65`  
		Last Modified: Fri, 01 Dec 2023 00:53:30 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:53e77cb29372098ba2fd977d53ba50ac8154c54a84cea4bc322e61482d9d4e8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24637924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ab6c7ed8e4623e24eddd58a7c7337bea60f62320b6dcd705f11315f1d24af1f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:07 GMT
ADD file:e5c66967d6570e36da50c9d42dd8f8f55e6c6a65b92c79601ea9e750c076fa2a in / 
# Thu, 30 Nov 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:22:38 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 01:22:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 01:23:27 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 01:23:28 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 01:23:28 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 01:23:28 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 01:23:28 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 01:23:28 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 01:23:28 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 01:23:28 GMT
USER fluent
# Fri, 01 Dec 2023 01:23:28 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 01:23:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b8180c93b172865af87a7c0e7e3c8bcb139e0d0c92e19c96467ff2cd4c8919ad`  
		Last Modified: Thu, 30 Nov 2023 23:11:45 GMT  
		Size: 3.3 MB (3258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d7c4792d95aa77caba915d7f24ceabae22f187850580e1ad0e01cea84136e8`  
		Last Modified: Fri, 01 Dec 2023 01:23:45 GMT  
		Size: 21.4 MB (21377358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f4e08a9b87816708c17ba6e01829a1fd06f74caad1dd46a4b15b86f3ccff64`  
		Last Modified: Fri, 01 Dec 2023 01:23:43 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01a50f1cc4c77c65525aa5b0740c20ea3e74bb94141821eb9e04fdd39aba936`  
		Last Modified: Fri, 01 Dec 2023 01:23:43 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e0c4b71bbb752c89c8b90a1cc304b96e20c798a4666246135b84a3e3ff9fb9`  
		Last Modified: Fri, 01 Dec 2023 01:23:43 GMT  
		Size: 461.0 B  
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
$ docker pull fluentd@sha256:5e9ce2a4e1a44810532a79820fef177b1bf79f0f92e007cdb34ca9b008bd1c13
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
$ docker pull fluentd@sha256:a4e91af5c2c5b4fe94670babe10bd382044adaf166138e53f73851530010d8b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25121008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5996c1f199123fe8af5a3e0b28bedae745ec7fc70e8aed237f6e1132d4340161`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:58 GMT
ADD file:80331a5d882ac8a70763f4b19e06f2e04ea3dca34ae6d92810815b170b3c806c in / 
# Thu, 30 Nov 2023 23:22:59 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:44:46 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 03:44:46 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 03:45:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 03:45:40 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 03:45:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 03:45:40 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 03:45:41 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 03:45:41 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 03:45:41 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 03:45:41 GMT
USER fluent
# Fri, 01 Dec 2023 03:45:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 03:45:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1207c741d8c9b028d98c4006013f9de959da3c55f85b91ed5e4583438a0112ca`  
		Last Modified: Thu, 30 Nov 2023 23:23:40 GMT  
		Size: 3.4 MB (3379323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76a3a1fd0ad4aa159c3974eff3353b9ad001c91f4cac3ac65e05834caed10b7`  
		Last Modified: Fri, 01 Dec 2023 03:45:55 GMT  
		Size: 21.7 MB (21739472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8e0bba4418fc5273315d4eabd20aea23bb83da441bd3c1f7a5b04f585b960d`  
		Last Modified: Fri, 01 Dec 2023 03:45:52 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168ad43ac562c4427586f655da8ed8376f859908f88eade6ed6c996fff973b51`  
		Last Modified: Fri, 01 Dec 2023 03:45:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cb712fbbcfa599bd991a8e5da01ff98aa4861e6943c91634867a18bdd54cef`  
		Last Modified: Fri, 01 Dec 2023 03:45:52 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:afedc2a33faeede6659a9921c0eae9beace4bb0a33bce0ac3b607ed23d46bee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23850373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d66b3410458227ab22fb76f46cbeb6e9bdbd07b6098d1dd61ef1f82784d8711c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:21 GMT
ADD file:90d3bdc6a557ead63796de0110e2fda87e65aa091070cbae612dfb2126568253 in / 
# Thu, 30 Nov 2023 22:49:21 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:52:01 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 00:52:01 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 00:53:06 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 00:53:08 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 00:53:08 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 00:53:09 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 00:53:09 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 00:53:09 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 00:53:09 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 00:53:10 GMT
USER fluent
# Fri, 01 Dec 2023 00:53:10 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 00:53:10 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f0440ff44d712e5fc701b84856116589b428157893ac461b633b1ab30b627eed`  
		Last Modified: Thu, 30 Nov 2023 22:49:52 GMT  
		Size: 3.1 MB (3113003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a065954eac3dc28635864bddc60436f4fb0c0b750d5b35de23b537576578b709`  
		Last Modified: Fri, 01 Dec 2023 00:53:33 GMT  
		Size: 20.7 MB (20735155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d1449c20b5b2fbf9dd9829f7492493ed5a2921c2477f633a87a9c66981fb91`  
		Last Modified: Fri, 01 Dec 2023 00:53:30 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57af02e674f92ad4845d7bdbd01f1f1f90cb50d8bef7a44ba2f409db0a2b89e1`  
		Last Modified: Fri, 01 Dec 2023 00:53:30 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e61f3299bc61397e27afa65898b9a506230f29195bb7ec589dac633e08aa65`  
		Last Modified: Fri, 01 Dec 2023 00:53:30 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:53e77cb29372098ba2fd977d53ba50ac8154c54a84cea4bc322e61482d9d4e8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24637924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ab6c7ed8e4623e24eddd58a7c7337bea60f62320b6dcd705f11315f1d24af1f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:07 GMT
ADD file:e5c66967d6570e36da50c9d42dd8f8f55e6c6a65b92c79601ea9e750c076fa2a in / 
# Thu, 30 Nov 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:22:38 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 01:22:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 01:23:27 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 01:23:28 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 01:23:28 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 01:23:28 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 01:23:28 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 01:23:28 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 01:23:28 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 01:23:28 GMT
USER fluent
# Fri, 01 Dec 2023 01:23:28 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 01:23:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b8180c93b172865af87a7c0e7e3c8bcb139e0d0c92e19c96467ff2cd4c8919ad`  
		Last Modified: Thu, 30 Nov 2023 23:11:45 GMT  
		Size: 3.3 MB (3258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d7c4792d95aa77caba915d7f24ceabae22f187850580e1ad0e01cea84136e8`  
		Last Modified: Fri, 01 Dec 2023 01:23:45 GMT  
		Size: 21.4 MB (21377358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f4e08a9b87816708c17ba6e01829a1fd06f74caad1dd46a4b15b86f3ccff64`  
		Last Modified: Fri, 01 Dec 2023 01:23:43 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01a50f1cc4c77c65525aa5b0740c20ea3e74bb94141821eb9e04fdd39aba936`  
		Last Modified: Fri, 01 Dec 2023 01:23:43 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e0c4b71bbb752c89c8b90a1cc304b96e20c798a4666246135b84a3e3ff9fb9`  
		Last Modified: Fri, 01 Dec 2023 01:23:43 GMT  
		Size: 461.0 B  
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
$ docker pull fluentd@sha256:b748f8a2134c84eba897795f2bccd1ab6d7b65b81aeb54a81e6aef7ba6f0c950
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
$ docker pull fluentd@sha256:67bf8cc4b785dced9955f78d6848d15cabff931dfca0351e362d3ac318dc428f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101938036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fad573ce99f27af8700927f79f8cf78044ee6c24effe1f2203306ed32fd65f53`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:26:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:26:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 09:26:50 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 09:38:20 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 09:38:20 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 09:38:20 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 09:40:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 09:40:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 09:40:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 09:40:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 09:40:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 09:40:37 GMT
CMD ["irb"]
# Tue, 21 Nov 2023 23:03:59 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Nov 2023 23:03:59 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 21 Nov 2023 23:04:00 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Nov 2023 23:06:36 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 21 Nov 2023 23:06:37 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Nov 2023 23:06:37 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Nov 2023 23:06:38 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Nov 2023 23:06:38 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Nov 2023 23:06:38 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Nov 2023 23:06:38 GMT
EXPOSE 24224 5140
# Tue, 21 Nov 2023 23:06:38 GMT
USER fluent
# Tue, 21 Nov 2023 23:06:38 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Nov 2023 23:06:38 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df56554bf9e5659f8d908064bd30aff825e045ee6c057d819b7699c28317ac9`  
		Last Modified: Tue, 21 Nov 2023 09:46:54 GMT  
		Size: 10.0 MB (10021801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff4c9edcdbd8a887810187da1ae0f0b29272d5a0423f6238fc54255c9e13fbe`  
		Last Modified: Tue, 21 Nov 2023 09:46:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c439040ba0cffdcb8af716cdfdce486c1013627b5d1a7850f5249a707358f4d`  
		Last Modified: Tue, 21 Nov 2023 09:48:13 GMT  
		Size: 32.6 MB (32626579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0ce47eddc12b16dbb0fd82ea2b462f8b6d226613ac73a8985ba073edf400d4`  
		Last Modified: Tue, 21 Nov 2023 09:48:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533643548a2cdca273507667f03c81cc463f1ee414b16350d145d5b34133c48d`  
		Last Modified: Tue, 21 Nov 2023 23:07:05 GMT  
		Size: 27.9 MB (27868753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc31d98cfa86707c7f373eff6c4e4938fb76bf0ea10670a6a7c58294063d84d`  
		Last Modified: Tue, 21 Nov 2023 23:07:02 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9278c9def9acb128e6239ce9920385dcacb125f758a09aff398786f865abafa`  
		Last Modified: Tue, 21 Nov 2023 23:07:02 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1389a127dc0ab105cb8551ac31eac6c878d35ba4311b4f296a8880207d6d1aa`  
		Last Modified: Tue, 21 Nov 2023 23:07:01 GMT  
		Size: 460.0 B  
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
$ docker pull fluentd@sha256:5496143b5b37e8d671765b31793a75006dbead022d6d108f989eff07d038c1c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98940119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47a82c0a9cee83d2e2fba1f5092f55f0bdfb09b93a7719ce4bd03ef738b973cd`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 19:58:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:58:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 19:58:22 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 20:14:23 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 20:14:23 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 20:14:23 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 20:16:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 20:16:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 20:16:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 20:16:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 20:16:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 20:16:09 GMT
CMD ["irb"]
# Wed, 22 Nov 2023 04:23:08 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 22 Nov 2023 04:23:08 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 22 Nov 2023 04:23:08 GMT
ENV TINI_VERSION=0.18.0
# Wed, 22 Nov 2023 04:25:26 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 22 Nov 2023 04:25:26 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 22 Nov 2023 04:25:27 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 22 Nov 2023 04:25:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 22 Nov 2023 04:25:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 22 Nov 2023 04:25:27 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 22 Nov 2023 04:25:27 GMT
EXPOSE 24224 5140
# Wed, 22 Nov 2023 04:25:27 GMT
USER fluent
# Wed, 22 Nov 2023 04:25:27 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 22 Nov 2023 04:25:27 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11511c223570c8b46a54437f5bb0f6c6f6c60a6633b8e314772f4bc2ac01d7a3`  
		Last Modified: Tue, 21 Nov 2023 20:24:47 GMT  
		Size: 9.2 MB (9242744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d692bb309eaae8566edb5b82d95bef2224538f23bda45c38772447d4809c1e`  
		Last Modified: Tue, 21 Nov 2023 20:24:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe18d369a89dab2febd3206f0205759833c62329e9c276986c8845f2796d2eb`  
		Last Modified: Tue, 21 Nov 2023 20:27:03 GMT  
		Size: 32.0 MB (31988156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2adfe3957d86ac109098c858b9bb8177d671537f90e7bbc6dc96bd2b8d70149`  
		Last Modified: Tue, 21 Nov 2023 20:27:01 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0408a1d946e27333557c75eec6e1f133145d5186e66e77c84dbd9f07bd1e2e99`  
		Last Modified: Wed, 22 Nov 2023 04:25:42 GMT  
		Size: 27.6 MB (27642014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad85a748c5c88b3febfba2a10d9341ec52bcc2e5cb2f58d77bee55bb1b11567`  
		Last Modified: Wed, 22 Nov 2023 04:25:39 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b866f0d092a1b9011fc9de9ef336d3c914071aa5c56880ab8f43f9f1c6dd8d4`  
		Last Modified: Wed, 22 Nov 2023 04:25:39 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72ca211ad088658e181aa401eb2ced61eb9f6439bd014efd4d85fcf66fbb9a8`  
		Last Modified: Wed, 22 Nov 2023 04:25:39 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:88de91f7f82613ad3ec7060b7c4a7fbb8bea453af09b81c1c007580c84df24d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102336037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:720024ec49dba5af8b9ed4ab38be82acd8b9e34e7576607d1c169af9cdaa0dab`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:38:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:38:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 14:38:58 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 14:56:17 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 14:56:17 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 14:56:17 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 15:00:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 15:00:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 15:00:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 15:00:04 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 15:00:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 15:00:04 GMT
CMD ["irb"]
# Wed, 22 Nov 2023 07:43:02 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 22 Nov 2023 07:43:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 22 Nov 2023 07:43:02 GMT
ENV TINI_VERSION=0.18.0
# Wed, 22 Nov 2023 07:46:28 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 22 Nov 2023 07:46:29 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 22 Nov 2023 07:46:29 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 22 Nov 2023 07:46:30 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 22 Nov 2023 07:46:30 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 22 Nov 2023 07:46:30 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 22 Nov 2023 07:46:30 GMT
EXPOSE 24224 5140
# Wed, 22 Nov 2023 07:46:30 GMT
USER fluent
# Wed, 22 Nov 2023 07:46:30 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 22 Nov 2023 07:46:30 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baac56b6ee8db7e90f384b20f403b4d1154ddbb4f7621e61394c66fa9f724604`  
		Last Modified: Tue, 21 Nov 2023 15:08:56 GMT  
		Size: 12.0 MB (11996876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321dcd90c939f73d74bcd3568edc306cc5f1aafc4767a51dd9ed6c58bdbefd6c`  
		Last Modified: Tue, 21 Nov 2023 15:08:52 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3d8bcd5fb57d13af31034860434c8220faff20ad0e7e7627fb12f3bc64851`  
		Last Modified: Tue, 21 Nov 2023 15:10:24 GMT  
		Size: 31.2 MB (31183192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37013d54985397ce5bbea1b863c575ee6718b87fbc7203dcaf571088526a8b8e`  
		Last Modified: Tue, 21 Nov 2023 15:10:20 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdc8af4d7408fa11ccdbfd005e6b4ddb8ead02b761251c26f50df7bdb5efb69`  
		Last Modified: Wed, 22 Nov 2023 07:46:53 GMT  
		Size: 26.8 MB (26750266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc0d4b8edf055cf6083349a9e9a5c1afc09064f6975f9446f1ccdc3aea5f0cc`  
		Last Modified: Wed, 22 Nov 2023 07:46:47 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af31bb5279ca8db38a85ecb0d20a6393e19b23ddd61a38fd2da2a877985dc27`  
		Last Modified: Wed, 22 Nov 2023 07:46:48 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a1dc2c11e914cb5fa5fca835e7139c8fd6225d9bf16c4e3796a142eddaeec2`  
		Last Modified: Wed, 22 Nov 2023 07:46:47 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:df87cfa0ca4b408ad01f9265f52b1956d232bf29e4e3aab6da3543d48197b818
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106930165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee270993262e9f43fc94cba91d2949247ddd588a3eb5283287e88ce1f9c3587b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:47:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:47:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 15:47:58 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 16:24:21 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 16:24:22 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 16:24:22 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 16:27:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 16:27:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 16:27:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 16:27:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 16:27:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 16:27:48 GMT
CMD ["irb"]
# Tue, 21 Nov 2023 23:35:19 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Nov 2023 23:35:19 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 21 Nov 2023 23:35:19 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Nov 2023 23:38:50 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 21 Nov 2023 23:38:52 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Nov 2023 23:38:52 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Nov 2023 23:38:53 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Nov 2023 23:38:53 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Nov 2023 23:38:53 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Nov 2023 23:38:53 GMT
EXPOSE 24224 5140
# Tue, 21 Nov 2023 23:38:54 GMT
USER fluent
# Tue, 21 Nov 2023 23:38:54 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Nov 2023 23:38:54 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728598e87ec79ca9c6c0b3d955f2b0bb7057312e22eff817e9731893e73121ca`  
		Last Modified: Tue, 21 Nov 2023 16:34:58 GMT  
		Size: 10.5 MB (10482039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d1d7a1e8706d8c68bba746b578794c2317e2c506e7494a6a6d7d921f15ba7f`  
		Last Modified: Tue, 21 Nov 2023 16:34:55 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f779a5504ad7dc6d4a1c808c877ad708a84634e419497568d2508773c0e8d1`  
		Last Modified: Tue, 21 Nov 2023 16:37:33 GMT  
		Size: 32.8 MB (32792373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040d40ccfdf1ddf70f6767c550a17469c02264c9ee2f08b0dc255f3779dc69c5`  
		Last Modified: Tue, 21 Nov 2023 16:37:30 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7fef0865dd9369bee4dbe79b917cff5db4ad1e4ca45ef3d96a173a93b98879`  
		Last Modified: Tue, 21 Nov 2023 23:39:10 GMT  
		Size: 28.4 MB (28358946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5c4dd06bb77da94859b747690a5f3c8acdd8ad4b99a35c822959692cc818ec`  
		Last Modified: Tue, 21 Nov 2023 23:39:05 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25790119b66061649bb49e62cda0a50a7bffa7e66d77f63177e7a388be6397e2`  
		Last Modified: Tue, 21 Nov 2023 23:39:05 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad299140239eaf0a33bc78fb7d7eab53b405b0fbdbe0e95d81d2e4f859c1cab`  
		Last Modified: Tue, 21 Nov 2023 23:39:05 GMT  
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
$ docker pull fluentd@sha256:5e9ce2a4e1a44810532a79820fef177b1bf79f0f92e007cdb34ca9b008bd1c13
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
$ docker pull fluentd@sha256:a4e91af5c2c5b4fe94670babe10bd382044adaf166138e53f73851530010d8b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25121008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5996c1f199123fe8af5a3e0b28bedae745ec7fc70e8aed237f6e1132d4340161`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:58 GMT
ADD file:80331a5d882ac8a70763f4b19e06f2e04ea3dca34ae6d92810815b170b3c806c in / 
# Thu, 30 Nov 2023 23:22:59 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:44:46 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 03:44:46 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 03:45:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 03:45:40 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 03:45:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 03:45:40 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 03:45:41 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 03:45:41 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 03:45:41 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 03:45:41 GMT
USER fluent
# Fri, 01 Dec 2023 03:45:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 03:45:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1207c741d8c9b028d98c4006013f9de959da3c55f85b91ed5e4583438a0112ca`  
		Last Modified: Thu, 30 Nov 2023 23:23:40 GMT  
		Size: 3.4 MB (3379323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76a3a1fd0ad4aa159c3974eff3353b9ad001c91f4cac3ac65e05834caed10b7`  
		Last Modified: Fri, 01 Dec 2023 03:45:55 GMT  
		Size: 21.7 MB (21739472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8e0bba4418fc5273315d4eabd20aea23bb83da441bd3c1f7a5b04f585b960d`  
		Last Modified: Fri, 01 Dec 2023 03:45:52 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168ad43ac562c4427586f655da8ed8376f859908f88eade6ed6c996fff973b51`  
		Last Modified: Fri, 01 Dec 2023 03:45:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cb712fbbcfa599bd991a8e5da01ff98aa4861e6943c91634867a18bdd54cef`  
		Last Modified: Fri, 01 Dec 2023 03:45:52 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:afedc2a33faeede6659a9921c0eae9beace4bb0a33bce0ac3b607ed23d46bee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23850373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d66b3410458227ab22fb76f46cbeb6e9bdbd07b6098d1dd61ef1f82784d8711c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:21 GMT
ADD file:90d3bdc6a557ead63796de0110e2fda87e65aa091070cbae612dfb2126568253 in / 
# Thu, 30 Nov 2023 22:49:21 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:52:01 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 00:52:01 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 00:53:06 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 00:53:08 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 00:53:08 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 00:53:09 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 00:53:09 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 00:53:09 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 00:53:09 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 00:53:10 GMT
USER fluent
# Fri, 01 Dec 2023 00:53:10 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 00:53:10 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f0440ff44d712e5fc701b84856116589b428157893ac461b633b1ab30b627eed`  
		Last Modified: Thu, 30 Nov 2023 22:49:52 GMT  
		Size: 3.1 MB (3113003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a065954eac3dc28635864bddc60436f4fb0c0b750d5b35de23b537576578b709`  
		Last Modified: Fri, 01 Dec 2023 00:53:33 GMT  
		Size: 20.7 MB (20735155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d1449c20b5b2fbf9dd9829f7492493ed5a2921c2477f633a87a9c66981fb91`  
		Last Modified: Fri, 01 Dec 2023 00:53:30 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57af02e674f92ad4845d7bdbd01f1f1f90cb50d8bef7a44ba2f409db0a2b89e1`  
		Last Modified: Fri, 01 Dec 2023 00:53:30 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e61f3299bc61397e27afa65898b9a506230f29195bb7ec589dac633e08aa65`  
		Last Modified: Fri, 01 Dec 2023 00:53:30 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:53e77cb29372098ba2fd977d53ba50ac8154c54a84cea4bc322e61482d9d4e8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24637924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ab6c7ed8e4623e24eddd58a7c7337bea60f62320b6dcd705f11315f1d24af1f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:07 GMT
ADD file:e5c66967d6570e36da50c9d42dd8f8f55e6c6a65b92c79601ea9e750c076fa2a in / 
# Thu, 30 Nov 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:22:38 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 01:22:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 01:23:27 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 01:23:28 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 01:23:28 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 01:23:28 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 01:23:28 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 01:23:28 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 01:23:28 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 01:23:28 GMT
USER fluent
# Fri, 01 Dec 2023 01:23:28 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 01:23:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b8180c93b172865af87a7c0e7e3c8bcb139e0d0c92e19c96467ff2cd4c8919ad`  
		Last Modified: Thu, 30 Nov 2023 23:11:45 GMT  
		Size: 3.3 MB (3258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d7c4792d95aa77caba915d7f24ceabae22f187850580e1ad0e01cea84136e8`  
		Last Modified: Fri, 01 Dec 2023 01:23:45 GMT  
		Size: 21.4 MB (21377358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f4e08a9b87816708c17ba6e01829a1fd06f74caad1dd46a4b15b86f3ccff64`  
		Last Modified: Fri, 01 Dec 2023 01:23:43 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01a50f1cc4c77c65525aa5b0740c20ea3e74bb94141821eb9e04fdd39aba936`  
		Last Modified: Fri, 01 Dec 2023 01:23:43 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e0c4b71bbb752c89c8b90a1cc304b96e20c798a4666246135b84a3e3ff9fb9`  
		Last Modified: Fri, 01 Dec 2023 01:23:43 GMT  
		Size: 461.0 B  
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
$ docker pull fluentd@sha256:b748f8a2134c84eba897795f2bccd1ab6d7b65b81aeb54a81e6aef7ba6f0c950
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
$ docker pull fluentd@sha256:67bf8cc4b785dced9955f78d6848d15cabff931dfca0351e362d3ac318dc428f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101938036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fad573ce99f27af8700927f79f8cf78044ee6c24effe1f2203306ed32fd65f53`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:26:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:26:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 09:26:50 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 09:38:20 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 09:38:20 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 09:38:20 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 09:40:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 09:40:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 09:40:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 09:40:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 09:40:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 09:40:37 GMT
CMD ["irb"]
# Tue, 21 Nov 2023 23:03:59 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Nov 2023 23:03:59 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 21 Nov 2023 23:04:00 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Nov 2023 23:06:36 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 21 Nov 2023 23:06:37 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Nov 2023 23:06:37 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Nov 2023 23:06:38 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Nov 2023 23:06:38 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Nov 2023 23:06:38 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Nov 2023 23:06:38 GMT
EXPOSE 24224 5140
# Tue, 21 Nov 2023 23:06:38 GMT
USER fluent
# Tue, 21 Nov 2023 23:06:38 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Nov 2023 23:06:38 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df56554bf9e5659f8d908064bd30aff825e045ee6c057d819b7699c28317ac9`  
		Last Modified: Tue, 21 Nov 2023 09:46:54 GMT  
		Size: 10.0 MB (10021801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff4c9edcdbd8a887810187da1ae0f0b29272d5a0423f6238fc54255c9e13fbe`  
		Last Modified: Tue, 21 Nov 2023 09:46:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c439040ba0cffdcb8af716cdfdce486c1013627b5d1a7850f5249a707358f4d`  
		Last Modified: Tue, 21 Nov 2023 09:48:13 GMT  
		Size: 32.6 MB (32626579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0ce47eddc12b16dbb0fd82ea2b462f8b6d226613ac73a8985ba073edf400d4`  
		Last Modified: Tue, 21 Nov 2023 09:48:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533643548a2cdca273507667f03c81cc463f1ee414b16350d145d5b34133c48d`  
		Last Modified: Tue, 21 Nov 2023 23:07:05 GMT  
		Size: 27.9 MB (27868753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc31d98cfa86707c7f373eff6c4e4938fb76bf0ea10670a6a7c58294063d84d`  
		Last Modified: Tue, 21 Nov 2023 23:07:02 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9278c9def9acb128e6239ce9920385dcacb125f758a09aff398786f865abafa`  
		Last Modified: Tue, 21 Nov 2023 23:07:02 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1389a127dc0ab105cb8551ac31eac6c878d35ba4311b4f296a8880207d6d1aa`  
		Last Modified: Tue, 21 Nov 2023 23:07:01 GMT  
		Size: 460.0 B  
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
$ docker pull fluentd@sha256:5496143b5b37e8d671765b31793a75006dbead022d6d108f989eff07d038c1c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98940119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47a82c0a9cee83d2e2fba1f5092f55f0bdfb09b93a7719ce4bd03ef738b973cd`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 19:58:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:58:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 19:58:22 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 20:14:23 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 20:14:23 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 20:14:23 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 20:16:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 20:16:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 20:16:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 20:16:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 20:16:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 20:16:09 GMT
CMD ["irb"]
# Wed, 22 Nov 2023 04:23:08 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 22 Nov 2023 04:23:08 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 22 Nov 2023 04:23:08 GMT
ENV TINI_VERSION=0.18.0
# Wed, 22 Nov 2023 04:25:26 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 22 Nov 2023 04:25:26 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 22 Nov 2023 04:25:27 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 22 Nov 2023 04:25:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 22 Nov 2023 04:25:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 22 Nov 2023 04:25:27 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 22 Nov 2023 04:25:27 GMT
EXPOSE 24224 5140
# Wed, 22 Nov 2023 04:25:27 GMT
USER fluent
# Wed, 22 Nov 2023 04:25:27 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 22 Nov 2023 04:25:27 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11511c223570c8b46a54437f5bb0f6c6f6c60a6633b8e314772f4bc2ac01d7a3`  
		Last Modified: Tue, 21 Nov 2023 20:24:47 GMT  
		Size: 9.2 MB (9242744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d692bb309eaae8566edb5b82d95bef2224538f23bda45c38772447d4809c1e`  
		Last Modified: Tue, 21 Nov 2023 20:24:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe18d369a89dab2febd3206f0205759833c62329e9c276986c8845f2796d2eb`  
		Last Modified: Tue, 21 Nov 2023 20:27:03 GMT  
		Size: 32.0 MB (31988156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2adfe3957d86ac109098c858b9bb8177d671537f90e7bbc6dc96bd2b8d70149`  
		Last Modified: Tue, 21 Nov 2023 20:27:01 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0408a1d946e27333557c75eec6e1f133145d5186e66e77c84dbd9f07bd1e2e99`  
		Last Modified: Wed, 22 Nov 2023 04:25:42 GMT  
		Size: 27.6 MB (27642014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad85a748c5c88b3febfba2a10d9341ec52bcc2e5cb2f58d77bee55bb1b11567`  
		Last Modified: Wed, 22 Nov 2023 04:25:39 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b866f0d092a1b9011fc9de9ef336d3c914071aa5c56880ab8f43f9f1c6dd8d4`  
		Last Modified: Wed, 22 Nov 2023 04:25:39 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72ca211ad088658e181aa401eb2ced61eb9f6439bd014efd4d85fcf66fbb9a8`  
		Last Modified: Wed, 22 Nov 2023 04:25:39 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; 386

```console
$ docker pull fluentd@sha256:88de91f7f82613ad3ec7060b7c4a7fbb8bea453af09b81c1c007580c84df24d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102336037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:720024ec49dba5af8b9ed4ab38be82acd8b9e34e7576607d1c169af9cdaa0dab`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:38:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:38:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 14:38:58 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 14:56:17 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 14:56:17 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 14:56:17 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 15:00:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 15:00:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 15:00:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 15:00:04 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 15:00:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 15:00:04 GMT
CMD ["irb"]
# Wed, 22 Nov 2023 07:43:02 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 22 Nov 2023 07:43:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 22 Nov 2023 07:43:02 GMT
ENV TINI_VERSION=0.18.0
# Wed, 22 Nov 2023 07:46:28 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 22 Nov 2023 07:46:29 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 22 Nov 2023 07:46:29 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 22 Nov 2023 07:46:30 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 22 Nov 2023 07:46:30 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 22 Nov 2023 07:46:30 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 22 Nov 2023 07:46:30 GMT
EXPOSE 24224 5140
# Wed, 22 Nov 2023 07:46:30 GMT
USER fluent
# Wed, 22 Nov 2023 07:46:30 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 22 Nov 2023 07:46:30 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baac56b6ee8db7e90f384b20f403b4d1154ddbb4f7621e61394c66fa9f724604`  
		Last Modified: Tue, 21 Nov 2023 15:08:56 GMT  
		Size: 12.0 MB (11996876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321dcd90c939f73d74bcd3568edc306cc5f1aafc4767a51dd9ed6c58bdbefd6c`  
		Last Modified: Tue, 21 Nov 2023 15:08:52 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3d8bcd5fb57d13af31034860434c8220faff20ad0e7e7627fb12f3bc64851`  
		Last Modified: Tue, 21 Nov 2023 15:10:24 GMT  
		Size: 31.2 MB (31183192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37013d54985397ce5bbea1b863c575ee6718b87fbc7203dcaf571088526a8b8e`  
		Last Modified: Tue, 21 Nov 2023 15:10:20 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdc8af4d7408fa11ccdbfd005e6b4ddb8ead02b761251c26f50df7bdb5efb69`  
		Last Modified: Wed, 22 Nov 2023 07:46:53 GMT  
		Size: 26.8 MB (26750266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc0d4b8edf055cf6083349a9e9a5c1afc09064f6975f9446f1ccdc3aea5f0cc`  
		Last Modified: Wed, 22 Nov 2023 07:46:47 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af31bb5279ca8db38a85ecb0d20a6393e19b23ddd61a38fd2da2a877985dc27`  
		Last Modified: Wed, 22 Nov 2023 07:46:48 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a1dc2c11e914cb5fa5fca835e7139c8fd6225d9bf16c4e3796a142eddaeec2`  
		Last Modified: Wed, 22 Nov 2023 07:46:47 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:df87cfa0ca4b408ad01f9265f52b1956d232bf29e4e3aab6da3543d48197b818
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106930165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee270993262e9f43fc94cba91d2949247ddd588a3eb5283287e88ce1f9c3587b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:47:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:47:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 15:47:58 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 16:24:21 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 16:24:22 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 16:24:22 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 16:27:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 16:27:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 16:27:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 16:27:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 16:27:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 16:27:48 GMT
CMD ["irb"]
# Tue, 21 Nov 2023 23:35:19 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Nov 2023 23:35:19 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 21 Nov 2023 23:35:19 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Nov 2023 23:38:50 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 21 Nov 2023 23:38:52 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Nov 2023 23:38:52 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Nov 2023 23:38:53 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Nov 2023 23:38:53 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Nov 2023 23:38:53 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Nov 2023 23:38:53 GMT
EXPOSE 24224 5140
# Tue, 21 Nov 2023 23:38:54 GMT
USER fluent
# Tue, 21 Nov 2023 23:38:54 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Nov 2023 23:38:54 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728598e87ec79ca9c6c0b3d955f2b0bb7057312e22eff817e9731893e73121ca`  
		Last Modified: Tue, 21 Nov 2023 16:34:58 GMT  
		Size: 10.5 MB (10482039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d1d7a1e8706d8c68bba746b578794c2317e2c506e7494a6a6d7d921f15ba7f`  
		Last Modified: Tue, 21 Nov 2023 16:34:55 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f779a5504ad7dc6d4a1c808c877ad708a84634e419497568d2508773c0e8d1`  
		Last Modified: Tue, 21 Nov 2023 16:37:33 GMT  
		Size: 32.8 MB (32792373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040d40ccfdf1ddf70f6767c550a17469c02264c9ee2f08b0dc255f3779dc69c5`  
		Last Modified: Tue, 21 Nov 2023 16:37:30 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7fef0865dd9369bee4dbe79b917cff5db4ad1e4ca45ef3d96a173a93b98879`  
		Last Modified: Tue, 21 Nov 2023 23:39:10 GMT  
		Size: 28.4 MB (28358946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5c4dd06bb77da94859b747690a5f3c8acdd8ad4b99a35c822959692cc818ec`  
		Last Modified: Tue, 21 Nov 2023 23:39:05 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25790119b66061649bb49e62cda0a50a7bffa7e66d77f63177e7a388be6397e2`  
		Last Modified: Tue, 21 Nov 2023 23:39:05 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad299140239eaf0a33bc78fb7d7eab53b405b0fbdbe0e95d81d2e4f859c1cab`  
		Last Modified: Tue, 21 Nov 2023 23:39:05 GMT  
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
