<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.14-1`](#fluentdv114-1)
-	[`fluentd:v1.14-debian-1`](#fluentdv114-debian-1)
-	[`fluentd:v1.14.0-1.0`](#fluentdv1140-10)
-	[`fluentd:v1.14.0-debian-1.0`](#fluentdv1140-debian-10)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:750f2da8e32b81833482a1ee8b8432678b0bd1d9e7a4380691b500e9c2dc46bd
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
$ docker pull fluentd@sha256:e50d2feff22570321cb513275f0ecb0610ff28fd04eb34fb0ba67b2c33025962
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19094524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b1c11fc4d5d2d98146f392efff53ded472fea834ad159104bd57d957aa2ea7f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:15:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 12 Nov 2021 22:15:04 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 12 Nov 2021 22:15:52 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 12 Nov 2021 22:15:53 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 12 Nov 2021 22:15:53 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 12 Nov 2021 22:15:53 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 12 Nov 2021 22:15:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 12 Nov 2021 22:15:54 GMT
ENV LD_PRELOAD=
# Fri, 12 Nov 2021 22:15:54 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 12 Nov 2021 22:15:54 GMT
EXPOSE 24224 5140
# Fri, 12 Nov 2021 22:15:54 GMT
USER fluent
# Fri, 12 Nov 2021 22:15:55 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 12 Nov 2021 22:15:55 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13204de4fb4b7965326c9d3d4a9e1d4c8f0eaf13259bf2a230215874aa01a92`  
		Last Modified: Fri, 12 Nov 2021 22:16:15 GMT  
		Size: 16.3 MB (16269891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b94277aa813c2d531beef97fb86f701863b0219e55a63f009a3b361518c5be`  
		Last Modified: Fri, 12 Nov 2021 22:16:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac90a2c4fa5786d073fc79443f891af792328a19a36605fac7371c354b567c2f`  
		Last Modified: Fri, 12 Nov 2021 22:16:13 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18385d5d22f344b404fb5d55a84dfa60dc01850637c88bea8f126009e0bebd6d`  
		Last Modified: Fri, 12 Nov 2021 22:16:13 GMT  
		Size: 461.0 B  
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
$ docker pull fluentd@sha256:513e632f2ba2f7fa53b0885e8107eeaf5b3f6bbc6edadda1a90d638b4fda34ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18932970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6612d0dd8244452c42bdd6d5f00372e1e9ac237f09babce368fca01c2d37d192`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 08:49:20 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Nov 2021 08:49:21 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 13 Nov 2021 08:50:16 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 13 Nov 2021 08:50:17 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Nov 2021 08:50:19 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Nov 2021 08:50:20 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 13 Nov 2021 08:50:20 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Nov 2021 08:50:21 GMT
ENV LD_PRELOAD=
# Sat, 13 Nov 2021 08:50:22 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 13 Nov 2021 08:50:23 GMT
EXPOSE 24224 5140
# Sat, 13 Nov 2021 08:50:24 GMT
USER fluent
# Sat, 13 Nov 2021 08:50:25 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Nov 2021 08:50:26 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b49e73e0bcd14e81224b4723baf1b707943dbf94afaf5993d1880540d376ec`  
		Last Modified: Sat, 13 Nov 2021 08:50:53 GMT  
		Size: 16.2 MB (16211176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11039029abdf325434cd897fff317b820840ef51e6cf8eeb6e7b30d53f2af814`  
		Last Modified: Sat, 13 Nov 2021 08:50:50 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae1d5a5c57cb7203d403c10cb5f210ab184f5b1f81a1a9fba0434302926681`  
		Last Modified: Sat, 13 Nov 2021 08:50:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1a8aba720763a9d4bdc150b480e664cc2d14b7f978e331b07673a6a32710c1`  
		Last Modified: Sat, 13 Nov 2021 08:50:50 GMT  
		Size: 460.0 B  
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
$ docker pull fluentd@sha256:750f2da8e32b81833482a1ee8b8432678b0bd1d9e7a4380691b500e9c2dc46bd
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
$ docker pull fluentd@sha256:e50d2feff22570321cb513275f0ecb0610ff28fd04eb34fb0ba67b2c33025962
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19094524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b1c11fc4d5d2d98146f392efff53ded472fea834ad159104bd57d957aa2ea7f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:15:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 12 Nov 2021 22:15:04 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 12 Nov 2021 22:15:52 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 12 Nov 2021 22:15:53 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 12 Nov 2021 22:15:53 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 12 Nov 2021 22:15:53 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 12 Nov 2021 22:15:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 12 Nov 2021 22:15:54 GMT
ENV LD_PRELOAD=
# Fri, 12 Nov 2021 22:15:54 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 12 Nov 2021 22:15:54 GMT
EXPOSE 24224 5140
# Fri, 12 Nov 2021 22:15:54 GMT
USER fluent
# Fri, 12 Nov 2021 22:15:55 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 12 Nov 2021 22:15:55 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13204de4fb4b7965326c9d3d4a9e1d4c8f0eaf13259bf2a230215874aa01a92`  
		Last Modified: Fri, 12 Nov 2021 22:16:15 GMT  
		Size: 16.3 MB (16269891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b94277aa813c2d531beef97fb86f701863b0219e55a63f009a3b361518c5be`  
		Last Modified: Fri, 12 Nov 2021 22:16:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac90a2c4fa5786d073fc79443f891af792328a19a36605fac7371c354b567c2f`  
		Last Modified: Fri, 12 Nov 2021 22:16:13 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18385d5d22f344b404fb5d55a84dfa60dc01850637c88bea8f126009e0bebd6d`  
		Last Modified: Fri, 12 Nov 2021 22:16:13 GMT  
		Size: 461.0 B  
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
$ docker pull fluentd@sha256:513e632f2ba2f7fa53b0885e8107eeaf5b3f6bbc6edadda1a90d638b4fda34ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18932970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6612d0dd8244452c42bdd6d5f00372e1e9ac237f09babce368fca01c2d37d192`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 08:49:20 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Nov 2021 08:49:21 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 13 Nov 2021 08:50:16 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 13 Nov 2021 08:50:17 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Nov 2021 08:50:19 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Nov 2021 08:50:20 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 13 Nov 2021 08:50:20 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Nov 2021 08:50:21 GMT
ENV LD_PRELOAD=
# Sat, 13 Nov 2021 08:50:22 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 13 Nov 2021 08:50:23 GMT
EXPOSE 24224 5140
# Sat, 13 Nov 2021 08:50:24 GMT
USER fluent
# Sat, 13 Nov 2021 08:50:25 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Nov 2021 08:50:26 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b49e73e0bcd14e81224b4723baf1b707943dbf94afaf5993d1880540d376ec`  
		Last Modified: Sat, 13 Nov 2021 08:50:53 GMT  
		Size: 16.2 MB (16211176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11039029abdf325434cd897fff317b820840ef51e6cf8eeb6e7b30d53f2af814`  
		Last Modified: Sat, 13 Nov 2021 08:50:50 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae1d5a5c57cb7203d403c10cb5f210ab184f5b1f81a1a9fba0434302926681`  
		Last Modified: Sat, 13 Nov 2021 08:50:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1a8aba720763a9d4bdc150b480e664cc2d14b7f978e331b07673a6a32710c1`  
		Last Modified: Sat, 13 Nov 2021 08:50:50 GMT  
		Size: 460.0 B  
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
$ docker pull fluentd@sha256:030a74a0c279165018374bcba82e49529ad33fd3cca86b0c2f76e0ba0928fb7d
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
$ docker pull fluentd@sha256:d35eab97b89d49d8af5c694f8737d033fa5e0f7c626a97f518906dd40a49c636
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83261603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae856f029ad5eb103171754d42735a25b4f345eae003b21f23de7f3ae8462ac`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 06:37:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 06:37:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 02 Mar 2022 06:37:59 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 07:14:25 GMT
ENV RUBY_MAJOR=2.6
# Wed, 02 Mar 2022 07:14:25 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 02 Mar 2022 07:14:25 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 02 Mar 2022 07:17:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 02 Mar 2022 07:17:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 02 Mar 2022 07:17:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 02 Mar 2022 07:17:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Mar 2022 07:17:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 02 Mar 2022 07:17:23 GMT
CMD ["irb"]
# Thu, 03 Mar 2022 06:23:52 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 03 Mar 2022 06:23:52 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 03 Mar 2022 06:23:52 GMT
ENV TINI_VERSION=0.18.0
# Thu, 03 Mar 2022 06:26:02 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 03 Mar 2022 06:26:03 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 03 Mar 2022 06:26:03 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 03 Mar 2022 06:26:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 03 Mar 2022 06:26:04 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 03 Mar 2022 06:26:04 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 03 Mar 2022 06:26:04 GMT
EXPOSE 24224 5140
# Thu, 03 Mar 2022 06:26:04 GMT
USER fluent
# Thu, 03 Mar 2022 06:26:04 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 03 Mar 2022 06:26:04 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31014161d8e618fb61f86969df63daed970d6e1848c94277df0747bd10af75af`  
		Last Modified: Wed, 02 Mar 2022 09:02:17 GMT  
		Size: 12.6 MB (12565160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30c4ecd853cc5b1b5ffed69b3d2a7800a624ca5fe649ed6a72dafce88d08540`  
		Last Modified: Wed, 02 Mar 2022 09:02:14 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabfe3ea6df0940904cf697f65cd68e18018a1f347c6d028167b5ad553ca089`  
		Last Modified: Wed, 02 Mar 2022 09:05:51 GMT  
		Size: 21.5 MB (21499018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e21e198a4703c49229131ebc39368e5e24a3d9a4fac041b18d0e3599f546b2`  
		Last Modified: Wed, 02 Mar 2022 09:05:48 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ceac730fa445e9b305322b0a26c2ac21274b553edb2b0e06900ead1a6a46dc0`  
		Last Modified: Thu, 03 Mar 2022 06:26:30 GMT  
		Size: 22.0 MB (22040608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd92d7fa522e144a43bd79a8b88ce7bc282a43b6b8b4248417734c544d8b903b`  
		Last Modified: Thu, 03 Mar 2022 06:26:27 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdba20276472981352b2a396295ff78906a41f2f8da440fe37f4220017c67435`  
		Last Modified: Thu, 03 Mar 2022 06:26:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae83baa42c9ff51153ecd81de10e823c0a48dbfb7a2988568b7d7f7fa56b0a9`  
		Last Modified: Thu, 03 Mar 2022 06:26:27 GMT  
		Size: 459.0 B  
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
$ docker pull fluentd@sha256:50b31ea7817f913210c552a1dec520e9877582b842a5c87189870e019a19584c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74377803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a31765a4823fe7e15e01ca706feca3660ccc2729c328c9153a7780d45abfc950`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 01 Mar 2022 02:04:06 GMT
ADD file:d73a3eaf767825b31d0c0189624b35193e5ad7c5907f839edf6f7917036c2d0b in / 
# Tue, 01 Mar 2022 02:04:07 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 21:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 21:30:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 01 Mar 2022 21:30:50 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 22:24:38 GMT
ENV RUBY_MAJOR=2.6
# Tue, 01 Mar 2022 22:24:38 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 01 Mar 2022 22:24:39 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 01 Mar 2022 22:28:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 01 Mar 2022 22:28:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 01 Mar 2022 22:28:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 01 Mar 2022 22:28:51 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 22:28:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 01 Mar 2022 22:28:53 GMT
CMD ["irb"]
# Thu, 03 Mar 2022 02:47:09 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 03 Mar 2022 02:47:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 03 Mar 2022 02:47:10 GMT
ENV TINI_VERSION=0.18.0
# Thu, 03 Mar 2022 02:50:46 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 03 Mar 2022 02:50:49 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 03 Mar 2022 02:50:49 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 03 Mar 2022 02:50:50 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 03 Mar 2022 02:50:50 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 03 Mar 2022 02:50:50 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 03 Mar 2022 02:50:51 GMT
EXPOSE 24224 5140
# Thu, 03 Mar 2022 02:50:51 GMT
USER fluent
# Thu, 03 Mar 2022 02:50:52 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 03 Mar 2022 02:50:52 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1acfd43b1a25aefe6117ba65bf2b46a19e3cf8e72b76f522a9fe299412e1c5f2`  
		Last Modified: Tue, 01 Mar 2022 02:20:32 GMT  
		Size: 22.8 MB (22754370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da2abb55ec2014008a51c97eb65b1d0ff890e36490ebf051bdc158c854fb718`  
		Last Modified: Tue, 01 Mar 2022 22:41:04 GMT  
		Size: 9.9 MB (9872753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d21f83104f598845b035e1bb76ed7031dc95def7440791f9e4628e235627317`  
		Last Modified: Tue, 01 Mar 2022 22:40:57 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1018bc3ff1b2f713c5e9041ac1fa7294dbd92e0e18395368cabc7a3c34ff22`  
		Last Modified: Tue, 01 Mar 2022 22:47:23 GMT  
		Size: 20.7 MB (20672461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa89236db0a63fff8cc0e88964c907e59f3064d65c3ba23ec9142c88162e771`  
		Last Modified: Tue, 01 Mar 2022 22:47:13 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c79fb8d0dae71a9bb80a32873495d7c4c6aa05ba10e1ea606d3897bb1e03eb9`  
		Last Modified: Thu, 03 Mar 2022 02:51:28 GMT  
		Size: 21.1 MB (21075145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8baa487ddd55d51b4b48b037c70e65d3cac4c0efd89219e1fd90c61b99b809`  
		Last Modified: Thu, 03 Mar 2022 02:51:15 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83af32d062cda08856bfb5d22bcfdc1d9aca2ddca2e22e51ace7b346a6dcb682`  
		Last Modified: Thu, 03 Mar 2022 02:51:15 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87c7dbee61102fe6d90f786a1c0b4f1875986382125c4df0e2b7bef87291f4e`  
		Last Modified: Thu, 03 Mar 2022 02:51:15 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:f7b96f8299f13d5849b8b6aeed7168173084e0e68a47e2dc2d4cdd103e97fa8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80133104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890b11a3885910418440f93f1798b378f09df4a81059652ca3535f28adfeea62`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:57 GMT
ADD file:7d35162eea06441e7115c6fd9508802eafee00f64b11a7529a8f125bc67fa95e in / 
# Tue, 01 Mar 2022 02:11:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 22:26:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 22:26:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 01 Mar 2022 22:26:02 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 22:50:03 GMT
ENV RUBY_MAJOR=2.6
# Tue, 01 Mar 2022 22:50:04 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 01 Mar 2022 22:50:05 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 01 Mar 2022 22:51:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 01 Mar 2022 22:51:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 01 Mar 2022 22:51:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 01 Mar 2022 22:51:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 22:51:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 01 Mar 2022 22:51:52 GMT
CMD ["irb"]
# Wed, 02 Mar 2022 15:57:17 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 02 Mar 2022 15:57:18 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 02 Mar 2022 15:57:19 GMT
ENV TINI_VERSION=0.18.0
# Wed, 02 Mar 2022 15:59:34 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 02 Mar 2022 15:59:35 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 02 Mar 2022 15:59:36 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 02 Mar 2022 15:59:37 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 02 Mar 2022 15:59:37 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 02 Mar 2022 15:59:38 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 02 Mar 2022 15:59:39 GMT
EXPOSE 24224 5140
# Wed, 02 Mar 2022 15:59:40 GMT
USER fluent
# Wed, 02 Mar 2022 15:59:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 02 Mar 2022 15:59:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:69bf0018a85cc0775a59a4dbda1b2f2e71086a2d817473f72336bf4d0a83b9d0`  
		Last Modified: Tue, 01 Mar 2022 02:19:15 GMT  
		Size: 25.9 MB (25923140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceee5ba8da281d2a743557f6778467e8e9dfbad986a09f16e0fa7cc205c8964`  
		Last Modified: Tue, 01 Mar 2022 22:57:10 GMT  
		Size: 11.3 MB (11261782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8009c9028d90626dd1772fd8c86937d72893d48be24bbe750559fce99d0c031d`  
		Last Modified: Tue, 01 Mar 2022 22:57:08 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58555dfcd5f907e1f392838e1a4363d4e44aba1dc3b26ad11b6d187b989c7507`  
		Last Modified: Tue, 01 Mar 2022 23:01:10 GMT  
		Size: 21.1 MB (21124056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3fcfe4afc9410bd036a230609d0a0e6a354dab1fa2da28da07e9a408904ca1`  
		Last Modified: Tue, 01 Mar 2022 23:01:07 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59edad34eb871720196b4939ed4ad6da80b69fc44caa785a062675f61207187`  
		Last Modified: Wed, 02 Mar 2022 16:00:18 GMT  
		Size: 21.8 MB (21821219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa469a332307b44fad9ebe951ab4df4951d9d277c8b422b94b018f4f648e853`  
		Last Modified: Wed, 02 Mar 2022 16:00:15 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad3b5a3914db2263bff214fe25ff7a658d581f1430a93944207335986a585f3`  
		Last Modified: Wed, 02 Mar 2022 16:00:15 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d53bcd11b67829ae9fa14b04c78fa4da86ef4d680eaa13dccf0b5ec118afc7`  
		Last Modified: Wed, 02 Mar 2022 16:00:15 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:c336a9108440bef4b2f322606efb98000fe55f936170fad549c1dd7e0d121bc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87197179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a16cbe1c0e12f86503ce50bf951ffd56c4da754c3c3f544c3cd41bd4bd6a86f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 02:59:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 02:59:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 02 Mar 2022 02:59:10 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 03:44:43 GMT
ENV RUBY_MAJOR=2.6
# Wed, 02 Mar 2022 03:44:44 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 02 Mar 2022 03:44:44 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 02 Mar 2022 03:48:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 02 Mar 2022 03:48:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 02 Mar 2022 03:48:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 02 Mar 2022 03:48:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Mar 2022 03:48:24 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 02 Mar 2022 03:48:24 GMT
CMD ["irb"]
# Wed, 02 Mar 2022 10:10:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 02 Mar 2022 10:10:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 02 Mar 2022 10:10:24 GMT
ENV TINI_VERSION=0.18.0
# Wed, 02 Mar 2022 10:12:30 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 02 Mar 2022 10:12:31 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 02 Mar 2022 10:12:31 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 02 Mar 2022 10:12:31 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 02 Mar 2022 10:12:31 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 02 Mar 2022 10:12:31 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 02 Mar 2022 10:12:31 GMT
EXPOSE 24224 5140
# Wed, 02 Mar 2022 10:12:32 GMT
USER fluent
# Wed, 02 Mar 2022 10:12:32 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 02 Mar 2022 10:12:32 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ed1194888e90e63d86556ce85bac8a45661ceb23698a8fc2547540a1174778`  
		Last Modified: Wed, 02 Mar 2022 03:56:07 GMT  
		Size: 17.2 MB (17227090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51133e06ddff3b1911da5c5eb7c6dfb4b1608a4e54e9ab357f37bfa0233b9d09`  
		Last Modified: Wed, 02 Mar 2022 03:56:01 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d17c445a984b466730ffd4738910240a28c9787671c352b2cfc70934c94595`  
		Last Modified: Wed, 02 Mar 2022 04:00:48 GMT  
		Size: 20.9 MB (20941747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f12e9958f193a6db6b201bf266764526324ab9acb7425d33e554da1a240bd11`  
		Last Modified: Wed, 02 Mar 2022 04:00:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3924958ebd108bf6bb7ca7e09cc8c71ea2e8b85111941fa797d1d8fccad9d357`  
		Last Modified: Wed, 02 Mar 2022 10:13:09 GMT  
		Size: 21.2 MB (21220681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38908ae4ba9221d06d93169b02d9b33ddb245b8a6c0b087ac8979f69972e9a5d`  
		Last Modified: Wed, 02 Mar 2022 10:13:05 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3270cb7aa634102732fc036b9175c4fb2af8b7bcd9e5228d44d18872cd761e2`  
		Last Modified: Wed, 02 Mar 2022 10:13:05 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b456f415a765a383728308b7e96c7c3c7ea5fec50e1daa42437994dbdc05ad9`  
		Last Modified: Wed, 02 Mar 2022 10:13:05 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:dcc8ea95c22d529ae660813cac6446e9850f90d1e217fa6471724f48e38bb5cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87907170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba1da740d403187a19c8d4ee67f850456247f102fe5a634828eb6171d38d245a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 01 Mar 2022 02:06:09 GMT
ADD file:005ec6e437fc9cf8458edb6369462ce53feb585501ea6b5e5f4a6264557b3a01 in / 
# Tue, 01 Mar 2022 02:06:14 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 00:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 00:23:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 02 Mar 2022 00:23:09 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 01:23:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 02 Mar 2022 01:24:06 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 02 Mar 2022 01:24:10 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 02 Mar 2022 01:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 02 Mar 2022 01:31:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 02 Mar 2022 01:31:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 02 Mar 2022 01:31:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Mar 2022 01:31:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 02 Mar 2022 01:31:46 GMT
CMD ["irb"]
# Wed, 02 Mar 2022 07:43:11 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 02 Mar 2022 07:43:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 02 Mar 2022 07:43:17 GMT
ENV TINI_VERSION=0.18.0
# Wed, 02 Mar 2022 07:48:05 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 02 Mar 2022 07:48:14 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 02 Mar 2022 07:48:16 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 02 Mar 2022 07:48:18 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 02 Mar 2022 07:48:21 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 02 Mar 2022 07:48:25 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 02 Mar 2022 07:48:32 GMT
EXPOSE 24224 5140
# Wed, 02 Mar 2022 07:48:37 GMT
USER fluent
# Wed, 02 Mar 2022 07:48:43 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 02 Mar 2022 07:48:46 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:3cee81bb9485c9d0b620c87842e566d7a1f93086ef88c00a4d7175fc776b7f3f`  
		Last Modified: Tue, 01 Mar 2022 02:16:22 GMT  
		Size: 30.6 MB (30562288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb09225757ed0aa03e31fc223822f8daf064f401d37bb27af5caf9311b37d33`  
		Last Modified: Wed, 02 Mar 2022 01:39:34 GMT  
		Size: 12.7 MB (12705517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15441b0cdc7c76c65f15bf5bd7812c7f8141ddebff934dcb4eafd7cc04e5bc6`  
		Last Modified: Wed, 02 Mar 2022 01:39:31 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2972f3dabe2bfb718f7e760fb42b87c569f9eca35748a0261caded8c1549f109`  
		Last Modified: Wed, 02 Mar 2022 01:44:09 GMT  
		Size: 22.0 MB (22023189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbe1c64ded660b1d9db475febc9b1e73eca1a108075b495d6bfe8122c45e88c`  
		Last Modified: Wed, 02 Mar 2022 01:44:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d8876c4ae9deca281c9fc7e926f124dd6265eedb3bf1f33fe4b8371c90a935`  
		Last Modified: Wed, 02 Mar 2022 07:49:16 GMT  
		Size: 22.6 MB (22613092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853cedeef014ae77c6fe30e0c7d00a6a08e2ec1c9079fe0d9f81f1e42b4e0b21`  
		Last Modified: Wed, 02 Mar 2022 07:49:12 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd5f99c41cb9d86770bf15943dc80543e9f5d510dc63c788433da42488dc91a`  
		Last Modified: Wed, 02 Mar 2022 07:49:12 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8a5af8334100b0f119724505d845e7d1c5a43f2f00da4521f95072a6f8f677`  
		Last Modified: Wed, 02 Mar 2022 07:49:12 GMT  
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
$ docker pull fluentd@sha256:750f2da8e32b81833482a1ee8b8432678b0bd1d9e7a4380691b500e9c2dc46bd
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
$ docker pull fluentd@sha256:e50d2feff22570321cb513275f0ecb0610ff28fd04eb34fb0ba67b2c33025962
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19094524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b1c11fc4d5d2d98146f392efff53ded472fea834ad159104bd57d957aa2ea7f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:15:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 12 Nov 2021 22:15:04 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 12 Nov 2021 22:15:52 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 12 Nov 2021 22:15:53 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 12 Nov 2021 22:15:53 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 12 Nov 2021 22:15:53 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 12 Nov 2021 22:15:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 12 Nov 2021 22:15:54 GMT
ENV LD_PRELOAD=
# Fri, 12 Nov 2021 22:15:54 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 12 Nov 2021 22:15:54 GMT
EXPOSE 24224 5140
# Fri, 12 Nov 2021 22:15:54 GMT
USER fluent
# Fri, 12 Nov 2021 22:15:55 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 12 Nov 2021 22:15:55 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13204de4fb4b7965326c9d3d4a9e1d4c8f0eaf13259bf2a230215874aa01a92`  
		Last Modified: Fri, 12 Nov 2021 22:16:15 GMT  
		Size: 16.3 MB (16269891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b94277aa813c2d531beef97fb86f701863b0219e55a63f009a3b361518c5be`  
		Last Modified: Fri, 12 Nov 2021 22:16:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac90a2c4fa5786d073fc79443f891af792328a19a36605fac7371c354b567c2f`  
		Last Modified: Fri, 12 Nov 2021 22:16:13 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18385d5d22f344b404fb5d55a84dfa60dc01850637c88bea8f126009e0bebd6d`  
		Last Modified: Fri, 12 Nov 2021 22:16:13 GMT  
		Size: 461.0 B  
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
$ docker pull fluentd@sha256:513e632f2ba2f7fa53b0885e8107eeaf5b3f6bbc6edadda1a90d638b4fda34ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18932970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6612d0dd8244452c42bdd6d5f00372e1e9ac237f09babce368fca01c2d37d192`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 08:49:20 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Nov 2021 08:49:21 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 13 Nov 2021 08:50:16 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 13 Nov 2021 08:50:17 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Nov 2021 08:50:19 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Nov 2021 08:50:20 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 13 Nov 2021 08:50:20 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Nov 2021 08:50:21 GMT
ENV LD_PRELOAD=
# Sat, 13 Nov 2021 08:50:22 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 13 Nov 2021 08:50:23 GMT
EXPOSE 24224 5140
# Sat, 13 Nov 2021 08:50:24 GMT
USER fluent
# Sat, 13 Nov 2021 08:50:25 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Nov 2021 08:50:26 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b49e73e0bcd14e81224b4723baf1b707943dbf94afaf5993d1880540d376ec`  
		Last Modified: Sat, 13 Nov 2021 08:50:53 GMT  
		Size: 16.2 MB (16211176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11039029abdf325434cd897fff317b820840ef51e6cf8eeb6e7b30d53f2af814`  
		Last Modified: Sat, 13 Nov 2021 08:50:50 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae1d5a5c57cb7203d403c10cb5f210ab184f5b1f81a1a9fba0434302926681`  
		Last Modified: Sat, 13 Nov 2021 08:50:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1a8aba720763a9d4bdc150b480e664cc2d14b7f978e331b07673a6a32710c1`  
		Last Modified: Sat, 13 Nov 2021 08:50:50 GMT  
		Size: 460.0 B  
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
$ docker pull fluentd@sha256:030a74a0c279165018374bcba82e49529ad33fd3cca86b0c2f76e0ba0928fb7d
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
$ docker pull fluentd@sha256:d35eab97b89d49d8af5c694f8737d033fa5e0f7c626a97f518906dd40a49c636
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83261603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae856f029ad5eb103171754d42735a25b4f345eae003b21f23de7f3ae8462ac`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 06:37:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 06:37:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 02 Mar 2022 06:37:59 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 07:14:25 GMT
ENV RUBY_MAJOR=2.6
# Wed, 02 Mar 2022 07:14:25 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 02 Mar 2022 07:14:25 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 02 Mar 2022 07:17:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 02 Mar 2022 07:17:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 02 Mar 2022 07:17:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 02 Mar 2022 07:17:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Mar 2022 07:17:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 02 Mar 2022 07:17:23 GMT
CMD ["irb"]
# Thu, 03 Mar 2022 06:23:52 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 03 Mar 2022 06:23:52 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 03 Mar 2022 06:23:52 GMT
ENV TINI_VERSION=0.18.0
# Thu, 03 Mar 2022 06:26:02 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 03 Mar 2022 06:26:03 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 03 Mar 2022 06:26:03 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 03 Mar 2022 06:26:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 03 Mar 2022 06:26:04 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 03 Mar 2022 06:26:04 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 03 Mar 2022 06:26:04 GMT
EXPOSE 24224 5140
# Thu, 03 Mar 2022 06:26:04 GMT
USER fluent
# Thu, 03 Mar 2022 06:26:04 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 03 Mar 2022 06:26:04 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31014161d8e618fb61f86969df63daed970d6e1848c94277df0747bd10af75af`  
		Last Modified: Wed, 02 Mar 2022 09:02:17 GMT  
		Size: 12.6 MB (12565160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30c4ecd853cc5b1b5ffed69b3d2a7800a624ca5fe649ed6a72dafce88d08540`  
		Last Modified: Wed, 02 Mar 2022 09:02:14 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabfe3ea6df0940904cf697f65cd68e18018a1f347c6d028167b5ad553ca089`  
		Last Modified: Wed, 02 Mar 2022 09:05:51 GMT  
		Size: 21.5 MB (21499018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e21e198a4703c49229131ebc39368e5e24a3d9a4fac041b18d0e3599f546b2`  
		Last Modified: Wed, 02 Mar 2022 09:05:48 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ceac730fa445e9b305322b0a26c2ac21274b553edb2b0e06900ead1a6a46dc0`  
		Last Modified: Thu, 03 Mar 2022 06:26:30 GMT  
		Size: 22.0 MB (22040608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd92d7fa522e144a43bd79a8b88ce7bc282a43b6b8b4248417734c544d8b903b`  
		Last Modified: Thu, 03 Mar 2022 06:26:27 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdba20276472981352b2a396295ff78906a41f2f8da440fe37f4220017c67435`  
		Last Modified: Thu, 03 Mar 2022 06:26:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae83baa42c9ff51153ecd81de10e823c0a48dbfb7a2988568b7d7f7fa56b0a9`  
		Last Modified: Thu, 03 Mar 2022 06:26:27 GMT  
		Size: 459.0 B  
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
$ docker pull fluentd@sha256:50b31ea7817f913210c552a1dec520e9877582b842a5c87189870e019a19584c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74377803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a31765a4823fe7e15e01ca706feca3660ccc2729c328c9153a7780d45abfc950`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 01 Mar 2022 02:04:06 GMT
ADD file:d73a3eaf767825b31d0c0189624b35193e5ad7c5907f839edf6f7917036c2d0b in / 
# Tue, 01 Mar 2022 02:04:07 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 21:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 21:30:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 01 Mar 2022 21:30:50 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 22:24:38 GMT
ENV RUBY_MAJOR=2.6
# Tue, 01 Mar 2022 22:24:38 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 01 Mar 2022 22:24:39 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 01 Mar 2022 22:28:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 01 Mar 2022 22:28:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 01 Mar 2022 22:28:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 01 Mar 2022 22:28:51 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 22:28:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 01 Mar 2022 22:28:53 GMT
CMD ["irb"]
# Thu, 03 Mar 2022 02:47:09 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 03 Mar 2022 02:47:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 03 Mar 2022 02:47:10 GMT
ENV TINI_VERSION=0.18.0
# Thu, 03 Mar 2022 02:50:46 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 03 Mar 2022 02:50:49 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 03 Mar 2022 02:50:49 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 03 Mar 2022 02:50:50 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 03 Mar 2022 02:50:50 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 03 Mar 2022 02:50:50 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 03 Mar 2022 02:50:51 GMT
EXPOSE 24224 5140
# Thu, 03 Mar 2022 02:50:51 GMT
USER fluent
# Thu, 03 Mar 2022 02:50:52 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 03 Mar 2022 02:50:52 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1acfd43b1a25aefe6117ba65bf2b46a19e3cf8e72b76f522a9fe299412e1c5f2`  
		Last Modified: Tue, 01 Mar 2022 02:20:32 GMT  
		Size: 22.8 MB (22754370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da2abb55ec2014008a51c97eb65b1d0ff890e36490ebf051bdc158c854fb718`  
		Last Modified: Tue, 01 Mar 2022 22:41:04 GMT  
		Size: 9.9 MB (9872753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d21f83104f598845b035e1bb76ed7031dc95def7440791f9e4628e235627317`  
		Last Modified: Tue, 01 Mar 2022 22:40:57 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1018bc3ff1b2f713c5e9041ac1fa7294dbd92e0e18395368cabc7a3c34ff22`  
		Last Modified: Tue, 01 Mar 2022 22:47:23 GMT  
		Size: 20.7 MB (20672461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa89236db0a63fff8cc0e88964c907e59f3064d65c3ba23ec9142c88162e771`  
		Last Modified: Tue, 01 Mar 2022 22:47:13 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c79fb8d0dae71a9bb80a32873495d7c4c6aa05ba10e1ea606d3897bb1e03eb9`  
		Last Modified: Thu, 03 Mar 2022 02:51:28 GMT  
		Size: 21.1 MB (21075145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8baa487ddd55d51b4b48b037c70e65d3cac4c0efd89219e1fd90c61b99b809`  
		Last Modified: Thu, 03 Mar 2022 02:51:15 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83af32d062cda08856bfb5d22bcfdc1d9aca2ddca2e22e51ace7b346a6dcb682`  
		Last Modified: Thu, 03 Mar 2022 02:51:15 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87c7dbee61102fe6d90f786a1c0b4f1875986382125c4df0e2b7bef87291f4e`  
		Last Modified: Thu, 03 Mar 2022 02:51:15 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:f7b96f8299f13d5849b8b6aeed7168173084e0e68a47e2dc2d4cdd103e97fa8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80133104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890b11a3885910418440f93f1798b378f09df4a81059652ca3535f28adfeea62`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:57 GMT
ADD file:7d35162eea06441e7115c6fd9508802eafee00f64b11a7529a8f125bc67fa95e in / 
# Tue, 01 Mar 2022 02:11:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 22:26:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 22:26:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 01 Mar 2022 22:26:02 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 22:50:03 GMT
ENV RUBY_MAJOR=2.6
# Tue, 01 Mar 2022 22:50:04 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 01 Mar 2022 22:50:05 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 01 Mar 2022 22:51:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 01 Mar 2022 22:51:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 01 Mar 2022 22:51:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 01 Mar 2022 22:51:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 22:51:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 01 Mar 2022 22:51:52 GMT
CMD ["irb"]
# Wed, 02 Mar 2022 15:57:17 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 02 Mar 2022 15:57:18 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 02 Mar 2022 15:57:19 GMT
ENV TINI_VERSION=0.18.0
# Wed, 02 Mar 2022 15:59:34 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 02 Mar 2022 15:59:35 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 02 Mar 2022 15:59:36 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 02 Mar 2022 15:59:37 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 02 Mar 2022 15:59:37 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 02 Mar 2022 15:59:38 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 02 Mar 2022 15:59:39 GMT
EXPOSE 24224 5140
# Wed, 02 Mar 2022 15:59:40 GMT
USER fluent
# Wed, 02 Mar 2022 15:59:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 02 Mar 2022 15:59:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:69bf0018a85cc0775a59a4dbda1b2f2e71086a2d817473f72336bf4d0a83b9d0`  
		Last Modified: Tue, 01 Mar 2022 02:19:15 GMT  
		Size: 25.9 MB (25923140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceee5ba8da281d2a743557f6778467e8e9dfbad986a09f16e0fa7cc205c8964`  
		Last Modified: Tue, 01 Mar 2022 22:57:10 GMT  
		Size: 11.3 MB (11261782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8009c9028d90626dd1772fd8c86937d72893d48be24bbe750559fce99d0c031d`  
		Last Modified: Tue, 01 Mar 2022 22:57:08 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58555dfcd5f907e1f392838e1a4363d4e44aba1dc3b26ad11b6d187b989c7507`  
		Last Modified: Tue, 01 Mar 2022 23:01:10 GMT  
		Size: 21.1 MB (21124056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3fcfe4afc9410bd036a230609d0a0e6a354dab1fa2da28da07e9a408904ca1`  
		Last Modified: Tue, 01 Mar 2022 23:01:07 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59edad34eb871720196b4939ed4ad6da80b69fc44caa785a062675f61207187`  
		Last Modified: Wed, 02 Mar 2022 16:00:18 GMT  
		Size: 21.8 MB (21821219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa469a332307b44fad9ebe951ab4df4951d9d277c8b422b94b018f4f648e853`  
		Last Modified: Wed, 02 Mar 2022 16:00:15 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad3b5a3914db2263bff214fe25ff7a658d581f1430a93944207335986a585f3`  
		Last Modified: Wed, 02 Mar 2022 16:00:15 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d53bcd11b67829ae9fa14b04c78fa4da86ef4d680eaa13dccf0b5ec118afc7`  
		Last Modified: Wed, 02 Mar 2022 16:00:15 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:c336a9108440bef4b2f322606efb98000fe55f936170fad549c1dd7e0d121bc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87197179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a16cbe1c0e12f86503ce50bf951ffd56c4da754c3c3f544c3cd41bd4bd6a86f`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 02:59:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 02:59:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 02 Mar 2022 02:59:10 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 03:44:43 GMT
ENV RUBY_MAJOR=2.6
# Wed, 02 Mar 2022 03:44:44 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 02 Mar 2022 03:44:44 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 02 Mar 2022 03:48:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 02 Mar 2022 03:48:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 02 Mar 2022 03:48:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 02 Mar 2022 03:48:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Mar 2022 03:48:24 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 02 Mar 2022 03:48:24 GMT
CMD ["irb"]
# Wed, 02 Mar 2022 10:10:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 02 Mar 2022 10:10:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 02 Mar 2022 10:10:24 GMT
ENV TINI_VERSION=0.18.0
# Wed, 02 Mar 2022 10:12:30 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 02 Mar 2022 10:12:31 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 02 Mar 2022 10:12:31 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 02 Mar 2022 10:12:31 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 02 Mar 2022 10:12:31 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 02 Mar 2022 10:12:31 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 02 Mar 2022 10:12:31 GMT
EXPOSE 24224 5140
# Wed, 02 Mar 2022 10:12:32 GMT
USER fluent
# Wed, 02 Mar 2022 10:12:32 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 02 Mar 2022 10:12:32 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ed1194888e90e63d86556ce85bac8a45661ceb23698a8fc2547540a1174778`  
		Last Modified: Wed, 02 Mar 2022 03:56:07 GMT  
		Size: 17.2 MB (17227090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51133e06ddff3b1911da5c5eb7c6dfb4b1608a4e54e9ab357f37bfa0233b9d09`  
		Last Modified: Wed, 02 Mar 2022 03:56:01 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d17c445a984b466730ffd4738910240a28c9787671c352b2cfc70934c94595`  
		Last Modified: Wed, 02 Mar 2022 04:00:48 GMT  
		Size: 20.9 MB (20941747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f12e9958f193a6db6b201bf266764526324ab9acb7425d33e554da1a240bd11`  
		Last Modified: Wed, 02 Mar 2022 04:00:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3924958ebd108bf6bb7ca7e09cc8c71ea2e8b85111941fa797d1d8fccad9d357`  
		Last Modified: Wed, 02 Mar 2022 10:13:09 GMT  
		Size: 21.2 MB (21220681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38908ae4ba9221d06d93169b02d9b33ddb245b8a6c0b087ac8979f69972e9a5d`  
		Last Modified: Wed, 02 Mar 2022 10:13:05 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3270cb7aa634102732fc036b9175c4fb2af8b7bcd9e5228d44d18872cd761e2`  
		Last Modified: Wed, 02 Mar 2022 10:13:05 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b456f415a765a383728308b7e96c7c3c7ea5fec50e1daa42437994dbdc05ad9`  
		Last Modified: Wed, 02 Mar 2022 10:13:05 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:dcc8ea95c22d529ae660813cac6446e9850f90d1e217fa6471724f48e38bb5cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87907170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba1da740d403187a19c8d4ee67f850456247f102fe5a634828eb6171d38d245a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 01 Mar 2022 02:06:09 GMT
ADD file:005ec6e437fc9cf8458edb6369462ce53feb585501ea6b5e5f4a6264557b3a01 in / 
# Tue, 01 Mar 2022 02:06:14 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 00:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 00:23:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 02 Mar 2022 00:23:09 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 01:23:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 02 Mar 2022 01:24:06 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 02 Mar 2022 01:24:10 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 02 Mar 2022 01:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 02 Mar 2022 01:31:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 02 Mar 2022 01:31:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 02 Mar 2022 01:31:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Mar 2022 01:31:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 02 Mar 2022 01:31:46 GMT
CMD ["irb"]
# Wed, 02 Mar 2022 07:43:11 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 02 Mar 2022 07:43:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 02 Mar 2022 07:43:17 GMT
ENV TINI_VERSION=0.18.0
# Wed, 02 Mar 2022 07:48:05 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 02 Mar 2022 07:48:14 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 02 Mar 2022 07:48:16 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 02 Mar 2022 07:48:18 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 02 Mar 2022 07:48:21 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 02 Mar 2022 07:48:25 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 02 Mar 2022 07:48:32 GMT
EXPOSE 24224 5140
# Wed, 02 Mar 2022 07:48:37 GMT
USER fluent
# Wed, 02 Mar 2022 07:48:43 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 02 Mar 2022 07:48:46 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:3cee81bb9485c9d0b620c87842e566d7a1f93086ef88c00a4d7175fc776b7f3f`  
		Last Modified: Tue, 01 Mar 2022 02:16:22 GMT  
		Size: 30.6 MB (30562288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb09225757ed0aa03e31fc223822f8daf064f401d37bb27af5caf9311b37d33`  
		Last Modified: Wed, 02 Mar 2022 01:39:34 GMT  
		Size: 12.7 MB (12705517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15441b0cdc7c76c65f15bf5bd7812c7f8141ddebff934dcb4eafd7cc04e5bc6`  
		Last Modified: Wed, 02 Mar 2022 01:39:31 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2972f3dabe2bfb718f7e760fb42b87c569f9eca35748a0261caded8c1549f109`  
		Last Modified: Wed, 02 Mar 2022 01:44:09 GMT  
		Size: 22.0 MB (22023189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbe1c64ded660b1d9db475febc9b1e73eca1a108075b495d6bfe8122c45e88c`  
		Last Modified: Wed, 02 Mar 2022 01:44:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d8876c4ae9deca281c9fc7e926f124dd6265eedb3bf1f33fe4b8371c90a935`  
		Last Modified: Wed, 02 Mar 2022 07:49:16 GMT  
		Size: 22.6 MB (22613092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853cedeef014ae77c6fe30e0c7d00a6a08e2ec1c9079fe0d9f81f1e42b4e0b21`  
		Last Modified: Wed, 02 Mar 2022 07:49:12 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd5f99c41cb9d86770bf15943dc80543e9f5d510dc63c788433da42488dc91a`  
		Last Modified: Wed, 02 Mar 2022 07:49:12 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8a5af8334100b0f119724505d845e7d1c5a43f2f00da4521f95072a6f8f677`  
		Last Modified: Wed, 02 Mar 2022 07:49:12 GMT  
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
