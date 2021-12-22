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
$ docker pull fluentd@sha256:70a5ca7828bfc5473148f4bbaf1dba0f838ee1fa1cda97a52ba0d07cb8afcdbd
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
$ docker pull fluentd@sha256:f4e2cb7d59ff1c0119db38316248e2851301a3b7fbd1f293d8d74833c5914c99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83226897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c651a62eb3ac4f9ba3a94f3dc08ea5ccb7b2da7ff1b074ca3cfc71dfa4b635b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 16:33:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 16:34:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 02 Dec 2021 16:34:00 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 17:23:57 GMT
ENV RUBY_MAJOR=2.6
# Thu, 02 Dec 2021 17:23:57 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 02 Dec 2021 17:23:57 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 02 Dec 2021 17:28:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 02 Dec 2021 17:28:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 02 Dec 2021 17:28:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 02 Dec 2021 17:28:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 17:28:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 02 Dec 2021 17:28:30 GMT
CMD ["irb"]
# Fri, 03 Dec 2021 20:15:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 03 Dec 2021 20:15:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 03 Dec 2021 20:15:51 GMT
ENV TINI_VERSION=0.18.0
# Fri, 03 Dec 2021 20:17:20 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 03 Dec 2021 20:17:21 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 03 Dec 2021 20:17:21 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 03 Dec 2021 20:17:21 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 03 Dec 2021 20:17:22 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 03 Dec 2021 20:17:22 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 03 Dec 2021 20:17:22 GMT
EXPOSE 24224 5140
# Fri, 03 Dec 2021 20:17:22 GMT
USER fluent
# Fri, 03 Dec 2021 20:17:22 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 03 Dec 2021 20:17:23 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90624b6090464f48417857b7235f0e54f5ee684d286beb9fbae0d710e785ad9d`  
		Last Modified: Thu, 02 Dec 2021 17:31:27 GMT  
		Size: 12.6 MB (12565241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e61194650215f6a06f21d197f04bd7bd30adcfec50d4a440007d025f5ce5a00`  
		Last Modified: Thu, 02 Dec 2021 17:31:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9759e3fcced8c41f62c3d81efdf9cde1b6745597f807981777e074b236336140`  
		Last Modified: Thu, 02 Dec 2021 17:35:48 GMT  
		Size: 21.5 MB (21499060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87aeecf53cc3a8f131775501d890e91b9a503dd655a85c503dc8886aac51e3c4`  
		Last Modified: Thu, 02 Dec 2021 17:35:45 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b203d149ab77f6dc5283c13db52d824675783ab8f322356abbb460644b1b6c`  
		Last Modified: Fri, 03 Dec 2021 20:17:42 GMT  
		Size: 22.0 MB (22005788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97d5fe2a854aa7a94018d87f50a3a3b43f9552acb6f6248432f28f35e3e23a1`  
		Last Modified: Fri, 03 Dec 2021 20:17:39 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bfd4a34cd0431187994ef8964e6dee5c71d995cabc2e6cfc655dffa3e9dd4a`  
		Last Modified: Fri, 03 Dec 2021 20:17:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649449a3cc2c0a571eb27b73aac98b60731382d8d864e43e6385b2e38abf695b`  
		Last Modified: Fri, 03 Dec 2021 20:17:39 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:fb087c7facb4bc19de0e91afc8beaeaa334bcf013bc4a391f9933592a23d54ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77163467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8962f16284b87cebed85ae5a45a83d73c32eb59410841b91a20a62a806bd97b0`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 02 Dec 2021 02:51:44 GMT
ADD file:b509d9889433e2e1b4e7d30f6a1461c93f9c6a2a6f60e1802710cbc20e7a0e81 in / 
# Thu, 02 Dec 2021 02:51:46 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 18:29:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 18:29:47 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 02 Dec 2021 18:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 19:26:22 GMT
ENV RUBY_MAJOR=2.6
# Thu, 02 Dec 2021 19:26:23 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 02 Dec 2021 19:26:23 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 02 Dec 2021 19:31:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 02 Dec 2021 19:31:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 02 Dec 2021 19:31:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 02 Dec 2021 19:31:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 19:31:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 02 Dec 2021 19:31:04 GMT
CMD ["irb"]
# Fri, 03 Dec 2021 12:00:20 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 03 Dec 2021 12:00:21 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 03 Dec 2021 12:00:21 GMT
ENV TINI_VERSION=0.18.0
# Fri, 03 Dec 2021 12:04:11 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 03 Dec 2021 12:04:13 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 03 Dec 2021 12:04:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 03 Dec 2021 12:04:14 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 03 Dec 2021 12:04:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 03 Dec 2021 12:04:15 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 03 Dec 2021 12:04:16 GMT
EXPOSE 24224 5140
# Fri, 03 Dec 2021 12:04:16 GMT
USER fluent
# Fri, 03 Dec 2021 12:04:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 03 Dec 2021 12:04:17 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6f8ed9eedee034be125ab31b8087fb60cf54bd4085e7e2dfbdc92ccae717fa06`  
		Last Modified: Thu, 02 Dec 2021 03:10:47 GMT  
		Size: 24.9 MB (24886215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1f479fa4a3748f0fef5a366b8d0fde6335efae4c82205ee39a0251f5268b1f`  
		Last Modified: Thu, 02 Dec 2021 19:37:33 GMT  
		Size: 10.3 MB (10349336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8304cc64213c19d90db6ca4c7b70875f05b7b6254e245602d1c0ea73c58525d4`  
		Last Modified: Thu, 02 Dec 2021 19:37:25 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f5114854aab1938b283522eef2f2e4e603b668451820af9832686b2a8d12c2`  
		Last Modified: Thu, 02 Dec 2021 19:44:02 GMT  
		Size: 20.8 MB (20760847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885e50742b080cdbb256a61c8ae944b59f4328b410347aecfc64f883961ad38b`  
		Last Modified: Thu, 02 Dec 2021 19:43:53 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f56870dfd4d0b927bfaab604650cb65a0973fde92f02862e44ee097f8dc711`  
		Last Modified: Fri, 03 Dec 2021 12:04:51 GMT  
		Size: 21.2 MB (21163990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf3e006ed2660f48a655796f12c723cc078eb7c5e48d71084d9d125b2d3915`  
		Last Modified: Fri, 03 Dec 2021 12:04:38 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc96a1d921f84da070bf09bcd95f732fcfc14034169b674df8c089af28cef47`  
		Last Modified: Fri, 03 Dec 2021 12:04:38 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba4a1d247c4ccb74a1174f2e2a31c4c37c9a3413ded5caf54ace93495f1f53e`  
		Last Modified: Fri, 03 Dec 2021 12:04:38 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:cd365ecdfbe7de785438e1134de3962cb81fd6773f92cb6ab890e4a9b4e7cdc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74361786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3792aaedd9759862599dc233bb4b5ca565bf7dfb27cc161deedfd3335113dc84`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 02 Dec 2021 09:06:21 GMT
ADD file:7b30d743b30e84b21888f23cb7f266caba09db98b7a4c8800abebcf03d28c01d in / 
# Thu, 02 Dec 2021 09:06:22 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 17:30:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 17:30:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Dec 2021 17:30:54 GMT
ENV LANG=C.UTF-8
# Fri, 03 Dec 2021 18:25:57 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Dec 2021 18:25:58 GMT
ENV RUBY_VERSION=2.6.9
# Fri, 03 Dec 2021 18:25:58 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Fri, 03 Dec 2021 18:30:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Dec 2021 18:30:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Dec 2021 18:30:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Dec 2021 18:30:20 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 18:30:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Dec 2021 18:30:22 GMT
CMD ["irb"]
# Sat, 04 Dec 2021 13:06:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 04 Dec 2021 13:06:55 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 04 Dec 2021 13:06:55 GMT
ENV TINI_VERSION=0.18.0
# Sat, 04 Dec 2021 13:10:22 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 04 Dec 2021 13:10:25 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 04 Dec 2021 13:10:25 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 04 Dec 2021 13:10:26 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 04 Dec 2021 13:10:26 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 04 Dec 2021 13:10:26 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 04 Dec 2021 13:10:27 GMT
EXPOSE 24224 5140
# Sat, 04 Dec 2021 13:10:27 GMT
USER fluent
# Sat, 04 Dec 2021 13:10:28 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 04 Dec 2021 13:10:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2aa85085c98821a25a3058f7fc2c6427064f2228ea8eac904e9e7db4dbdaa01a`  
		Last Modified: Thu, 02 Dec 2021 09:22:26 GMT  
		Size: 22.8 MB (22754365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1787793a37de8674853036139b8cf3e6e54fd257e9b3ab8bba1175936ee679a1`  
		Last Modified: Fri, 03 Dec 2021 18:39:48 GMT  
		Size: 9.9 MB (9872859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db8fa492ac8e0b37299aa54782addae92722be6c2556d52ea0cac13628daf48`  
		Last Modified: Fri, 03 Dec 2021 18:39:41 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ec4eaf26d10fe9f8d194a2e4be3c5eeb4be9dcff43764fd50525a047660c44`  
		Last Modified: Fri, 03 Dec 2021 18:48:12 GMT  
		Size: 20.7 MB (20672372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3fd9faf09387da0c08147c32bda36b125afcd439b82ae807a435bf942ba1cb`  
		Last Modified: Fri, 03 Dec 2021 18:48:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dd07ff9a63af31eaf54520e07933583ddae004c2c9e875f40381b485a72d21`  
		Last Modified: Sat, 04 Dec 2021 13:11:08 GMT  
		Size: 21.1 MB (21059112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1dea72de2c2db67126d825d66f36152c5426b8f008fa6f413a6c9aeac3a129`  
		Last Modified: Sat, 04 Dec 2021 13:10:55 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716a652b22b831eb9525de54552d99c89bd728cf75b8df5369b785cc030db608`  
		Last Modified: Sat, 04 Dec 2021 13:10:55 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75635a05ae6821be2004fd073860603016298cf22cf81fed86c3e4030556dcd8`  
		Last Modified: Sat, 04 Dec 2021 13:10:55 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:3e751cecaa6634cefdf80c05880592708235fcf08b06de8a6b354c312d919fd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80111639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b14b6d5f8a0b0b86afdd30a7f5b6e11b9ffc06c97d0e0f3a03a00978593b2929`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:46:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 13:46:11 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 14:10:29 GMT
ENV RUBY_MAJOR=2.6
# Tue, 21 Dec 2021 14:10:29 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 21 Dec 2021 14:10:30 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 21 Dec 2021 14:12:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Dec 2021 14:12:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Dec 2021 14:12:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Dec 2021 14:12:20 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 14:12:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 21 Dec 2021 14:12:22 GMT
CMD ["irb"]
# Wed, 22 Dec 2021 03:51:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 22 Dec 2021 03:51:00 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 22 Dec 2021 03:51:01 GMT
ENV TINI_VERSION=0.18.0
# Wed, 22 Dec 2021 03:52:24 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 22 Dec 2021 03:52:25 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 22 Dec 2021 03:52:26 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 22 Dec 2021 03:52:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 22 Dec 2021 03:52:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 22 Dec 2021 03:52:28 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 22 Dec 2021 03:52:29 GMT
EXPOSE 24224 5140
# Wed, 22 Dec 2021 03:52:30 GMT
USER fluent
# Wed, 22 Dec 2021 03:52:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 22 Dec 2021 03:52:32 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df957e92572da886c36ceee88919e1780eaacc4ffe81dba01dadcc234d3b4636`  
		Last Modified: Tue, 21 Dec 2021 14:16:30 GMT  
		Size: 11.3 MB (11261786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f498124153b35570162f92f7962aa50fd000b9fb69e0789e5e1127c014cca38`  
		Last Modified: Tue, 21 Dec 2021 14:16:28 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a3ef5a630f83e12655230af7f4d10ac168fc0701920fe0f2e360b4abf291f1`  
		Last Modified: Tue, 21 Dec 2021 14:20:59 GMT  
		Size: 21.1 MB (21124034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d482d015a092f5c5f5b629b7feba2fdda0c10846fed360fe6451df8002b392`  
		Last Modified: Tue, 21 Dec 2021 14:20:56 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c328f8ceb37104a193ea29ca76ab226e273186b1c468ae21149e3630767edb`  
		Last Modified: Wed, 22 Dec 2021 03:53:00 GMT  
		Size: 21.8 MB (21799763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530ba1892cb3ef185de3ad2e5d3296354de65ba4a2c05b89a0291fe88133289a`  
		Last Modified: Wed, 22 Dec 2021 03:52:57 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0521121f54a1b28056a0d2d438a7c2d21e3d1f789080e85a90354165922e00`  
		Last Modified: Wed, 22 Dec 2021 03:52:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117365658371b2f9d3f2adcfe3db27dc96e3e303814556facd47e755ab325f2e`  
		Last Modified: Wed, 22 Dec 2021 03:52:57 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:7bc5db914344425078ea36a7a2e592d6c3e65d924ee6f317bdf294a33df52e87
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87180681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c25bfc2846e7607c175bf6b3fd90e0b924db910601cea8059ee188ab66f38ce`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 20:07:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 20:07:40 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 20:07:41 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 21:02:00 GMT
ENV RUBY_MAJOR=2.6
# Tue, 21 Dec 2021 21:02:01 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 21 Dec 2021 21:02:01 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 21 Dec 2021 21:06:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Dec 2021 21:06:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Dec 2021 21:06:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Dec 2021 21:06:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 21:06:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 21 Dec 2021 21:06:52 GMT
CMD ["irb"]
# Wed, 22 Dec 2021 10:02:44 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 22 Dec 2021 10:02:45 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 22 Dec 2021 10:02:45 GMT
ENV TINI_VERSION=0.18.0
# Wed, 22 Dec 2021 10:04:27 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 22 Dec 2021 10:04:28 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 22 Dec 2021 10:04:29 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 22 Dec 2021 10:04:29 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 22 Dec 2021 10:04:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 22 Dec 2021 10:04:29 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 22 Dec 2021 10:04:30 GMT
EXPOSE 24224 5140
# Wed, 22 Dec 2021 10:04:30 GMT
USER fluent
# Wed, 22 Dec 2021 10:04:30 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 22 Dec 2021 10:04:30 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1066d2070153fbad5494fe979ad171707d9eab3b32f3fd90979531049d8b27`  
		Last Modified: Tue, 21 Dec 2021 21:13:06 GMT  
		Size: 17.2 MB (17227036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5157ccdbc4b0d00d4ffd83478d4385983d9d4f8c22959750d2de032fa02a762d`  
		Last Modified: Tue, 21 Dec 2021 21:12:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d31ac662dfab3810c94a2f54d83a6b00952df811a3830c497d694013ac2c58`  
		Last Modified: Tue, 21 Dec 2021 21:19:01 GMT  
		Size: 20.9 MB (20941790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5912b3a1ff5cce1ac5778138fd2f43b02157837e653685699edc98c49eb381a`  
		Last Modified: Tue, 21 Dec 2021 21:18:58 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbeffd0be92c865380286e4ab5b5f786fc9755f7b5e88fca0ee5346875945283`  
		Last Modified: Wed, 22 Dec 2021 10:05:00 GMT  
		Size: 21.2 MB (21204209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225daa9efae801281529f36cb084a2f027a1aca199a75f02fd39814e58e29c3e`  
		Last Modified: Wed, 22 Dec 2021 10:04:55 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b441b9d8e0b9e011ec55fd3944a4a8068903eed9a40164f3b1184254134f47`  
		Last Modified: Wed, 22 Dec 2021 10:04:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957155b3dad1d80709391f91ceaadba109c0e2201c7233d4aadfeb69e1d2ffe7`  
		Last Modified: Wed, 22 Dec 2021 10:04:55 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:64194d2506feca34168225d5cb01ba7847c4fc5fc4c79772d7f0a01f428c7192
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87879267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2893e3b93f0bbfd84a21a57d5c776b2c64d70a6cbc02b34be3b3cb8c899fe7ba`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 02 Dec 2021 07:22:12 GMT
ADD file:b9b5697bc2dd3ded7a158d973abc939cc5d197f1f0d9ff1fa8b3db3b7906de7a in / 
# Thu, 02 Dec 2021 07:22:18 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 07:58:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 07:58:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Dec 2021 07:58:41 GMT
ENV LANG=C.UTF-8
# Fri, 03 Dec 2021 09:09:13 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Dec 2021 09:09:15 GMT
ENV RUBY_VERSION=2.6.9
# Fri, 03 Dec 2021 09:09:17 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Fri, 03 Dec 2021 09:16:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Dec 2021 09:16:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Dec 2021 09:16:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Dec 2021 09:16:38 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 09:16:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Dec 2021 09:16:44 GMT
CMD ["irb"]
# Sat, 04 Dec 2021 02:09:22 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 04 Dec 2021 02:09:23 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 04 Dec 2021 02:09:25 GMT
ENV TINI_VERSION=0.18.0
# Sat, 04 Dec 2021 02:13:08 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 04 Dec 2021 02:13:15 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 04 Dec 2021 02:13:16 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 04 Dec 2021 02:13:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 04 Dec 2021 02:13:18 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 04 Dec 2021 02:13:20 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 04 Dec 2021 02:13:22 GMT
EXPOSE 24224 5140
# Sat, 04 Dec 2021 02:13:23 GMT
USER fluent
# Sat, 04 Dec 2021 02:13:25 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 04 Dec 2021 02:13:27 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:da5263f5d65ecaf2dcd9400908302b4c477c13afa707110e4d85b4b946e9a3ae`  
		Last Modified: Thu, 02 Dec 2021 07:32:41 GMT  
		Size: 30.6 MB (30562306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5617a28440e343caa8dd30cc324bdd708ebe1f964ec11fd26f132068879ed4e`  
		Last Modified: Fri, 03 Dec 2021 09:21:11 GMT  
		Size: 12.7 MB (12705552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96de5a56dc2e1824f750d121f9d5244c505b423f1f8a35f736ff60ef67908f0b`  
		Last Modified: Fri, 03 Dec 2021 09:21:08 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d842a33f7d39fa300527a467e6bba3ff5e53e4d9d6f4df2996576cf1642efa14`  
		Last Modified: Fri, 03 Dec 2021 09:26:06 GMT  
		Size: 22.0 MB (22023323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03648056dfafebc33cc627e0af6017e5566f34b428ed9e1c303f4c5c82b1ca41`  
		Last Modified: Fri, 03 Dec 2021 09:26:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c3c72a12d41f318d5779e85bbbf449bad44ed9e5a7ad69e5146310522f6acc`  
		Last Modified: Sat, 04 Dec 2021 02:13:53 GMT  
		Size: 22.6 MB (22584998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e837d43a9b725089dff53fdf8c2afb40d3fe5ff825574a7afc89628e83c09006`  
		Last Modified: Sat, 04 Dec 2021 02:13:49 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7940e8b758c81281c247c3832bf8ab53cebeb5ad5c55be6ccac845b8f7318`  
		Last Modified: Sat, 04 Dec 2021 02:13:49 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffc6e91fb84cbe49fc5de0107eb8c2a5a266f6949abff341300e65c07c8725d`  
		Last Modified: Sat, 04 Dec 2021 02:13:49 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:15fde5998f955c71d60cf4513932c2dac854ba1e975b1d0c5c5e43f55399f1ca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80418926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aa22ed864620743d477ffee21b6f727416b62ec28aa23d48d22821e1014bf30`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:57 GMT
ADD file:33e37861eefa46f6e5f7f4967ce8ae3167e28bc817c3c71ff90a3d51e2376a0f in / 
# Tue, 21 Dec 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:50:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:50:51 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 10:50:51 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 11:13:38 GMT
ENV RUBY_MAJOR=2.6
# Tue, 21 Dec 2021 11:13:38 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 21 Dec 2021 11:13:38 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 21 Dec 2021 11:15:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Dec 2021 11:15:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Dec 2021 11:15:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Dec 2021 11:15:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 11:15:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 21 Dec 2021 11:15:13 GMT
CMD ["irb"]
# Tue, 21 Dec 2021 19:08:18 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Dec 2021 19:08:18 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 21 Dec 2021 19:08:18 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Dec 2021 19:09:31 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 21 Dec 2021 19:09:33 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Dec 2021 19:09:33 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Dec 2021 19:09:33 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Dec 2021 19:09:33 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Dec 2021 19:09:33 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Dec 2021 19:09:33 GMT
EXPOSE 24224 5140
# Tue, 21 Dec 2021 19:09:33 GMT
USER fluent
# Tue, 21 Dec 2021 19:09:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Dec 2021 19:09:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:10979941d091693f28e3dc033cc6ca88996acf42a0aace27ad85fbd894945e20`  
		Last Modified: Tue, 21 Dec 2021 01:48:51 GMT  
		Size: 25.8 MB (25769051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a6f3c4642cf35166efc3bc51ae42418989834c8eca28809948ada296bb9c5`  
		Last Modified: Tue, 21 Dec 2021 11:19:14 GMT  
		Size: 10.8 MB (10815241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c51d7f208d075afa3e35cffb33a4058bc2e6b09617649fda7a7cd8522e52308`  
		Last Modified: Tue, 21 Dec 2021 11:19:12 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3583c6a7801e70c598ceeaa29d28a8b10ca7ed50621ad0bb0a532073490164`  
		Last Modified: Tue, 21 Dec 2021 11:22:22 GMT  
		Size: 21.6 MB (21644657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3860c73eac66c9c46296dd704b1cb3012f7b7b882323b3bfdc4b17c1e35d7b84`  
		Last Modified: Tue, 21 Dec 2021 11:22:20 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c84bf6f760ca89f215e4de174cf90bdfdab55b57d4e4d9f1fe91031dc78fe`  
		Last Modified: Tue, 21 Dec 2021 19:10:11 GMT  
		Size: 22.2 MB (22186889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2229bae05d587e80d19d20b6f204ed4bb286f8b9503cd7cb523cb967b1f0afc4`  
		Last Modified: Tue, 21 Dec 2021 19:10:08 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d54fcdf40517dc3b1b49c5018c0ce24b7effeaa185dd951294523810efec81`  
		Last Modified: Tue, 21 Dec 2021 19:10:09 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f2fcc7ca912dcfb1df196696c5db99d6ef78b85c944c614608651408e9cd9`  
		Last Modified: Tue, 21 Dec 2021 19:10:08 GMT  
		Size: 457.0 B  
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
$ docker pull fluentd@sha256:70a5ca7828bfc5473148f4bbaf1dba0f838ee1fa1cda97a52ba0d07cb8afcdbd
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
$ docker pull fluentd@sha256:f4e2cb7d59ff1c0119db38316248e2851301a3b7fbd1f293d8d74833c5914c99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83226897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c651a62eb3ac4f9ba3a94f3dc08ea5ccb7b2da7ff1b074ca3cfc71dfa4b635b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 16:33:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 16:34:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 02 Dec 2021 16:34:00 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 17:23:57 GMT
ENV RUBY_MAJOR=2.6
# Thu, 02 Dec 2021 17:23:57 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 02 Dec 2021 17:23:57 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 02 Dec 2021 17:28:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 02 Dec 2021 17:28:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 02 Dec 2021 17:28:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 02 Dec 2021 17:28:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 17:28:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 02 Dec 2021 17:28:30 GMT
CMD ["irb"]
# Fri, 03 Dec 2021 20:15:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 03 Dec 2021 20:15:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 03 Dec 2021 20:15:51 GMT
ENV TINI_VERSION=0.18.0
# Fri, 03 Dec 2021 20:17:20 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 03 Dec 2021 20:17:21 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 03 Dec 2021 20:17:21 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 03 Dec 2021 20:17:21 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 03 Dec 2021 20:17:22 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 03 Dec 2021 20:17:22 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 03 Dec 2021 20:17:22 GMT
EXPOSE 24224 5140
# Fri, 03 Dec 2021 20:17:22 GMT
USER fluent
# Fri, 03 Dec 2021 20:17:22 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 03 Dec 2021 20:17:23 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90624b6090464f48417857b7235f0e54f5ee684d286beb9fbae0d710e785ad9d`  
		Last Modified: Thu, 02 Dec 2021 17:31:27 GMT  
		Size: 12.6 MB (12565241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e61194650215f6a06f21d197f04bd7bd30adcfec50d4a440007d025f5ce5a00`  
		Last Modified: Thu, 02 Dec 2021 17:31:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9759e3fcced8c41f62c3d81efdf9cde1b6745597f807981777e074b236336140`  
		Last Modified: Thu, 02 Dec 2021 17:35:48 GMT  
		Size: 21.5 MB (21499060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87aeecf53cc3a8f131775501d890e91b9a503dd655a85c503dc8886aac51e3c4`  
		Last Modified: Thu, 02 Dec 2021 17:35:45 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b203d149ab77f6dc5283c13db52d824675783ab8f322356abbb460644b1b6c`  
		Last Modified: Fri, 03 Dec 2021 20:17:42 GMT  
		Size: 22.0 MB (22005788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97d5fe2a854aa7a94018d87f50a3a3b43f9552acb6f6248432f28f35e3e23a1`  
		Last Modified: Fri, 03 Dec 2021 20:17:39 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bfd4a34cd0431187994ef8964e6dee5c71d995cabc2e6cfc655dffa3e9dd4a`  
		Last Modified: Fri, 03 Dec 2021 20:17:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649449a3cc2c0a571eb27b73aac98b60731382d8d864e43e6385b2e38abf695b`  
		Last Modified: Fri, 03 Dec 2021 20:17:39 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:fb087c7facb4bc19de0e91afc8beaeaa334bcf013bc4a391f9933592a23d54ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77163467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8962f16284b87cebed85ae5a45a83d73c32eb59410841b91a20a62a806bd97b0`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 02 Dec 2021 02:51:44 GMT
ADD file:b509d9889433e2e1b4e7d30f6a1461c93f9c6a2a6f60e1802710cbc20e7a0e81 in / 
# Thu, 02 Dec 2021 02:51:46 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 18:29:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 18:29:47 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 02 Dec 2021 18:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 19:26:22 GMT
ENV RUBY_MAJOR=2.6
# Thu, 02 Dec 2021 19:26:23 GMT
ENV RUBY_VERSION=2.6.9
# Thu, 02 Dec 2021 19:26:23 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Thu, 02 Dec 2021 19:31:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 02 Dec 2021 19:31:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 02 Dec 2021 19:31:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 02 Dec 2021 19:31:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 19:31:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 02 Dec 2021 19:31:04 GMT
CMD ["irb"]
# Fri, 03 Dec 2021 12:00:20 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 03 Dec 2021 12:00:21 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Fri, 03 Dec 2021 12:00:21 GMT
ENV TINI_VERSION=0.18.0
# Fri, 03 Dec 2021 12:04:11 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Fri, 03 Dec 2021 12:04:13 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 03 Dec 2021 12:04:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 03 Dec 2021 12:04:14 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 03 Dec 2021 12:04:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 03 Dec 2021 12:04:15 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 03 Dec 2021 12:04:16 GMT
EXPOSE 24224 5140
# Fri, 03 Dec 2021 12:04:16 GMT
USER fluent
# Fri, 03 Dec 2021 12:04:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 03 Dec 2021 12:04:17 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6f8ed9eedee034be125ab31b8087fb60cf54bd4085e7e2dfbdc92ccae717fa06`  
		Last Modified: Thu, 02 Dec 2021 03:10:47 GMT  
		Size: 24.9 MB (24886215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1f479fa4a3748f0fef5a366b8d0fde6335efae4c82205ee39a0251f5268b1f`  
		Last Modified: Thu, 02 Dec 2021 19:37:33 GMT  
		Size: 10.3 MB (10349336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8304cc64213c19d90db6ca4c7b70875f05b7b6254e245602d1c0ea73c58525d4`  
		Last Modified: Thu, 02 Dec 2021 19:37:25 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f5114854aab1938b283522eef2f2e4e603b668451820af9832686b2a8d12c2`  
		Last Modified: Thu, 02 Dec 2021 19:44:02 GMT  
		Size: 20.8 MB (20760847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885e50742b080cdbb256a61c8ae944b59f4328b410347aecfc64f883961ad38b`  
		Last Modified: Thu, 02 Dec 2021 19:43:53 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f56870dfd4d0b927bfaab604650cb65a0973fde92f02862e44ee097f8dc711`  
		Last Modified: Fri, 03 Dec 2021 12:04:51 GMT  
		Size: 21.2 MB (21163990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf3e006ed2660f48a655796f12c723cc078eb7c5e48d71084d9d125b2d3915`  
		Last Modified: Fri, 03 Dec 2021 12:04:38 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc96a1d921f84da070bf09bcd95f732fcfc14034169b674df8c089af28cef47`  
		Last Modified: Fri, 03 Dec 2021 12:04:38 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba4a1d247c4ccb74a1174f2e2a31c4c37c9a3413ded5caf54ace93495f1f53e`  
		Last Modified: Fri, 03 Dec 2021 12:04:38 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:cd365ecdfbe7de785438e1134de3962cb81fd6773f92cb6ab890e4a9b4e7cdc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74361786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3792aaedd9759862599dc233bb4b5ca565bf7dfb27cc161deedfd3335113dc84`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 02 Dec 2021 09:06:21 GMT
ADD file:7b30d743b30e84b21888f23cb7f266caba09db98b7a4c8800abebcf03d28c01d in / 
# Thu, 02 Dec 2021 09:06:22 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 17:30:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 17:30:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Dec 2021 17:30:54 GMT
ENV LANG=C.UTF-8
# Fri, 03 Dec 2021 18:25:57 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Dec 2021 18:25:58 GMT
ENV RUBY_VERSION=2.6.9
# Fri, 03 Dec 2021 18:25:58 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Fri, 03 Dec 2021 18:30:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Dec 2021 18:30:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Dec 2021 18:30:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Dec 2021 18:30:20 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 18:30:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Dec 2021 18:30:22 GMT
CMD ["irb"]
# Sat, 04 Dec 2021 13:06:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 04 Dec 2021 13:06:55 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 04 Dec 2021 13:06:55 GMT
ENV TINI_VERSION=0.18.0
# Sat, 04 Dec 2021 13:10:22 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 04 Dec 2021 13:10:25 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 04 Dec 2021 13:10:25 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 04 Dec 2021 13:10:26 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 04 Dec 2021 13:10:26 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 04 Dec 2021 13:10:26 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 04 Dec 2021 13:10:27 GMT
EXPOSE 24224 5140
# Sat, 04 Dec 2021 13:10:27 GMT
USER fluent
# Sat, 04 Dec 2021 13:10:28 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 04 Dec 2021 13:10:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2aa85085c98821a25a3058f7fc2c6427064f2228ea8eac904e9e7db4dbdaa01a`  
		Last Modified: Thu, 02 Dec 2021 09:22:26 GMT  
		Size: 22.8 MB (22754365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1787793a37de8674853036139b8cf3e6e54fd257e9b3ab8bba1175936ee679a1`  
		Last Modified: Fri, 03 Dec 2021 18:39:48 GMT  
		Size: 9.9 MB (9872859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db8fa492ac8e0b37299aa54782addae92722be6c2556d52ea0cac13628daf48`  
		Last Modified: Fri, 03 Dec 2021 18:39:41 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ec4eaf26d10fe9f8d194a2e4be3c5eeb4be9dcff43764fd50525a047660c44`  
		Last Modified: Fri, 03 Dec 2021 18:48:12 GMT  
		Size: 20.7 MB (20672372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3fd9faf09387da0c08147c32bda36b125afcd439b82ae807a435bf942ba1cb`  
		Last Modified: Fri, 03 Dec 2021 18:48:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dd07ff9a63af31eaf54520e07933583ddae004c2c9e875f40381b485a72d21`  
		Last Modified: Sat, 04 Dec 2021 13:11:08 GMT  
		Size: 21.1 MB (21059112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1dea72de2c2db67126d825d66f36152c5426b8f008fa6f413a6c9aeac3a129`  
		Last Modified: Sat, 04 Dec 2021 13:10:55 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716a652b22b831eb9525de54552d99c89bd728cf75b8df5369b785cc030db608`  
		Last Modified: Sat, 04 Dec 2021 13:10:55 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75635a05ae6821be2004fd073860603016298cf22cf81fed86c3e4030556dcd8`  
		Last Modified: Sat, 04 Dec 2021 13:10:55 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:3e751cecaa6634cefdf80c05880592708235fcf08b06de8a6b354c312d919fd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80111639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b14b6d5f8a0b0b86afdd30a7f5b6e11b9ffc06c97d0e0f3a03a00978593b2929`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:46:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 13:46:11 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 14:10:29 GMT
ENV RUBY_MAJOR=2.6
# Tue, 21 Dec 2021 14:10:29 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 21 Dec 2021 14:10:30 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 21 Dec 2021 14:12:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Dec 2021 14:12:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Dec 2021 14:12:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Dec 2021 14:12:20 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 14:12:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 21 Dec 2021 14:12:22 GMT
CMD ["irb"]
# Wed, 22 Dec 2021 03:51:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 22 Dec 2021 03:51:00 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 22 Dec 2021 03:51:01 GMT
ENV TINI_VERSION=0.18.0
# Wed, 22 Dec 2021 03:52:24 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 22 Dec 2021 03:52:25 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 22 Dec 2021 03:52:26 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 22 Dec 2021 03:52:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 22 Dec 2021 03:52:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 22 Dec 2021 03:52:28 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 22 Dec 2021 03:52:29 GMT
EXPOSE 24224 5140
# Wed, 22 Dec 2021 03:52:30 GMT
USER fluent
# Wed, 22 Dec 2021 03:52:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 22 Dec 2021 03:52:32 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df957e92572da886c36ceee88919e1780eaacc4ffe81dba01dadcc234d3b4636`  
		Last Modified: Tue, 21 Dec 2021 14:16:30 GMT  
		Size: 11.3 MB (11261786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f498124153b35570162f92f7962aa50fd000b9fb69e0789e5e1127c014cca38`  
		Last Modified: Tue, 21 Dec 2021 14:16:28 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a3ef5a630f83e12655230af7f4d10ac168fc0701920fe0f2e360b4abf291f1`  
		Last Modified: Tue, 21 Dec 2021 14:20:59 GMT  
		Size: 21.1 MB (21124034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d482d015a092f5c5f5b629b7feba2fdda0c10846fed360fe6451df8002b392`  
		Last Modified: Tue, 21 Dec 2021 14:20:56 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c328f8ceb37104a193ea29ca76ab226e273186b1c468ae21149e3630767edb`  
		Last Modified: Wed, 22 Dec 2021 03:53:00 GMT  
		Size: 21.8 MB (21799763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530ba1892cb3ef185de3ad2e5d3296354de65ba4a2c05b89a0291fe88133289a`  
		Last Modified: Wed, 22 Dec 2021 03:52:57 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0521121f54a1b28056a0d2d438a7c2d21e3d1f789080e85a90354165922e00`  
		Last Modified: Wed, 22 Dec 2021 03:52:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117365658371b2f9d3f2adcfe3db27dc96e3e303814556facd47e755ab325f2e`  
		Last Modified: Wed, 22 Dec 2021 03:52:57 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:7bc5db914344425078ea36a7a2e592d6c3e65d924ee6f317bdf294a33df52e87
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87180681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c25bfc2846e7607c175bf6b3fd90e0b924db910601cea8059ee188ab66f38ce`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 20:07:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 20:07:40 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 20:07:41 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 21:02:00 GMT
ENV RUBY_MAJOR=2.6
# Tue, 21 Dec 2021 21:02:01 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 21 Dec 2021 21:02:01 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 21 Dec 2021 21:06:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Dec 2021 21:06:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Dec 2021 21:06:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Dec 2021 21:06:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 21:06:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 21 Dec 2021 21:06:52 GMT
CMD ["irb"]
# Wed, 22 Dec 2021 10:02:44 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 22 Dec 2021 10:02:45 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 22 Dec 2021 10:02:45 GMT
ENV TINI_VERSION=0.18.0
# Wed, 22 Dec 2021 10:04:27 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 22 Dec 2021 10:04:28 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 22 Dec 2021 10:04:29 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 22 Dec 2021 10:04:29 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 22 Dec 2021 10:04:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 22 Dec 2021 10:04:29 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 22 Dec 2021 10:04:30 GMT
EXPOSE 24224 5140
# Wed, 22 Dec 2021 10:04:30 GMT
USER fluent
# Wed, 22 Dec 2021 10:04:30 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 22 Dec 2021 10:04:30 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1066d2070153fbad5494fe979ad171707d9eab3b32f3fd90979531049d8b27`  
		Last Modified: Tue, 21 Dec 2021 21:13:06 GMT  
		Size: 17.2 MB (17227036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5157ccdbc4b0d00d4ffd83478d4385983d9d4f8c22959750d2de032fa02a762d`  
		Last Modified: Tue, 21 Dec 2021 21:12:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d31ac662dfab3810c94a2f54d83a6b00952df811a3830c497d694013ac2c58`  
		Last Modified: Tue, 21 Dec 2021 21:19:01 GMT  
		Size: 20.9 MB (20941790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5912b3a1ff5cce1ac5778138fd2f43b02157837e653685699edc98c49eb381a`  
		Last Modified: Tue, 21 Dec 2021 21:18:58 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbeffd0be92c865380286e4ab5b5f786fc9755f7b5e88fca0ee5346875945283`  
		Last Modified: Wed, 22 Dec 2021 10:05:00 GMT  
		Size: 21.2 MB (21204209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225daa9efae801281529f36cb084a2f027a1aca199a75f02fd39814e58e29c3e`  
		Last Modified: Wed, 22 Dec 2021 10:04:55 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b441b9d8e0b9e011ec55fd3944a4a8068903eed9a40164f3b1184254134f47`  
		Last Modified: Wed, 22 Dec 2021 10:04:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957155b3dad1d80709391f91ceaadba109c0e2201c7233d4aadfeb69e1d2ffe7`  
		Last Modified: Wed, 22 Dec 2021 10:04:55 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:64194d2506feca34168225d5cb01ba7847c4fc5fc4c79772d7f0a01f428c7192
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87879267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2893e3b93f0bbfd84a21a57d5c776b2c64d70a6cbc02b34be3b3cb8c899fe7ba`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 02 Dec 2021 07:22:12 GMT
ADD file:b9b5697bc2dd3ded7a158d973abc939cc5d197f1f0d9ff1fa8b3db3b7906de7a in / 
# Thu, 02 Dec 2021 07:22:18 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 07:58:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 07:58:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Dec 2021 07:58:41 GMT
ENV LANG=C.UTF-8
# Fri, 03 Dec 2021 09:09:13 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Dec 2021 09:09:15 GMT
ENV RUBY_VERSION=2.6.9
# Fri, 03 Dec 2021 09:09:17 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Fri, 03 Dec 2021 09:16:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Dec 2021 09:16:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Dec 2021 09:16:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Dec 2021 09:16:38 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 09:16:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Dec 2021 09:16:44 GMT
CMD ["irb"]
# Sat, 04 Dec 2021 02:09:22 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 04 Dec 2021 02:09:23 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 04 Dec 2021 02:09:25 GMT
ENV TINI_VERSION=0.18.0
# Sat, 04 Dec 2021 02:13:08 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 04 Dec 2021 02:13:15 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 04 Dec 2021 02:13:16 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 04 Dec 2021 02:13:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 04 Dec 2021 02:13:18 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 04 Dec 2021 02:13:20 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 04 Dec 2021 02:13:22 GMT
EXPOSE 24224 5140
# Sat, 04 Dec 2021 02:13:23 GMT
USER fluent
# Sat, 04 Dec 2021 02:13:25 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 04 Dec 2021 02:13:27 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:da5263f5d65ecaf2dcd9400908302b4c477c13afa707110e4d85b4b946e9a3ae`  
		Last Modified: Thu, 02 Dec 2021 07:32:41 GMT  
		Size: 30.6 MB (30562306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5617a28440e343caa8dd30cc324bdd708ebe1f964ec11fd26f132068879ed4e`  
		Last Modified: Fri, 03 Dec 2021 09:21:11 GMT  
		Size: 12.7 MB (12705552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96de5a56dc2e1824f750d121f9d5244c505b423f1f8a35f736ff60ef67908f0b`  
		Last Modified: Fri, 03 Dec 2021 09:21:08 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d842a33f7d39fa300527a467e6bba3ff5e53e4d9d6f4df2996576cf1642efa14`  
		Last Modified: Fri, 03 Dec 2021 09:26:06 GMT  
		Size: 22.0 MB (22023323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03648056dfafebc33cc627e0af6017e5566f34b428ed9e1c303f4c5c82b1ca41`  
		Last Modified: Fri, 03 Dec 2021 09:26:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c3c72a12d41f318d5779e85bbbf449bad44ed9e5a7ad69e5146310522f6acc`  
		Last Modified: Sat, 04 Dec 2021 02:13:53 GMT  
		Size: 22.6 MB (22584998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e837d43a9b725089dff53fdf8c2afb40d3fe5ff825574a7afc89628e83c09006`  
		Last Modified: Sat, 04 Dec 2021 02:13:49 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7940e8b758c81281c247c3832bf8ab53cebeb5ad5c55be6ccac845b8f7318`  
		Last Modified: Sat, 04 Dec 2021 02:13:49 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffc6e91fb84cbe49fc5de0107eb8c2a5a266f6949abff341300e65c07c8725d`  
		Last Modified: Sat, 04 Dec 2021 02:13:49 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:15fde5998f955c71d60cf4513932c2dac854ba1e975b1d0c5c5e43f55399f1ca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80418926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aa22ed864620743d477ffee21b6f727416b62ec28aa23d48d22821e1014bf30`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:57 GMT
ADD file:33e37861eefa46f6e5f7f4967ce8ae3167e28bc817c3c71ff90a3d51e2376a0f in / 
# Tue, 21 Dec 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:50:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:50:51 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 10:50:51 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 11:13:38 GMT
ENV RUBY_MAJOR=2.6
# Tue, 21 Dec 2021 11:13:38 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 21 Dec 2021 11:13:38 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 21 Dec 2021 11:15:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Dec 2021 11:15:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Dec 2021 11:15:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Dec 2021 11:15:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 11:15:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 21 Dec 2021 11:15:13 GMT
CMD ["irb"]
# Tue, 21 Dec 2021 19:08:18 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 21 Dec 2021 19:08:18 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 21 Dec 2021 19:08:18 GMT
ENV TINI_VERSION=0.18.0
# Tue, 21 Dec 2021 19:09:31 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 21 Dec 2021 19:09:33 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 21 Dec 2021 19:09:33 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 21 Dec 2021 19:09:33 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 21 Dec 2021 19:09:33 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 21 Dec 2021 19:09:33 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 21 Dec 2021 19:09:33 GMT
EXPOSE 24224 5140
# Tue, 21 Dec 2021 19:09:33 GMT
USER fluent
# Tue, 21 Dec 2021 19:09:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 21 Dec 2021 19:09:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:10979941d091693f28e3dc033cc6ca88996acf42a0aace27ad85fbd894945e20`  
		Last Modified: Tue, 21 Dec 2021 01:48:51 GMT  
		Size: 25.8 MB (25769051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a6f3c4642cf35166efc3bc51ae42418989834c8eca28809948ada296bb9c5`  
		Last Modified: Tue, 21 Dec 2021 11:19:14 GMT  
		Size: 10.8 MB (10815241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c51d7f208d075afa3e35cffb33a4058bc2e6b09617649fda7a7cd8522e52308`  
		Last Modified: Tue, 21 Dec 2021 11:19:12 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3583c6a7801e70c598ceeaa29d28a8b10ca7ed50621ad0bb0a532073490164`  
		Last Modified: Tue, 21 Dec 2021 11:22:22 GMT  
		Size: 21.6 MB (21644657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3860c73eac66c9c46296dd704b1cb3012f7b7b882323b3bfdc4b17c1e35d7b84`  
		Last Modified: Tue, 21 Dec 2021 11:22:20 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c84bf6f760ca89f215e4de174cf90bdfdab55b57d4e4d9f1fe91031dc78fe`  
		Last Modified: Tue, 21 Dec 2021 19:10:11 GMT  
		Size: 22.2 MB (22186889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2229bae05d587e80d19d20b6f204ed4bb286f8b9503cd7cb523cb967b1f0afc4`  
		Last Modified: Tue, 21 Dec 2021 19:10:08 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d54fcdf40517dc3b1b49c5018c0ce24b7effeaa185dd951294523810efec81`  
		Last Modified: Tue, 21 Dec 2021 19:10:09 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f2fcc7ca912dcfb1df196696c5db99d6ef78b85c944c614608651408e9cd9`  
		Last Modified: Tue, 21 Dec 2021 19:10:08 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
