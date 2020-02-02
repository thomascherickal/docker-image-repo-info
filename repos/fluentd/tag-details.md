<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.8-1`](#fluentdv18-1)
-	[`fluentd:v1.8.1-1.0`](#fluentdv181-10)
-	[`fluentd:v1.8.1-debian-1.0`](#fluentdv181-debian-10)
-	[`fluentd:v1.8-debian-1`](#fluentdv18-debian-1)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:ad8d88f1600fca4fd624a149bd5f49a941193a36af6fa509f1baf714eb5238d6
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
$ docker pull fluentd@sha256:75ce5020648cf6b41f8149ae2fa2f589c381dcdb61987e8bb1264f425c32ce95
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16477381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41a6ad1233ce7c9046c13db2fd1f97364149ad549a512ab72dedd2bef5e63b6b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:21:40 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:21:40 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:22:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:22:40 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:22:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:22:41 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:22:41 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:22:41 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:22:42 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:22:42 GMT
USER fluent
# Thu, 23 Jan 2020 17:22:42 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:22:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c614808f1174d32d67b7ecac4800e05ef3e411ae8bdedbb6240136c10a2f27`  
		Last Modified: Thu, 23 Jan 2020 17:23:19 GMT  
		Size: 13.7 MB (13711041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8bdd560291478d1c7f7cdb57fa5e1c5bb60ac5288f5cbd06068a192a400d9f`  
		Last Modified: Thu, 23 Jan 2020 17:23:06 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db832aa9e885329454cf3b2cc8a6c1154f5c31cd0b2565f9a4efdfff5b19f40`  
		Last Modified: Thu, 23 Jan 2020 17:23:05 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ae6fb92ee376b443db0999d49d19f43be88f5ecad0f24d9f9e0d37236f6bb5`  
		Last Modified: Thu, 23 Jan 2020 17:23:05 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:035a4e0ca4ec279d5b7efdc2ae1530b85b99f41cfac44cacbe86e8cf449bb15c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15926470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1d866d3935af22c17334b093ea3ed54f50c6eb4e6346381cd5771c3a783c877`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:09:48 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:11:27 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:11:37 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:11:38 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:11:39 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:11:40 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:11:41 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:11:42 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:11:42 GMT
USER fluent
# Thu, 23 Jan 2020 17:11:44 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:11:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61745ca2853b92fe876640e1120b69f2d6b0c5b53023a31e2efebea54c40ae2`  
		Last Modified: Thu, 23 Jan 2020 17:12:15 GMT  
		Size: 13.4 MB (13376576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637eb510f29cae52739de271c15f8d31d790c4fe77536740b05b62170c26bd05`  
		Last Modified: Thu, 23 Jan 2020 17:12:07 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cf50affa812e536c41281a121805e4b4478df66e432e132a54c89f174eb2df`  
		Last Modified: Thu, 23 Jan 2020 17:12:06 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1fbd8f4b19cf7d8acebe443fe90cb27438c633a4068d982842434f387a9db6`  
		Last Modified: Thu, 23 Jan 2020 17:12:06 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:610e4cd77b8f533d63b50e882ec044dd8ec729436f4ac7bbc6f8520f542c855f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16403315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36fb10a77e8f3c7d101a2f503ce225ff5b1b2f53d172c1f069d8c41f7fc4bb19`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:33:30 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:33:30 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:34:37 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:34:41 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:34:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:34:42 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:34:43 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:34:43 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:34:44 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:34:44 GMT
USER fluent
# Thu, 23 Jan 2020 17:34:45 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:34:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6b5c46a574799e0b946dbc6cc66cabfc6207b5ddcd573b123802551ea94f0f`  
		Last Modified: Thu, 23 Jan 2020 17:35:14 GMT  
		Size: 13.7 MB (13707861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d094f07cfa4b841c62b9dfae9c888180da1e4ef0c5f81ca834fc5f2a700768`  
		Last Modified: Thu, 23 Jan 2020 17:35:09 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aa646bd931e5a5d4279cc93b90231836817be0bae159b3043dce5c2e26b1ea`  
		Last Modified: Thu, 23 Jan 2020 17:35:08 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb631140a5800779637c95a8dcb92f4daeabb23dec32c970e7cf465c53c4eb`  
		Last Modified: Thu, 23 Jan 2020 17:35:08 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; 386

```console
$ docker pull fluentd@sha256:815f5dfb686d66717312114a34134b2d3776f3a909b45fd022353a40b94089b8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16381360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512d48c879211f5661da8e2f939e23e8d23cc3c9b4bbab459e5b7503d4d6d64d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:55:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:55:00 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:56:08 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:56:10 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:56:10 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:56:11 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:56:11 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:56:11 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:56:11 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:56:12 GMT
USER fluent
# Thu, 23 Jan 2020 17:56:12 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:56:12 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b8f6237861e49130cb68a766ee538a9dd868bb0613e052f95b04a3d8caf608`  
		Last Modified: Thu, 23 Jan 2020 17:56:43 GMT  
		Size: 13.6 MB (13610672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79633fb3e15c107605467c3bc079032fcb43992fccc3cc2fc389bcc216eafd`  
		Last Modified: Thu, 23 Jan 2020 17:56:38 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e4c942e6b974a2b7cf5f42624d47d6d555a98b2a21fbe228e7bee4e6fc3ae5`  
		Last Modified: Thu, 23 Jan 2020 17:56:38 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d7eb29f7a6c6f3b0ec43bb0e541253e271fb77b8517ffc1df29ba4101898d7`  
		Last Modified: Thu, 23 Jan 2020 17:56:38 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:33a5ca24b27bfe9ca6f4ff579d1fbe08fe7039f94e9c8378de0dd571d07b5a64
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16911283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a57d87b4e6f55a2bd3a52207151facd32cfe5a54d4640c28d84f3f5527b9d6cf`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:58:09 GMT
ADD file:b06f16ae13d177baa99c50f4b42de9479a24ae5b68aa967b17dbe98760ed809e in / 
# Thu, 23 Jan 2020 16:58:10 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:14:31 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:14:35 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:15:43 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:15:53 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:15:54 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:15:56 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:15:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:16:02 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:16:06 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:16:09 GMT
USER fluent
# Thu, 23 Jan 2020 17:16:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2ef848e1434ec427ca147408f3c6f1cec160019050a04c8a2040f35872ab661b`  
		Last Modified: Thu, 23 Jan 2020 16:58:55 GMT  
		Size: 2.8 MB (2786373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d8bdf10b187c1ca45fe47a4ef50135c9d99b67f6b4d85a39393c5dcb845e6`  
		Last Modified: Thu, 23 Jan 2020 17:16:51 GMT  
		Size: 14.1 MB (14122691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138bd852fdb69bf8e38738e5e504a7191ae928168788f8c83532952225e0b264`  
		Last Modified: Thu, 23 Jan 2020 17:16:40 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748b67f558bcb92af2081528139dcb2fa37ca0a7d8fb7e1a61c9cf3f3f7ce0d3`  
		Last Modified: Thu, 23 Jan 2020 17:16:40 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25aaa684ac282e02e36ce16dc19d2c7272c32da084e2b0e246b96306897a96b3`  
		Last Modified: Thu, 23 Jan 2020 17:16:40 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:6a46692938f6ee9b718f592bc32084afdbbae1d41014bb9dcdb56f58722bfdde
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16391842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ca0024734079e1ae4f6e753780eea50407b87086244deee3b491bc58efc4c1`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:49 GMT
ADD file:ca26e76455f243cd87071ecd6ebfbcde01ead913deefd2db5f75d99c561f9e65 in / 
# Thu, 23 Jan 2020 16:52:49 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:21:24 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:21:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:21:50 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:21:51 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:21:51 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:21:51 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:21:52 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:21:52 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:21:52 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:21:52 GMT
USER fluent
# Thu, 23 Jan 2020 17:21:53 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:21:53 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:62196161acf1e37f5a84921c7279f3a67078d6e98ce1deee27c00599e561af83`  
		Last Modified: Thu, 23 Jan 2020 16:53:12 GMT  
		Size: 2.5 MB (2549400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9874d3cc980ccb6c8250930173c5546fb6380cdf6c03cf3f435813d330c81f`  
		Last Modified: Thu, 23 Jan 2020 17:22:08 GMT  
		Size: 13.8 MB (13840280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438f2df4f4c1307f2015d187a95ad39268f861e8ad671791268932e65c2fca5d`  
		Last Modified: Thu, 23 Jan 2020 17:22:06 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac93fb83fc53559469fb48efbef4d1080291fd379f8b79e24fc930768fc155ac`  
		Last Modified: Thu, 23 Jan 2020 17:22:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683a942f732a50d31b9ac338fa89b616a6b4fbe7ef92797d5f261ba1bbd34bba`  
		Last Modified: Thu, 23 Jan 2020 17:22:06 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.8-1`

```console
$ docker pull fluentd@sha256:ad8d88f1600fca4fd624a149bd5f49a941193a36af6fa509f1baf714eb5238d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.8-1` - linux; amd64

```console
$ docker pull fluentd@sha256:75ce5020648cf6b41f8149ae2fa2f589c381dcdb61987e8bb1264f425c32ce95
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16477381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41a6ad1233ce7c9046c13db2fd1f97364149ad549a512ab72dedd2bef5e63b6b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:21:40 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:21:40 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:22:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:22:40 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:22:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:22:41 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:22:41 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:22:41 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:22:42 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:22:42 GMT
USER fluent
# Thu, 23 Jan 2020 17:22:42 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:22:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c614808f1174d32d67b7ecac4800e05ef3e411ae8bdedbb6240136c10a2f27`  
		Last Modified: Thu, 23 Jan 2020 17:23:19 GMT  
		Size: 13.7 MB (13711041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8bdd560291478d1c7f7cdb57fa5e1c5bb60ac5288f5cbd06068a192a400d9f`  
		Last Modified: Thu, 23 Jan 2020 17:23:06 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db832aa9e885329454cf3b2cc8a6c1154f5c31cd0b2565f9a4efdfff5b19f40`  
		Last Modified: Thu, 23 Jan 2020 17:23:05 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ae6fb92ee376b443db0999d49d19f43be88f5ecad0f24d9f9e0d37236f6bb5`  
		Last Modified: Thu, 23 Jan 2020 17:23:05 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:035a4e0ca4ec279d5b7efdc2ae1530b85b99f41cfac44cacbe86e8cf449bb15c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15926470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1d866d3935af22c17334b093ea3ed54f50c6eb4e6346381cd5771c3a783c877`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:09:48 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:11:27 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:11:37 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:11:38 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:11:39 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:11:40 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:11:41 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:11:42 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:11:42 GMT
USER fluent
# Thu, 23 Jan 2020 17:11:44 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:11:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61745ca2853b92fe876640e1120b69f2d6b0c5b53023a31e2efebea54c40ae2`  
		Last Modified: Thu, 23 Jan 2020 17:12:15 GMT  
		Size: 13.4 MB (13376576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637eb510f29cae52739de271c15f8d31d790c4fe77536740b05b62170c26bd05`  
		Last Modified: Thu, 23 Jan 2020 17:12:07 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cf50affa812e536c41281a121805e4b4478df66e432e132a54c89f174eb2df`  
		Last Modified: Thu, 23 Jan 2020 17:12:06 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1fbd8f4b19cf7d8acebe443fe90cb27438c633a4068d982842434f387a9db6`  
		Last Modified: Thu, 23 Jan 2020 17:12:06 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:610e4cd77b8f533d63b50e882ec044dd8ec729436f4ac7bbc6f8520f542c855f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16403315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36fb10a77e8f3c7d101a2f503ce225ff5b1b2f53d172c1f069d8c41f7fc4bb19`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:33:30 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:33:30 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:34:37 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:34:41 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:34:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:34:42 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:34:43 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:34:43 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:34:44 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:34:44 GMT
USER fluent
# Thu, 23 Jan 2020 17:34:45 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:34:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6b5c46a574799e0b946dbc6cc66cabfc6207b5ddcd573b123802551ea94f0f`  
		Last Modified: Thu, 23 Jan 2020 17:35:14 GMT  
		Size: 13.7 MB (13707861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d094f07cfa4b841c62b9dfae9c888180da1e4ef0c5f81ca834fc5f2a700768`  
		Last Modified: Thu, 23 Jan 2020 17:35:09 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aa646bd931e5a5d4279cc93b90231836817be0bae159b3043dce5c2e26b1ea`  
		Last Modified: Thu, 23 Jan 2020 17:35:08 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb631140a5800779637c95a8dcb92f4daeabb23dec32c970e7cf465c53c4eb`  
		Last Modified: Thu, 23 Jan 2020 17:35:08 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-1` - linux; 386

```console
$ docker pull fluentd@sha256:815f5dfb686d66717312114a34134b2d3776f3a909b45fd022353a40b94089b8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16381360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512d48c879211f5661da8e2f939e23e8d23cc3c9b4bbab459e5b7503d4d6d64d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:55:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:55:00 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:56:08 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:56:10 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:56:10 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:56:11 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:56:11 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:56:11 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:56:11 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:56:12 GMT
USER fluent
# Thu, 23 Jan 2020 17:56:12 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:56:12 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b8f6237861e49130cb68a766ee538a9dd868bb0613e052f95b04a3d8caf608`  
		Last Modified: Thu, 23 Jan 2020 17:56:43 GMT  
		Size: 13.6 MB (13610672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79633fb3e15c107605467c3bc079032fcb43992fccc3cc2fc389bcc216eafd`  
		Last Modified: Thu, 23 Jan 2020 17:56:38 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e4c942e6b974a2b7cf5f42624d47d6d555a98b2a21fbe228e7bee4e6fc3ae5`  
		Last Modified: Thu, 23 Jan 2020 17:56:38 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d7eb29f7a6c6f3b0ec43bb0e541253e271fb77b8517ffc1df29ba4101898d7`  
		Last Modified: Thu, 23 Jan 2020 17:56:38 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:33a5ca24b27bfe9ca6f4ff579d1fbe08fe7039f94e9c8378de0dd571d07b5a64
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16911283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a57d87b4e6f55a2bd3a52207151facd32cfe5a54d4640c28d84f3f5527b9d6cf`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:58:09 GMT
ADD file:b06f16ae13d177baa99c50f4b42de9479a24ae5b68aa967b17dbe98760ed809e in / 
# Thu, 23 Jan 2020 16:58:10 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:14:31 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:14:35 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:15:43 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:15:53 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:15:54 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:15:56 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:15:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:16:02 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:16:06 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:16:09 GMT
USER fluent
# Thu, 23 Jan 2020 17:16:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2ef848e1434ec427ca147408f3c6f1cec160019050a04c8a2040f35872ab661b`  
		Last Modified: Thu, 23 Jan 2020 16:58:55 GMT  
		Size: 2.8 MB (2786373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d8bdf10b187c1ca45fe47a4ef50135c9d99b67f6b4d85a39393c5dcb845e6`  
		Last Modified: Thu, 23 Jan 2020 17:16:51 GMT  
		Size: 14.1 MB (14122691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138bd852fdb69bf8e38738e5e504a7191ae928168788f8c83532952225e0b264`  
		Last Modified: Thu, 23 Jan 2020 17:16:40 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748b67f558bcb92af2081528139dcb2fa37ca0a7d8fb7e1a61c9cf3f3f7ce0d3`  
		Last Modified: Thu, 23 Jan 2020 17:16:40 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25aaa684ac282e02e36ce16dc19d2c7272c32da084e2b0e246b96306897a96b3`  
		Last Modified: Thu, 23 Jan 2020 17:16:40 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-1` - linux; s390x

```console
$ docker pull fluentd@sha256:6a46692938f6ee9b718f592bc32084afdbbae1d41014bb9dcdb56f58722bfdde
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16391842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ca0024734079e1ae4f6e753780eea50407b87086244deee3b491bc58efc4c1`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:49 GMT
ADD file:ca26e76455f243cd87071ecd6ebfbcde01ead913deefd2db5f75d99c561f9e65 in / 
# Thu, 23 Jan 2020 16:52:49 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:21:24 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:21:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:21:50 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:21:51 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:21:51 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:21:51 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:21:52 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:21:52 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:21:52 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:21:52 GMT
USER fluent
# Thu, 23 Jan 2020 17:21:53 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:21:53 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:62196161acf1e37f5a84921c7279f3a67078d6e98ce1deee27c00599e561af83`  
		Last Modified: Thu, 23 Jan 2020 16:53:12 GMT  
		Size: 2.5 MB (2549400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9874d3cc980ccb6c8250930173c5546fb6380cdf6c03cf3f435813d330c81f`  
		Last Modified: Thu, 23 Jan 2020 17:22:08 GMT  
		Size: 13.8 MB (13840280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438f2df4f4c1307f2015d187a95ad39268f861e8ad671791268932e65c2fca5d`  
		Last Modified: Thu, 23 Jan 2020 17:22:06 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac93fb83fc53559469fb48efbef4d1080291fd379f8b79e24fc930768fc155ac`  
		Last Modified: Thu, 23 Jan 2020 17:22:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683a942f732a50d31b9ac338fa89b616a6b4fbe7ef92797d5f261ba1bbd34bba`  
		Last Modified: Thu, 23 Jan 2020 17:22:06 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.8.1-1.0`

```console
$ docker pull fluentd@sha256:ad8d88f1600fca4fd624a149bd5f49a941193a36af6fa509f1baf714eb5238d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:v1.8.1-1.0` - linux; amd64

```console
$ docker pull fluentd@sha256:75ce5020648cf6b41f8149ae2fa2f589c381dcdb61987e8bb1264f425c32ce95
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16477381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41a6ad1233ce7c9046c13db2fd1f97364149ad549a512ab72dedd2bef5e63b6b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:21:40 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:21:40 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:22:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:22:40 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:22:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:22:41 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:22:41 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:22:41 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:22:42 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:22:42 GMT
USER fluent
# Thu, 23 Jan 2020 17:22:42 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:22:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c614808f1174d32d67b7ecac4800e05ef3e411ae8bdedbb6240136c10a2f27`  
		Last Modified: Thu, 23 Jan 2020 17:23:19 GMT  
		Size: 13.7 MB (13711041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8bdd560291478d1c7f7cdb57fa5e1c5bb60ac5288f5cbd06068a192a400d9f`  
		Last Modified: Thu, 23 Jan 2020 17:23:06 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db832aa9e885329454cf3b2cc8a6c1154f5c31cd0b2565f9a4efdfff5b19f40`  
		Last Modified: Thu, 23 Jan 2020 17:23:05 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ae6fb92ee376b443db0999d49d19f43be88f5ecad0f24d9f9e0d37236f6bb5`  
		Last Modified: Thu, 23 Jan 2020 17:23:05 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-1.0` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:035a4e0ca4ec279d5b7efdc2ae1530b85b99f41cfac44cacbe86e8cf449bb15c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15926470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1d866d3935af22c17334b093ea3ed54f50c6eb4e6346381cd5771c3a783c877`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:09:48 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:11:27 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:11:37 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:11:38 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:11:39 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:11:40 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:11:41 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:11:42 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:11:42 GMT
USER fluent
# Thu, 23 Jan 2020 17:11:44 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:11:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61745ca2853b92fe876640e1120b69f2d6b0c5b53023a31e2efebea54c40ae2`  
		Last Modified: Thu, 23 Jan 2020 17:12:15 GMT  
		Size: 13.4 MB (13376576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637eb510f29cae52739de271c15f8d31d790c4fe77536740b05b62170c26bd05`  
		Last Modified: Thu, 23 Jan 2020 17:12:07 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cf50affa812e536c41281a121805e4b4478df66e432e132a54c89f174eb2df`  
		Last Modified: Thu, 23 Jan 2020 17:12:06 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1fbd8f4b19cf7d8acebe443fe90cb27438c633a4068d982842434f387a9db6`  
		Last Modified: Thu, 23 Jan 2020 17:12:06 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:610e4cd77b8f533d63b50e882ec044dd8ec729436f4ac7bbc6f8520f542c855f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16403315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36fb10a77e8f3c7d101a2f503ce225ff5b1b2f53d172c1f069d8c41f7fc4bb19`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:33:30 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:33:30 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:34:37 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:34:41 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:34:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:34:42 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:34:43 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:34:43 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:34:44 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:34:44 GMT
USER fluent
# Thu, 23 Jan 2020 17:34:45 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:34:45 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6b5c46a574799e0b946dbc6cc66cabfc6207b5ddcd573b123802551ea94f0f`  
		Last Modified: Thu, 23 Jan 2020 17:35:14 GMT  
		Size: 13.7 MB (13707861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d094f07cfa4b841c62b9dfae9c888180da1e4ef0c5f81ca834fc5f2a700768`  
		Last Modified: Thu, 23 Jan 2020 17:35:09 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aa646bd931e5a5d4279cc93b90231836817be0bae159b3043dce5c2e26b1ea`  
		Last Modified: Thu, 23 Jan 2020 17:35:08 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cb631140a5800779637c95a8dcb92f4daeabb23dec32c970e7cf465c53c4eb`  
		Last Modified: Thu, 23 Jan 2020 17:35:08 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:815f5dfb686d66717312114a34134b2d3776f3a909b45fd022353a40b94089b8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16381360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512d48c879211f5661da8e2f939e23e8d23cc3c9b4bbab459e5b7503d4d6d64d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:55:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:55:00 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:56:08 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:56:10 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:56:10 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:56:11 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:56:11 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:56:11 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:56:11 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:56:12 GMT
USER fluent
# Thu, 23 Jan 2020 17:56:12 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:56:12 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b8f6237861e49130cb68a766ee538a9dd868bb0613e052f95b04a3d8caf608`  
		Last Modified: Thu, 23 Jan 2020 17:56:43 GMT  
		Size: 13.6 MB (13610672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79633fb3e15c107605467c3bc079032fcb43992fccc3cc2fc389bcc216eafd`  
		Last Modified: Thu, 23 Jan 2020 17:56:38 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e4c942e6b974a2b7cf5f42624d47d6d555a98b2a21fbe228e7bee4e6fc3ae5`  
		Last Modified: Thu, 23 Jan 2020 17:56:38 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d7eb29f7a6c6f3b0ec43bb0e541253e271fb77b8517ffc1df29ba4101898d7`  
		Last Modified: Thu, 23 Jan 2020 17:56:38 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:33a5ca24b27bfe9ca6f4ff579d1fbe08fe7039f94e9c8378de0dd571d07b5a64
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16911283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a57d87b4e6f55a2bd3a52207151facd32cfe5a54d4640c28d84f3f5527b9d6cf`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:58:09 GMT
ADD file:b06f16ae13d177baa99c50f4b42de9479a24ae5b68aa967b17dbe98760ed809e in / 
# Thu, 23 Jan 2020 16:58:10 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:14:31 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:14:35 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:15:43 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:15:53 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:15:54 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:15:56 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:15:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:16:02 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:16:06 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:16:09 GMT
USER fluent
# Thu, 23 Jan 2020 17:16:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2ef848e1434ec427ca147408f3c6f1cec160019050a04c8a2040f35872ab661b`  
		Last Modified: Thu, 23 Jan 2020 16:58:55 GMT  
		Size: 2.8 MB (2786373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d8bdf10b187c1ca45fe47a4ef50135c9d99b67f6b4d85a39393c5dcb845e6`  
		Last Modified: Thu, 23 Jan 2020 17:16:51 GMT  
		Size: 14.1 MB (14122691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138bd852fdb69bf8e38738e5e504a7191ae928168788f8c83532952225e0b264`  
		Last Modified: Thu, 23 Jan 2020 17:16:40 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748b67f558bcb92af2081528139dcb2fa37ca0a7d8fb7e1a61c9cf3f3f7ce0d3`  
		Last Modified: Thu, 23 Jan 2020 17:16:40 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25aaa684ac282e02e36ce16dc19d2c7272c32da084e2b0e246b96306897a96b3`  
		Last Modified: Thu, 23 Jan 2020 17:16:40 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:6a46692938f6ee9b718f592bc32084afdbbae1d41014bb9dcdb56f58722bfdde
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16391842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ca0024734079e1ae4f6e753780eea50407b87086244deee3b491bc58efc4c1`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:49 GMT
ADD file:ca26e76455f243cd87071ecd6ebfbcde01ead913deefd2db5f75d99c561f9e65 in / 
# Thu, 23 Jan 2020 16:52:49 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:21:24 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 23 Jan 2020 17:21:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Thu, 23 Jan 2020 17:21:50 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Thu, 23 Jan 2020 17:21:51 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 23 Jan 2020 17:21:51 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 23 Jan 2020 17:21:51 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Thu, 23 Jan 2020 17:21:52 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 23 Jan 2020 17:21:52 GMT
ENV LD_PRELOAD=
# Thu, 23 Jan 2020 17:21:52 GMT
EXPOSE 24224 5140
# Thu, 23 Jan 2020 17:21:52 GMT
USER fluent
# Thu, 23 Jan 2020 17:21:53 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 23 Jan 2020 17:21:53 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:62196161acf1e37f5a84921c7279f3a67078d6e98ce1deee27c00599e561af83`  
		Last Modified: Thu, 23 Jan 2020 16:53:12 GMT  
		Size: 2.5 MB (2549400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9874d3cc980ccb6c8250930173c5546fb6380cdf6c03cf3f435813d330c81f`  
		Last Modified: Thu, 23 Jan 2020 17:22:08 GMT  
		Size: 13.8 MB (13840280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438f2df4f4c1307f2015d187a95ad39268f861e8ad671791268932e65c2fca5d`  
		Last Modified: Thu, 23 Jan 2020 17:22:06 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac93fb83fc53559469fb48efbef4d1080291fd379f8b79e24fc930768fc155ac`  
		Last Modified: Thu, 23 Jan 2020 17:22:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683a942f732a50d31b9ac338fa89b616a6b4fbe7ef92797d5f261ba1bbd34bba`  
		Last Modified: Thu, 23 Jan 2020 17:22:06 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.8.1-debian-1.0`

```console
$ docker pull fluentd@sha256:b138ff1951db887643647a208dd37d7dc0cc8e0ed479148eff23ba3fed2ef7f0
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

### `fluentd:v1.8.1-debian-1.0` - linux; amd64

```console
$ docker pull fluentd@sha256:a64cdb4bbac48a629c79295ebe2133a6d6e79040d18cc251cbdf8d674d5fc94f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85570637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec073742f8ca722d877c9b27322d6f756b291e277caa00987e10f3984bab553d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Wed, 15 Jan 2020 21:22:19 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 21:22:19 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 21:22:20 GMT
ENV TINI_VERSION=0.18.0
# Wed, 15 Jan 2020 21:23:46 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:23:47 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:23:47 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:23:47 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:23:47 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:23:47 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 15 Jan 2020 21:23:47 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:23:48 GMT
USER fluent
# Wed, 15 Jan 2020 21:23:48 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:23:48 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079ac5a2be903ccbc485014962ecb5c563c753d64dfe8e8c65ef04d281675eb3`  
		Last Modified: Wed, 15 Jan 2020 21:24:17 GMT  
		Size: 24.5 MB (24489949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fea7c59af3371639d1a62bb0611e7c093b4460820f3ed55ede3ca2cf8341f0`  
		Last Modified: Wed, 15 Jan 2020 21:24:13 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fffeac033ba4e5458ac62102425a6fadb288f91f860dbbd1fe8f1c9430f900`  
		Last Modified: Wed, 15 Jan 2020 21:24:13 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4b4200a9ee32aa7af74a90e37beba6cd1f21f074f62229f1f4bbc78a9b45c1`  
		Last Modified: Wed, 15 Jan 2020 21:24:13 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-debian-1.0` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:e63a2ab2a0acbb6f6d79325e35819e08fa1080e0d5855713108e0cf0ae667597
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.5 MB (79522088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a20d4e72b52e7694a85271a7c9655fa39fa51c9ade14ce0c691dd6b7569db477`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 02:16:09 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 02:16:12 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 02:16:13 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 02:19:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 02:19:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 02:19:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 02:20:03 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 10:09:40 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 10:09:41 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 10:09:42 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 10:12:43 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 10:12:47 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 10:12:47 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 10:12:48 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 10:12:49 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 10:12:49 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 10:12:50 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 10:12:50 GMT
USER fluent
# Sun, 02 Feb 2020 10:12:51 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 10:12:52 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecb489e800f7f428b98c5f257bb143dc6d911d3b076c3d9e0940d04f0f2557c`  
		Last Modified: Sun, 02 Feb 2020 03:16:08 GMT  
		Size: 10.3 MB (10326074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cddfcf800a56c64451730cbfd34ac7b3da09bfe974245010cf9db34bc74f681`  
		Last Modified: Sun, 02 Feb 2020 03:16:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdd05ffdd7888092a6ef03be377963c297edec0344ce762bb6b3e1e2f114b94`  
		Last Modified: Sun, 02 Feb 2020 03:16:40 GMT  
		Size: 20.7 MB (20712712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e99c39d252f8cf22fae4749b2764aec83374848c63b8546989494f7f7a1cd2`  
		Last Modified: Sun, 02 Feb 2020 03:16:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272ff14bfe1c70f6e16f8b5e962156835236c5b69df49d87291aef395b8e94b1`  
		Last Modified: Sun, 02 Feb 2020 10:13:07 GMT  
		Size: 23.7 MB (23650559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e68d8abb9d4c888a42a18c0a3f367a005d2d295f0e152867c599b73073944f8`  
		Last Modified: Sun, 02 Feb 2020 10:13:00 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b8e6d3ea9f0cff60df32c221dd5bca551c7b72445819cfa860591b853c9737`  
		Last Modified: Sun, 02 Feb 2020 10:13:01 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc03de087a4dc6cad6775f206dc8accb7b18334d6b00a683b061090217ecec58`  
		Last Modified: Sun, 02 Feb 2020 10:13:00 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-debian-1.0` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:6d7d26be5423b9043a31b7648bab37fe76a4f12bcb3dc4083c8bb31804d9efef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.7 MB (76714029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb00294e9587616f0f3f447c12782d203f0a24c212f06a5758b892c8681670f7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:26:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:26:33 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 03:44:54 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 03:44:55 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 03:44:56 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 03:49:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 03:49:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 03:49:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 03:49:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 03:49:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 03:49:19 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 18:19:27 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 18:19:28 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 18:19:29 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 18:22:29 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 18:22:33 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 18:22:33 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 18:22:34 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 18:22:35 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 18:22:35 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 18:22:36 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 18:22:36 GMT
USER fluent
# Sun, 02 Feb 2020 18:22:37 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 18:22:38 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d4814dc35805320e4b9357cbbb08a16b2fdf6fb2cc515726d081a934c414ad`  
		Last Modified: Sun, 02 Feb 2020 04:37:50 GMT  
		Size: 9.8 MB (9847353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02fe22250f5be96c8fee4c95a756bd855486de1468bbaab88889cb9a99919ce`  
		Last Modified: Sun, 02 Feb 2020 04:37:47 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8fb6d3f67479293696c0ab1862f3d3cc1ccc4c655c60fe8a6b96d3958a13be`  
		Last Modified: Sun, 02 Feb 2020 04:38:21 GMT  
		Size: 20.6 MB (20620356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b57ca0c1f7b3cf1cf1382ec1048a03d8dd1fdd32b795c902f5305133d27c78`  
		Last Modified: Sun, 02 Feb 2020 04:38:17 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a701c96ddb9b7a0fd924bbca1161f17fccb1ad504494e2369dc682b2026cc0a`  
		Last Modified: Sun, 02 Feb 2020 18:23:08 GMT  
		Size: 23.5 MB (23544118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b25b66e5c88dcfbd253f947fe9f3c2cba130cbe35c6f090bc0d45c473a996f`  
		Last Modified: Sun, 02 Feb 2020 18:23:00 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1e7a614c23f69e9a7b665e0befa3122e6dc70fd6b992912e18798eb9805f46`  
		Last Modified: Sun, 02 Feb 2020 18:23:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abd739dd941e418b8d845b27a6489eb3b0745c91d4dd6b68325037e9abe6f99`  
		Last Modified: Sun, 02 Feb 2020 18:23:00 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-debian-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:7149cf9eb546f88186c1dd7e1bb68a2ca19bd246252afdf94eaa9cfa545ecdae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82877836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40ea5cd2ba60e02a8b4612e1c248045af0fb66518d12988af07d3b32edc35003`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 09:57:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:57:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 10:05:44 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 10:05:44 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 10:05:45 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 10:09:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 10:09:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 10:09:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 10:09:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 10:09:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 10:09:34 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 19:51:38 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 19:51:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 19:51:39 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 19:54:14 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 19:54:19 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 19:54:20 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 19:54:20 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 19:54:21 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 19:54:22 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 19:54:22 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 19:54:23 GMT
USER fluent
# Sun, 02 Feb 2020 19:54:23 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 19:54:24 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7c2697ff6f058d7f0b17dfdf123fffce9a007b3f302b77c8b9bdc9fd7685d9`  
		Last Modified: Sun, 02 Feb 2020 10:58:01 GMT  
		Size: 11.2 MB (11244496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783fe382da6383f2efde489fb27e5a517200e0b81cb49935ae0f0ce2a8d5e152`  
		Last Modified: Sun, 02 Feb 2020 10:57:57 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e033592aeac21c0ce386b8333f16f6235250b4a12589032d45952f28aae99`  
		Last Modified: Sun, 02 Feb 2020 10:58:31 GMT  
		Size: 21.3 MB (21281648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4967683b60ada551e77eafdd485daad99a6f1942cf491c5976877e6a7ca01`  
		Last Modified: Sun, 02 Feb 2020 10:58:26 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d81ffd5e931d1616eee580f5f19ea8c6301a56b0b53850af2dbab9f6758739c`  
		Last Modified: Sun, 02 Feb 2020 19:54:51 GMT  
		Size: 24.5 MB (24497945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18c3d5326caa39b3fb45e5c73e79f64173464fc0fb40bd84e0f7296727a5a65`  
		Last Modified: Sun, 02 Feb 2020 19:54:44 GMT  
		Size: 1.9 KB (1857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486436f3a7c9cf6400be0babd697ae9d80bcaf0663db85bda9cd54f7621462c5`  
		Last Modified: Sun, 02 Feb 2020 19:54:44 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cad2875e49a6a05c3a7887a0ee49996e2e6deb33f8d10fadd0bd386c1db226`  
		Last Modified: Sun, 02 Feb 2020 19:54:44 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-debian-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:c136028e77500f5471acde23a3d63ba5383c95ae1807e180e310601fc456f9c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89541432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64b5fd240746cd4512b4249002a05191e11eaaa37346696887ec2361b38fbc5f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 09:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:39:05 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 09:48:03 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 09:48:03 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 09:48:03 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 09:52:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 09:52:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 09:52:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 09:52:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 09:52:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 09:52:15 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 13:30:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 13:30:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 13:30:48 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 13:32:45 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 13:32:46 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 13:32:46 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 13:32:47 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 13:32:47 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 13:32:47 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 13:32:47 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 13:32:47 GMT
USER fluent
# Sun, 02 Feb 2020 13:32:48 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 13:32:48 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd448d2713c41a4a7de819558285e075713444e2664f5e9180ae765e0168be4`  
		Last Modified: Sun, 02 Feb 2020 10:40:01 GMT  
		Size: 17.2 MB (17205970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b44fb48efbb69a28436d9d68bf4e52520dc4f725a894f8e270181ce6fcb40ef`  
		Last Modified: Sun, 02 Feb 2020 10:39:54 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7e5d604e111de701bacf8c6952c8658d23d38b32c40a699c9ffdd0a50c9f45`  
		Last Modified: Sun, 02 Feb 2020 10:40:28 GMT  
		Size: 20.9 MB (20885510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5640ed0b4362227a298cdba0f568b4516440d1041650eed93add06c421dec473`  
		Last Modified: Sun, 02 Feb 2020 10:40:24 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d56ff40ed5b0d88c1c15d1a48c5f50f4f211d6a40ba93816e01af838ab9d60`  
		Last Modified: Sun, 02 Feb 2020 13:33:11 GMT  
		Size: 23.7 MB (23699906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c53d869d95852008e19c18a00149c3ad36a0cb7535504619273e616d93e0b66`  
		Last Modified: Sun, 02 Feb 2020 13:33:04 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8669f29229d8663d7060b3400bc999238b71ad07ed6a48fd33cca361124bae3d`  
		Last Modified: Sun, 02 Feb 2020 13:33:04 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2614953e46b4c0f2da1b2447d1591e7d9dfd488c50be1805366b21eac4326aed`  
		Last Modified: Sun, 02 Feb 2020 13:33:04 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:d35a08020b5a977ed9ce2e3e2e59f6ed843d418cbbcbac16531dc520a138718b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90227417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5559fa820d01b780a04fcdb681343dc4223bb9688db817a568175e568128a619`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 17:18:04 GMT
ADD file:aadd94011800934ec665edb193029ab2be0aeb668c566ba4bc52bd678e71a735 in / 
# Sat, 01 Feb 2020 17:18:06 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:56:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:56:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 07:10:22 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 07:10:25 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 07:10:27 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 07:18:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 07:18:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 07:18:17 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 07:18:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 07:18:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 07:18:37 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 16:54:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 16:54:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 16:54:59 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 16:58:51 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 16:59:11 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 16:59:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 16:59:16 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 16:59:19 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 16:59:23 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 16:59:26 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 16:59:31 GMT
USER fluent
# Sun, 02 Feb 2020 16:59:34 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 16:59:37 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:16a7e1c5b23ec3cf93421f5f868c1cf2cda468cfebb1b2bc62f4d533d99d256b`  
		Last Modified: Sat, 01 Feb 2020 17:26:05 GMT  
		Size: 30.5 MB (30517693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d44bc1840f426f48fc6d4cc23113f86c02e7f46ef4c400ce5b4c76010c72a2`  
		Last Modified: Sun, 02 Feb 2020 08:19:33 GMT  
		Size: 12.7 MB (12688850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e418c294c298ad8987cb27fc2adff7ce43dee0e55af3c86e59af9271e4c490`  
		Last Modified: Sun, 02 Feb 2020 08:19:29 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ed4fdb4090425730dd3e443c0fd27af2b2cff3415260f22a0056d8ff639b99`  
		Last Modified: Sun, 02 Feb 2020 08:20:20 GMT  
		Size: 22.0 MB (21968679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3472d9aadeeb03ff16dda03cf908dc2438dfbe262d09c2f3fe38ba8a9a8a9a8`  
		Last Modified: Sun, 02 Feb 2020 08:20:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f6ea37b6222ce5baa419db61c379c349818d5d08d103a15fbc9955c8167e62`  
		Last Modified: Sun, 02 Feb 2020 17:00:02 GMT  
		Size: 25.0 MB (25049107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd0768d534b7c90cd7d57da4b3f7463e0b18fa3e373b2f0d79303e131116b38`  
		Last Modified: Sun, 02 Feb 2020 16:59:56 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f9362111330afcb05168897cacc5d890dfeee23984212d6b8ed657a2dbca28`  
		Last Modified: Sun, 02 Feb 2020 16:59:56 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592335602dbd25ea7322c3707e5ba35f9ca1bf5be746a180c9bf32ab93c4e100`  
		Last Modified: Sun, 02 Feb 2020 16:59:56 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-debian-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:d03b0bf781c2274e8de992cb2935ca0ee4e754260f5e7b27d2accee2cc3c346c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.7 MB (82749146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:432486d4d4b647921e2bc8317f30ef256e1201c66845b002a1c62d06d3a68512`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:24:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_MAJOR=2.6
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 01 Feb 2020 22:36:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 01 Feb 2020 22:36:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:36:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 01 Feb 2020 22:36:07 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 03:37:02 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 03:37:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 03:37:02 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 03:38:21 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 03:38:23 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 03:38:24 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 03:38:24 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 03:38:24 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 03:38:24 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 03:38:24 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 03:38:24 GMT
USER fluent
# Sun, 02 Feb 2020 03:38:25 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 03:38:25 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17d8d1356b8293f168a2578ba81c34f07ee79d7a56bd579e776ad498d0b2e8`  
		Last Modified: Sat, 01 Feb 2020 22:56:51 GMT  
		Size: 10.8 MB (10795999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d180073499f34bb9340ecac840eeb00fab127188f731188ba78e76e435b62c`  
		Last Modified: Sat, 01 Feb 2020 22:56:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351f50ba1593f8ab66d1deaf12e190c35ecfea96815beda37efe10f1246f342b`  
		Last Modified: Sat, 01 Feb 2020 22:57:18 GMT  
		Size: 21.6 MB (21592569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8a5d1fd225888733445fbc5a03464b232ab7c659a3bf619e93c5670a0ca594`  
		Last Modified: Sat, 01 Feb 2020 22:57:14 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c81d9fd7daa9ad2dc6a948e05bb47fec6e87ddd58b48e6aaa9c2f8b8f4f59e`  
		Last Modified: Sun, 02 Feb 2020 03:38:40 GMT  
		Size: 24.7 MB (24652127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae4932f4e7f17509dd1c3aed04301daf0bc843b7e3fe8c5e5ad957e3c7850b3`  
		Last Modified: Sun, 02 Feb 2020 03:38:42 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e18c5cd131a8accf4498060f449e239093b9b52c2696449733ffaaf023ae19f`  
		Last Modified: Sun, 02 Feb 2020 03:38:37 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd85d0826acc444b2e46d021d2352fb54757b9ea410c2baec476ef2078eed7a`  
		Last Modified: Sun, 02 Feb 2020 03:38:42 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.8-debian-1`

```console
$ docker pull fluentd@sha256:b138ff1951db887643647a208dd37d7dc0cc8e0ed479148eff23ba3fed2ef7f0
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

### `fluentd:v1.8-debian-1` - linux; amd64

```console
$ docker pull fluentd@sha256:a64cdb4bbac48a629c79295ebe2133a6d6e79040d18cc251cbdf8d674d5fc94f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85570637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec073742f8ca722d877c9b27322d6f756b291e277caa00987e10f3984bab553d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Wed, 15 Jan 2020 21:22:19 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 21:22:19 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 21:22:20 GMT
ENV TINI_VERSION=0.18.0
# Wed, 15 Jan 2020 21:23:46 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:23:47 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:23:47 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:23:47 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:23:47 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:23:47 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 15 Jan 2020 21:23:47 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:23:48 GMT
USER fluent
# Wed, 15 Jan 2020 21:23:48 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:23:48 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079ac5a2be903ccbc485014962ecb5c563c753d64dfe8e8c65ef04d281675eb3`  
		Last Modified: Wed, 15 Jan 2020 21:24:17 GMT  
		Size: 24.5 MB (24489949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fea7c59af3371639d1a62bb0611e7c093b4460820f3ed55ede3ca2cf8341f0`  
		Last Modified: Wed, 15 Jan 2020 21:24:13 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fffeac033ba4e5458ac62102425a6fadb288f91f860dbbd1fe8f1c9430f900`  
		Last Modified: Wed, 15 Jan 2020 21:24:13 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4b4200a9ee32aa7af74a90e37beba6cd1f21f074f62229f1f4bbc78a9b45c1`  
		Last Modified: Wed, 15 Jan 2020 21:24:13 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:e63a2ab2a0acbb6f6d79325e35819e08fa1080e0d5855713108e0cf0ae667597
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.5 MB (79522088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a20d4e72b52e7694a85271a7c9655fa39fa51c9ade14ce0c691dd6b7569db477`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 02:16:09 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 02:16:12 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 02:16:13 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 02:19:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 02:19:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 02:19:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 02:20:03 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 10:09:40 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 10:09:41 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 10:09:42 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 10:12:43 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 10:12:47 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 10:12:47 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 10:12:48 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 10:12:49 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 10:12:49 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 10:12:50 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 10:12:50 GMT
USER fluent
# Sun, 02 Feb 2020 10:12:51 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 10:12:52 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecb489e800f7f428b98c5f257bb143dc6d911d3b076c3d9e0940d04f0f2557c`  
		Last Modified: Sun, 02 Feb 2020 03:16:08 GMT  
		Size: 10.3 MB (10326074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cddfcf800a56c64451730cbfd34ac7b3da09bfe974245010cf9db34bc74f681`  
		Last Modified: Sun, 02 Feb 2020 03:16:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdd05ffdd7888092a6ef03be377963c297edec0344ce762bb6b3e1e2f114b94`  
		Last Modified: Sun, 02 Feb 2020 03:16:40 GMT  
		Size: 20.7 MB (20712712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e99c39d252f8cf22fae4749b2764aec83374848c63b8546989494f7f7a1cd2`  
		Last Modified: Sun, 02 Feb 2020 03:16:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272ff14bfe1c70f6e16f8b5e962156835236c5b69df49d87291aef395b8e94b1`  
		Last Modified: Sun, 02 Feb 2020 10:13:07 GMT  
		Size: 23.7 MB (23650559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e68d8abb9d4c888a42a18c0a3f367a005d2d295f0e152867c599b73073944f8`  
		Last Modified: Sun, 02 Feb 2020 10:13:00 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b8e6d3ea9f0cff60df32c221dd5bca551c7b72445819cfa860591b853c9737`  
		Last Modified: Sun, 02 Feb 2020 10:13:01 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc03de087a4dc6cad6775f206dc8accb7b18334d6b00a683b061090217ecec58`  
		Last Modified: Sun, 02 Feb 2020 10:13:00 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:6d7d26be5423b9043a31b7648bab37fe76a4f12bcb3dc4083c8bb31804d9efef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.7 MB (76714029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb00294e9587616f0f3f447c12782d203f0a24c212f06a5758b892c8681670f7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:26:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:26:33 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 03:44:54 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 03:44:55 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 03:44:56 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 03:49:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 03:49:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 03:49:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 03:49:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 03:49:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 03:49:19 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 18:19:27 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 18:19:28 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 18:19:29 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 18:22:29 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 18:22:33 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 18:22:33 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 18:22:34 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 18:22:35 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 18:22:35 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 18:22:36 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 18:22:36 GMT
USER fluent
# Sun, 02 Feb 2020 18:22:37 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 18:22:38 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d4814dc35805320e4b9357cbbb08a16b2fdf6fb2cc515726d081a934c414ad`  
		Last Modified: Sun, 02 Feb 2020 04:37:50 GMT  
		Size: 9.8 MB (9847353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02fe22250f5be96c8fee4c95a756bd855486de1468bbaab88889cb9a99919ce`  
		Last Modified: Sun, 02 Feb 2020 04:37:47 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8fb6d3f67479293696c0ab1862f3d3cc1ccc4c655c60fe8a6b96d3958a13be`  
		Last Modified: Sun, 02 Feb 2020 04:38:21 GMT  
		Size: 20.6 MB (20620356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b57ca0c1f7b3cf1cf1382ec1048a03d8dd1fdd32b795c902f5305133d27c78`  
		Last Modified: Sun, 02 Feb 2020 04:38:17 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a701c96ddb9b7a0fd924bbca1161f17fccb1ad504494e2369dc682b2026cc0a`  
		Last Modified: Sun, 02 Feb 2020 18:23:08 GMT  
		Size: 23.5 MB (23544118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b25b66e5c88dcfbd253f947fe9f3c2cba130cbe35c6f090bc0d45c473a996f`  
		Last Modified: Sun, 02 Feb 2020 18:23:00 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1e7a614c23f69e9a7b665e0befa3122e6dc70fd6b992912e18798eb9805f46`  
		Last Modified: Sun, 02 Feb 2020 18:23:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abd739dd941e418b8d845b27a6489eb3b0745c91d4dd6b68325037e9abe6f99`  
		Last Modified: Sun, 02 Feb 2020 18:23:00 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:7149cf9eb546f88186c1dd7e1bb68a2ca19bd246252afdf94eaa9cfa545ecdae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82877836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40ea5cd2ba60e02a8b4612e1c248045af0fb66518d12988af07d3b32edc35003`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 09:57:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:57:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 10:05:44 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 10:05:44 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 10:05:45 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 10:09:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 10:09:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 10:09:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 10:09:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 10:09:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 10:09:34 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 19:51:38 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 19:51:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 19:51:39 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 19:54:14 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 19:54:19 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 19:54:20 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 19:54:20 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 19:54:21 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 19:54:22 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 19:54:22 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 19:54:23 GMT
USER fluent
# Sun, 02 Feb 2020 19:54:23 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 19:54:24 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7c2697ff6f058d7f0b17dfdf123fffce9a007b3f302b77c8b9bdc9fd7685d9`  
		Last Modified: Sun, 02 Feb 2020 10:58:01 GMT  
		Size: 11.2 MB (11244496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783fe382da6383f2efde489fb27e5a517200e0b81cb49935ae0f0ce2a8d5e152`  
		Last Modified: Sun, 02 Feb 2020 10:57:57 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e033592aeac21c0ce386b8333f16f6235250b4a12589032d45952f28aae99`  
		Last Modified: Sun, 02 Feb 2020 10:58:31 GMT  
		Size: 21.3 MB (21281648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4967683b60ada551e77eafdd485daad99a6f1942cf491c5976877e6a7ca01`  
		Last Modified: Sun, 02 Feb 2020 10:58:26 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d81ffd5e931d1616eee580f5f19ea8c6301a56b0b53850af2dbab9f6758739c`  
		Last Modified: Sun, 02 Feb 2020 19:54:51 GMT  
		Size: 24.5 MB (24497945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18c3d5326caa39b3fb45e5c73e79f64173464fc0fb40bd84e0f7296727a5a65`  
		Last Modified: Sun, 02 Feb 2020 19:54:44 GMT  
		Size: 1.9 KB (1857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486436f3a7c9cf6400be0babd697ae9d80bcaf0663db85bda9cd54f7621462c5`  
		Last Modified: Sun, 02 Feb 2020 19:54:44 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cad2875e49a6a05c3a7887a0ee49996e2e6deb33f8d10fadd0bd386c1db226`  
		Last Modified: Sun, 02 Feb 2020 19:54:44 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:c136028e77500f5471acde23a3d63ba5383c95ae1807e180e310601fc456f9c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89541432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64b5fd240746cd4512b4249002a05191e11eaaa37346696887ec2361b38fbc5f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 09:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:39:05 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 09:48:03 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 09:48:03 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 09:48:03 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 09:52:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 09:52:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 09:52:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 09:52:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 09:52:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 09:52:15 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 13:30:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 13:30:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 13:30:48 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 13:32:45 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 13:32:46 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 13:32:46 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 13:32:47 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 13:32:47 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 13:32:47 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 13:32:47 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 13:32:47 GMT
USER fluent
# Sun, 02 Feb 2020 13:32:48 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 13:32:48 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd448d2713c41a4a7de819558285e075713444e2664f5e9180ae765e0168be4`  
		Last Modified: Sun, 02 Feb 2020 10:40:01 GMT  
		Size: 17.2 MB (17205970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b44fb48efbb69a28436d9d68bf4e52520dc4f725a894f8e270181ce6fcb40ef`  
		Last Modified: Sun, 02 Feb 2020 10:39:54 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7e5d604e111de701bacf8c6952c8658d23d38b32c40a699c9ffdd0a50c9f45`  
		Last Modified: Sun, 02 Feb 2020 10:40:28 GMT  
		Size: 20.9 MB (20885510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5640ed0b4362227a298cdba0f568b4516440d1041650eed93add06c421dec473`  
		Last Modified: Sun, 02 Feb 2020 10:40:24 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d56ff40ed5b0d88c1c15d1a48c5f50f4f211d6a40ba93816e01af838ab9d60`  
		Last Modified: Sun, 02 Feb 2020 13:33:11 GMT  
		Size: 23.7 MB (23699906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c53d869d95852008e19c18a00149c3ad36a0cb7535504619273e616d93e0b66`  
		Last Modified: Sun, 02 Feb 2020 13:33:04 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8669f29229d8663d7060b3400bc999238b71ad07ed6a48fd33cca361124bae3d`  
		Last Modified: Sun, 02 Feb 2020 13:33:04 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2614953e46b4c0f2da1b2447d1591e7d9dfd488c50be1805366b21eac4326aed`  
		Last Modified: Sun, 02 Feb 2020 13:33:04 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:d35a08020b5a977ed9ce2e3e2e59f6ed843d418cbbcbac16531dc520a138718b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90227417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5559fa820d01b780a04fcdb681343dc4223bb9688db817a568175e568128a619`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 17:18:04 GMT
ADD file:aadd94011800934ec665edb193029ab2be0aeb668c566ba4bc52bd678e71a735 in / 
# Sat, 01 Feb 2020 17:18:06 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:56:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:56:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 07:10:22 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 07:10:25 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 07:10:27 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 07:18:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 07:18:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 07:18:17 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 07:18:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 07:18:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 07:18:37 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 16:54:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 16:54:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 16:54:59 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 16:58:51 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 16:59:11 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 16:59:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 16:59:16 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 16:59:19 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 16:59:23 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 16:59:26 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 16:59:31 GMT
USER fluent
# Sun, 02 Feb 2020 16:59:34 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 16:59:37 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:16a7e1c5b23ec3cf93421f5f868c1cf2cda468cfebb1b2bc62f4d533d99d256b`  
		Last Modified: Sat, 01 Feb 2020 17:26:05 GMT  
		Size: 30.5 MB (30517693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d44bc1840f426f48fc6d4cc23113f86c02e7f46ef4c400ce5b4c76010c72a2`  
		Last Modified: Sun, 02 Feb 2020 08:19:33 GMT  
		Size: 12.7 MB (12688850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e418c294c298ad8987cb27fc2adff7ce43dee0e55af3c86e59af9271e4c490`  
		Last Modified: Sun, 02 Feb 2020 08:19:29 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ed4fdb4090425730dd3e443c0fd27af2b2cff3415260f22a0056d8ff639b99`  
		Last Modified: Sun, 02 Feb 2020 08:20:20 GMT  
		Size: 22.0 MB (21968679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3472d9aadeeb03ff16dda03cf908dc2438dfbe262d09c2f3fe38ba8a9a8a9a8`  
		Last Modified: Sun, 02 Feb 2020 08:20:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f6ea37b6222ce5baa419db61c379c349818d5d08d103a15fbc9955c8167e62`  
		Last Modified: Sun, 02 Feb 2020 17:00:02 GMT  
		Size: 25.0 MB (25049107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd0768d534b7c90cd7d57da4b3f7463e0b18fa3e373b2f0d79303e131116b38`  
		Last Modified: Sun, 02 Feb 2020 16:59:56 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f9362111330afcb05168897cacc5d890dfeee23984212d6b8ed657a2dbca28`  
		Last Modified: Sun, 02 Feb 2020 16:59:56 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592335602dbd25ea7322c3707e5ba35f9ca1bf5be746a180c9bf32ab93c4e100`  
		Last Modified: Sun, 02 Feb 2020 16:59:56 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:d03b0bf781c2274e8de992cb2935ca0ee4e754260f5e7b27d2accee2cc3c346c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.7 MB (82749146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:432486d4d4b647921e2bc8317f30ef256e1201c66845b002a1c62d06d3a68512`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:24:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_MAJOR=2.6
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 01 Feb 2020 22:36:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 01 Feb 2020 22:36:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:36:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 01 Feb 2020 22:36:07 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 03:37:02 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sun, 02 Feb 2020 03:37:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Sun, 02 Feb 2020 03:37:02 GMT
ENV TINI_VERSION=0.18.0
# Sun, 02 Feb 2020 03:38:21 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Sun, 02 Feb 2020 03:38:23 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sun, 02 Feb 2020 03:38:24 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sun, 02 Feb 2020 03:38:24 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Sun, 02 Feb 2020 03:38:24 GMT
ENV FLUENTD_CONF=fluent.conf
# Sun, 02 Feb 2020 03:38:24 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sun, 02 Feb 2020 03:38:24 GMT
EXPOSE 24224 5140
# Sun, 02 Feb 2020 03:38:24 GMT
USER fluent
# Sun, 02 Feb 2020 03:38:25 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sun, 02 Feb 2020 03:38:25 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17d8d1356b8293f168a2578ba81c34f07ee79d7a56bd579e776ad498d0b2e8`  
		Last Modified: Sat, 01 Feb 2020 22:56:51 GMT  
		Size: 10.8 MB (10795999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d180073499f34bb9340ecac840eeb00fab127188f731188ba78e76e435b62c`  
		Last Modified: Sat, 01 Feb 2020 22:56:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351f50ba1593f8ab66d1deaf12e190c35ecfea96815beda37efe10f1246f342b`  
		Last Modified: Sat, 01 Feb 2020 22:57:18 GMT  
		Size: 21.6 MB (21592569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8a5d1fd225888733445fbc5a03464b232ab7c659a3bf619e93c5670a0ca594`  
		Last Modified: Sat, 01 Feb 2020 22:57:14 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c81d9fd7daa9ad2dc6a948e05bb47fec6e87ddd58b48e6aaa9c2f8b8f4f59e`  
		Last Modified: Sun, 02 Feb 2020 03:38:40 GMT  
		Size: 24.7 MB (24652127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae4932f4e7f17509dd1c3aed04301daf0bc843b7e3fe8c5e5ad957e3c7850b3`  
		Last Modified: Sun, 02 Feb 2020 03:38:42 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e18c5cd131a8accf4498060f449e239093b9b52c2696449733ffaaf023ae19f`  
		Last Modified: Sun, 02 Feb 2020 03:38:37 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd85d0826acc444b2e46d021d2352fb54757b9ea410c2baec476ef2078eed7a`  
		Last Modified: Sun, 02 Feb 2020 03:38:42 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
