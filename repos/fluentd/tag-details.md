<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.14-1`](#fluentdv114-1)
-	[`fluentd:v1.14-debian-1`](#fluentdv114-debian-1)
-	[`fluentd:v1.14.0-1.0`](#fluentdv1140-10)
-	[`fluentd:v1.14.0-debian-1.0`](#fluentdv1140-debian-10)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:f2c7a2d130414c8d3d980fc968bf60fcca3e91e093df5123f3a96cc642e15e14
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
$ docker pull fluentd@sha256:21303421f4f8e3cf8b3398e4522a5756ed3967dac22c59e4a86596fc55086bdd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19079844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3134b06b92a81f10483c2a8787351fd5f29558f2f102b9d10cac903c05fabb42`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:20:55 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:20:55 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:21:40 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:21:41 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:21:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:21:42 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:21:42 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:21:42 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:21:42 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:21:42 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:21:42 GMT
USER fluent
# Tue, 07 Sep 2021 20:21:43 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:21:43 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d74db1dcb580089442caaa14445aae91594a0d03f053028dbd9f4296834bd3`  
		Last Modified: Tue, 07 Sep 2021 20:23:38 GMT  
		Size: 16.3 MB (16263561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e54056b9038af025f41617e6d10336bf82aa74cd2a95c91388cb8b86c8cbd2`  
		Last Modified: Tue, 07 Sep 2021 20:23:36 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3929dea8cde2a8c168df44bab12475fece2ff2ad7a3a18ba505a9e9e1e84705`  
		Last Modified: Tue, 07 Sep 2021 20:23:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f55539abe84d550d6beb0b7616282c8a6a80bb37c98fa52f2ccd0cf38f8e35`  
		Last Modified: Tue, 07 Sep 2021 20:23:36 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:7a9f0318abd7506571a1310972643835aa01e2d0dcfd515cad796e276d4bfda0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18379793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c8dd8c66dad580d0dbbc14c100e3194bf847cb7c7d9cbd3fef6ea49dd86a558`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:49:32 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:49:32 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:51:35 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:51:37 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:51:38 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:51:38 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:51:39 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:51:39 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:51:39 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:51:40 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:51:40 GMT
USER fluent
# Tue, 07 Sep 2021 20:51:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:51:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7eb7b880f9690fc3a824c1e4374b086d271a59aeac72b5763a0f592e813bfa8`  
		Last Modified: Tue, 07 Sep 2021 20:52:19 GMT  
		Size: 15.8 MB (15753830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ccd7060727423d045560f366399836e66303b3a68c8fff86d452ff9ebf8bf6`  
		Last Modified: Tue, 07 Sep 2021 20:52:08 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78f045961f7fbb18aeba1d62761bec1c08e3cbaddd73c78c79ba641b2c1fafd`  
		Last Modified: Tue, 07 Sep 2021 20:52:08 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40192417ee3da1f482280fa20b7f1e56441190170f0a201d65db6425bad2898`  
		Last Modified: Tue, 07 Sep 2021 20:52:08 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:6973a417985c4fc8d9c5fe1e767ed70c6e7eb876ad1bf5434a1745bfa0565e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18914520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e456d07428a00db805ae510a3baf9179ce2d716d38b2f90bda1f53b58dbece1`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:39:41 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:39:41 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:40:33 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:40:34 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:40:34 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:40:34 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:40:34 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:40:34 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:40:35 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:40:35 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:40:35 GMT
USER fluent
# Tue, 07 Sep 2021 20:40:35 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:40:35 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9f218f0ecc4e04f6a426e447ba103887996acb73bbbfb735a8504719c2a549`  
		Last Modified: Tue, 07 Sep 2021 20:42:56 GMT  
		Size: 16.2 MB (16199306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c571f6aa232babf2732f4e0ab8c0f742981c4ee96bc6e8088302a7f4acc69b`  
		Last Modified: Tue, 07 Sep 2021 20:42:53 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89010683c983c10c6cd5cfc085f65b7fe21c8a23ae7c00c038b73ce99b18f3a`  
		Last Modified: Tue, 07 Sep 2021 20:42:53 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e36aac88b93082338b205b201149d8c3382c877b47c9e98886518d55fe74b7`  
		Last Modified: Tue, 07 Sep 2021 20:42:53 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; 386

```console
$ docker pull fluentd@sha256:507bfb76f1e7f4cf106e82a22b8feca0ddeabec72d54018185c38b71d6cc2efd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18610135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf4e08554bde9771b13000042d41d7ab6b4ba302562df1f2c438d82d54c905a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:38:57 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:38:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:39:50 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:39:51 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:39:52 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:39:52 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:39:52 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:39:52 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:39:52 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:39:53 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:39:53 GMT
USER fluent
# Tue, 07 Sep 2021 20:39:53 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:39:53 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839ea22df0bc2e8d07e4813e30c7ca185a40ee3d13fa58743a31fa30a15af5bf`  
		Last Modified: Tue, 07 Sep 2021 20:42:12 GMT  
		Size: 15.8 MB (15786839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba35a8cc0c8001d1c49febce49c713b8e5f6f003cece0be7bdaf0419e2770b57`  
		Last Modified: Tue, 07 Sep 2021 20:42:09 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848011ed348ffb82fd1282d2320030b9be8f3b2c6709a036772bff944b81c4b1`  
		Last Modified: Tue, 07 Sep 2021 20:42:09 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0b8201a679c29d06d372d77acf1764115098c283bb63a06cf78d792a96d81c`  
		Last Modified: Tue, 07 Sep 2021 20:42:09 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:aab9d909252af4256baec64f9fda57ce36dd0a75df59be1bb7a002f9c7219700
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19145994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3cc52353d6416fa4e1d7d9d7427f578e3770d0b32fde1b259bd27d78e0ac544`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Sep 2021 02:42:40 GMT
ADD file:07a51f1a2f818bd1c1651832ce63cb1e0046a57994724cda6a20ff1a2a685295 in / 
# Wed, 01 Sep 2021 02:42:41 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:16:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:16:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:18:18 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:18:33 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:18:37 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:18:42 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:18:46 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:18:52 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:18:56 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:19:01 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:19:09 GMT
USER fluent
# Tue, 07 Sep 2021 20:19:14 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:19:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:39d9bf63205258fe1d085fd596101e6fc46ff796cda8d3ba2983e166a25b74db`  
		Last Modified: Wed, 01 Sep 2021 02:43:53 GMT  
		Size: 2.8 MB (2814813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3214731170d95d46d51466ca736dcae549ca4cb2cd89ff7bb8834f08371cc830`  
		Last Modified: Tue, 07 Sep 2021 20:27:04 GMT  
		Size: 16.3 MB (16328974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b953a57f1c8b1d34fbdba7c739fc68549f8a4f848d0caff4cfe6489d90b94`  
		Last Modified: Tue, 07 Sep 2021 20:27:00 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cb3ad67c383333d29832f2970b813793e4aa74b50669b481cd80b19408ba78`  
		Last Modified: Tue, 07 Sep 2021 20:27:01 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb74a463295355bce6d358068c04bc86fbd2211f74a78be02e2f77300696707`  
		Last Modified: Tue, 07 Sep 2021 20:27:01 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:ead3e7fe4bae3c87994a3d55e2c4340d13b4807e6ab3ffd221bd7ecb8566b90d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18787715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a5c8c592bac991df94d8370c013eec31e3d447a5a886f6b0d0516b3b92b1b79`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Sep 2021 01:15:21 GMT
ADD file:def74c9e73d87d3c8b94cc0200f2723aea3a7462f8d2e0852db9da25c19855ac in / 
# Wed, 01 Sep 2021 01:15:22 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:41:37 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:41:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:42:25 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:42:28 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:42:28 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:42:29 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:42:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:42:29 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:42:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:42:30 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:42:30 GMT
USER fluent
# Tue, 07 Sep 2021 20:42:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:42:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c1d78e8a87395f597d24b8eb78423ccdcfd404846906154e15aea8be9541c3ae`  
		Last Modified: Wed, 01 Sep 2021 01:16:19 GMT  
		Size: 2.6 MB (2604390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fb52069d70b8339548c913c62816a1041e2b58492eed2ecafd0ebe8dfbd291`  
		Last Modified: Tue, 07 Sep 2021 20:45:06 GMT  
		Size: 16.2 MB (16181126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf205afdde7410ba47394a3fad5fed8e4973131a11c9363aa6b4b7ba3bc930a`  
		Last Modified: Tue, 07 Sep 2021 20:45:04 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3628a5e9b4e88cb3095f8b1042bfbde9c592dc862d157982d7e9130151466d5`  
		Last Modified: Tue, 07 Sep 2021 20:45:03 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf74414db9a2e48243f98b424ada7c935664a9bb7b25e633adb1738b50d6cd0`  
		Last Modified: Tue, 07 Sep 2021 20:45:03 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14-1`

```console
$ docker pull fluentd@sha256:f2c7a2d130414c8d3d980fc968bf60fcca3e91e093df5123f3a96cc642e15e14
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
$ docker pull fluentd@sha256:21303421f4f8e3cf8b3398e4522a5756ed3967dac22c59e4a86596fc55086bdd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19079844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3134b06b92a81f10483c2a8787351fd5f29558f2f102b9d10cac903c05fabb42`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:20:55 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:20:55 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:21:40 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:21:41 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:21:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:21:42 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:21:42 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:21:42 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:21:42 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:21:42 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:21:42 GMT
USER fluent
# Tue, 07 Sep 2021 20:21:43 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:21:43 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d74db1dcb580089442caaa14445aae91594a0d03f053028dbd9f4296834bd3`  
		Last Modified: Tue, 07 Sep 2021 20:23:38 GMT  
		Size: 16.3 MB (16263561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e54056b9038af025f41617e6d10336bf82aa74cd2a95c91388cb8b86c8cbd2`  
		Last Modified: Tue, 07 Sep 2021 20:23:36 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3929dea8cde2a8c168df44bab12475fece2ff2ad7a3a18ba505a9e9e1e84705`  
		Last Modified: Tue, 07 Sep 2021 20:23:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f55539abe84d550d6beb0b7616282c8a6a80bb37c98fa52f2ccd0cf38f8e35`  
		Last Modified: Tue, 07 Sep 2021 20:23:36 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:7a9f0318abd7506571a1310972643835aa01e2d0dcfd515cad796e276d4bfda0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18379793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c8dd8c66dad580d0dbbc14c100e3194bf847cb7c7d9cbd3fef6ea49dd86a558`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:49:32 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:49:32 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:51:35 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:51:37 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:51:38 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:51:38 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:51:39 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:51:39 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:51:39 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:51:40 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:51:40 GMT
USER fluent
# Tue, 07 Sep 2021 20:51:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:51:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7eb7b880f9690fc3a824c1e4374b086d271a59aeac72b5763a0f592e813bfa8`  
		Last Modified: Tue, 07 Sep 2021 20:52:19 GMT  
		Size: 15.8 MB (15753830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ccd7060727423d045560f366399836e66303b3a68c8fff86d452ff9ebf8bf6`  
		Last Modified: Tue, 07 Sep 2021 20:52:08 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78f045961f7fbb18aeba1d62761bec1c08e3cbaddd73c78c79ba641b2c1fafd`  
		Last Modified: Tue, 07 Sep 2021 20:52:08 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40192417ee3da1f482280fa20b7f1e56441190170f0a201d65db6425bad2898`  
		Last Modified: Tue, 07 Sep 2021 20:52:08 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:6973a417985c4fc8d9c5fe1e767ed70c6e7eb876ad1bf5434a1745bfa0565e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18914520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e456d07428a00db805ae510a3baf9179ce2d716d38b2f90bda1f53b58dbece1`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:39:41 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:39:41 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:40:33 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:40:34 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:40:34 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:40:34 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:40:34 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:40:34 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:40:35 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:40:35 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:40:35 GMT
USER fluent
# Tue, 07 Sep 2021 20:40:35 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:40:35 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9f218f0ecc4e04f6a426e447ba103887996acb73bbbfb735a8504719c2a549`  
		Last Modified: Tue, 07 Sep 2021 20:42:56 GMT  
		Size: 16.2 MB (16199306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c571f6aa232babf2732f4e0ab8c0f742981c4ee96bc6e8088302a7f4acc69b`  
		Last Modified: Tue, 07 Sep 2021 20:42:53 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89010683c983c10c6cd5cfc085f65b7fe21c8a23ae7c00c038b73ce99b18f3a`  
		Last Modified: Tue, 07 Sep 2021 20:42:53 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e36aac88b93082338b205b201149d8c3382c877b47c9e98886518d55fe74b7`  
		Last Modified: Tue, 07 Sep 2021 20:42:53 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; 386

```console
$ docker pull fluentd@sha256:507bfb76f1e7f4cf106e82a22b8feca0ddeabec72d54018185c38b71d6cc2efd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18610135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf4e08554bde9771b13000042d41d7ab6b4ba302562df1f2c438d82d54c905a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:38:57 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:38:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:39:50 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:39:51 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:39:52 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:39:52 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:39:52 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:39:52 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:39:52 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:39:53 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:39:53 GMT
USER fluent
# Tue, 07 Sep 2021 20:39:53 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:39:53 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839ea22df0bc2e8d07e4813e30c7ca185a40ee3d13fa58743a31fa30a15af5bf`  
		Last Modified: Tue, 07 Sep 2021 20:42:12 GMT  
		Size: 15.8 MB (15786839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba35a8cc0c8001d1c49febce49c713b8e5f6f003cece0be7bdaf0419e2770b57`  
		Last Modified: Tue, 07 Sep 2021 20:42:09 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848011ed348ffb82fd1282d2320030b9be8f3b2c6709a036772bff944b81c4b1`  
		Last Modified: Tue, 07 Sep 2021 20:42:09 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0b8201a679c29d06d372d77acf1764115098c283bb63a06cf78d792a96d81c`  
		Last Modified: Tue, 07 Sep 2021 20:42:09 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:aab9d909252af4256baec64f9fda57ce36dd0a75df59be1bb7a002f9c7219700
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19145994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3cc52353d6416fa4e1d7d9d7427f578e3770d0b32fde1b259bd27d78e0ac544`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Sep 2021 02:42:40 GMT
ADD file:07a51f1a2f818bd1c1651832ce63cb1e0046a57994724cda6a20ff1a2a685295 in / 
# Wed, 01 Sep 2021 02:42:41 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:16:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:16:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:18:18 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:18:33 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:18:37 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:18:42 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:18:46 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:18:52 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:18:56 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:19:01 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:19:09 GMT
USER fluent
# Tue, 07 Sep 2021 20:19:14 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:19:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:39d9bf63205258fe1d085fd596101e6fc46ff796cda8d3ba2983e166a25b74db`  
		Last Modified: Wed, 01 Sep 2021 02:43:53 GMT  
		Size: 2.8 MB (2814813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3214731170d95d46d51466ca736dcae549ca4cb2cd89ff7bb8834f08371cc830`  
		Last Modified: Tue, 07 Sep 2021 20:27:04 GMT  
		Size: 16.3 MB (16328974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b953a57f1c8b1d34fbdba7c739fc68549f8a4f848d0caff4cfe6489d90b94`  
		Last Modified: Tue, 07 Sep 2021 20:27:00 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cb3ad67c383333d29832f2970b813793e4aa74b50669b481cd80b19408ba78`  
		Last Modified: Tue, 07 Sep 2021 20:27:01 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb74a463295355bce6d358068c04bc86fbd2211f74a78be02e2f77300696707`  
		Last Modified: Tue, 07 Sep 2021 20:27:01 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; s390x

```console
$ docker pull fluentd@sha256:ead3e7fe4bae3c87994a3d55e2c4340d13b4807e6ab3ffd221bd7ecb8566b90d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18787715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a5c8c592bac991df94d8370c013eec31e3d447a5a886f6b0d0516b3b92b1b79`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Sep 2021 01:15:21 GMT
ADD file:def74c9e73d87d3c8b94cc0200f2723aea3a7462f8d2e0852db9da25c19855ac in / 
# Wed, 01 Sep 2021 01:15:22 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:41:37 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:41:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:42:25 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:42:28 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:42:28 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:42:29 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:42:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:42:29 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:42:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:42:30 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:42:30 GMT
USER fluent
# Tue, 07 Sep 2021 20:42:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:42:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c1d78e8a87395f597d24b8eb78423ccdcfd404846906154e15aea8be9541c3ae`  
		Last Modified: Wed, 01 Sep 2021 01:16:19 GMT  
		Size: 2.6 MB (2604390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fb52069d70b8339548c913c62816a1041e2b58492eed2ecafd0ebe8dfbd291`  
		Last Modified: Tue, 07 Sep 2021 20:45:06 GMT  
		Size: 16.2 MB (16181126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf205afdde7410ba47394a3fad5fed8e4973131a11c9363aa6b4b7ba3bc930a`  
		Last Modified: Tue, 07 Sep 2021 20:45:04 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3628a5e9b4e88cb3095f8b1042bfbde9c592dc862d157982d7e9130151466d5`  
		Last Modified: Tue, 07 Sep 2021 20:45:03 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf74414db9a2e48243f98b424ada7c935664a9bb7b25e633adb1738b50d6cd0`  
		Last Modified: Tue, 07 Sep 2021 20:45:03 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14-debian-1`

```console
$ docker pull fluentd@sha256:ddfc0bfb65bd6e47547082bc73e9f6c752e291f7ad7d71763eca3026769f3cf2
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
$ docker pull fluentd@sha256:76eaf8e73d659d13c1e713594f3b68372d480ca95c820447cc689b8e55b62909
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83180692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15ff5fd042fb948a693a51e42273e864db79af89977afed27fc0eccee169bbe5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 15:37:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:37:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:37:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:37:06 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:14:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 12 Oct 2021 20:14:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 12 Oct 2021 20:14:52 GMT
ENV TINI_VERSION=0.18.0
# Tue, 12 Oct 2021 20:17:00 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 12 Oct 2021 20:17:01 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 12 Oct 2021 20:17:01 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 12 Oct 2021 20:17:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 12 Oct 2021 20:17:01 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 12 Oct 2021 20:17:02 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 12 Oct 2021 20:17:02 GMT
EXPOSE 24224 5140
# Tue, 12 Oct 2021 20:17:02 GMT
USER fluent
# Tue, 12 Oct 2021 20:17:02 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 12 Oct 2021 20:17:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc3e5ccddf2ccfcc978381549c751e1167cdf41ce60580404b33cb6fdd7aa5`  
		Last Modified: Tue, 12 Oct 2021 15:41:15 GMT  
		Size: 21.5 MB (21467885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b99a224b661061fbbe799d6efb95f01221754e6a73aec4d536865d1e304d63`  
		Last Modified: Tue, 12 Oct 2021 15:41:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce54581d99048d7f94f97b4e2d2f317ee3c9fdce5eb3c0d3cdb52072016660b7`  
		Last Modified: Tue, 12 Oct 2021 20:17:28 GMT  
		Size: 22.0 MB (22005026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daefdd420359fc022652bcdcc007e5e9d88c221bc93405f002f4cda2a25c8352`  
		Last Modified: Tue, 12 Oct 2021 20:17:24 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ded521f316c8b6d5264c9aef16c282663d5051d018db5dbaacee8fa8bee89b`  
		Last Modified: Tue, 12 Oct 2021 20:17:24 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cf6d98e001ee961ab070e0f4f81bb6752cf4b55a2681854b36c4052e3ef3e7`  
		Last Modified: Tue, 12 Oct 2021 20:17:24 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:6a62088d86817f5a29595eb1fc2ab816f6ec2c59e8a15f61569ded5c72c12512
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77116535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132b1e23200a63720a954040b718efbd99af50060ab64bba419ffbb9be2c97cd`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:42 GMT
ADD file:6524935705c59a0eda67f61fe1005a28b4b388258e2d5636dd5b831333200dc8 in / 
# Tue, 28 Sep 2021 01:51:43 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 18:48:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 18:48:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 28 Sep 2021 18:48:33 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 19:23:53 GMT
ENV RUBY_MAJOR=2.6
# Tue, 28 Sep 2021 19:23:53 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 28 Sep 2021 19:23:53 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 28 Sep 2021 19:28:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 28 Sep 2021 19:28:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 28 Sep 2021 19:28:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 28 Sep 2021 19:28:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 19:28:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 28 Sep 2021 19:28:24 GMT
CMD ["irb"]
# Wed, 29 Sep 2021 05:17:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 29 Sep 2021 05:17:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 29 Sep 2021 05:17:48 GMT
ENV TINI_VERSION=0.18.0
# Wed, 29 Sep 2021 05:21:28 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 29 Sep 2021 05:21:30 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 29 Sep 2021 05:21:31 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 29 Sep 2021 05:21:31 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 29 Sep 2021 05:21:31 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 29 Sep 2021 05:21:32 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 29 Sep 2021 05:21:32 GMT
EXPOSE 24224 5140
# Wed, 29 Sep 2021 05:21:33 GMT
USER fluent
# Wed, 29 Sep 2021 05:21:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 29 Sep 2021 05:21:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:85d14771cf32dc23d1c8e99a9aad844b3db9d67f4781455c81749ffe43b05513`  
		Last Modified: Tue, 28 Sep 2021 02:08:05 GMT  
		Size: 24.9 MB (24879067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67219e91075b17466704e8b77ae390b755ce0be763738dadf133450a8ff33b7`  
		Last Modified: Tue, 28 Sep 2021 19:34:50 GMT  
		Size: 10.3 MB (10348969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd11b3d5ad959051b468e4d6e1b98b58b9884dede42b4b9057de720132ba0628`  
		Last Modified: Tue, 28 Sep 2021 19:34:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48524c724f2b3b71b7bfc402fe4e371499a6bf88d9344c60a37b34ecd55dabd`  
		Last Modified: Tue, 28 Sep 2021 19:38:42 GMT  
		Size: 20.7 MB (20733397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a6f57f87784af7c75889748c13944d3abb353ffe4d36ccf8d6e8d69729dd26`  
		Last Modified: Tue, 28 Sep 2021 19:38:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f4d2dd963d05d6de7a50aa91138738a6c4a67bffb70cbf10548110eb85c332`  
		Last Modified: Wed, 29 Sep 2021 05:22:15 GMT  
		Size: 21.2 MB (21152033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2becef1bc430cfcf5318b0a899e2c67478de042c1588e82ee860fc3e69fcd12c`  
		Last Modified: Wed, 29 Sep 2021 05:22:02 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83777e50a34ce82c13d2a2b221ed64e9b57019776dbb6257c9cd17423efb2a8`  
		Last Modified: Wed, 29 Sep 2021 05:22:02 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1cb5df629ba47e397fe3930a7d96c42b995c19be2fa2536c9b70bfa1c6337`  
		Last Modified: Wed, 29 Sep 2021 05:22:02 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:954d67234440fc680257048451a422ae47c9b7abe44f2eeb172c480ea86e23db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74321495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99a8410e90ad45fe64a9d660c969c504ead37d96b6b13ebb14f42f06a1d6a412`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Sep 2021 18:04:11 GMT
ADD file:e71f315aa894d483f75b32109fff32974c43ce2e684cd28eb6492bc6fc450931 in / 
# Thu, 30 Sep 2021 18:04:12 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 22:39:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 22:39:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 01 Oct 2021 22:39:22 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 23:26:40 GMT
ENV RUBY_MAJOR=2.6
# Fri, 01 Oct 2021 23:26:40 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 01 Oct 2021 23:26:40 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 01 Oct 2021 23:30:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 01 Oct 2021 23:30:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 01 Oct 2021 23:30:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 01 Oct 2021 23:30:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 23:30:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 01 Oct 2021 23:30:58 GMT
CMD ["irb"]
# Sat, 02 Oct 2021 19:45:37 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 02 Oct 2021 19:45:37 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 02 Oct 2021 19:45:38 GMT
ENV TINI_VERSION=0.18.0
# Sat, 02 Oct 2021 19:49:00 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 02 Oct 2021 19:49:02 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 02 Oct 2021 19:49:02 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 02 Oct 2021 19:49:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 02 Oct 2021 19:49:04 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 02 Oct 2021 19:49:04 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 02 Oct 2021 19:49:04 GMT
EXPOSE 24224 5140
# Sat, 02 Oct 2021 19:49:05 GMT
USER fluent
# Sat, 02 Oct 2021 19:49:05 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 02 Oct 2021 19:49:06 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:421f17c521234da0c5b07d4f6e44314149dc3790ef12134e85e61741452c9f96`  
		Last Modified: Thu, 30 Sep 2021 18:20:50 GMT  
		Size: 22.7 MB (22746246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0692ba1be6ebb6fe7fa2b8bf57a9dd0a4bb5354fbf13889f4b1035ed696c0baf`  
		Last Modified: Fri, 01 Oct 2021 23:38:49 GMT  
		Size: 9.9 MB (9872884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad1e8259356fdfb6c253c6c9dd4fff4d43cf28352a4c5f3216e67ddf4017fc2`  
		Last Modified: Fri, 01 Oct 2021 23:38:42 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6d848e6f9c9ad88f7c45c255801665fb3963a4adc43e3d6152fd874c1c317d`  
		Last Modified: Fri, 01 Oct 2021 23:42:54 GMT  
		Size: 20.6 MB (20643672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78592b256a1308d1146591647f808abc5a8de61af0288d7aa9b6adcb65c4e193`  
		Last Modified: Fri, 01 Oct 2021 23:42:46 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2575c1e72ae369804222eeaeddf4dc36f32d2d11bb4e638c874622e7d3f349c8`  
		Last Modified: Sat, 02 Oct 2021 19:49:48 GMT  
		Size: 21.1 MB (21055621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9cba1af80a06fa863a6dacd703131b2f9d384556d824f2471b7c7bc0a0977e`  
		Last Modified: Sat, 02 Oct 2021 19:49:35 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7d29ba2a73cdafb343028c628bb1f6dba91bb23fda9f62b8dd0054ef28fe7`  
		Last Modified: Sat, 02 Oct 2021 19:49:35 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace3248313b562881c10fe0d8e5d2159e323840ecb4f7e5dd2930f66b04de42c`  
		Last Modified: Sat, 02 Oct 2021 19:49:35 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:791cddf6300c4a3148adec03057d6d79a377062f7dd1bffb7b9a4fb88de05223
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80494194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a6ab60a8670f3a0ab00056a7171244da2c02014970934e617da87942916eab`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:13 GMT
ADD file:3e2426765cfe2b896fc847bcb435624930753c72ac00b87d2c73f4a81c813fd4 in / 
# Tue, 28 Sep 2021 01:41:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:12:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:12:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 28 Sep 2021 15:12:43 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 15:31:05 GMT
ENV RUBY_MAJOR=2.6
# Tue, 28 Sep 2021 15:31:05 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 28 Sep 2021 15:31:06 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 28 Sep 2021 15:33:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 28 Sep 2021 15:33:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 28 Sep 2021 15:33:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 28 Sep 2021 15:33:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 15:33:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 28 Sep 2021 15:33:16 GMT
CMD ["irb"]
# Wed, 29 Sep 2021 09:22:06 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 29 Sep 2021 09:22:06 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 29 Sep 2021 09:22:06 GMT
ENV TINI_VERSION=0.18.0
# Wed, 29 Sep 2021 09:23:50 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 29 Sep 2021 09:23:51 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 29 Sep 2021 09:23:52 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 29 Sep 2021 09:23:52 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 29 Sep 2021 09:23:52 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 29 Sep 2021 09:23:52 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 29 Sep 2021 09:23:52 GMT
EXPOSE 24224 5140
# Wed, 29 Sep 2021 09:23:52 GMT
USER fluent
# Wed, 29 Sep 2021 09:23:53 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 29 Sep 2021 09:23:53 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:896f18f54b28590b15a0f3354b13e8ea2f88a05f13de4117720f88cef30206ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:22 GMT  
		Size: 25.9 MB (25915039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cc0acef2e6aaa1fdfe65e13d5362898ed0d7e5e35620c50bee88bba231876d`  
		Last Modified: Tue, 28 Sep 2021 15:37:58 GMT  
		Size: 11.3 MB (11264477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2697264550a8ae7404f264263f6aff3741597dedc7ae31f97fd618c75fe3d366`  
		Last Modified: Tue, 28 Sep 2021 15:37:56 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42bc4b58d1156250b31014d7f12b2c6372cbef1733b6a7320094c8fcfe4a9ae`  
		Last Modified: Tue, 28 Sep 2021 15:40:50 GMT  
		Size: 21.3 MB (21309053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c904706c80aefa58a0674a4a2edd5e45aa322483116fb9de7574f18851ecd3`  
		Last Modified: Tue, 28 Sep 2021 15:40:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bca7f20eaa5d33c16efb4a35f5ae2fd77f47183cae3c43d98aef79b7dcbac22`  
		Last Modified: Wed, 29 Sep 2021 09:24:23 GMT  
		Size: 22.0 MB (22002546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bd5e7506d30b7f3b83e13f98d54c7e8372340112b85c3fc166d40f3b5cce3f`  
		Last Modified: Wed, 29 Sep 2021 09:24:19 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8b38098ec516f741dee50a8597ba4275d9944b1f5a9876778a9befbe3de7c0`  
		Last Modified: Wed, 29 Sep 2021 09:24:19 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34778854989ab5166ef55550cdee24bc4f3d1d1081cd84d341748c2288848427`  
		Last Modified: Wed, 29 Sep 2021 09:24:19 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:8b7d46815d25056c3b50e56879bfde7c64d2b0efac91a5dd4cd08ad826b9c01a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87126661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:807296930ed673ac8b6a3e1438b4f5d61501981e0745322ad64b0db589294e48`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:49 GMT
ADD file:c090abbb3afcfebf797e06e2ac4b778acb4e97d5dca79c29d1927f43cf14b23e in / 
# Tue, 28 Sep 2021 01:40:49 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 19:31:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 19:31:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 28 Sep 2021 19:31:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 20:00:41 GMT
ENV RUBY_MAJOR=2.6
# Tue, 28 Sep 2021 20:00:41 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 28 Sep 2021 20:00:41 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 28 Sep 2021 20:04:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 28 Sep 2021 20:04:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 28 Sep 2021 20:04:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 28 Sep 2021 20:04:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 20:04:16 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 28 Sep 2021 20:04:16 GMT
CMD ["irb"]
# Wed, 29 Sep 2021 06:40:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 29 Sep 2021 06:40:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 29 Sep 2021 06:40:52 GMT
ENV TINI_VERSION=0.18.0
# Wed, 29 Sep 2021 06:42:38 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 29 Sep 2021 06:42:39 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 29 Sep 2021 06:42:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 29 Sep 2021 06:42:40 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 29 Sep 2021 06:42:40 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 29 Sep 2021 06:42:41 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 29 Sep 2021 06:42:41 GMT
EXPOSE 24224 5140
# Wed, 29 Sep 2021 06:42:41 GMT
USER fluent
# Wed, 29 Sep 2021 06:42:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 29 Sep 2021 06:42:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:82f7c8b98609aee82696182c03cb09ae62ceab1b17f8eec1e233a68180876d41`  
		Last Modified: Tue, 28 Sep 2021 01:50:06 GMT  
		Size: 27.8 MB (27797629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd6ebe81fc32debaaf3e9bb15488927bad3277f8beccdc792bd3b6288995ee2`  
		Last Modified: Tue, 28 Sep 2021 20:09:31 GMT  
		Size: 17.2 MB (17226895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e1d8264f8156ea49a18e394b6b9eb180f17ac714622e30c2851d1572106784`  
		Last Modified: Tue, 28 Sep 2021 20:09:26 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2170515daa1310cdd92c2ec0f53c39022cd1b2bc2271f84154f77ed9daa91b`  
		Last Modified: Tue, 28 Sep 2021 20:12:47 GMT  
		Size: 20.9 MB (20910156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6af7a177e4c7bd2c13e2b8e6cc71dc32f4825d07356b6ad330601966c2aafe`  
		Last Modified: Tue, 28 Sep 2021 20:12:44 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28f813b6e684bc312a1769c6db8775f2c34a86ac11f329a00a48e6b03310d46`  
		Last Modified: Wed, 29 Sep 2021 06:43:12 GMT  
		Size: 21.2 MB (21188911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69d5bfb1a001c333fd9991574175f21106414b15f158aac10e9089aca0825a3`  
		Last Modified: Wed, 29 Sep 2021 06:43:06 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61db522f42ad3e0f546d9e7537119e694098414203d6d1f0fd7bc4bdbeede29`  
		Last Modified: Wed, 29 Sep 2021 06:43:06 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4312211c71347b20d0808077cc5c3968c0d3c3af1bc45bdc62fedebad2c4567e`  
		Last Modified: Wed, 29 Sep 2021 06:43:06 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:5ff9497480bac4a7e28f26d2f8840a4532d7ded41980baa094a543acd828d007
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87829230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d46a2394782b64591f2b709da27cbef3265233c47a80abbe874e0d153e9d04`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Oct 2021 17:56:14 GMT
ADD file:0b55ec14c2e9aa78512985a5bff3881b6fabf6794ce4406bb874b173d5a60799 in / 
# Mon, 04 Oct 2021 17:56:20 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 03:06:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 03:06:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 06 Oct 2021 03:06:23 GMT
ENV LANG=C.UTF-8
# Wed, 06 Oct 2021 03:52:55 GMT
ENV RUBY_MAJOR=2.6
# Wed, 06 Oct 2021 03:52:58 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 06 Oct 2021 03:53:00 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 06 Oct 2021 03:58:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 06 Oct 2021 03:58:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 06 Oct 2021 03:58:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 06 Oct 2021 03:58:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Oct 2021 03:58:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 06 Oct 2021 03:58:52 GMT
CMD ["irb"]
# Thu, 07 Oct 2021 05:16:48 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 07 Oct 2021 05:16:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 07 Oct 2021 05:17:01 GMT
ENV TINI_VERSION=0.18.0
# Thu, 07 Oct 2021 05:23:05 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 07 Oct 2021 05:23:14 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 07 Oct 2021 05:23:19 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 07 Oct 2021 05:23:20 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 07 Oct 2021 05:23:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 07 Oct 2021 05:23:31 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 07 Oct 2021 05:23:39 GMT
EXPOSE 24224 5140
# Thu, 07 Oct 2021 05:23:44 GMT
USER fluent
# Thu, 07 Oct 2021 05:23:52 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 07 Oct 2021 05:23:55 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:5736db2c6d2424206be3309412da520d7fe1fe4933cc2cc72641b311dd7d9099`  
		Last Modified: Mon, 04 Oct 2021 18:08:33 GMT  
		Size: 30.6 MB (30553728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3354ef54cd0e1052f9a547f02b1010929ef000aff902d0a370850998c897e3f6`  
		Last Modified: Wed, 06 Oct 2021 04:04:03 GMT  
		Size: 12.7 MB (12705362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bbab896c6e7a16a08fe33deb7eed7486092decdc1e5538684d5ba398e30390`  
		Last Modified: Wed, 06 Oct 2021 04:03:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf32a0e0567609d494382315cc5596d259b73adcc26d11a939dd971e9bbb65c`  
		Last Modified: Wed, 06 Oct 2021 04:07:23 GMT  
		Size: 22.0 MB (21984877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3ee4a3cdda80cbdd4c480d4d75a0893866585cbf00618cab4d2bab368496e`  
		Last Modified: Wed, 06 Oct 2021 04:07:21 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5616380b61838713c1ae2bf0758e79888afb65d11125a30241bb6d955cbfd2`  
		Last Modified: Thu, 07 Oct 2021 05:24:38 GMT  
		Size: 22.6 MB (22582171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427c23afd267d2099a889585e0531ef3e643f9babb47039f6c238e43310990bd`  
		Last Modified: Thu, 07 Oct 2021 05:24:29 GMT  
		Size: 1.9 KB (1851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b5358a5b979d699868997fe387d492664b19e48e02e5483a890bf092b15d19`  
		Last Modified: Thu, 07 Oct 2021 05:24:30 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a71dc2efd6d8ec1a1000311899164a3318d110ce0ccf85ff55cc4e9b52f209`  
		Last Modified: Thu, 07 Oct 2021 05:24:29 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:504be05ce004e64f11b088e7ceb13d5a218b611216e40efb7df1420ef416db3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80379203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd54a5a61800cf433f1ee567eb3ce0af1d1c66afec2ecad866642dc2bfa2d52`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:05:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:05:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 04:05:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:26:01 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 04:27:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 04:27:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 04:27:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 04:27:33 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 09:45:22 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 12 Oct 2021 09:45:22 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 12 Oct 2021 09:45:22 GMT
ENV TINI_VERSION=0.18.0
# Tue, 12 Oct 2021 09:46:40 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 12 Oct 2021 09:46:41 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 12 Oct 2021 09:46:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 12 Oct 2021 09:46:41 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 12 Oct 2021 09:46:42 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 12 Oct 2021 09:46:42 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 12 Oct 2021 09:46:42 GMT
EXPOSE 24224 5140
# Tue, 12 Oct 2021 09:46:42 GMT
USER fluent
# Tue, 12 Oct 2021 09:46:42 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 12 Oct 2021 09:46:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152601da1f670f23930e38f542a251b56290100e816cebfc101161c8e9d9823`  
		Last Modified: Tue, 12 Oct 2021 04:30:27 GMT  
		Size: 10.8 MB (10815329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379c6f49f1643cab68ffcf8d485cf085a0799907e6458c13a589142d6763809`  
		Last Modified: Tue, 12 Oct 2021 04:30:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58406908df2376127547311dc0ea98d9ef92a8573d1e0cb811fefa665bb3a84`  
		Last Modified: Tue, 12 Oct 2021 04:31:30 GMT  
		Size: 21.6 MB (21619749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb4ab84de8ab158c29c0c84a1b4726fd7c89ab7ff6fb27c139956d200f492b2`  
		Last Modified: Tue, 12 Oct 2021 04:31:29 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2694c92480617a6fe54d01b8a550ff5ecc516c2a899e78c76a15ccf410079ff`  
		Last Modified: Tue, 12 Oct 2021 09:47:11 GMT  
		Size: 22.2 MB (22186790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efee31c2b4b049cf332d1ffdca7978d2e15b630925f006435840c2b4b3366c68`  
		Last Modified: Tue, 12 Oct 2021 09:47:08 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff58fd2fae77d1de9c09fcf0fc811f28f51c66070043ac5015f1fa3c09d14172`  
		Last Modified: Tue, 12 Oct 2021 09:47:08 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ea6081abd1da3fb20e89016e642285b18972d4d0eba80a7e421a195afbc615`  
		Last Modified: Tue, 12 Oct 2021 09:47:08 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14.0-1.0`

```console
$ docker pull fluentd@sha256:f2c7a2d130414c8d3d980fc968bf60fcca3e91e093df5123f3a96cc642e15e14
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
$ docker pull fluentd@sha256:21303421f4f8e3cf8b3398e4522a5756ed3967dac22c59e4a86596fc55086bdd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19079844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3134b06b92a81f10483c2a8787351fd5f29558f2f102b9d10cac903c05fabb42`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:20:55 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:20:55 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:21:40 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:21:41 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:21:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:21:42 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:21:42 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:21:42 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:21:42 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:21:42 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:21:42 GMT
USER fluent
# Tue, 07 Sep 2021 20:21:43 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:21:43 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d74db1dcb580089442caaa14445aae91594a0d03f053028dbd9f4296834bd3`  
		Last Modified: Tue, 07 Sep 2021 20:23:38 GMT  
		Size: 16.3 MB (16263561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e54056b9038af025f41617e6d10336bf82aa74cd2a95c91388cb8b86c8cbd2`  
		Last Modified: Tue, 07 Sep 2021 20:23:36 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3929dea8cde2a8c168df44bab12475fece2ff2ad7a3a18ba505a9e9e1e84705`  
		Last Modified: Tue, 07 Sep 2021 20:23:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f55539abe84d550d6beb0b7616282c8a6a80bb37c98fa52f2ccd0cf38f8e35`  
		Last Modified: Tue, 07 Sep 2021 20:23:36 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:7a9f0318abd7506571a1310972643835aa01e2d0dcfd515cad796e276d4bfda0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18379793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c8dd8c66dad580d0dbbc14c100e3194bf847cb7c7d9cbd3fef6ea49dd86a558`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:49:32 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:49:32 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:51:35 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:51:37 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:51:38 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:51:38 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:51:39 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:51:39 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:51:39 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:51:40 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:51:40 GMT
USER fluent
# Tue, 07 Sep 2021 20:51:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:51:41 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7eb7b880f9690fc3a824c1e4374b086d271a59aeac72b5763a0f592e813bfa8`  
		Last Modified: Tue, 07 Sep 2021 20:52:19 GMT  
		Size: 15.8 MB (15753830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ccd7060727423d045560f366399836e66303b3a68c8fff86d452ff9ebf8bf6`  
		Last Modified: Tue, 07 Sep 2021 20:52:08 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78f045961f7fbb18aeba1d62761bec1c08e3cbaddd73c78c79ba641b2c1fafd`  
		Last Modified: Tue, 07 Sep 2021 20:52:08 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40192417ee3da1f482280fa20b7f1e56441190170f0a201d65db6425bad2898`  
		Last Modified: Tue, 07 Sep 2021 20:52:08 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:6973a417985c4fc8d9c5fe1e767ed70c6e7eb876ad1bf5434a1745bfa0565e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18914520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e456d07428a00db805ae510a3baf9179ce2d716d38b2f90bda1f53b58dbece1`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:39:41 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:39:41 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:40:33 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:40:34 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:40:34 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:40:34 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:40:34 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:40:34 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:40:35 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:40:35 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:40:35 GMT
USER fluent
# Tue, 07 Sep 2021 20:40:35 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:40:35 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9f218f0ecc4e04f6a426e447ba103887996acb73bbbfb735a8504719c2a549`  
		Last Modified: Tue, 07 Sep 2021 20:42:56 GMT  
		Size: 16.2 MB (16199306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c571f6aa232babf2732f4e0ab8c0f742981c4ee96bc6e8088302a7f4acc69b`  
		Last Modified: Tue, 07 Sep 2021 20:42:53 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89010683c983c10c6cd5cfc085f65b7fe21c8a23ae7c00c038b73ce99b18f3a`  
		Last Modified: Tue, 07 Sep 2021 20:42:53 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e36aac88b93082338b205b201149d8c3382c877b47c9e98886518d55fe74b7`  
		Last Modified: Tue, 07 Sep 2021 20:42:53 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:507bfb76f1e7f4cf106e82a22b8feca0ddeabec72d54018185c38b71d6cc2efd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18610135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf4e08554bde9771b13000042d41d7ab6b4ba302562df1f2c438d82d54c905a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:38:57 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:38:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:39:50 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:39:51 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:39:52 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:39:52 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:39:52 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:39:52 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:39:52 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:39:53 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:39:53 GMT
USER fluent
# Tue, 07 Sep 2021 20:39:53 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:39:53 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839ea22df0bc2e8d07e4813e30c7ca185a40ee3d13fa58743a31fa30a15af5bf`  
		Last Modified: Tue, 07 Sep 2021 20:42:12 GMT  
		Size: 15.8 MB (15786839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba35a8cc0c8001d1c49febce49c713b8e5f6f003cece0be7bdaf0419e2770b57`  
		Last Modified: Tue, 07 Sep 2021 20:42:09 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848011ed348ffb82fd1282d2320030b9be8f3b2c6709a036772bff944b81c4b1`  
		Last Modified: Tue, 07 Sep 2021 20:42:09 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0b8201a679c29d06d372d77acf1764115098c283bb63a06cf78d792a96d81c`  
		Last Modified: Tue, 07 Sep 2021 20:42:09 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:aab9d909252af4256baec64f9fda57ce36dd0a75df59be1bb7a002f9c7219700
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19145994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3cc52353d6416fa4e1d7d9d7427f578e3770d0b32fde1b259bd27d78e0ac544`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Sep 2021 02:42:40 GMT
ADD file:07a51f1a2f818bd1c1651832ce63cb1e0046a57994724cda6a20ff1a2a685295 in / 
# Wed, 01 Sep 2021 02:42:41 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:16:43 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:16:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:18:18 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:18:33 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:18:37 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:18:42 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:18:46 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:18:52 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:18:56 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:19:01 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:19:09 GMT
USER fluent
# Tue, 07 Sep 2021 20:19:14 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:19:18 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:39d9bf63205258fe1d085fd596101e6fc46ff796cda8d3ba2983e166a25b74db`  
		Last Modified: Wed, 01 Sep 2021 02:43:53 GMT  
		Size: 2.8 MB (2814813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3214731170d95d46d51466ca736dcae549ca4cb2cd89ff7bb8834f08371cc830`  
		Last Modified: Tue, 07 Sep 2021 20:27:04 GMT  
		Size: 16.3 MB (16328974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18b953a57f1c8b1d34fbdba7c739fc68549f8a4f848d0caff4cfe6489d90b94`  
		Last Modified: Tue, 07 Sep 2021 20:27:00 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cb3ad67c383333d29832f2970b813793e4aa74b50669b481cd80b19408ba78`  
		Last Modified: Tue, 07 Sep 2021 20:27:01 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb74a463295355bce6d358068c04bc86fbd2211f74a78be02e2f77300696707`  
		Last Modified: Tue, 07 Sep 2021 20:27:01 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:ead3e7fe4bae3c87994a3d55e2c4340d13b4807e6ab3ffd221bd7ecb8566b90d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18787715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a5c8c592bac991df94d8370c013eec31e3d447a5a886f6b0d0516b3b92b1b79`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 01 Sep 2021 01:15:21 GMT
ADD file:def74c9e73d87d3c8b94cc0200f2723aea3a7462f8d2e0852db9da25c19855ac in / 
# Wed, 01 Sep 2021 01:15:22 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 20:41:37 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 07 Sep 2021 20:41:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 07 Sep 2021 20:42:25 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 07 Sep 2021 20:42:28 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 07 Sep 2021 20:42:28 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 07 Sep 2021 20:42:29 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 07 Sep 2021 20:42:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 07 Sep 2021 20:42:29 GMT
ENV LD_PRELOAD=
# Tue, 07 Sep 2021 20:42:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 07 Sep 2021 20:42:30 GMT
EXPOSE 24224 5140
# Tue, 07 Sep 2021 20:42:30 GMT
USER fluent
# Tue, 07 Sep 2021 20:42:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 07 Sep 2021 20:42:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c1d78e8a87395f597d24b8eb78423ccdcfd404846906154e15aea8be9541c3ae`  
		Last Modified: Wed, 01 Sep 2021 01:16:19 GMT  
		Size: 2.6 MB (2604390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fb52069d70b8339548c913c62816a1041e2b58492eed2ecafd0ebe8dfbd291`  
		Last Modified: Tue, 07 Sep 2021 20:45:06 GMT  
		Size: 16.2 MB (16181126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf205afdde7410ba47394a3fad5fed8e4973131a11c9363aa6b4b7ba3bc930a`  
		Last Modified: Tue, 07 Sep 2021 20:45:04 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3628a5e9b4e88cb3095f8b1042bfbde9c592dc862d157982d7e9130151466d5`  
		Last Modified: Tue, 07 Sep 2021 20:45:03 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf74414db9a2e48243f98b424ada7c935664a9bb7b25e633adb1738b50d6cd0`  
		Last Modified: Tue, 07 Sep 2021 20:45:03 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14.0-debian-1.0`

```console
$ docker pull fluentd@sha256:ddfc0bfb65bd6e47547082bc73e9f6c752e291f7ad7d71763eca3026769f3cf2
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
$ docker pull fluentd@sha256:76eaf8e73d659d13c1e713594f3b68372d480ca95c820447cc689b8e55b62909
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83180692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15ff5fd042fb948a693a51e42273e864db79af89977afed27fc0eccee169bbe5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 15:37:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:37:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:37:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:37:06 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:14:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 12 Oct 2021 20:14:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 12 Oct 2021 20:14:52 GMT
ENV TINI_VERSION=0.18.0
# Tue, 12 Oct 2021 20:17:00 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 12 Oct 2021 20:17:01 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 12 Oct 2021 20:17:01 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 12 Oct 2021 20:17:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 12 Oct 2021 20:17:01 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 12 Oct 2021 20:17:02 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 12 Oct 2021 20:17:02 GMT
EXPOSE 24224 5140
# Tue, 12 Oct 2021 20:17:02 GMT
USER fluent
# Tue, 12 Oct 2021 20:17:02 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 12 Oct 2021 20:17:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc3e5ccddf2ccfcc978381549c751e1167cdf41ce60580404b33cb6fdd7aa5`  
		Last Modified: Tue, 12 Oct 2021 15:41:15 GMT  
		Size: 21.5 MB (21467885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b99a224b661061fbbe799d6efb95f01221754e6a73aec4d536865d1e304d63`  
		Last Modified: Tue, 12 Oct 2021 15:41:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce54581d99048d7f94f97b4e2d2f317ee3c9fdce5eb3c0d3cdb52072016660b7`  
		Last Modified: Tue, 12 Oct 2021 20:17:28 GMT  
		Size: 22.0 MB (22005026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daefdd420359fc022652bcdcc007e5e9d88c221bc93405f002f4cda2a25c8352`  
		Last Modified: Tue, 12 Oct 2021 20:17:24 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ded521f316c8b6d5264c9aef16c282663d5051d018db5dbaacee8fa8bee89b`  
		Last Modified: Tue, 12 Oct 2021 20:17:24 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cf6d98e001ee961ab070e0f4f81bb6752cf4b55a2681854b36c4052e3ef3e7`  
		Last Modified: Tue, 12 Oct 2021 20:17:24 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:6a62088d86817f5a29595eb1fc2ab816f6ec2c59e8a15f61569ded5c72c12512
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77116535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132b1e23200a63720a954040b718efbd99af50060ab64bba419ffbb9be2c97cd`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:42 GMT
ADD file:6524935705c59a0eda67f61fe1005a28b4b388258e2d5636dd5b831333200dc8 in / 
# Tue, 28 Sep 2021 01:51:43 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 18:48:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 18:48:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 28 Sep 2021 18:48:33 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 19:23:53 GMT
ENV RUBY_MAJOR=2.6
# Tue, 28 Sep 2021 19:23:53 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 28 Sep 2021 19:23:53 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 28 Sep 2021 19:28:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 28 Sep 2021 19:28:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 28 Sep 2021 19:28:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 28 Sep 2021 19:28:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 19:28:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 28 Sep 2021 19:28:24 GMT
CMD ["irb"]
# Wed, 29 Sep 2021 05:17:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 29 Sep 2021 05:17:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 29 Sep 2021 05:17:48 GMT
ENV TINI_VERSION=0.18.0
# Wed, 29 Sep 2021 05:21:28 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 29 Sep 2021 05:21:30 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 29 Sep 2021 05:21:31 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 29 Sep 2021 05:21:31 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 29 Sep 2021 05:21:31 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 29 Sep 2021 05:21:32 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 29 Sep 2021 05:21:32 GMT
EXPOSE 24224 5140
# Wed, 29 Sep 2021 05:21:33 GMT
USER fluent
# Wed, 29 Sep 2021 05:21:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 29 Sep 2021 05:21:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:85d14771cf32dc23d1c8e99a9aad844b3db9d67f4781455c81749ffe43b05513`  
		Last Modified: Tue, 28 Sep 2021 02:08:05 GMT  
		Size: 24.9 MB (24879067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67219e91075b17466704e8b77ae390b755ce0be763738dadf133450a8ff33b7`  
		Last Modified: Tue, 28 Sep 2021 19:34:50 GMT  
		Size: 10.3 MB (10348969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd11b3d5ad959051b468e4d6e1b98b58b9884dede42b4b9057de720132ba0628`  
		Last Modified: Tue, 28 Sep 2021 19:34:42 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48524c724f2b3b71b7bfc402fe4e371499a6bf88d9344c60a37b34ecd55dabd`  
		Last Modified: Tue, 28 Sep 2021 19:38:42 GMT  
		Size: 20.7 MB (20733397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a6f57f87784af7c75889748c13944d3abb353ffe4d36ccf8d6e8d69729dd26`  
		Last Modified: Tue, 28 Sep 2021 19:38:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f4d2dd963d05d6de7a50aa91138738a6c4a67bffb70cbf10548110eb85c332`  
		Last Modified: Wed, 29 Sep 2021 05:22:15 GMT  
		Size: 21.2 MB (21152033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2becef1bc430cfcf5318b0a899e2c67478de042c1588e82ee860fc3e69fcd12c`  
		Last Modified: Wed, 29 Sep 2021 05:22:02 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83777e50a34ce82c13d2a2b221ed64e9b57019776dbb6257c9cd17423efb2a8`  
		Last Modified: Wed, 29 Sep 2021 05:22:02 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1cb5df629ba47e397fe3930a7d96c42b995c19be2fa2536c9b70bfa1c6337`  
		Last Modified: Wed, 29 Sep 2021 05:22:02 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:954d67234440fc680257048451a422ae47c9b7abe44f2eeb172c480ea86e23db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74321495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99a8410e90ad45fe64a9d660c969c504ead37d96b6b13ebb14f42f06a1d6a412`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Sep 2021 18:04:11 GMT
ADD file:e71f315aa894d483f75b32109fff32974c43ce2e684cd28eb6492bc6fc450931 in / 
# Thu, 30 Sep 2021 18:04:12 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 22:39:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 22:39:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 01 Oct 2021 22:39:22 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 23:26:40 GMT
ENV RUBY_MAJOR=2.6
# Fri, 01 Oct 2021 23:26:40 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 01 Oct 2021 23:26:40 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 01 Oct 2021 23:30:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 01 Oct 2021 23:30:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 01 Oct 2021 23:30:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 01 Oct 2021 23:30:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 23:30:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 01 Oct 2021 23:30:58 GMT
CMD ["irb"]
# Sat, 02 Oct 2021 19:45:37 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Sat, 02 Oct 2021 19:45:37 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Sat, 02 Oct 2021 19:45:38 GMT
ENV TINI_VERSION=0.18.0
# Sat, 02 Oct 2021 19:49:00 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Sat, 02 Oct 2021 19:49:02 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Sat, 02 Oct 2021 19:49:02 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Sat, 02 Oct 2021 19:49:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Sat, 02 Oct 2021 19:49:04 GMT
ENV FLUENTD_CONF=fluent.conf
# Sat, 02 Oct 2021 19:49:04 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Sat, 02 Oct 2021 19:49:04 GMT
EXPOSE 24224 5140
# Sat, 02 Oct 2021 19:49:05 GMT
USER fluent
# Sat, 02 Oct 2021 19:49:05 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Sat, 02 Oct 2021 19:49:06 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:421f17c521234da0c5b07d4f6e44314149dc3790ef12134e85e61741452c9f96`  
		Last Modified: Thu, 30 Sep 2021 18:20:50 GMT  
		Size: 22.7 MB (22746246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0692ba1be6ebb6fe7fa2b8bf57a9dd0a4bb5354fbf13889f4b1035ed696c0baf`  
		Last Modified: Fri, 01 Oct 2021 23:38:49 GMT  
		Size: 9.9 MB (9872884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad1e8259356fdfb6c253c6c9dd4fff4d43cf28352a4c5f3216e67ddf4017fc2`  
		Last Modified: Fri, 01 Oct 2021 23:38:42 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6d848e6f9c9ad88f7c45c255801665fb3963a4adc43e3d6152fd874c1c317d`  
		Last Modified: Fri, 01 Oct 2021 23:42:54 GMT  
		Size: 20.6 MB (20643672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78592b256a1308d1146591647f808abc5a8de61af0288d7aa9b6adcb65c4e193`  
		Last Modified: Fri, 01 Oct 2021 23:42:46 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2575c1e72ae369804222eeaeddf4dc36f32d2d11bb4e638c874622e7d3f349c8`  
		Last Modified: Sat, 02 Oct 2021 19:49:48 GMT  
		Size: 21.1 MB (21055621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9cba1af80a06fa863a6dacd703131b2f9d384556d824f2471b7c7bc0a0977e`  
		Last Modified: Sat, 02 Oct 2021 19:49:35 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7d29ba2a73cdafb343028c628bb1f6dba91bb23fda9f62b8dd0054ef28fe7`  
		Last Modified: Sat, 02 Oct 2021 19:49:35 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace3248313b562881c10fe0d8e5d2159e323840ecb4f7e5dd2930f66b04de42c`  
		Last Modified: Sat, 02 Oct 2021 19:49:35 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:791cddf6300c4a3148adec03057d6d79a377062f7dd1bffb7b9a4fb88de05223
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80494194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a6ab60a8670f3a0ab00056a7171244da2c02014970934e617da87942916eab`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:13 GMT
ADD file:3e2426765cfe2b896fc847bcb435624930753c72ac00b87d2c73f4a81c813fd4 in / 
# Tue, 28 Sep 2021 01:41:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:12:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:12:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 28 Sep 2021 15:12:43 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 15:31:05 GMT
ENV RUBY_MAJOR=2.6
# Tue, 28 Sep 2021 15:31:05 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 28 Sep 2021 15:31:06 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 28 Sep 2021 15:33:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 28 Sep 2021 15:33:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 28 Sep 2021 15:33:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 28 Sep 2021 15:33:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 15:33:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 28 Sep 2021 15:33:16 GMT
CMD ["irb"]
# Wed, 29 Sep 2021 09:22:06 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 29 Sep 2021 09:22:06 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 29 Sep 2021 09:22:06 GMT
ENV TINI_VERSION=0.18.0
# Wed, 29 Sep 2021 09:23:50 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 29 Sep 2021 09:23:51 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 29 Sep 2021 09:23:52 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 29 Sep 2021 09:23:52 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 29 Sep 2021 09:23:52 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 29 Sep 2021 09:23:52 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 29 Sep 2021 09:23:52 GMT
EXPOSE 24224 5140
# Wed, 29 Sep 2021 09:23:52 GMT
USER fluent
# Wed, 29 Sep 2021 09:23:53 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 29 Sep 2021 09:23:53 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:896f18f54b28590b15a0f3354b13e8ea2f88a05f13de4117720f88cef30206ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:22 GMT  
		Size: 25.9 MB (25915039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cc0acef2e6aaa1fdfe65e13d5362898ed0d7e5e35620c50bee88bba231876d`  
		Last Modified: Tue, 28 Sep 2021 15:37:58 GMT  
		Size: 11.3 MB (11264477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2697264550a8ae7404f264263f6aff3741597dedc7ae31f97fd618c75fe3d366`  
		Last Modified: Tue, 28 Sep 2021 15:37:56 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42bc4b58d1156250b31014d7f12b2c6372cbef1733b6a7320094c8fcfe4a9ae`  
		Last Modified: Tue, 28 Sep 2021 15:40:50 GMT  
		Size: 21.3 MB (21309053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c904706c80aefa58a0674a4a2edd5e45aa322483116fb9de7574f18851ecd3`  
		Last Modified: Tue, 28 Sep 2021 15:40:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bca7f20eaa5d33c16efb4a35f5ae2fd77f47183cae3c43d98aef79b7dcbac22`  
		Last Modified: Wed, 29 Sep 2021 09:24:23 GMT  
		Size: 22.0 MB (22002546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bd5e7506d30b7f3b83e13f98d54c7e8372340112b85c3fc166d40f3b5cce3f`  
		Last Modified: Wed, 29 Sep 2021 09:24:19 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8b38098ec516f741dee50a8597ba4275d9944b1f5a9876778a9befbe3de7c0`  
		Last Modified: Wed, 29 Sep 2021 09:24:19 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34778854989ab5166ef55550cdee24bc4f3d1d1081cd84d341748c2288848427`  
		Last Modified: Wed, 29 Sep 2021 09:24:19 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:8b7d46815d25056c3b50e56879bfde7c64d2b0efac91a5dd4cd08ad826b9c01a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87126661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:807296930ed673ac8b6a3e1438b4f5d61501981e0745322ad64b0db589294e48`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:49 GMT
ADD file:c090abbb3afcfebf797e06e2ac4b778acb4e97d5dca79c29d1927f43cf14b23e in / 
# Tue, 28 Sep 2021 01:40:49 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 19:31:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 19:31:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 28 Sep 2021 19:31:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 20:00:41 GMT
ENV RUBY_MAJOR=2.6
# Tue, 28 Sep 2021 20:00:41 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 28 Sep 2021 20:00:41 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 28 Sep 2021 20:04:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 28 Sep 2021 20:04:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 28 Sep 2021 20:04:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 28 Sep 2021 20:04:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 20:04:16 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 28 Sep 2021 20:04:16 GMT
CMD ["irb"]
# Wed, 29 Sep 2021 06:40:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 29 Sep 2021 06:40:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 29 Sep 2021 06:40:52 GMT
ENV TINI_VERSION=0.18.0
# Wed, 29 Sep 2021 06:42:38 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 29 Sep 2021 06:42:39 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 29 Sep 2021 06:42:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 29 Sep 2021 06:42:40 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 29 Sep 2021 06:42:40 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 29 Sep 2021 06:42:41 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 29 Sep 2021 06:42:41 GMT
EXPOSE 24224 5140
# Wed, 29 Sep 2021 06:42:41 GMT
USER fluent
# Wed, 29 Sep 2021 06:42:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 29 Sep 2021 06:42:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:82f7c8b98609aee82696182c03cb09ae62ceab1b17f8eec1e233a68180876d41`  
		Last Modified: Tue, 28 Sep 2021 01:50:06 GMT  
		Size: 27.8 MB (27797629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd6ebe81fc32debaaf3e9bb15488927bad3277f8beccdc792bd3b6288995ee2`  
		Last Modified: Tue, 28 Sep 2021 20:09:31 GMT  
		Size: 17.2 MB (17226895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e1d8264f8156ea49a18e394b6b9eb180f17ac714622e30c2851d1572106784`  
		Last Modified: Tue, 28 Sep 2021 20:09:26 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2170515daa1310cdd92c2ec0f53c39022cd1b2bc2271f84154f77ed9daa91b`  
		Last Modified: Tue, 28 Sep 2021 20:12:47 GMT  
		Size: 20.9 MB (20910156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6af7a177e4c7bd2c13e2b8e6cc71dc32f4825d07356b6ad330601966c2aafe`  
		Last Modified: Tue, 28 Sep 2021 20:12:44 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28f813b6e684bc312a1769c6db8775f2c34a86ac11f329a00a48e6b03310d46`  
		Last Modified: Wed, 29 Sep 2021 06:43:12 GMT  
		Size: 21.2 MB (21188911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69d5bfb1a001c333fd9991574175f21106414b15f158aac10e9089aca0825a3`  
		Last Modified: Wed, 29 Sep 2021 06:43:06 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61db522f42ad3e0f546d9e7537119e694098414203d6d1f0fd7bc4bdbeede29`  
		Last Modified: Wed, 29 Sep 2021 06:43:06 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4312211c71347b20d0808077cc5c3968c0d3c3af1bc45bdc62fedebad2c4567e`  
		Last Modified: Wed, 29 Sep 2021 06:43:06 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:5ff9497480bac4a7e28f26d2f8840a4532d7ded41980baa094a543acd828d007
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87829230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d46a2394782b64591f2b709da27cbef3265233c47a80abbe874e0d153e9d04`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Oct 2021 17:56:14 GMT
ADD file:0b55ec14c2e9aa78512985a5bff3881b6fabf6794ce4406bb874b173d5a60799 in / 
# Mon, 04 Oct 2021 17:56:20 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 03:06:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 03:06:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 06 Oct 2021 03:06:23 GMT
ENV LANG=C.UTF-8
# Wed, 06 Oct 2021 03:52:55 GMT
ENV RUBY_MAJOR=2.6
# Wed, 06 Oct 2021 03:52:58 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 06 Oct 2021 03:53:00 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 06 Oct 2021 03:58:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 06 Oct 2021 03:58:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 06 Oct 2021 03:58:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 06 Oct 2021 03:58:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Oct 2021 03:58:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 06 Oct 2021 03:58:52 GMT
CMD ["irb"]
# Thu, 07 Oct 2021 05:16:48 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 07 Oct 2021 05:16:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 07 Oct 2021 05:17:01 GMT
ENV TINI_VERSION=0.18.0
# Thu, 07 Oct 2021 05:23:05 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 07 Oct 2021 05:23:14 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 07 Oct 2021 05:23:19 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 07 Oct 2021 05:23:20 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 07 Oct 2021 05:23:29 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 07 Oct 2021 05:23:31 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 07 Oct 2021 05:23:39 GMT
EXPOSE 24224 5140
# Thu, 07 Oct 2021 05:23:44 GMT
USER fluent
# Thu, 07 Oct 2021 05:23:52 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 07 Oct 2021 05:23:55 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:5736db2c6d2424206be3309412da520d7fe1fe4933cc2cc72641b311dd7d9099`  
		Last Modified: Mon, 04 Oct 2021 18:08:33 GMT  
		Size: 30.6 MB (30553728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3354ef54cd0e1052f9a547f02b1010929ef000aff902d0a370850998c897e3f6`  
		Last Modified: Wed, 06 Oct 2021 04:04:03 GMT  
		Size: 12.7 MB (12705362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bbab896c6e7a16a08fe33deb7eed7486092decdc1e5538684d5ba398e30390`  
		Last Modified: Wed, 06 Oct 2021 04:03:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf32a0e0567609d494382315cc5596d259b73adcc26d11a939dd971e9bbb65c`  
		Last Modified: Wed, 06 Oct 2021 04:07:23 GMT  
		Size: 22.0 MB (21984877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3ee4a3cdda80cbdd4c480d4d75a0893866585cbf00618cab4d2bab368496e`  
		Last Modified: Wed, 06 Oct 2021 04:07:21 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5616380b61838713c1ae2bf0758e79888afb65d11125a30241bb6d955cbfd2`  
		Last Modified: Thu, 07 Oct 2021 05:24:38 GMT  
		Size: 22.6 MB (22582171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427c23afd267d2099a889585e0531ef3e643f9babb47039f6c238e43310990bd`  
		Last Modified: Thu, 07 Oct 2021 05:24:29 GMT  
		Size: 1.9 KB (1851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b5358a5b979d699868997fe387d492664b19e48e02e5483a890bf092b15d19`  
		Last Modified: Thu, 07 Oct 2021 05:24:30 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a71dc2efd6d8ec1a1000311899164a3318d110ce0ccf85ff55cc4e9b52f209`  
		Last Modified: Thu, 07 Oct 2021 05:24:29 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:504be05ce004e64f11b088e7ceb13d5a218b611216e40efb7df1420ef416db3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80379203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd54a5a61800cf433f1ee567eb3ce0af1d1c66afec2ecad866642dc2bfa2d52`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:05:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:05:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 04:05:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:26:01 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 04:27:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 04:27:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 04:27:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 04:27:33 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 09:45:22 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 12 Oct 2021 09:45:22 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 12 Oct 2021 09:45:22 GMT
ENV TINI_VERSION=0.18.0
# Tue, 12 Oct 2021 09:46:40 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 12 Oct 2021 09:46:41 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 12 Oct 2021 09:46:41 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 12 Oct 2021 09:46:41 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 12 Oct 2021 09:46:42 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 12 Oct 2021 09:46:42 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 12 Oct 2021 09:46:42 GMT
EXPOSE 24224 5140
# Tue, 12 Oct 2021 09:46:42 GMT
USER fluent
# Tue, 12 Oct 2021 09:46:42 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 12 Oct 2021 09:46:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152601da1f670f23930e38f542a251b56290100e816cebfc101161c8e9d9823`  
		Last Modified: Tue, 12 Oct 2021 04:30:27 GMT  
		Size: 10.8 MB (10815329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379c6f49f1643cab68ffcf8d485cf085a0799907e6458c13a589142d6763809`  
		Last Modified: Tue, 12 Oct 2021 04:30:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58406908df2376127547311dc0ea98d9ef92a8573d1e0cb811fefa665bb3a84`  
		Last Modified: Tue, 12 Oct 2021 04:31:30 GMT  
		Size: 21.6 MB (21619749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb4ab84de8ab158c29c0c84a1b4726fd7c89ab7ff6fb27c139956d200f492b2`  
		Last Modified: Tue, 12 Oct 2021 04:31:29 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2694c92480617a6fe54d01b8a550ff5ecc516c2a899e78c76a15ccf410079ff`  
		Last Modified: Tue, 12 Oct 2021 09:47:11 GMT  
		Size: 22.2 MB (22186790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efee31c2b4b049cf332d1ffdca7978d2e15b630925f006435840c2b4b3366c68`  
		Last Modified: Tue, 12 Oct 2021 09:47:08 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff58fd2fae77d1de9c09fcf0fc811f28f51c66070043ac5015f1fa3c09d14172`  
		Last Modified: Tue, 12 Oct 2021 09:47:08 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ea6081abd1da3fb20e89016e642285b18972d4d0eba80a7e421a195afbc615`  
		Last Modified: Tue, 12 Oct 2021 09:47:08 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
