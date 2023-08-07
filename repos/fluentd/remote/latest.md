## `fluentd:latest`

```console
$ docker pull fluentd@sha256:71f8cf2118a9a77fba7cc6263644497f7c54366698a3096283123ec84ef7eca8
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
$ docker pull fluentd@sha256:d07aaa6eba6a96328e2b3a0a0ccb586e556e629f1937141c7f1bd8689798cd30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25138920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d619c23c9ae269bd4d905563b3b29e8cf52f3b43a98e608ae7f3bc9f3813a07d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:33:29 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 14 Jun 2023 22:33:29 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 14 Jun 2023 22:34:23 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 14 Jun 2023 22:34:23 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 14 Jun 2023 22:34:23 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 14 Jun 2023 22:34:23 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 14 Jun 2023 22:34:23 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 14 Jun 2023 22:34:24 GMT
ENV LD_PRELOAD=
# Wed, 14 Jun 2023 22:34:24 GMT
EXPOSE 24224 5140
# Wed, 14 Jun 2023 22:34:24 GMT
USER fluent
# Wed, 14 Jun 2023 22:34:24 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 14 Jun 2023 22:34:24 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e89884591749689529cd5fa296197dbf2d081b89aa1acf0d521f4c2c6f96bf`  
		Last Modified: Wed, 14 Jun 2023 22:34:37 GMT  
		Size: 21.8 MB (21761995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390a858b50010d973d4e1a5f6da84ba514b82536de40dc734fc35889c5579cca`  
		Last Modified: Wed, 14 Jun 2023 22:34:34 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d69a60bc67d80beffeb819bcf5409aa6ac1cece761ac175179bcbd081de713`  
		Last Modified: Wed, 14 Jun 2023 22:34:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b15490d254354e083d9cecd8372dd8a7d24f42f48553b5be44087f846d3cb`  
		Last Modified: Wed, 14 Jun 2023 22:34:34 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:4c7a522f2f52fded55c7e7eb1cbfbf95071cb89602efd1c16d10173e1052bc19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23818795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9449002b91a5e83fa600b072a1849a3bde33395ab9912736df9ebcf0af9ca07a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:39:12 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 14 Jun 2023 20:39:12 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 14 Jun 2023 20:40:14 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 14 Jun 2023 20:40:14 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 14 Jun 2023 20:40:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 14 Jun 2023 20:40:15 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 14 Jun 2023 20:40:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 14 Jun 2023 20:40:15 GMT
ENV LD_PRELOAD=
# Wed, 14 Jun 2023 20:40:15 GMT
EXPOSE 24224 5140
# Wed, 14 Jun 2023 20:40:15 GMT
USER fluent
# Wed, 14 Jun 2023 20:40:15 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 14 Jun 2023 20:40:15 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff90db882f9f0c92f1e98e1b0070fce952033d478a6d6f2139bc6b8deccf4c1`  
		Last Modified: Wed, 14 Jun 2023 20:40:32 GMT  
		Size: 20.7 MB (20705668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409eb899470f9c46b8b52fef13f7747862956ea44d1131402ecdf43a4e62cd4e`  
		Last Modified: Wed, 14 Jun 2023 20:40:28 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8c355cf22653f5ecf08a38e9747568282212437249dbde1843db76413ac703`  
		Last Modified: Wed, 14 Jun 2023 20:40:28 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d173e8e240a98c6b2fead4204509ef9ee0ef181fa18818047b1a21744741ef6`  
		Last Modified: Wed, 14 Jun 2023 20:40:28 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:5504f34bf0fdd8c584dde9ece653aef92fab0ec0488b02d09c0c60773873fec0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24615958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625b9c7556aca650f5c149011e1045a1f41a52c022bf6c00d120a443212a2135`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 23:16:29 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 14 Jun 2023 23:16:29 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Wed, 14 Jun 2023 23:17:17 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 14 Jun 2023 23:17:18 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 14 Jun 2023 23:17:18 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 14 Jun 2023 23:17:18 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 14 Jun 2023 23:17:18 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 14 Jun 2023 23:17:18 GMT
ENV LD_PRELOAD=
# Wed, 14 Jun 2023 23:17:18 GMT
EXPOSE 24224 5140
# Wed, 14 Jun 2023 23:17:18 GMT
USER fluent
# Wed, 14 Jun 2023 23:17:18 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 14 Jun 2023 23:17:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c596c0811598d44ad0388635c2457814da7ec0aeeaa500f5a227ea1ef522859`  
		Last Modified: Wed, 14 Jun 2023 23:17:36 GMT  
		Size: 21.4 MB (21352606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdb87eceb2348af0bce9ef18e4af5f4138cce349e7ddfa9e358e589f1a61928`  
		Last Modified: Wed, 14 Jun 2023 23:17:34 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8277de9dddc2b555e88ca9500be77262f4bfd85ec1150f4f0bbd390d5d0a86`  
		Last Modified: Wed, 14 Jun 2023 23:17:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2236a61df5e8c4f1cb997555c37c1bec0623a75612f1541cbac90f9f00ffe7b6`  
		Last Modified: Wed, 14 Jun 2023 23:17:34 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; 386

```console
$ docker pull fluentd@sha256:39a75b2171984f895bad267615d2a0f22bc36b24f823d8208170a4d29e194ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24419766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3105df073c5919362ae4ae41dfc99a239bd1a686e61f981c1173e70cd9dfbfb`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:24:48 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Mon, 07 Aug 2023 21:24:48 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Mon, 07 Aug 2023 21:25:51 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Mon, 07 Aug 2023 21:25:52 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Mon, 07 Aug 2023 21:25:52 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Mon, 07 Aug 2023 21:25:52 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Mon, 07 Aug 2023 21:25:52 GMT
ENV FLUENTD_CONF=fluent.conf
# Mon, 07 Aug 2023 21:25:52 GMT
ENV LD_PRELOAD=
# Mon, 07 Aug 2023 21:25:53 GMT
EXPOSE 24224 5140
# Mon, 07 Aug 2023 21:25:53 GMT
USER fluent
# Mon, 07 Aug 2023 21:25:53 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Mon, 07 Aug 2023 21:25:53 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e180d68a6784e287fbd112203e9d4ec2f2d74e0e2d8bc178c61bf9fb8e91ddc`  
		Last Modified: Mon, 07 Aug 2023 21:26:11 GMT  
		Size: 21.0 MB (21003778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5f11c2e94ea5541f00dda08086a095742ca1a0d80afc235860d18863cdac5c`  
		Last Modified: Mon, 07 Aug 2023 21:26:07 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06bbf332266ca282817341b04518c3cc87cafaa20c087bc76b44e51e06c199a4`  
		Last Modified: Mon, 07 Aug 2023 21:26:07 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c068f06a2e3f7536a8bbd8290592b69f4348d82c50e10d45e37dc85620017a`  
		Last Modified: Mon, 07 Aug 2023 21:26:06 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:e657b8a0462629b862aef1ddd616c3705eb84a12f2572477884fc650da5cdbf1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (24994027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f16729145cd752aa811ffdbb5311976ad8ef6402dca14343d17dd93e1d7d7d15`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:06:25 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Mon, 07 Aug 2023 21:06:26 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Mon, 07 Aug 2023 21:08:31 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Mon, 07 Aug 2023 21:08:36 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Mon, 07 Aug 2023 21:08:38 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Mon, 07 Aug 2023 21:08:38 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Mon, 07 Aug 2023 21:08:39 GMT
ENV FLUENTD_CONF=fluent.conf
# Mon, 07 Aug 2023 21:08:39 GMT
ENV LD_PRELOAD=
# Mon, 07 Aug 2023 21:08:40 GMT
EXPOSE 24224 5140
# Mon, 07 Aug 2023 21:08:41 GMT
USER fluent
# Mon, 07 Aug 2023 21:08:42 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Mon, 07 Aug 2023 21:08:43 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ddfce8ff2f2b7be76fc6d618deefa2282d9d9f7633d981d29d351c5e0bdaea`  
		Last Modified: Mon, 07 Aug 2023 21:09:09 GMT  
		Size: 21.6 MB (21600461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cbd13befcd8b8bce1f86cc5544d64cba12edd18a285fb3e19051f8d64fc9b5`  
		Last Modified: Mon, 07 Aug 2023 21:09:03 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6812f97e8a8535d190c506510893fd75a499f7dad7473591664a510174854e4d`  
		Last Modified: Mon, 07 Aug 2023 21:09:03 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5366a4f8d0fc4127db1580d845e4a97721553d8b57c161afebe42bcd1fb5fba`  
		Last Modified: Mon, 07 Aug 2023 21:09:03 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:89ffe3f0d5665ed8fffb7793fecde61036f8d1bdde33976bd4b8e09a19b36909
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24353859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc17258134d6b5a069ab70676271ad0cb35ef9a0c6a891ddf2abe2a25ea7dd18`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:17:28 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Mon, 07 Aug 2023 20:17:28 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.0
# Mon, 07 Aug 2023 20:18:21 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.14.2  && gem install json -v 2.6.3  && gem install rexml -v 3.2.5  && gem install async -v 1.30.3  && gem install async-http -v 0.56.6  && gem install fluentd -v 1.16.0  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Mon, 07 Aug 2023 20:18:23 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Mon, 07 Aug 2023 20:18:23 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Mon, 07 Aug 2023 20:18:23 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Mon, 07 Aug 2023 20:18:23 GMT
ENV FLUENTD_CONF=fluent.conf
# Mon, 07 Aug 2023 20:18:23 GMT
ENV LD_PRELOAD=
# Mon, 07 Aug 2023 20:18:24 GMT
EXPOSE 24224 5140
# Mon, 07 Aug 2023 20:18:24 GMT
USER fluent
# Mon, 07 Aug 2023 20:18:24 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Mon, 07 Aug 2023 20:18:24 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79062a3efcf019be904e5ae4b1fbbe799fefdc6fe332da1cc2200c682770a8b9`  
		Last Modified: Mon, 07 Aug 2023 20:18:53 GMT  
		Size: 21.2 MB (21175672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad859df790fc4746c6b7c74231af5a72c52bce2c893e4aa5586dcb7e7d1b9e1d`  
		Last Modified: Mon, 07 Aug 2023 20:18:50 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ff47ba17005f172794ae4f5c7c150a4662a67c98076be03c155c1637c76e3d`  
		Last Modified: Mon, 07 Aug 2023 20:18:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c86c53fee1184d9bed9db6a1ca8bea390f1c5851e6763574eeb83a0e609221`  
		Last Modified: Mon, 07 Aug 2023 20:18:51 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
