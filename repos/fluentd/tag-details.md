<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.14-1`](#fluentdv114-1)
-	[`fluentd:v1.14-debian-1`](#fluentdv114-debian-1)
-	[`fluentd:v1.14.0-1.0`](#fluentdv1140-10)
-	[`fluentd:v1.14.0-debian-1.0`](#fluentdv1140-debian-10)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:3dee97712e6814f55e625c10ec00061ad0245ebc418c37fef10baa37acb5ea48
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
$ docker pull fluentd@sha256:65a6a197f958f1377eeb170c66127ad81e6658eb4afb37e34dd1ea29adc00969
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18399672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8230937f87367b64bce083b46594408cc94f1bc9eb3a30fe45a55c288e8c0a45`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:10:18 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 12 Nov 2021 17:10:18 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 12 Nov 2021 17:12:25 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 12 Nov 2021 17:12:27 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 12 Nov 2021 17:12:28 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 12 Nov 2021 17:12:28 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 12 Nov 2021 17:12:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 12 Nov 2021 17:12:29 GMT
ENV LD_PRELOAD=
# Fri, 12 Nov 2021 17:12:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 12 Nov 2021 17:12:30 GMT
EXPOSE 24224 5140
# Fri, 12 Nov 2021 17:12:30 GMT
USER fluent
# Fri, 12 Nov 2021 17:12:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 12 Nov 2021 17:12:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff475b9767d8c8b660254919cdacfb07d41726bcf6ae57bd82df1ab92964973`  
		Last Modified: Fri, 12 Nov 2021 17:13:19 GMT  
		Size: 15.8 MB (15764124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688a0000f32840ee0b24105fa7e0a8961a424e9cc972883a857a725d352294e0`  
		Last Modified: Fri, 12 Nov 2021 17:13:07 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bca9fcdd7bd010eb56f1658123023630d8a2feff9eb6e7dc663d84b97c1cac`  
		Last Modified: Fri, 12 Nov 2021 17:13:07 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cfca946685484b3ea43c9624c073dd8ae63bf180f0cbdba40ed2ed0a6d594c`  
		Last Modified: Fri, 12 Nov 2021 17:13:07 GMT  
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
$ docker pull fluentd@sha256:6dfdd776a8dd8b6655b7fc118a432b474931cd7101cb9d9791eb933d50f4e767
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18627613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8324bde6076998fe36358be5951135c71d7514c142da41074094b7e9e79a5606`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:46:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Nov 2021 05:46:04 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 13 Nov 2021 05:47:01 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 13 Nov 2021 05:47:02 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Nov 2021 05:47:02 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Nov 2021 05:47:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 13 Nov 2021 05:47:03 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Nov 2021 05:47:03 GMT
ENV LD_PRELOAD=
# Sat, 13 Nov 2021 05:47:03 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 13 Nov 2021 05:47:03 GMT
EXPOSE 24224 5140
# Sat, 13 Nov 2021 05:47:04 GMT
USER fluent
# Sat, 13 Nov 2021 05:47:04 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Nov 2021 05:47:04 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b4c0afc72421dadac58d84e5af4b2e3a16b7f2d6734b0749960a0f3a99fbe9`  
		Last Modified: Sat, 13 Nov 2021 05:47:36 GMT  
		Size: 15.8 MB (15796601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4345f72b9ac989cfe5a73d7da793eb81dae91292cb88e92ea863177fdbdbdc23`  
		Last Modified: Sat, 13 Nov 2021 05:47:33 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1e56be2212cf2bac7d78b5b74f00a84ff6f225959282ec73b07562770d737a`  
		Last Modified: Sat, 13 Nov 2021 05:47:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc8507a9023a335223baff561db76d3c4e74d11dc0a86396ceb2ab83a76a7cf`  
		Last Modified: Sat, 13 Nov 2021 05:47:33 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:8fd5d9e285f3fc0a115f2de1b8aa2d8dece14edbf48b5a1980a6a2437a70530f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19165522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33a2aab15001f20ad0220e97bc94fadc3ac1fcb19187c2898b3328461e0e440`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:25 GMT
ADD file:f7216323de17450e653f77c86d2c1e2e8ec01e1133e93f29c515761b3e9d8f7d in / 
# Fri, 12 Nov 2021 21:18:28 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:31:52 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Nov 2021 15:31:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 13 Nov 2021 15:33:14 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 13 Nov 2021 15:33:25 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Nov 2021 15:33:32 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Nov 2021 15:33:38 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 13 Nov 2021 15:33:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Nov 2021 15:33:56 GMT
ENV LD_PRELOAD=
# Sat, 13 Nov 2021 15:34:07 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 13 Nov 2021 15:34:09 GMT
EXPOSE 24224 5140
# Sat, 13 Nov 2021 15:34:15 GMT
USER fluent
# Sat, 13 Nov 2021 15:34:18 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Nov 2021 15:34:20 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6729720a3e6b58511df148134bb67d786ad90f9fce1c02ba5bbfd31f33055fbe`  
		Last Modified: Fri, 12 Nov 2021 21:19:49 GMT  
		Size: 2.8 MB (2820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198dd1f78cd797f2648276619a592f94742f5b209730c5dd95e2f0ec0820a5de`  
		Last Modified: Sat, 13 Nov 2021 15:34:53 GMT  
		Size: 16.3 MB (16342800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df93171f11aee7e79e119605b6b629fe2b6b23a553e2496c1163d5b7c6fab289`  
		Last Modified: Sat, 13 Nov 2021 15:34:49 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d44d6ee555a88c35c0b2c281f2f52340e02388a29c35f5ea61f1081597fb442`  
		Last Modified: Sat, 13 Nov 2021 15:34:49 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9187a13c71c5c260b3b4bf04a227a36ecc837ceee1d0e1c191f8aa2844a7636e`  
		Last Modified: Sat, 13 Nov 2021 15:34:49 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:6044314a53964ecc154c09d49350727e8c6917de12bbc62c957ee363fb937a14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18799969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64f549dd1ad1b82e6a232731613dc468b569d4f9500433e6ef441ccc7634f12c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:44 GMT
ADD file:637f327c9b07758709ef7dbc42eb472c888d221acde89b1c3775553864334d5c in / 
# Fri, 12 Nov 2021 16:41:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:16:50 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 12 Nov 2021 22:16:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 12 Nov 2021 22:17:26 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 12 Nov 2021 22:17:27 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 12 Nov 2021 22:17:27 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 12 Nov 2021 22:17:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 12 Nov 2021 22:17:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 12 Nov 2021 22:17:28 GMT
ENV LD_PRELOAD=
# Fri, 12 Nov 2021 22:17:28 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 12 Nov 2021 22:17:28 GMT
EXPOSE 24224 5140
# Fri, 12 Nov 2021 22:17:28 GMT
USER fluent
# Fri, 12 Nov 2021 22:17:28 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 12 Nov 2021 22:17:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b872f056719bde6e6722091afb2a3376d720c69c142b91ac352050080dd79615`  
		Last Modified: Fri, 12 Nov 2021 16:42:54 GMT  
		Size: 2.6 MB (2611155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70e8f50864afa9912f5e959e79bff07cf414db20b131883f209b1ab81b6577`  
		Last Modified: Fri, 12 Nov 2021 22:18:11 GMT  
		Size: 16.2 MB (16186611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91cb6e8f074b6be6273edd016fb2ac5fbc2036973b56626990849083048622c`  
		Last Modified: Fri, 12 Nov 2021 22:18:00 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230dbc436d65d2c8a7d1fe391a46813c024611ebe5d8c72df6670e5cd501ac94`  
		Last Modified: Fri, 12 Nov 2021 22:18:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cdd6f6256dd88c8aa99df54e444c178b276b5db074a734ef1ff747cdc34597`  
		Last Modified: Fri, 12 Nov 2021 22:18:00 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14-1`

```console
$ docker pull fluentd@sha256:3dee97712e6814f55e625c10ec00061ad0245ebc418c37fef10baa37acb5ea48
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
$ docker pull fluentd@sha256:65a6a197f958f1377eeb170c66127ad81e6658eb4afb37e34dd1ea29adc00969
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18399672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8230937f87367b64bce083b46594408cc94f1bc9eb3a30fe45a55c288e8c0a45`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:10:18 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 12 Nov 2021 17:10:18 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 12 Nov 2021 17:12:25 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 12 Nov 2021 17:12:27 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 12 Nov 2021 17:12:28 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 12 Nov 2021 17:12:28 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 12 Nov 2021 17:12:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 12 Nov 2021 17:12:29 GMT
ENV LD_PRELOAD=
# Fri, 12 Nov 2021 17:12:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 12 Nov 2021 17:12:30 GMT
EXPOSE 24224 5140
# Fri, 12 Nov 2021 17:12:30 GMT
USER fluent
# Fri, 12 Nov 2021 17:12:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 12 Nov 2021 17:12:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff475b9767d8c8b660254919cdacfb07d41726bcf6ae57bd82df1ab92964973`  
		Last Modified: Fri, 12 Nov 2021 17:13:19 GMT  
		Size: 15.8 MB (15764124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688a0000f32840ee0b24105fa7e0a8961a424e9cc972883a857a725d352294e0`  
		Last Modified: Fri, 12 Nov 2021 17:13:07 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bca9fcdd7bd010eb56f1658123023630d8a2feff9eb6e7dc663d84b97c1cac`  
		Last Modified: Fri, 12 Nov 2021 17:13:07 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cfca946685484b3ea43c9624c073dd8ae63bf180f0cbdba40ed2ed0a6d594c`  
		Last Modified: Fri, 12 Nov 2021 17:13:07 GMT  
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
$ docker pull fluentd@sha256:6dfdd776a8dd8b6655b7fc118a432b474931cd7101cb9d9791eb933d50f4e767
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18627613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8324bde6076998fe36358be5951135c71d7514c142da41074094b7e9e79a5606`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:46:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Nov 2021 05:46:04 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 13 Nov 2021 05:47:01 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 13 Nov 2021 05:47:02 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Nov 2021 05:47:02 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Nov 2021 05:47:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 13 Nov 2021 05:47:03 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Nov 2021 05:47:03 GMT
ENV LD_PRELOAD=
# Sat, 13 Nov 2021 05:47:03 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 13 Nov 2021 05:47:03 GMT
EXPOSE 24224 5140
# Sat, 13 Nov 2021 05:47:04 GMT
USER fluent
# Sat, 13 Nov 2021 05:47:04 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Nov 2021 05:47:04 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b4c0afc72421dadac58d84e5af4b2e3a16b7f2d6734b0749960a0f3a99fbe9`  
		Last Modified: Sat, 13 Nov 2021 05:47:36 GMT  
		Size: 15.8 MB (15796601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4345f72b9ac989cfe5a73d7da793eb81dae91292cb88e92ea863177fdbdbdc23`  
		Last Modified: Sat, 13 Nov 2021 05:47:33 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1e56be2212cf2bac7d78b5b74f00a84ff6f225959282ec73b07562770d737a`  
		Last Modified: Sat, 13 Nov 2021 05:47:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc8507a9023a335223baff561db76d3c4e74d11dc0a86396ceb2ab83a76a7cf`  
		Last Modified: Sat, 13 Nov 2021 05:47:33 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:8fd5d9e285f3fc0a115f2de1b8aa2d8dece14edbf48b5a1980a6a2437a70530f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19165522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33a2aab15001f20ad0220e97bc94fadc3ac1fcb19187c2898b3328461e0e440`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:25 GMT
ADD file:f7216323de17450e653f77c86d2c1e2e8ec01e1133e93f29c515761b3e9d8f7d in / 
# Fri, 12 Nov 2021 21:18:28 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:31:52 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Nov 2021 15:31:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 13 Nov 2021 15:33:14 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 13 Nov 2021 15:33:25 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Nov 2021 15:33:32 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Nov 2021 15:33:38 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 13 Nov 2021 15:33:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Nov 2021 15:33:56 GMT
ENV LD_PRELOAD=
# Sat, 13 Nov 2021 15:34:07 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 13 Nov 2021 15:34:09 GMT
EXPOSE 24224 5140
# Sat, 13 Nov 2021 15:34:15 GMT
USER fluent
# Sat, 13 Nov 2021 15:34:18 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Nov 2021 15:34:20 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6729720a3e6b58511df148134bb67d786ad90f9fce1c02ba5bbfd31f33055fbe`  
		Last Modified: Fri, 12 Nov 2021 21:19:49 GMT  
		Size: 2.8 MB (2820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198dd1f78cd797f2648276619a592f94742f5b209730c5dd95e2f0ec0820a5de`  
		Last Modified: Sat, 13 Nov 2021 15:34:53 GMT  
		Size: 16.3 MB (16342800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df93171f11aee7e79e119605b6b629fe2b6b23a553e2496c1163d5b7c6fab289`  
		Last Modified: Sat, 13 Nov 2021 15:34:49 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d44d6ee555a88c35c0b2c281f2f52340e02388a29c35f5ea61f1081597fb442`  
		Last Modified: Sat, 13 Nov 2021 15:34:49 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9187a13c71c5c260b3b4bf04a227a36ecc837ceee1d0e1c191f8aa2844a7636e`  
		Last Modified: Sat, 13 Nov 2021 15:34:49 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; s390x

```console
$ docker pull fluentd@sha256:6044314a53964ecc154c09d49350727e8c6917de12bbc62c957ee363fb937a14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18799969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64f549dd1ad1b82e6a232731613dc468b569d4f9500433e6ef441ccc7634f12c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:44 GMT
ADD file:637f327c9b07758709ef7dbc42eb472c888d221acde89b1c3775553864334d5c in / 
# Fri, 12 Nov 2021 16:41:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:16:50 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 12 Nov 2021 22:16:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 12 Nov 2021 22:17:26 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 12 Nov 2021 22:17:27 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 12 Nov 2021 22:17:27 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 12 Nov 2021 22:17:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 12 Nov 2021 22:17:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 12 Nov 2021 22:17:28 GMT
ENV LD_PRELOAD=
# Fri, 12 Nov 2021 22:17:28 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 12 Nov 2021 22:17:28 GMT
EXPOSE 24224 5140
# Fri, 12 Nov 2021 22:17:28 GMT
USER fluent
# Fri, 12 Nov 2021 22:17:28 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 12 Nov 2021 22:17:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b872f056719bde6e6722091afb2a3376d720c69c142b91ac352050080dd79615`  
		Last Modified: Fri, 12 Nov 2021 16:42:54 GMT  
		Size: 2.6 MB (2611155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70e8f50864afa9912f5e959e79bff07cf414db20b131883f209b1ab81b6577`  
		Last Modified: Fri, 12 Nov 2021 22:18:11 GMT  
		Size: 16.2 MB (16186611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91cb6e8f074b6be6273edd016fb2ac5fbc2036973b56626990849083048622c`  
		Last Modified: Fri, 12 Nov 2021 22:18:00 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230dbc436d65d2c8a7d1fe391a46813c024611ebe5d8c72df6670e5cd501ac94`  
		Last Modified: Fri, 12 Nov 2021 22:18:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cdd6f6256dd88c8aa99df54e444c178b276b5db074a734ef1ff747cdc34597`  
		Last Modified: Fri, 12 Nov 2021 22:18:00 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14-debian-1`

```console
$ docker pull fluentd@sha256:4ec18d3436880613323f88f0007abf6008368fb7d021400f03f69da12a4a5a9c
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
$ docker pull fluentd@sha256:c57851f56a69cc832016bbd62a97161180e790292d8336e0475d13424298fa35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83226860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf117c13a521249553d25d5ba96d5f8636537e90df992e1baf4445a23cfc1e8`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 23:05:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 23:05:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 23:05:39 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 23:44:19 GMT
ENV RUBY_MAJOR=2.6
# Wed, 24 Nov 2021 21:50:40 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 24 Nov 2021 21:50:40 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 24 Nov 2021 21:53:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 21:53:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 21:53:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 21:53:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 21:53:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 21:53:34 GMT
CMD ["irb"]
# Wed, 24 Nov 2021 22:19:02 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 24 Nov 2021 22:19:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 24 Nov 2021 22:19:02 GMT
ENV TINI_VERSION=0.18.0
# Wed, 24 Nov 2021 22:20:35 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 24 Nov 2021 22:20:36 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 24 Nov 2021 22:20:37 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 24 Nov 2021 22:20:37 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 24 Nov 2021 22:20:37 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 24 Nov 2021 22:20:37 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 24 Nov 2021 22:20:38 GMT
EXPOSE 24224 5140
# Wed, 24 Nov 2021 22:20:38 GMT
USER fluent
# Wed, 24 Nov 2021 22:20:38 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 24 Nov 2021 22:20:38 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d04e01f945ee4b2edd0451f178f17023c43f67737d0372eb309e5c83b9bc3e0`  
		Last Modified: Wed, 17 Nov 2021 23:49:59 GMT  
		Size: 12.6 MB (12565151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272911037384bdfabca8cbdd7eebb7290e527e81caa0a3f775b71d09b39ca4e`  
		Last Modified: Wed, 17 Nov 2021 23:49:56 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56cef09a8db7d612f653a8e25e4bb0dceebb0b1497ddd21af00298d5e93c24b`  
		Last Modified: Wed, 24 Nov 2021 22:07:19 GMT  
		Size: 21.5 MB (21499331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40eeef25c87db5feb734fb0a2e380c17eb22b797214848e791efda47888ff4ea`  
		Last Modified: Wed, 24 Nov 2021 22:07:17 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba9558ac7af784bbfd90d3f752f8a874f0298b34bc9fede1fcb866aeade2049`  
		Last Modified: Wed, 24 Nov 2021 22:21:08 GMT  
		Size: 22.0 MB (22005612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64821a28ac7893f4f275b333c5ac92698304de193c3249ea074a0af50fe5eb3d`  
		Last Modified: Wed, 24 Nov 2021 22:21:05 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da5fdd0b3441ff237ea26216cb84a83ed049724c8f00e580ba56dadfd4c44d9`  
		Last Modified: Wed, 24 Nov 2021 22:21:05 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c24435612b28b4bbb27679cf8a6f16060e6d4ea6319c6b6d328a6b2c87e47d4`  
		Last Modified: Wed, 24 Nov 2021 22:21:05 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:bc41a711dd5a5fc04a034c0bf6142433ce3042c19d321e7d708b17a413c5dc9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77162983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a75543860b88eb6a9bdf04252bbab2d1b93d08448488781a18c49752e29beb4d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:51:39 GMT
ADD file:e580d4d2066301375327ea51dd8db3af956e5a465495bf09d69d6deec9b0bfae in / 
# Wed, 17 Nov 2021 02:51:40 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 20:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 20:53:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 20:53:28 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:48:32 GMT
ENV RUBY_MAJOR=2.6
# Wed, 24 Nov 2021 20:40:11 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 24 Nov 2021 20:40:11 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 24 Nov 2021 20:44:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 20:44:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 20:44:43 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 20:44:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 20:44:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 20:44:45 GMT
CMD ["irb"]
# Wed, 24 Nov 2021 21:15:20 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 24 Nov 2021 21:15:20 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 24 Nov 2021 21:15:21 GMT
ENV TINI_VERSION=0.18.0
# Wed, 24 Nov 2021 21:19:03 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 24 Nov 2021 21:19:05 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 24 Nov 2021 21:19:06 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 24 Nov 2021 21:19:07 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 24 Nov 2021 21:19:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 24 Nov 2021 21:19:08 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 24 Nov 2021 21:19:08 GMT
EXPOSE 24224 5140
# Wed, 24 Nov 2021 21:19:09 GMT
USER fluent
# Wed, 24 Nov 2021 21:19:09 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 24 Nov 2021 21:19:09 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:dba255a4b166bb02562ca152d0da236ba8f211de5bf9d79e35ee023b1fce203e`  
		Last Modified: Wed, 17 Nov 2021 03:07:41 GMT  
		Size: 24.9 MB (24886310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b58fbebb8e6e22b1601002ddb4252e30c3750edfb93b87424f6c1a971c665bf`  
		Last Modified: Wed, 17 Nov 2021 21:59:40 GMT  
		Size: 10.3 MB (10349405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484eb5c97eceafe50be8deba254566cb365fd68cb0baa2e5418ecece614c2728`  
		Last Modified: Wed, 17 Nov 2021 21:59:32 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec676eb68c8105a1bbcfa111e2ca4032620d833b9d631f6132e10639f5c19d7`  
		Last Modified: Wed, 24 Nov 2021 20:56:06 GMT  
		Size: 20.8 MB (20760191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8be7a1ab157424413f57ad1f9a8b2955b765ec396a8653269ee3caf0a1a3e6`  
		Last Modified: Wed, 24 Nov 2021 20:55:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6e520e83e562a3d3cd6629b78d08387043f70edf286ef9d5aa754125f6bff4`  
		Last Modified: Wed, 24 Nov 2021 21:19:47 GMT  
		Size: 21.2 MB (21163992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68873a214d96f189e75f75fc1e55bb22035eab00a8ab9ea081208170c7b996d9`  
		Last Modified: Wed, 24 Nov 2021 21:19:37 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52aa581a7bc242ce502645b7cdba851d1e8ae13667806ea0a7e78a39945da6b1`  
		Last Modified: Wed, 24 Nov 2021 21:19:37 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4324b996594c795a8883404590e95df53678e981705915fc18b76e4d9f012a08`  
		Last Modified: Wed, 24 Nov 2021 21:19:37 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:ec438c42d6e15e24ea4b88bb2b026a34533400ffdeb7f7b6a7b89d5e6c40a3e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74330352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8f4ecb4f0e62722f24d362f2c44a2194f64715cf15dd5970e8282d3c8dd3d8`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Thu, 18 Nov 2021 08:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 08:17:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 18 Nov 2021 08:17:06 GMT
ENV LANG=C.UTF-8
# Thu, 18 Nov 2021 09:11:05 GMT
ENV RUBY_MAJOR=2.6
# Thu, 18 Nov 2021 09:11:06 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 18 Nov 2021 09:11:06 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 18 Nov 2021 09:15:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 18 Nov 2021 09:15:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 18 Nov 2021 09:15:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 18 Nov 2021 09:15:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 09:15:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 18 Nov 2021 09:15:18 GMT
CMD ["irb"]
# Thu, 18 Nov 2021 19:54:34 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 18 Nov 2021 19:54:35 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 18 Nov 2021 19:54:35 GMT
ENV TINI_VERSION=0.18.0
# Thu, 18 Nov 2021 19:57:58 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 18 Nov 2021 19:58:00 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 18 Nov 2021 19:58:01 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 18 Nov 2021 19:58:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 18 Nov 2021 19:58:01 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 18 Nov 2021 19:58:02 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 18 Nov 2021 19:58:02 GMT
EXPOSE 24224 5140
# Thu, 18 Nov 2021 19:58:03 GMT
USER fluent
# Thu, 18 Nov 2021 19:58:03 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 18 Nov 2021 19:58:04 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c8e57706e11dcf2202a1ed28d022f7fe3daa306f06bf5311fee3d20b17f772`  
		Last Modified: Thu, 18 Nov 2021 09:24:19 GMT  
		Size: 9.9 MB (9872912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caad345207fbbb28e02d7546fe9ec9b203219b39a7b6fe1a2c55d63e665ce8dd`  
		Last Modified: Thu, 18 Nov 2021 09:24:12 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb93faf1d4d1280ed90b904594838922fe363b19f403a1b9f79ea35b777e723`  
		Last Modified: Thu, 18 Nov 2021 09:31:29 GMT  
		Size: 20.6 MB (20643872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0931e5d4868154d483cf1176a216b4308c09ff1d5974bdf06aa52e79249b1b`  
		Last Modified: Thu, 18 Nov 2021 09:31:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e539878792cda106f034ac7e02ef711041594f12de56d47458c5568cad6acbbb`  
		Last Modified: Thu, 18 Nov 2021 19:58:50 GMT  
		Size: 21.1 MB (21056132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97647d3c914de5d030739ff70fc64e3703751dfd13d7de38fd657681262011b1`  
		Last Modified: Thu, 18 Nov 2021 19:58:37 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22a479987c5051e73bde92407f288948b7c54336f19594dceefbbc9cc800952`  
		Last Modified: Thu, 18 Nov 2021 19:58:37 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c7889dd5809ea7a0b1a940cc38038d498b6c68bede760c0905d9f9f779ce4a`  
		Last Modified: Thu, 18 Nov 2021 19:58:37 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:46589db7e29b7a49f4538f3612707a9918d99e0cf68e512252c72e8f11b2affd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80111378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:431fcfb49cb266ad0046e48beff5b5b97543d556f9f7b7c11150f08fb18397dd`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:31:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:31:01 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 09:31:02 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:46:01 GMT
ENV RUBY_MAJOR=2.6
# Wed, 24 Nov 2021 20:17:07 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 24 Nov 2021 20:17:08 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 24 Nov 2021 20:18:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 20:18:56 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 20:18:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 20:18:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 20:18:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 20:19:00 GMT
CMD ["irb"]
# Wed, 24 Nov 2021 21:47:16 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 24 Nov 2021 21:47:17 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 24 Nov 2021 21:47:18 GMT
ENV TINI_VERSION=0.18.0
# Wed, 24 Nov 2021 21:48:51 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 24 Nov 2021 21:48:52 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 24 Nov 2021 21:48:54 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 24 Nov 2021 21:48:55 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 24 Nov 2021 21:48:55 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 24 Nov 2021 21:48:56 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 24 Nov 2021 21:48:57 GMT
EXPOSE 24224 5140
# Wed, 24 Nov 2021 21:48:58 GMT
USER fluent
# Wed, 24 Nov 2021 21:48:59 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 24 Nov 2021 21:49:00 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8443a8ec909433d7156b8dcbeaf77f4e53d6a44b253a3f03b95126547154d55`  
		Last Modified: Wed, 17 Nov 2021 09:51:43 GMT  
		Size: 11.3 MB (11261808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f57122fa0ffe176f788d35a4a8f12a76819fa3bab198ac16e26d2961047a1d`  
		Last Modified: Wed, 17 Nov 2021 09:51:41 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9af3c6e2dd6af17eb358df3a3e3cd87a3e9dbe81fdbc4bd90bfe81d5b0cc6a`  
		Last Modified: Wed, 24 Nov 2021 20:32:29 GMT  
		Size: 21.1 MB (21123634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc85b546d70296e57b6541cf114b3816a54cd2d35fd0a07fe5e4334043508fb`  
		Last Modified: Wed, 24 Nov 2021 20:32:26 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c73f9b02cbe564eb7ae928c329162c8fdbdfbb04a125ef161cbbe1c8dd6948`  
		Last Modified: Wed, 24 Nov 2021 21:49:31 GMT  
		Size: 21.8 MB (21799902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21b62dadabc40e3264770b9a186d24bf3a7ad43631bdbfbbdb58dfab5bb46b0`  
		Last Modified: Wed, 24 Nov 2021 21:49:28 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4eccd89838bb419f0adc04ff8a31da06ea8b490784daefa3b9fc4e4465b4cd`  
		Last Modified: Wed, 24 Nov 2021 21:49:28 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41d632b0b9770c06cfa6ac1c720d7e60d2b0d608b6a7b7f1b944c048934794a`  
		Last Modified: Wed, 24 Nov 2021 21:49:28 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:f979d525ae77379bdd3675812a1f167ad70fc5533a2a0c6c83ae032fe05149fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87180308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f5c356e59cc67837def744ca276120c2e3d24192b0935877ad111c01c64d9d5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:22 GMT
ADD file:2adea3474b7ebda2bf77361304ee3e6966a9118aafd8220b81c4027be1f4d583 in / 
# Wed, 17 Nov 2021 02:40:22 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 18:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 18:38:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 18:38:25 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 19:07:29 GMT
ENV RUBY_MAJOR=2.6
# Wed, 24 Nov 2021 20:29:53 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 24 Nov 2021 20:29:53 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 24 Nov 2021 20:32:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 20:32:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 20:32:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 20:32:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 20:32:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 20:32:48 GMT
CMD ["irb"]
# Wed, 24 Nov 2021 21:38:03 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 24 Nov 2021 21:38:03 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 24 Nov 2021 21:38:04 GMT
ENV TINI_VERSION=0.18.0
# Wed, 24 Nov 2021 21:40:15 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 24 Nov 2021 21:40:16 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 24 Nov 2021 21:40:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 24 Nov 2021 21:40:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 24 Nov 2021 21:40:18 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 24 Nov 2021 21:40:18 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 24 Nov 2021 21:40:18 GMT
EXPOSE 24224 5140
# Wed, 24 Nov 2021 21:40:18 GMT
USER fluent
# Wed, 24 Nov 2021 21:40:19 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 24 Nov 2021 21:40:19 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7af5c9e671306e395c50a515c7bbe33d6f418ea08535b01c884457f78114eb08`  
		Last Modified: Wed, 17 Nov 2021 02:48:49 GMT  
		Size: 27.8 MB (27804550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1742b7e5e1e5bca675e7f251c9f6fe8778a1bb1548e5b418f8547277f14e2e33`  
		Last Modified: Wed, 17 Nov 2021 19:17:19 GMT  
		Size: 17.2 MB (17227026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ef5459771b89c49219d5c15641c7215faf156712422f01efee40ad955a52c5`  
		Last Modified: Wed, 17 Nov 2021 19:17:10 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5524d75cc2c74897404dae6de3a69d047ca4cc51c8b736de1dd47d163071049`  
		Last Modified: Wed, 24 Nov 2021 20:50:25 GMT  
		Size: 20.9 MB (20941381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea806f269473956d6c5b54454f99172fc77b585cb64755c74a5902f3fbcc388f`  
		Last Modified: Wed, 24 Nov 2021 20:50:22 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808c6b5af8ee5a5fbc2d8bb8135dbf023273179214bce2792f796fe88715770d`  
		Last Modified: Wed, 24 Nov 2021 21:40:56 GMT  
		Size: 21.2 MB (21204274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074b0bda43ffaf99bd7862cfb5666b4706661b86e0888e5acfd0b9435352e1bf`  
		Last Modified: Wed, 24 Nov 2021 21:40:50 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3543e7aff127e577f1a6ea76e9f22561c1f83c535b7d39d2029b3f741069f9b`  
		Last Modified: Wed, 24 Nov 2021 21:40:50 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7537b5afa25a253fa26f4fc8ad8d04292fb48305256f743f3a7bb5648d5f208`  
		Last Modified: Wed, 24 Nov 2021 21:40:50 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:95915295391c3c5984247067cb6657f0f4e5ea044b4c52f794d47590d3c7b56f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87837789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01d9264500ddcc8f3f9cb11c9738ba38cf5f05c311a64edb1575cb4548d6c5c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 03:30:22 GMT
ADD file:c0f8b5d4d419bef7a494df5330ecf7bbea3cbb6462308ca0b2f26771f125dea0 in / 
# Wed, 17 Nov 2021 03:30:29 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:17:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:17:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 13:17:28 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 14:18:19 GMT
ENV RUBY_MAJOR=2.6
# Wed, 17 Nov 2021 14:18:21 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 17 Nov 2021 14:18:23 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 17 Nov 2021 14:24:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 17 Nov 2021 14:24:47 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 17 Nov 2021 14:24:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 17 Nov 2021 14:24:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 14:25:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 17 Nov 2021 14:25:02 GMT
CMD ["irb"]
# Thu, 18 Nov 2021 12:55:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 18 Nov 2021 12:55:56 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 18 Nov 2021 12:56:01 GMT
ENV TINI_VERSION=0.18.0
# Thu, 18 Nov 2021 12:59:38 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 18 Nov 2021 12:59:50 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 18 Nov 2021 12:59:52 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 18 Nov 2021 12:59:52 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 18 Nov 2021 12:59:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 18 Nov 2021 13:00:00 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 18 Nov 2021 13:00:03 GMT
EXPOSE 24224 5140
# Thu, 18 Nov 2021 13:00:07 GMT
USER fluent
# Thu, 18 Nov 2021 13:00:12 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 18 Nov 2021 13:00:14 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:459de0a111d5c931674a5150ef4ae6bb1ffb1685380f4aafdba04a37d556c5de`  
		Last Modified: Wed, 17 Nov 2021 03:58:14 GMT  
		Size: 30.6 MB (30562278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4a8cb8add512175dbaeb682e1d37722eb039847e94d43b2c548f6bf9f4566`  
		Last Modified: Wed, 17 Nov 2021 14:30:35 GMT  
		Size: 12.7 MB (12705482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02accf8c69e0fb54236daa23b1409d80e215845f8d744672e8be1de6353c73f4`  
		Last Modified: Wed, 17 Nov 2021 14:30:32 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecde72085a62fc055b92d08be845488e745acea10ff923c9db7192bc696536f9`  
		Last Modified: Wed, 17 Nov 2021 14:35:36 GMT  
		Size: 22.0 MB (21985050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528aeb277a5e499d35f24f6a6cf6b7ff6d8081b0d8d6aebe5fd6ed9e1acc2ae9`  
		Last Modified: Wed, 17 Nov 2021 14:35:32 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d889167a6bdac835f4eda37dd4e41104a79cf847b7ec40a9a897bf51250d66c`  
		Last Modified: Thu, 18 Nov 2021 13:00:41 GMT  
		Size: 22.6 MB (22581887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4ae1c9d09e2fb95243a7b474becb9a242a5aa36fdf955bc6d0a1e954d89e62`  
		Last Modified: Thu, 18 Nov 2021 13:00:36 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ead0d83e706d394de56c9c6767f8579a8ed6d9ec3b90937ebec81392e01827`  
		Last Modified: Thu, 18 Nov 2021 13:00:36 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b66089533840caf7ab39440a1422305b22ba95dd3620deae2451391f6818577`  
		Last Modified: Thu, 18 Nov 2021 13:00:37 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:5b0029983a5113e7f0797e8c8df99585597d6648ed5bec9fcd18cac37bbb6e4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80419053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e318659054287dafbf9e4d2fffe4e3bf24143c13aefde8ca31b6e70676bc90e8`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:59 GMT
ADD file:3ff5fbc9c53cf76aad0fe0e1a525cb0bc0d70e8f2a3d5741dfb8b3b8a9448ffd in / 
# Wed, 17 Nov 2021 02:43:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:21:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:21:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 09:21:07 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:42:36 GMT
ENV RUBY_MAJOR=2.6
# Wed, 24 Nov 2021 20:13:56 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 24 Nov 2021 20:13:56 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 24 Nov 2021 20:15:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 20:15:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 20:15:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 20:15:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 20:15:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 20:15:34 GMT
CMD ["irb"]
# Wed, 24 Nov 2021 21:39:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 24 Nov 2021 21:39:43 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 24 Nov 2021 21:39:43 GMT
ENV TINI_VERSION=0.18.0
# Wed, 24 Nov 2021 21:40:58 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 24 Nov 2021 21:41:00 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 24 Nov 2021 21:41:00 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 24 Nov 2021 21:41:00 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 24 Nov 2021 21:41:00 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 24 Nov 2021 21:41:00 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 24 Nov 2021 21:41:01 GMT
EXPOSE 24224 5140
# Wed, 24 Nov 2021 21:41:01 GMT
USER fluent
# Wed, 24 Nov 2021 21:41:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 24 Nov 2021 21:41:01 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b8b917e61b3be882db10e68210f73caf5cc788bfb07aec0a659e30f4796b476b`  
		Last Modified: Wed, 17 Nov 2021 02:49:01 GMT  
		Size: 25.8 MB (25769063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e574c6d046371657ec033b78bc3df865890056f711b30df7505d0128446e36`  
		Last Modified: Wed, 17 Nov 2021 09:48:11 GMT  
		Size: 10.8 MB (10815243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bfb1613df50da70222f9b1cd395c4b509f6e6631cf6a13ce6c6b9c8c4cf181`  
		Last Modified: Wed, 17 Nov 2021 09:48:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373586c1d46c483775f8e0050fe4982f10b9ddfc251e549f639fafb1c3bb75ed`  
		Last Modified: Wed, 24 Nov 2021 20:26:33 GMT  
		Size: 21.6 MB (21644583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ab78d394ba7b06dcf2fd747295da98041460de5c7dc0bc3967843980ced8d2`  
		Last Modified: Wed, 24 Nov 2021 20:26:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c6173ab24577d30d0723847c55b4f1924137ab015e3fd7106d984b10e6e77e`  
		Last Modified: Wed, 24 Nov 2021 21:41:37 GMT  
		Size: 22.2 MB (22187081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd65e4fe334a299c24859ab60fe9645843c7e08842542336113a378587eb28e`  
		Last Modified: Wed, 24 Nov 2021 21:41:34 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eec492bbafa4db778db8834d624dfdf2a271cca32f5544712b7b8228e86eab6`  
		Last Modified: Wed, 24 Nov 2021 21:41:34 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3114d93a6beb021a9b347a6a5bea1ad2a6a1a1bcfcb341a32d06f827dc33b4`  
		Last Modified: Wed, 24 Nov 2021 21:41:34 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14.0-1.0`

```console
$ docker pull fluentd@sha256:3dee97712e6814f55e625c10ec00061ad0245ebc418c37fef10baa37acb5ea48
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
$ docker pull fluentd@sha256:65a6a197f958f1377eeb170c66127ad81e6658eb4afb37e34dd1ea29adc00969
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18399672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8230937f87367b64bce083b46594408cc94f1bc9eb3a30fe45a55c288e8c0a45`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:10:18 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 12 Nov 2021 17:10:18 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 12 Nov 2021 17:12:25 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 12 Nov 2021 17:12:27 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 12 Nov 2021 17:12:28 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 12 Nov 2021 17:12:28 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 12 Nov 2021 17:12:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 12 Nov 2021 17:12:29 GMT
ENV LD_PRELOAD=
# Fri, 12 Nov 2021 17:12:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 12 Nov 2021 17:12:30 GMT
EXPOSE 24224 5140
# Fri, 12 Nov 2021 17:12:30 GMT
USER fluent
# Fri, 12 Nov 2021 17:12:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 12 Nov 2021 17:12:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff475b9767d8c8b660254919cdacfb07d41726bcf6ae57bd82df1ab92964973`  
		Last Modified: Fri, 12 Nov 2021 17:13:19 GMT  
		Size: 15.8 MB (15764124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688a0000f32840ee0b24105fa7e0a8961a424e9cc972883a857a725d352294e0`  
		Last Modified: Fri, 12 Nov 2021 17:13:07 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bca9fcdd7bd010eb56f1658123023630d8a2feff9eb6e7dc663d84b97c1cac`  
		Last Modified: Fri, 12 Nov 2021 17:13:07 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cfca946685484b3ea43c9624c073dd8ae63bf180f0cbdba40ed2ed0a6d594c`  
		Last Modified: Fri, 12 Nov 2021 17:13:07 GMT  
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
$ docker pull fluentd@sha256:6dfdd776a8dd8b6655b7fc118a432b474931cd7101cb9d9791eb933d50f4e767
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18627613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8324bde6076998fe36358be5951135c71d7514c142da41074094b7e9e79a5606`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:46:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Nov 2021 05:46:04 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 13 Nov 2021 05:47:01 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 13 Nov 2021 05:47:02 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Nov 2021 05:47:02 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Nov 2021 05:47:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 13 Nov 2021 05:47:03 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Nov 2021 05:47:03 GMT
ENV LD_PRELOAD=
# Sat, 13 Nov 2021 05:47:03 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 13 Nov 2021 05:47:03 GMT
EXPOSE 24224 5140
# Sat, 13 Nov 2021 05:47:04 GMT
USER fluent
# Sat, 13 Nov 2021 05:47:04 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Nov 2021 05:47:04 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b4c0afc72421dadac58d84e5af4b2e3a16b7f2d6734b0749960a0f3a99fbe9`  
		Last Modified: Sat, 13 Nov 2021 05:47:36 GMT  
		Size: 15.8 MB (15796601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4345f72b9ac989cfe5a73d7da793eb81dae91292cb88e92ea863177fdbdbdc23`  
		Last Modified: Sat, 13 Nov 2021 05:47:33 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1e56be2212cf2bac7d78b5b74f00a84ff6f225959282ec73b07562770d737a`  
		Last Modified: Sat, 13 Nov 2021 05:47:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc8507a9023a335223baff561db76d3c4e74d11dc0a86396ceb2ab83a76a7cf`  
		Last Modified: Sat, 13 Nov 2021 05:47:33 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:8fd5d9e285f3fc0a115f2de1b8aa2d8dece14edbf48b5a1980a6a2437a70530f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19165522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33a2aab15001f20ad0220e97bc94fadc3ac1fcb19187c2898b3328461e0e440`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:25 GMT
ADD file:f7216323de17450e653f77c86d2c1e2e8ec01e1133e93f29c515761b3e9d8f7d in / 
# Fri, 12 Nov 2021 21:18:28 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:31:52 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 13 Nov 2021 15:31:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 13 Nov 2021 15:33:14 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 13 Nov 2021 15:33:25 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 13 Nov 2021 15:33:32 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 13 Nov 2021 15:33:38 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 13 Nov 2021 15:33:45 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 13 Nov 2021 15:33:56 GMT
ENV LD_PRELOAD=
# Sat, 13 Nov 2021 15:34:07 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Sat, 13 Nov 2021 15:34:09 GMT
EXPOSE 24224 5140
# Sat, 13 Nov 2021 15:34:15 GMT
USER fluent
# Sat, 13 Nov 2021 15:34:18 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 13 Nov 2021 15:34:20 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6729720a3e6b58511df148134bb67d786ad90f9fce1c02ba5bbfd31f33055fbe`  
		Last Modified: Fri, 12 Nov 2021 21:19:49 GMT  
		Size: 2.8 MB (2820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198dd1f78cd797f2648276619a592f94742f5b209730c5dd95e2f0ec0820a5de`  
		Last Modified: Sat, 13 Nov 2021 15:34:53 GMT  
		Size: 16.3 MB (16342800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df93171f11aee7e79e119605b6b629fe2b6b23a553e2496c1163d5b7c6fab289`  
		Last Modified: Sat, 13 Nov 2021 15:34:49 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d44d6ee555a88c35c0b2c281f2f52340e02388a29c35f5ea61f1081597fb442`  
		Last Modified: Sat, 13 Nov 2021 15:34:49 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9187a13c71c5c260b3b4bf04a227a36ecc837ceee1d0e1c191f8aa2844a7636e`  
		Last Modified: Sat, 13 Nov 2021 15:34:49 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:6044314a53964ecc154c09d49350727e8c6917de12bbc62c957ee363fb937a14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18799969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64f549dd1ad1b82e6a232731613dc468b569d4f9500433e6ef441ccc7634f12c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:44 GMT
ADD file:637f327c9b07758709ef7dbc42eb472c888d221acde89b1c3775553864334d5c in / 
# Fri, 12 Nov 2021 16:41:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:16:50 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 12 Nov 2021 22:16:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 12 Nov 2021 22:17:26 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 12 Nov 2021 22:17:27 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 12 Nov 2021 22:17:27 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 12 Nov 2021 22:17:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 12 Nov 2021 22:17:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 12 Nov 2021 22:17:28 GMT
ENV LD_PRELOAD=
# Fri, 12 Nov 2021 22:17:28 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Fri, 12 Nov 2021 22:17:28 GMT
EXPOSE 24224 5140
# Fri, 12 Nov 2021 22:17:28 GMT
USER fluent
# Fri, 12 Nov 2021 22:17:28 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 12 Nov 2021 22:17:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b872f056719bde6e6722091afb2a3376d720c69c142b91ac352050080dd79615`  
		Last Modified: Fri, 12 Nov 2021 16:42:54 GMT  
		Size: 2.6 MB (2611155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70e8f50864afa9912f5e959e79bff07cf414db20b131883f209b1ab81b6577`  
		Last Modified: Fri, 12 Nov 2021 22:18:11 GMT  
		Size: 16.2 MB (16186611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91cb6e8f074b6be6273edd016fb2ac5fbc2036973b56626990849083048622c`  
		Last Modified: Fri, 12 Nov 2021 22:18:00 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230dbc436d65d2c8a7d1fe391a46813c024611ebe5d8c72df6670e5cd501ac94`  
		Last Modified: Fri, 12 Nov 2021 22:18:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cdd6f6256dd88c8aa99df54e444c178b276b5db074a734ef1ff747cdc34597`  
		Last Modified: Fri, 12 Nov 2021 22:18:00 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14.0-debian-1.0`

```console
$ docker pull fluentd@sha256:4ec18d3436880613323f88f0007abf6008368fb7d021400f03f69da12a4a5a9c
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
$ docker pull fluentd@sha256:c57851f56a69cc832016bbd62a97161180e790292d8336e0475d13424298fa35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83226860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf117c13a521249553d25d5ba96d5f8636537e90df992e1baf4445a23cfc1e8`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 23:05:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 23:05:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 23:05:39 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 23:44:19 GMT
ENV RUBY_MAJOR=2.6
# Wed, 24 Nov 2021 21:50:40 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 24 Nov 2021 21:50:40 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 24 Nov 2021 21:53:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 21:53:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 21:53:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 21:53:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 21:53:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 21:53:34 GMT
CMD ["irb"]
# Wed, 24 Nov 2021 22:19:02 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 24 Nov 2021 22:19:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 24 Nov 2021 22:19:02 GMT
ENV TINI_VERSION=0.18.0
# Wed, 24 Nov 2021 22:20:35 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 24 Nov 2021 22:20:36 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 24 Nov 2021 22:20:37 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 24 Nov 2021 22:20:37 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 24 Nov 2021 22:20:37 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 24 Nov 2021 22:20:37 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 24 Nov 2021 22:20:38 GMT
EXPOSE 24224 5140
# Wed, 24 Nov 2021 22:20:38 GMT
USER fluent
# Wed, 24 Nov 2021 22:20:38 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 24 Nov 2021 22:20:38 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d04e01f945ee4b2edd0451f178f17023c43f67737d0372eb309e5c83b9bc3e0`  
		Last Modified: Wed, 17 Nov 2021 23:49:59 GMT  
		Size: 12.6 MB (12565151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272911037384bdfabca8cbdd7eebb7290e527e81caa0a3f775b71d09b39ca4e`  
		Last Modified: Wed, 17 Nov 2021 23:49:56 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56cef09a8db7d612f653a8e25e4bb0dceebb0b1497ddd21af00298d5e93c24b`  
		Last Modified: Wed, 24 Nov 2021 22:07:19 GMT  
		Size: 21.5 MB (21499331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40eeef25c87db5feb734fb0a2e380c17eb22b797214848e791efda47888ff4ea`  
		Last Modified: Wed, 24 Nov 2021 22:07:17 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba9558ac7af784bbfd90d3f752f8a874f0298b34bc9fede1fcb866aeade2049`  
		Last Modified: Wed, 24 Nov 2021 22:21:08 GMT  
		Size: 22.0 MB (22005612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64821a28ac7893f4f275b333c5ac92698304de193c3249ea074a0af50fe5eb3d`  
		Last Modified: Wed, 24 Nov 2021 22:21:05 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da5fdd0b3441ff237ea26216cb84a83ed049724c8f00e580ba56dadfd4c44d9`  
		Last Modified: Wed, 24 Nov 2021 22:21:05 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c24435612b28b4bbb27679cf8a6f16060e6d4ea6319c6b6d328a6b2c87e47d4`  
		Last Modified: Wed, 24 Nov 2021 22:21:05 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:bc41a711dd5a5fc04a034c0bf6142433ce3042c19d321e7d708b17a413c5dc9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77162983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a75543860b88eb6a9bdf04252bbab2d1b93d08448488781a18c49752e29beb4d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:51:39 GMT
ADD file:e580d4d2066301375327ea51dd8db3af956e5a465495bf09d69d6deec9b0bfae in / 
# Wed, 17 Nov 2021 02:51:40 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 20:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 20:53:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 20:53:28 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:48:32 GMT
ENV RUBY_MAJOR=2.6
# Wed, 24 Nov 2021 20:40:11 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 24 Nov 2021 20:40:11 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 24 Nov 2021 20:44:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 20:44:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 20:44:43 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 20:44:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 20:44:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 20:44:45 GMT
CMD ["irb"]
# Wed, 24 Nov 2021 21:15:20 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 24 Nov 2021 21:15:20 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 24 Nov 2021 21:15:21 GMT
ENV TINI_VERSION=0.18.0
# Wed, 24 Nov 2021 21:19:03 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 24 Nov 2021 21:19:05 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 24 Nov 2021 21:19:06 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 24 Nov 2021 21:19:07 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 24 Nov 2021 21:19:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 24 Nov 2021 21:19:08 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 24 Nov 2021 21:19:08 GMT
EXPOSE 24224 5140
# Wed, 24 Nov 2021 21:19:09 GMT
USER fluent
# Wed, 24 Nov 2021 21:19:09 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 24 Nov 2021 21:19:09 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:dba255a4b166bb02562ca152d0da236ba8f211de5bf9d79e35ee023b1fce203e`  
		Last Modified: Wed, 17 Nov 2021 03:07:41 GMT  
		Size: 24.9 MB (24886310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b58fbebb8e6e22b1601002ddb4252e30c3750edfb93b87424f6c1a971c665bf`  
		Last Modified: Wed, 17 Nov 2021 21:59:40 GMT  
		Size: 10.3 MB (10349405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484eb5c97eceafe50be8deba254566cb365fd68cb0baa2e5418ecece614c2728`  
		Last Modified: Wed, 17 Nov 2021 21:59:32 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec676eb68c8105a1bbcfa111e2ca4032620d833b9d631f6132e10639f5c19d7`  
		Last Modified: Wed, 24 Nov 2021 20:56:06 GMT  
		Size: 20.8 MB (20760191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8be7a1ab157424413f57ad1f9a8b2955b765ec396a8653269ee3caf0a1a3e6`  
		Last Modified: Wed, 24 Nov 2021 20:55:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6e520e83e562a3d3cd6629b78d08387043f70edf286ef9d5aa754125f6bff4`  
		Last Modified: Wed, 24 Nov 2021 21:19:47 GMT  
		Size: 21.2 MB (21163992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68873a214d96f189e75f75fc1e55bb22035eab00a8ab9ea081208170c7b996d9`  
		Last Modified: Wed, 24 Nov 2021 21:19:37 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52aa581a7bc242ce502645b7cdba851d1e8ae13667806ea0a7e78a39945da6b1`  
		Last Modified: Wed, 24 Nov 2021 21:19:37 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4324b996594c795a8883404590e95df53678e981705915fc18b76e4d9f012a08`  
		Last Modified: Wed, 24 Nov 2021 21:19:37 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:ec438c42d6e15e24ea4b88bb2b026a34533400ffdeb7f7b6a7b89d5e6c40a3e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74330352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8f4ecb4f0e62722f24d362f2c44a2194f64715cf15dd5970e8282d3c8dd3d8`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Thu, 18 Nov 2021 08:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 08:17:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 18 Nov 2021 08:17:06 GMT
ENV LANG=C.UTF-8
# Thu, 18 Nov 2021 09:11:05 GMT
ENV RUBY_MAJOR=2.6
# Thu, 18 Nov 2021 09:11:06 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 18 Nov 2021 09:11:06 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 18 Nov 2021 09:15:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 18 Nov 2021 09:15:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 18 Nov 2021 09:15:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 18 Nov 2021 09:15:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 09:15:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 18 Nov 2021 09:15:18 GMT
CMD ["irb"]
# Thu, 18 Nov 2021 19:54:34 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 18 Nov 2021 19:54:35 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 18 Nov 2021 19:54:35 GMT
ENV TINI_VERSION=0.18.0
# Thu, 18 Nov 2021 19:57:58 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 18 Nov 2021 19:58:00 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 18 Nov 2021 19:58:01 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 18 Nov 2021 19:58:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 18 Nov 2021 19:58:01 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 18 Nov 2021 19:58:02 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 18 Nov 2021 19:58:02 GMT
EXPOSE 24224 5140
# Thu, 18 Nov 2021 19:58:03 GMT
USER fluent
# Thu, 18 Nov 2021 19:58:03 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 18 Nov 2021 19:58:04 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c8e57706e11dcf2202a1ed28d022f7fe3daa306f06bf5311fee3d20b17f772`  
		Last Modified: Thu, 18 Nov 2021 09:24:19 GMT  
		Size: 9.9 MB (9872912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caad345207fbbb28e02d7546fe9ec9b203219b39a7b6fe1a2c55d63e665ce8dd`  
		Last Modified: Thu, 18 Nov 2021 09:24:12 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb93faf1d4d1280ed90b904594838922fe363b19f403a1b9f79ea35b777e723`  
		Last Modified: Thu, 18 Nov 2021 09:31:29 GMT  
		Size: 20.6 MB (20643872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0931e5d4868154d483cf1176a216b4308c09ff1d5974bdf06aa52e79249b1b`  
		Last Modified: Thu, 18 Nov 2021 09:31:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e539878792cda106f034ac7e02ef711041594f12de56d47458c5568cad6acbbb`  
		Last Modified: Thu, 18 Nov 2021 19:58:50 GMT  
		Size: 21.1 MB (21056132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97647d3c914de5d030739ff70fc64e3703751dfd13d7de38fd657681262011b1`  
		Last Modified: Thu, 18 Nov 2021 19:58:37 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22a479987c5051e73bde92407f288948b7c54336f19594dceefbbc9cc800952`  
		Last Modified: Thu, 18 Nov 2021 19:58:37 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c7889dd5809ea7a0b1a940cc38038d498b6c68bede760c0905d9f9f779ce4a`  
		Last Modified: Thu, 18 Nov 2021 19:58:37 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:46589db7e29b7a49f4538f3612707a9918d99e0cf68e512252c72e8f11b2affd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80111378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:431fcfb49cb266ad0046e48beff5b5b97543d556f9f7b7c11150f08fb18397dd`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:44 GMT
ADD file:b7921dd77c7620d46a18a4b5952557620210bf7ad9de20fe8e695a371188122a in / 
# Wed, 17 Nov 2021 02:40:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:31:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:31:01 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 09:31:02 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:46:01 GMT
ENV RUBY_MAJOR=2.6
# Wed, 24 Nov 2021 20:17:07 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 24 Nov 2021 20:17:08 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 24 Nov 2021 20:18:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 20:18:56 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 20:18:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 20:18:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 20:18:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 20:19:00 GMT
CMD ["irb"]
# Wed, 24 Nov 2021 21:47:16 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 24 Nov 2021 21:47:17 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 24 Nov 2021 21:47:18 GMT
ENV TINI_VERSION=0.18.0
# Wed, 24 Nov 2021 21:48:51 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 24 Nov 2021 21:48:52 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 24 Nov 2021 21:48:54 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 24 Nov 2021 21:48:55 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 24 Nov 2021 21:48:55 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 24 Nov 2021 21:48:56 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 24 Nov 2021 21:48:57 GMT
EXPOSE 24224 5140
# Wed, 24 Nov 2021 21:48:58 GMT
USER fluent
# Wed, 24 Nov 2021 21:48:59 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 24 Nov 2021 21:49:00 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:8ccb9871ed7bebcea8889b08e06fe5bd0116711ca7b110429b987475bf4d40e8`  
		Last Modified: Wed, 17 Nov 2021 02:48:07 GMT  
		Size: 25.9 MB (25923117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8443a8ec909433d7156b8dcbeaf77f4e53d6a44b253a3f03b95126547154d55`  
		Last Modified: Wed, 17 Nov 2021 09:51:43 GMT  
		Size: 11.3 MB (11261808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f57122fa0ffe176f788d35a4a8f12a76819fa3bab198ac16e26d2961047a1d`  
		Last Modified: Wed, 17 Nov 2021 09:51:41 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9af3c6e2dd6af17eb358df3a3e3cd87a3e9dbe81fdbc4bd90bfe81d5b0cc6a`  
		Last Modified: Wed, 24 Nov 2021 20:32:29 GMT  
		Size: 21.1 MB (21123634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc85b546d70296e57b6541cf114b3816a54cd2d35fd0a07fe5e4334043508fb`  
		Last Modified: Wed, 24 Nov 2021 20:32:26 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c73f9b02cbe564eb7ae928c329162c8fdbdfbb04a125ef161cbbe1c8dd6948`  
		Last Modified: Wed, 24 Nov 2021 21:49:31 GMT  
		Size: 21.8 MB (21799902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21b62dadabc40e3264770b9a186d24bf3a7ad43631bdbfbbdb58dfab5bb46b0`  
		Last Modified: Wed, 24 Nov 2021 21:49:28 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4eccd89838bb419f0adc04ff8a31da06ea8b490784daefa3b9fc4e4465b4cd`  
		Last Modified: Wed, 24 Nov 2021 21:49:28 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41d632b0b9770c06cfa6ac1c720d7e60d2b0d608b6a7b7f1b944c048934794a`  
		Last Modified: Wed, 24 Nov 2021 21:49:28 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:f979d525ae77379bdd3675812a1f167ad70fc5533a2a0c6c83ae032fe05149fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87180308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f5c356e59cc67837def744ca276120c2e3d24192b0935877ad111c01c64d9d5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:22 GMT
ADD file:2adea3474b7ebda2bf77361304ee3e6966a9118aafd8220b81c4027be1f4d583 in / 
# Wed, 17 Nov 2021 02:40:22 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 18:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 18:38:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 18:38:25 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 19:07:29 GMT
ENV RUBY_MAJOR=2.6
# Wed, 24 Nov 2021 20:29:53 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 24 Nov 2021 20:29:53 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 24 Nov 2021 20:32:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 20:32:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 20:32:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 20:32:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 20:32:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 20:32:48 GMT
CMD ["irb"]
# Wed, 24 Nov 2021 21:38:03 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 24 Nov 2021 21:38:03 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 24 Nov 2021 21:38:04 GMT
ENV TINI_VERSION=0.18.0
# Wed, 24 Nov 2021 21:40:15 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 24 Nov 2021 21:40:16 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 24 Nov 2021 21:40:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 24 Nov 2021 21:40:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 24 Nov 2021 21:40:18 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 24 Nov 2021 21:40:18 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 24 Nov 2021 21:40:18 GMT
EXPOSE 24224 5140
# Wed, 24 Nov 2021 21:40:18 GMT
USER fluent
# Wed, 24 Nov 2021 21:40:19 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 24 Nov 2021 21:40:19 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7af5c9e671306e395c50a515c7bbe33d6f418ea08535b01c884457f78114eb08`  
		Last Modified: Wed, 17 Nov 2021 02:48:49 GMT  
		Size: 27.8 MB (27804550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1742b7e5e1e5bca675e7f251c9f6fe8778a1bb1548e5b418f8547277f14e2e33`  
		Last Modified: Wed, 17 Nov 2021 19:17:19 GMT  
		Size: 17.2 MB (17227026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ef5459771b89c49219d5c15641c7215faf156712422f01efee40ad955a52c5`  
		Last Modified: Wed, 17 Nov 2021 19:17:10 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5524d75cc2c74897404dae6de3a69d047ca4cc51c8b736de1dd47d163071049`  
		Last Modified: Wed, 24 Nov 2021 20:50:25 GMT  
		Size: 20.9 MB (20941381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea806f269473956d6c5b54454f99172fc77b585cb64755c74a5902f3fbcc388f`  
		Last Modified: Wed, 24 Nov 2021 20:50:22 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808c6b5af8ee5a5fbc2d8bb8135dbf023273179214bce2792f796fe88715770d`  
		Last Modified: Wed, 24 Nov 2021 21:40:56 GMT  
		Size: 21.2 MB (21204274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074b0bda43ffaf99bd7862cfb5666b4706661b86e0888e5acfd0b9435352e1bf`  
		Last Modified: Wed, 24 Nov 2021 21:40:50 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3543e7aff127e577f1a6ea76e9f22561c1f83c535b7d39d2029b3f741069f9b`  
		Last Modified: Wed, 24 Nov 2021 21:40:50 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7537b5afa25a253fa26f4fc8ad8d04292fb48305256f743f3a7bb5648d5f208`  
		Last Modified: Wed, 24 Nov 2021 21:40:50 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:95915295391c3c5984247067cb6657f0f4e5ea044b4c52f794d47590d3c7b56f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87837789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01d9264500ddcc8f3f9cb11c9738ba38cf5f05c311a64edb1575cb4548d6c5c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 03:30:22 GMT
ADD file:c0f8b5d4d419bef7a494df5330ecf7bbea3cbb6462308ca0b2f26771f125dea0 in / 
# Wed, 17 Nov 2021 03:30:29 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:17:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:17:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 13:17:28 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 14:18:19 GMT
ENV RUBY_MAJOR=2.6
# Wed, 17 Nov 2021 14:18:21 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 17 Nov 2021 14:18:23 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 17 Nov 2021 14:24:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 17 Nov 2021 14:24:47 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 17 Nov 2021 14:24:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 17 Nov 2021 14:24:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 14:25:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 17 Nov 2021 14:25:02 GMT
CMD ["irb"]
# Thu, 18 Nov 2021 12:55:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 18 Nov 2021 12:55:56 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 18 Nov 2021 12:56:01 GMT
ENV TINI_VERSION=0.18.0
# Thu, 18 Nov 2021 12:59:38 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 18 Nov 2021 12:59:50 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 18 Nov 2021 12:59:52 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 18 Nov 2021 12:59:52 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 18 Nov 2021 12:59:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 18 Nov 2021 13:00:00 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 18 Nov 2021 13:00:03 GMT
EXPOSE 24224 5140
# Thu, 18 Nov 2021 13:00:07 GMT
USER fluent
# Thu, 18 Nov 2021 13:00:12 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 18 Nov 2021 13:00:14 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:459de0a111d5c931674a5150ef4ae6bb1ffb1685380f4aafdba04a37d556c5de`  
		Last Modified: Wed, 17 Nov 2021 03:58:14 GMT  
		Size: 30.6 MB (30562278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4a8cb8add512175dbaeb682e1d37722eb039847e94d43b2c548f6bf9f4566`  
		Last Modified: Wed, 17 Nov 2021 14:30:35 GMT  
		Size: 12.7 MB (12705482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02accf8c69e0fb54236daa23b1409d80e215845f8d744672e8be1de6353c73f4`  
		Last Modified: Wed, 17 Nov 2021 14:30:32 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecde72085a62fc055b92d08be845488e745acea10ff923c9db7192bc696536f9`  
		Last Modified: Wed, 17 Nov 2021 14:35:36 GMT  
		Size: 22.0 MB (21985050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528aeb277a5e499d35f24f6a6cf6b7ff6d8081b0d8d6aebe5fd6ed9e1acc2ae9`  
		Last Modified: Wed, 17 Nov 2021 14:35:32 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d889167a6bdac835f4eda37dd4e41104a79cf847b7ec40a9a897bf51250d66c`  
		Last Modified: Thu, 18 Nov 2021 13:00:41 GMT  
		Size: 22.6 MB (22581887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4ae1c9d09e2fb95243a7b474becb9a242a5aa36fdf955bc6d0a1e954d89e62`  
		Last Modified: Thu, 18 Nov 2021 13:00:36 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ead0d83e706d394de56c9c6767f8579a8ed6d9ec3b90937ebec81392e01827`  
		Last Modified: Thu, 18 Nov 2021 13:00:36 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b66089533840caf7ab39440a1422305b22ba95dd3620deae2451391f6818577`  
		Last Modified: Thu, 18 Nov 2021 13:00:37 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:5b0029983a5113e7f0797e8c8df99585597d6648ed5bec9fcd18cac37bbb6e4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80419053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e318659054287dafbf9e4d2fffe4e3bf24143c13aefde8ca31b6e70676bc90e8`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:59 GMT
ADD file:3ff5fbc9c53cf76aad0fe0e1a525cb0bc0d70e8f2a3d5741dfb8b3b8a9448ffd in / 
# Wed, 17 Nov 2021 02:43:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:21:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:21:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 09:21:07 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:42:36 GMT
ENV RUBY_MAJOR=2.6
# Wed, 24 Nov 2021 20:13:56 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 24 Nov 2021 20:13:56 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 24 Nov 2021 20:15:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 20:15:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 20:15:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 20:15:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 20:15:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 20:15:34 GMT
CMD ["irb"]
# Wed, 24 Nov 2021 21:39:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 24 Nov 2021 21:39:43 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 24 Nov 2021 21:39:43 GMT
ENV TINI_VERSION=0.18.0
# Wed, 24 Nov 2021 21:40:58 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 24 Nov 2021 21:41:00 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 24 Nov 2021 21:41:00 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 24 Nov 2021 21:41:00 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 24 Nov 2021 21:41:00 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 24 Nov 2021 21:41:00 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 24 Nov 2021 21:41:01 GMT
EXPOSE 24224 5140
# Wed, 24 Nov 2021 21:41:01 GMT
USER fluent
# Wed, 24 Nov 2021 21:41:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 24 Nov 2021 21:41:01 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b8b917e61b3be882db10e68210f73caf5cc788bfb07aec0a659e30f4796b476b`  
		Last Modified: Wed, 17 Nov 2021 02:49:01 GMT  
		Size: 25.8 MB (25769063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e574c6d046371657ec033b78bc3df865890056f711b30df7505d0128446e36`  
		Last Modified: Wed, 17 Nov 2021 09:48:11 GMT  
		Size: 10.8 MB (10815243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bfb1613df50da70222f9b1cd395c4b509f6e6631cf6a13ce6c6b9c8c4cf181`  
		Last Modified: Wed, 17 Nov 2021 09:48:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373586c1d46c483775f8e0050fe4982f10b9ddfc251e549f639fafb1c3bb75ed`  
		Last Modified: Wed, 24 Nov 2021 20:26:33 GMT  
		Size: 21.6 MB (21644583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ab78d394ba7b06dcf2fd747295da98041460de5c7dc0bc3967843980ced8d2`  
		Last Modified: Wed, 24 Nov 2021 20:26:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c6173ab24577d30d0723847c55b4f1924137ab015e3fd7106d984b10e6e77e`  
		Last Modified: Wed, 24 Nov 2021 21:41:37 GMT  
		Size: 22.2 MB (22187081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd65e4fe334a299c24859ab60fe9645843c7e08842542336113a378587eb28e`  
		Last Modified: Wed, 24 Nov 2021 21:41:34 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eec492bbafa4db778db8834d624dfdf2a271cca32f5544712b7b8228e86eab6`  
		Last Modified: Wed, 24 Nov 2021 21:41:34 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3114d93a6beb021a9b347a6a5bea1ad2a6a1a1bcfcb341a32d06f827dc33b4`  
		Last Modified: Wed, 24 Nov 2021 21:41:34 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
