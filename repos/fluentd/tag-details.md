<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.8-1`](#fluentdv18-1)
-	[`fluentd:v1.8.1-1.0`](#fluentdv181-10)
-	[`fluentd:v1.8.1-debian-1.0`](#fluentdv181-debian-10)
-	[`fluentd:v1.8-debian-1`](#fluentdv18-debian-1)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:3fff5265207b8cd790c1e8733ea508cd98233e040c8eb3e6aef0e323c7ad60f0
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
$ docker pull fluentd@sha256:1020de1880a1e3cdcd9751441acf92039390f924eb40619f89951bbd8b389ec6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16878568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae89db7897cdef8cf033f76dc4f780e299e5db0154dda91673b0596680fcfbac`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 11 May 2019 00:07:03 GMT
ADD file:a86aea1f3a7d68f6ae03397b99ea77f2e9ee901c5c59e59f76f93adbb4035913 in / 
# Sat, 11 May 2019 00:07:03 GMT
CMD ["/bin/sh"]
# Sat, 11 May 2019 00:24:36 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 21:21:34 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 21:22:09 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:22:10 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:22:10 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:22:10 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:22:10 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:22:11 GMT
ENV LD_PRELOAD=
# Wed, 15 Jan 2020 21:22:11 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:22:11 GMT
USER fluent
# Wed, 15 Jan 2020 21:22:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:22:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:e7c96db7181be991f19a9fb6975cdbbd73c65f4a2681348e63a141a2192a5f10`  
		Last Modified: Sat, 11 May 2019 00:07:31 GMT  
		Size: 2.8 MB (2757034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab1ec9335521ed77e09126d175b5c275712b4dba3fb6bc0627b3dafd00acc7`  
		Last Modified: Wed, 15 Jan 2020 21:24:09 GMT  
		Size: 14.1 MB (14119367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dbf5c4400f2b2cde4878179a5668f795e16b52d9f49fdf9a8db037ee2647c5`  
		Last Modified: Wed, 15 Jan 2020 21:24:06 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0b82f9911874434f7b73de84542fd5ab1fccae134ba53e7572e1261124b8c6`  
		Last Modified: Wed, 15 Jan 2020 21:24:06 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12d780b5526a5baf9c5ab5dc3f52e4c94fe2627013b86f16bc2c1e40add8b7b`  
		Last Modified: Wed, 15 Jan 2020 21:24:07 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:c9c94597258293d3d07ee071d0ab71e4624ac94b29856c82a21fd312bbb1776a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15650611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df31a2dfb76f44532a341888f455032e6b0e7596790af2b42db86fdf2ea0d31`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 11 May 2019 07:49:31 GMT
ADD file:202469fe868f49927884e8dd109fb8bb596ab6e435dc1bfc9f75f03e50e82325 in / 
# Sat, 11 May 2019 07:49:31 GMT
CMD ["/bin/sh"]
# Sat, 11 May 2019 09:12:16 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 Jul 2019 17:49:26 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.6.2
# Tue, 23 Jul 2019 17:50:47 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.3.10  && gem install json -v 2.2.0  && gem install async-http -v 0.46.3  && gem install fluentd -v 1.6.2  && gem install bigdecimal -v 1.3.5  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Tue, 23 Jul 2019 17:50:49 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 Jul 2019 17:50:50 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 Jul 2019 17:50:50 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Tue, 23 Jul 2019 17:50:51 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 Jul 2019 17:50:51 GMT
ENV LD_PRELOAD=
# Tue, 23 Jul 2019 17:50:52 GMT
EXPOSE 24224 5140
# Tue, 23 Jul 2019 17:50:52 GMT
USER fluent
# Tue, 23 Jul 2019 17:50:52 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 Jul 2019 17:50:53 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6e39823df636e42cc4ea056843af98c9bec31b5ae0a75cdc5628cd19b589189c`  
		Last Modified: Sat, 11 May 2019 07:50:08 GMT  
		Size: 2.5 MB (2543427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5988b39e4cd58fe4589f896746b6b9c920e1cc38143c392d88848c8dfbe0f926`  
		Last Modified: Tue, 23 Jul 2019 17:51:20 GMT  
		Size: 13.1 MB (13104967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc73eaf0b7e8a98f5a419380b1433058d9ad29c45d3c80109752af1cd804ed0`  
		Last Modified: Tue, 23 Jul 2019 17:51:15 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e02b6566e1011adaf5c3463ddb555bb75b10c2cb61f2ef2c9fd2c2f856e73c`  
		Last Modified: Tue, 23 Jul 2019 17:51:15 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77877b107aec3baad54040757107545d0a529fb0294245c8b98eba8608538261`  
		Last Modified: Tue, 23 Jul 2019 17:51:15 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:49a3624add40e34757519008f392cf6a32c142be73c08b936c5ee6702f6d4884
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16134428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ec7fa1f9950e7b290b1fb126751ba8a3e86e62f199d3fdcf4264be6c9192021`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 19 Jun 2019 20:39:47 GMT
ADD file:66f49017dd7ba295602526dbf210046e47fd097298c17a3f268a47487b5b6379 in / 
# Wed, 19 Jun 2019 20:39:47 GMT
CMD ["/bin/sh"]
# Wed, 19 Jun 2019 22:09:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 Jul 2019 18:31:42 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.6.2
# Tue, 23 Jul 2019 18:32:46 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.3.10  && gem install json -v 2.2.0  && gem install async-http -v 0.46.3  && gem install fluentd -v 1.6.2  && gem install bigdecimal -v 1.3.5  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Tue, 23 Jul 2019 18:32:48 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 Jul 2019 18:32:48 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 Jul 2019 18:32:49 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Tue, 23 Jul 2019 18:32:49 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 Jul 2019 18:32:49 GMT
ENV LD_PRELOAD=
# Tue, 23 Jul 2019 18:32:50 GMT
EXPOSE 24224 5140
# Tue, 23 Jul 2019 18:32:50 GMT
USER fluent
# Tue, 23 Jul 2019 18:32:50 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 Jul 2019 18:32:51 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:0362ad1dd800a9d92f8982fa28f173f9120266153830f990f7486f44b068968a`  
		Last Modified: Sat, 11 May 2019 08:44:25 GMT  
		Size: 2.7 MB (2688779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04dbe467249b909d448fd5ee00e2422d11bc196a4db7d6810b086140c22673f0`  
		Last Modified: Tue, 23 Jul 2019 18:35:55 GMT  
		Size: 13.4 MB (13443430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f4d6ddcbab0d7ae03c8d3720651029f14c559a8b4278b35a5e87db6a93b00e`  
		Last Modified: Tue, 23 Jul 2019 18:35:49 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d419eeeef5d99c6635d32858f71e1858a2057ff52e928961ce44114b5e1aca63`  
		Last Modified: Tue, 23 Jul 2019 18:35:49 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dabf0983f1ca1e6a6d1c14181ccb664287ae8b7f29fca4bbba078fd305b1db5`  
		Last Modified: Tue, 23 Jul 2019 18:35:49 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; 386

```console
$ docker pull fluentd@sha256:11025deae69bcd73054a9fd073f283f73192aa8cd64ab97ccee1eebf4dc3ac74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16101902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dee0c0a59069cbc3cab5f66d35669c2a1f64663b43b4e3e1fb2210d3b71a905b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 11 May 2019 10:39:25 GMT
ADD file:6bcacb93c2814cb9c833dfb82a5ef000ef21e6864d9f0b20a7a68b6e16801700 in / 
# Sat, 11 May 2019 10:39:25 GMT
CMD ["/bin/sh"]
# Sat, 11 May 2019 11:06:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 Jul 2019 18:44:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.6.2
# Tue, 23 Jul 2019 18:44:51 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.3.10  && gem install json -v 2.2.0  && gem install async-http -v 0.46.3  && gem install fluentd -v 1.6.2  && gem install bigdecimal -v 1.3.5  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Tue, 23 Jul 2019 18:44:52 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 Jul 2019 18:44:53 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 Jul 2019 18:44:53 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Tue, 23 Jul 2019 18:44:53 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 Jul 2019 18:44:53 GMT
ENV LD_PRELOAD=
# Tue, 23 Jul 2019 18:44:53 GMT
EXPOSE 24224 5140
# Tue, 23 Jul 2019 18:44:53 GMT
USER fluent
# Tue, 23 Jul 2019 18:44:54 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 Jul 2019 18:44:54 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:d0c434c0359e2da36b788ae4f5a3a70015d83ee20070aa412e714c7feecca465`  
		Last Modified: Sat, 11 May 2019 10:39:46 GMT  
		Size: 2.8 MB (2752091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5574c0413876c751040a7e2c0b5c7e742a1e14f504d082f8fc6be260e7b59`  
		Last Modified: Tue, 23 Jul 2019 18:47:09 GMT  
		Size: 13.3 MB (13347647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69a652f2cc6e74098c31f2a49290e4ca8279a5344a1c8c15c48ac585d256768`  
		Last Modified: Tue, 23 Jul 2019 18:47:05 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339eae27ca3420ea34af0f776c8ce6ea9d4ce59d3914e5fc2885fc8211cc1ba3`  
		Last Modified: Tue, 23 Jul 2019 18:47:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d0660c4fac158193e2e499dd2281b051a172f86ec48a0f753b77a32506d6c`  
		Last Modified: Tue, 23 Jul 2019 18:47:05 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:d83cee41e43cf6eaaa5981dbd6dd244ac965afc9d4b95bc2d4704f6004f5f054
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17322057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a9a2a410cee08e3a77ab24a666d8073d57807d28b6b3c030bef34b8816d9da`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 19 Jun 2019 21:20:35 GMT
ADD file:109b3a992e029fdd5c3d6b378474c32a2c36cc5e549c83c3df3330dbc4eb7dd7 in / 
# Wed, 19 Jun 2019 21:20:36 GMT
CMD ["/bin/sh"]
# Wed, 19 Jun 2019 23:01:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 21:16:26 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 21:17:30 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:17:40 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:17:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:17:42 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:17:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:17:47 GMT
ENV LD_PRELOAD=
# Wed, 15 Jan 2020 21:17:49 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:17:53 GMT
USER fluent
# Wed, 15 Jan 2020 21:17:55 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:17:59 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:221c32b360a801e69a8aac598d495aaac3512642f967704a9d9bc5d6b4b4709e`  
		Last Modified: Sat, 11 May 2019 08:30:16 GMT  
		Size: 2.8 MB (2781019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e653d12daea2c002f332dee73502493d035407bf5d0fb0a5f237288eb6b714`  
		Last Modified: Wed, 15 Jan 2020 21:22:27 GMT  
		Size: 14.5 MB (14538816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5de5ed627b4d3193b9a341ae26788a9e6234943b4c73066461d90105f16f5ab`  
		Last Modified: Wed, 15 Jan 2020 21:22:23 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2726dcf4b2f9ab99e2303037d16cf5771c55a4c4006543370e59e33841cfb6`  
		Last Modified: Wed, 15 Jan 2020 21:22:23 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9acb98bfdb75a368a3911f868f3c9728b8bdc2d8b33f84bba2c73d5772567d`  
		Last Modified: Wed, 15 Jan 2020 21:22:23 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:f19f4e55bc5f9e7ae6904c796dad563e9bcd3918e66678ceafe58ab5d15b0066
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16118731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71aeb940543ea3d7e8b4bbbe2674184a2b552fc6cf847dc2b681ab068f84f1d6`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 11 May 2019 11:41:43 GMT
ADD file:6b519ed40566a3088c7bf57b3f1624dadc83f9e56839d5cde42489b54a0a1e90 in / 
# Sat, 11 May 2019 11:41:43 GMT
CMD ["/bin/sh"]
# Sat, 11 May 2019 12:02:14 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 23 Jul 2019 19:29:11 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.6.2
# Tue, 23 Jul 2019 19:29:45 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.3.10  && gem install json -v 2.2.0  && gem install async-http -v 0.46.3  && gem install fluentd -v 1.6.2  && gem install bigdecimal -v 1.3.5  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Tue, 23 Jul 2019 19:29:46 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 23 Jul 2019 19:29:47 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 23 Jul 2019 19:29:47 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Tue, 23 Jul 2019 19:29:47 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 23 Jul 2019 19:29:47 GMT
ENV LD_PRELOAD=
# Tue, 23 Jul 2019 19:29:48 GMT
EXPOSE 24224 5140
# Tue, 23 Jul 2019 19:29:48 GMT
USER fluent
# Tue, 23 Jul 2019 19:29:48 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 23 Jul 2019 19:29:48 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:bea4f04d8b33c5bd68ccb34849e615333c5ef00958b400841a03970dd2d5e9ae`  
		Last Modified: Sat, 11 May 2019 11:42:13 GMT  
		Size: 2.5 MB (2543331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d1e3d04ec5c6271be20447282836b8eea877f981596d9020a928b4d1708385`  
		Last Modified: Tue, 23 Jul 2019 19:31:50 GMT  
		Size: 13.6 MB (13573234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8f7af0bce382bfeeaf7340e542259aafa6d0186b1e3b4866e236a473b8d2bc`  
		Last Modified: Tue, 23 Jul 2019 19:31:47 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1642c42523c7e4eded026fbd980583efd7b822d5c05dda3e3fc3abdb031c201`  
		Last Modified: Tue, 23 Jul 2019 19:31:47 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8fd9119c25453c1fa1f776e3873bf14b48de4d0222d54fd147f99e0b9772fb`  
		Last Modified: Tue, 23 Jul 2019 19:31:47 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.8-1`

```console
$ docker pull fluentd@sha256:c57f5fe46f7cae8648885e58014ceb10390a530ecb3726be2753381db7d851e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le

### `fluentd:v1.8-1` - linux; amd64

```console
$ docker pull fluentd@sha256:1020de1880a1e3cdcd9751441acf92039390f924eb40619f89951bbd8b389ec6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16878568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae89db7897cdef8cf033f76dc4f780e299e5db0154dda91673b0596680fcfbac`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 11 May 2019 00:07:03 GMT
ADD file:a86aea1f3a7d68f6ae03397b99ea77f2e9ee901c5c59e59f76f93adbb4035913 in / 
# Sat, 11 May 2019 00:07:03 GMT
CMD ["/bin/sh"]
# Sat, 11 May 2019 00:24:36 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 21:21:34 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 21:22:09 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:22:10 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:22:10 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:22:10 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:22:10 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:22:11 GMT
ENV LD_PRELOAD=
# Wed, 15 Jan 2020 21:22:11 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:22:11 GMT
USER fluent
# Wed, 15 Jan 2020 21:22:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:22:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:e7c96db7181be991f19a9fb6975cdbbd73c65f4a2681348e63a141a2192a5f10`  
		Last Modified: Sat, 11 May 2019 00:07:31 GMT  
		Size: 2.8 MB (2757034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab1ec9335521ed77e09126d175b5c275712b4dba3fb6bc0627b3dafd00acc7`  
		Last Modified: Wed, 15 Jan 2020 21:24:09 GMT  
		Size: 14.1 MB (14119367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dbf5c4400f2b2cde4878179a5668f795e16b52d9f49fdf9a8db037ee2647c5`  
		Last Modified: Wed, 15 Jan 2020 21:24:06 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0b82f9911874434f7b73de84542fd5ab1fccae134ba53e7572e1261124b8c6`  
		Last Modified: Wed, 15 Jan 2020 21:24:06 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12d780b5526a5baf9c5ab5dc3f52e4c94fe2627013b86f16bc2c1e40add8b7b`  
		Last Modified: Wed, 15 Jan 2020 21:24:07 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:d83cee41e43cf6eaaa5981dbd6dd244ac965afc9d4b95bc2d4704f6004f5f054
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17322057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a9a2a410cee08e3a77ab24a666d8073d57807d28b6b3c030bef34b8816d9da`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 19 Jun 2019 21:20:35 GMT
ADD file:109b3a992e029fdd5c3d6b378474c32a2c36cc5e549c83c3df3330dbc4eb7dd7 in / 
# Wed, 19 Jun 2019 21:20:36 GMT
CMD ["/bin/sh"]
# Wed, 19 Jun 2019 23:01:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 21:16:26 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 21:17:30 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:17:40 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:17:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:17:42 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:17:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:17:47 GMT
ENV LD_PRELOAD=
# Wed, 15 Jan 2020 21:17:49 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:17:53 GMT
USER fluent
# Wed, 15 Jan 2020 21:17:55 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:17:59 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:221c32b360a801e69a8aac598d495aaac3512642f967704a9d9bc5d6b4b4709e`  
		Last Modified: Sat, 11 May 2019 08:30:16 GMT  
		Size: 2.8 MB (2781019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e653d12daea2c002f332dee73502493d035407bf5d0fb0a5f237288eb6b714`  
		Last Modified: Wed, 15 Jan 2020 21:22:27 GMT  
		Size: 14.5 MB (14538816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5de5ed627b4d3193b9a341ae26788a9e6234943b4c73066461d90105f16f5ab`  
		Last Modified: Wed, 15 Jan 2020 21:22:23 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2726dcf4b2f9ab99e2303037d16cf5771c55a4c4006543370e59e33841cfb6`  
		Last Modified: Wed, 15 Jan 2020 21:22:23 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9acb98bfdb75a368a3911f868f3c9728b8bdc2d8b33f84bba2c73d5772567d`  
		Last Modified: Wed, 15 Jan 2020 21:22:23 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.8.1-1.0`

```console
$ docker pull fluentd@sha256:c57f5fe46f7cae8648885e58014ceb10390a530ecb3726be2753381db7d851e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le

### `fluentd:v1.8.1-1.0` - linux; amd64

```console
$ docker pull fluentd@sha256:1020de1880a1e3cdcd9751441acf92039390f924eb40619f89951bbd8b389ec6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16878568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae89db7897cdef8cf033f76dc4f780e299e5db0154dda91673b0596680fcfbac`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 11 May 2019 00:07:03 GMT
ADD file:a86aea1f3a7d68f6ae03397b99ea77f2e9ee901c5c59e59f76f93adbb4035913 in / 
# Sat, 11 May 2019 00:07:03 GMT
CMD ["/bin/sh"]
# Sat, 11 May 2019 00:24:36 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 21:21:34 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 21:22:09 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:22:10 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:22:10 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:22:10 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:22:10 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:22:11 GMT
ENV LD_PRELOAD=
# Wed, 15 Jan 2020 21:22:11 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:22:11 GMT
USER fluent
# Wed, 15 Jan 2020 21:22:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:22:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:e7c96db7181be991f19a9fb6975cdbbd73c65f4a2681348e63a141a2192a5f10`  
		Last Modified: Sat, 11 May 2019 00:07:31 GMT  
		Size: 2.8 MB (2757034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab1ec9335521ed77e09126d175b5c275712b4dba3fb6bc0627b3dafd00acc7`  
		Last Modified: Wed, 15 Jan 2020 21:24:09 GMT  
		Size: 14.1 MB (14119367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dbf5c4400f2b2cde4878179a5668f795e16b52d9f49fdf9a8db037ee2647c5`  
		Last Modified: Wed, 15 Jan 2020 21:24:06 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0b82f9911874434f7b73de84542fd5ab1fccae134ba53e7572e1261124b8c6`  
		Last Modified: Wed, 15 Jan 2020 21:24:06 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12d780b5526a5baf9c5ab5dc3f52e4c94fe2627013b86f16bc2c1e40add8b7b`  
		Last Modified: Wed, 15 Jan 2020 21:24:07 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:d83cee41e43cf6eaaa5981dbd6dd244ac965afc9d4b95bc2d4704f6004f5f054
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17322057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a9a2a410cee08e3a77ab24a666d8073d57807d28b6b3c030bef34b8816d9da`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 19 Jun 2019 21:20:35 GMT
ADD file:109b3a992e029fdd5c3d6b378474c32a2c36cc5e549c83c3df3330dbc4eb7dd7 in / 
# Wed, 19 Jun 2019 21:20:36 GMT
CMD ["/bin/sh"]
# Wed, 19 Jun 2019 23:01:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 21:16:26 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 21:17:30 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:17:40 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:17:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:17:42 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:17:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:17:47 GMT
ENV LD_PRELOAD=
# Wed, 15 Jan 2020 21:17:49 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:17:53 GMT
USER fluent
# Wed, 15 Jan 2020 21:17:55 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:17:59 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:221c32b360a801e69a8aac598d495aaac3512642f967704a9d9bc5d6b4b4709e`  
		Last Modified: Sat, 11 May 2019 08:30:16 GMT  
		Size: 2.8 MB (2781019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e653d12daea2c002f332dee73502493d035407bf5d0fb0a5f237288eb6b714`  
		Last Modified: Wed, 15 Jan 2020 21:22:27 GMT  
		Size: 14.5 MB (14538816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5de5ed627b4d3193b9a341ae26788a9e6234943b4c73066461d90105f16f5ab`  
		Last Modified: Wed, 15 Jan 2020 21:22:23 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2726dcf4b2f9ab99e2303037d16cf5771c55a4c4006543370e59e33841cfb6`  
		Last Modified: Wed, 15 Jan 2020 21:22:23 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9acb98bfdb75a368a3911f868f3c9728b8bdc2d8b33f84bba2c73d5772567d`  
		Last Modified: Wed, 15 Jan 2020 21:22:23 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.8.1-debian-1.0`

```console
$ docker pull fluentd@sha256:7807bfc5486a75e27d042ca0403e039ece3a8bf3a55acedcad497c02ff983b00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; ppc64le

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

### `fluentd:v1.8.1-debian-1.0` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:30cadcfa0fe3291c75291086cd1b3c7ead35512bb85094625496b50d23a9c68d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.7 MB (76713314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcc42a8c1ec9e5c5b4d5346be99e202dfd9fa1561dc9230d61fb452dc18dc598`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 21:07:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 21:07:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 21:19:31 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 21:22:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 21:22:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 03:12:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 03:12:51 GMT
CMD ["irb"]
# Wed, 15 Jan 2020 20:57:36 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 20:57:36 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 20:57:37 GMT
ENV TINI_VERSION=0.18.0
# Wed, 15 Jan 2020 21:00:18 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:00:21 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:00:21 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:00:22 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:00:22 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:00:23 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 15 Jan 2020 21:00:23 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:00:24 GMT
USER fluent
# Wed, 15 Jan 2020 21:00:24 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:00:25 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73268a651977563b4fdcb5f5dfd7b8f7b4b65290a1568813853d244ebf46cca`  
		Last Modified: Sat, 28 Dec 2019 22:12:53 GMT  
		Size: 9.8 MB (9847375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf46deaa8f015b62913dcf008d3f023ffdd9757f740be11a46eb091bf40916a`  
		Last Modified: Sat, 28 Dec 2019 22:12:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4c32e3c622deadf3234025d30c88895c18ae7eac94288d4e42f903c4a72f5`  
		Last Modified: Sat, 28 Dec 2019 22:13:25 GMT  
		Size: 20.6 MB (20620161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe49bcffa8c82983470bbf0074d2412dacbf1f325bcc2ffb85fddcbda7c7da8`  
		Last Modified: Tue, 07 Jan 2020 03:17:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c557e58636d2dc8da1de17b29fd4ab24a164d74d73f39b73e57760414d24559a`  
		Last Modified: Wed, 15 Jan 2020 21:00:48 GMT  
		Size: 23.5 MB (23543586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453119a7086350da0f01d6eb7f2b001cc4bbbf3f552b04ca04f6e726afa8600d`  
		Last Modified: Wed, 15 Jan 2020 21:00:42 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70366686ee131c898edcab0ddce0e99949306880b0b2052e40b316e660cb5ea9`  
		Last Modified: Wed, 15 Jan 2020 21:00:42 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20817e4a4e42c52040518ec103a55f6e7ae681d25c7cc41256fd49ee20adc557`  
		Last Modified: Wed, 15 Jan 2020 21:00:42 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8.1-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:84f2f9054ec7c6b15dc496878c376e87c0d48d9a688befe693d9558f9becda3e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90225863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:178d429e9d697fa293043720bd974fd4233e4e94fef137169f89b6ee8b27c74b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:37:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:37:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 04:44:05 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 04:44:07 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 04:44:10 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 04:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 04:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:18:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:18:58 GMT
CMD ["irb"]
# Wed, 15 Jan 2020 21:18:06 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 21:18:11 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 21:18:14 GMT
ENV TINI_VERSION=0.18.0
# Wed, 15 Jan 2020 21:21:42 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:21:51 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:21:53 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:21:55 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:21:57 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:21:59 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 15 Jan 2020 21:22:01 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:22:04 GMT
USER fluent
# Wed, 15 Jan 2020 21:22:06 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:22:08 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e10577c89c450ecfcb6cd75777c15ce8a9c0118a86cd89b181c32ae50e530`  
		Last Modified: Sat, 28 Dec 2019 05:29:25 GMT  
		Size: 12.7 MB (12688889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20f2864ed98b31f7d1955c54fb2f0f3eaabae93374f8c0f8bc6f6e4d871b33c`  
		Last Modified: Sat, 28 Dec 2019 05:29:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd8219d68aec763d8d91942869b8dd9ef7233da0ba814028c00dce26b61b1ec`  
		Last Modified: Sat, 28 Dec 2019 05:29:59 GMT  
		Size: 22.0 MB (21968340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88418e7313544081130ec82f1125b007f6673672ed6fe3f2815a8bc0836d834d`  
		Last Modified: Tue, 07 Jan 2020 02:27:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c87f0054344351d607d46ab19aaf94ff4db80a5658ad543624875d8fe99d13`  
		Last Modified: Wed, 15 Jan 2020 21:22:44 GMT  
		Size: 25.0 MB (25048020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2695d831095af6674cce487ec88c4a688f4697c5b29cc2911e97002077f816d`  
		Last Modified: Wed, 15 Jan 2020 21:22:39 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7b9b68f8fdc3fc3948b08ba4a3a7c5b4ae2a00dc1709295360a976c9e2e37b`  
		Last Modified: Wed, 15 Jan 2020 21:22:39 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80d35cb39e04eed7b41e1615b4b9da4cdd90da1d404cffabd4caee8d8ca105d`  
		Last Modified: Wed, 15 Jan 2020 21:22:39 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.8-debian-1`

```console
$ docker pull fluentd@sha256:7807bfc5486a75e27d042ca0403e039ece3a8bf3a55acedcad497c02ff983b00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; ppc64le

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

### `fluentd:v1.8-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:30cadcfa0fe3291c75291086cd1b3c7ead35512bb85094625496b50d23a9c68d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.7 MB (76713314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcc42a8c1ec9e5c5b4d5346be99e202dfd9fa1561dc9230d61fb452dc18dc598`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 21:07:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 21:07:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 21:19:31 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 21:22:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 21:22:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 03:12:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 03:12:51 GMT
CMD ["irb"]
# Wed, 15 Jan 2020 20:57:36 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 20:57:36 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 20:57:37 GMT
ENV TINI_VERSION=0.18.0
# Wed, 15 Jan 2020 21:00:18 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:00:21 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:00:21 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:00:22 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:00:22 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:00:23 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 15 Jan 2020 21:00:23 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:00:24 GMT
USER fluent
# Wed, 15 Jan 2020 21:00:24 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:00:25 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73268a651977563b4fdcb5f5dfd7b8f7b4b65290a1568813853d244ebf46cca`  
		Last Modified: Sat, 28 Dec 2019 22:12:53 GMT  
		Size: 9.8 MB (9847375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf46deaa8f015b62913dcf008d3f023ffdd9757f740be11a46eb091bf40916a`  
		Last Modified: Sat, 28 Dec 2019 22:12:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4c32e3c622deadf3234025d30c88895c18ae7eac94288d4e42f903c4a72f5`  
		Last Modified: Sat, 28 Dec 2019 22:13:25 GMT  
		Size: 20.6 MB (20620161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe49bcffa8c82983470bbf0074d2412dacbf1f325bcc2ffb85fddcbda7c7da8`  
		Last Modified: Tue, 07 Jan 2020 03:17:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c557e58636d2dc8da1de17b29fd4ab24a164d74d73f39b73e57760414d24559a`  
		Last Modified: Wed, 15 Jan 2020 21:00:48 GMT  
		Size: 23.5 MB (23543586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453119a7086350da0f01d6eb7f2b001cc4bbbf3f552b04ca04f6e726afa8600d`  
		Last Modified: Wed, 15 Jan 2020 21:00:42 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70366686ee131c898edcab0ddce0e99949306880b0b2052e40b316e660cb5ea9`  
		Last Modified: Wed, 15 Jan 2020 21:00:42 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20817e4a4e42c52040518ec103a55f6e7ae681d25c7cc41256fd49ee20adc557`  
		Last Modified: Wed, 15 Jan 2020 21:00:42 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.8-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:84f2f9054ec7c6b15dc496878c376e87c0d48d9a688befe693d9558f9becda3e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90225863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:178d429e9d697fa293043720bd974fd4233e4e94fef137169f89b6ee8b27c74b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:37:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:37:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 04:44:05 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 04:44:07 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 04:44:10 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 04:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 04:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:18:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:18:58 GMT
CMD ["irb"]
# Wed, 15 Jan 2020 21:18:06 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 15 Jan 2020 21:18:11 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.8.1
# Wed, 15 Jan 2020 21:18:14 GMT
ENV TINI_VERSION=0.18.0
# Wed, 15 Jan 2020 21:21:42 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.8.1  && gem install json -v 2.2.0  && gem install async-http -v 0.49.1  && gem install fluentd -v 1.8.1  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
# Wed, 15 Jan 2020 21:21:51 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 15 Jan 2020 21:21:53 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 15 Jan 2020 21:21:55 GMT
COPY file:f70a6a04a7c32c744ebb989e7d706ca5f78829c1489be8d165d4b1b682c9eaf8 in /bin/ 
# Wed, 15 Jan 2020 21:21:57 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 15 Jan 2020 21:21:59 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 15 Jan 2020 21:22:01 GMT
EXPOSE 24224 5140
# Wed, 15 Jan 2020 21:22:04 GMT
USER fluent
# Wed, 15 Jan 2020 21:22:06 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 15 Jan 2020 21:22:08 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e10577c89c450ecfcb6cd75777c15ce8a9c0118a86cd89b181c32ae50e530`  
		Last Modified: Sat, 28 Dec 2019 05:29:25 GMT  
		Size: 12.7 MB (12688889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20f2864ed98b31f7d1955c54fb2f0f3eaabae93374f8c0f8bc6f6e4d871b33c`  
		Last Modified: Sat, 28 Dec 2019 05:29:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd8219d68aec763d8d91942869b8dd9ef7233da0ba814028c00dce26b61b1ec`  
		Last Modified: Sat, 28 Dec 2019 05:29:59 GMT  
		Size: 22.0 MB (21968340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88418e7313544081130ec82f1125b007f6673672ed6fe3f2815a8bc0836d834d`  
		Last Modified: Tue, 07 Jan 2020 02:27:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c87f0054344351d607d46ab19aaf94ff4db80a5658ad543624875d8fe99d13`  
		Last Modified: Wed, 15 Jan 2020 21:22:44 GMT  
		Size: 25.0 MB (25048020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2695d831095af6674cce487ec88c4a688f4697c5b29cc2911e97002077f816d`  
		Last Modified: Wed, 15 Jan 2020 21:22:39 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7b9b68f8fdc3fc3948b08ba4a3a7c5b4ae2a00dc1709295360a976c9e2e37b`  
		Last Modified: Wed, 15 Jan 2020 21:22:39 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80d35cb39e04eed7b41e1615b4b9da4cdd90da1d404cffabd4caee8d8ca105d`  
		Last Modified: Wed, 15 Jan 2020 21:22:39 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
