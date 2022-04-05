<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.14-1`](#fluentdv114-1)
-	[`fluentd:v1.14-debian-1`](#fluentdv114-debian-1)
-	[`fluentd:v1.14.0-1.0`](#fluentdv1140-10)
-	[`fluentd:v1.14.0-debian-1.0`](#fluentdv1140-debian-10)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:58e12480b6e2c165033acecb19839aa30540011292f896f1ce7d311594b12d8c
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
$ docker pull fluentd@sha256:9624d5acdaf03449120293a1f5332154dc9c2796fddf4b1f998aeee5aaca7027
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19140452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67baae9b19cfb841cf601e71744c8ca21215ace602e9f9f19a067db195f59fe2`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:31:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 05:31:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 05:31:53 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 05:31:54 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 05:31:54 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 05:31:54 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 05:31:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 05:31:54 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 05:31:55 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 05:31:55 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 05:31:55 GMT
USER fluent
# Tue, 05 Apr 2022 05:31:55 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 05:31:55 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936d25ead3b8f27d0334b355d9b92e616d40d9cc8430663aad2f5a7dae97fe70`  
		Last Modified: Tue, 05 Apr 2022 05:32:11 GMT  
		Size: 16.3 MB (16318942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17136e407c73d69fe22c40b78d0fd8362ad64a6ee12ac86078963008ed8de6ce`  
		Last Modified: Tue, 05 Apr 2022 05:32:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc407e43b50c4b653f48a4cb801756f119be7c9578a9426dfee249b75e1c095`  
		Last Modified: Tue, 05 Apr 2022 05:32:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16866cbcbbe2b12afffe51d9bb77aaacf05a7f77fa90414cca23ccb8b42d3a7d`  
		Last Modified: Tue, 05 Apr 2022 05:32:08 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:eccd3db54f9bc90a198b634e0e6a3987b7f35bd61ae36362b73d62afe8f9868f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18418380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c900544d36a12e0801f94e8e89f1a434d311239fe52840ec45b4596417731ab`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:47:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 03:47:01 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 03:49:04 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 03:49:07 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 03:49:07 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 03:49:08 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 03:49:08 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 03:49:09 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 03:49:09 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 03:49:10 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 03:49:10 GMT
USER fluent
# Tue, 05 Apr 2022 03:49:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 03:49:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba04dedd066e85ce0deb0792036097ac770d1cb776c943190c4aaad2ceaaaed9`  
		Last Modified: Tue, 05 Apr 2022 03:49:50 GMT  
		Size: 15.8 MB (15791034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9882a5266134e1ff2c8a0f5ccbf7fbdf77b9813066d0aac67351dc607bd22f1`  
		Last Modified: Tue, 05 Apr 2022 03:49:38 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b311ddae61d7c4492bbca6f8cee231eb0a43e5db843fee98d54fd0d1a5ccef81`  
		Last Modified: Tue, 05 Apr 2022 03:49:38 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5bd91546af2bfd1dd7cc77fb8d6e9583ed5abd335c2d626f51adaa57111b3f`  
		Last Modified: Tue, 05 Apr 2022 03:49:38 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:9c0a4a84381fbbeb0395dde2fe0bee86b10175d37a709e26fd605d8f9067ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18972013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e0fbbb0f44e27ef9cc9444a08b96deccfa95b0a1ca69617abe6de2a22cdad5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:48:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 07:48:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 07:49:14 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 07:49:15 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 07:49:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 07:49:18 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 07:49:18 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 07:49:19 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 07:49:20 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 07:49:21 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 07:49:22 GMT
USER fluent
# Tue, 05 Apr 2022 07:49:23 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 07:49:24 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4d143b870226d5f39fdb8712aa4a5601a1f92e4b54f9dada0506bc3bb13b45`  
		Last Modified: Tue, 05 Apr 2022 07:49:54 GMT  
		Size: 16.2 MB (16248964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4683f09bd99f0a5d12da8c36d87c3f80cf54f591b19de3b614b1517ed3799a0d`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120b5acf02cc6a091e3e5c982d71e683eebcbfe34dc73d38a806c24cf01ab732`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f8e42a7770e420773b29e879e7fcf9d5a5c9f80bf8b6eaf7f78448964ebcf1`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; 386

```console
$ docker pull fluentd@sha256:299d9671ba5bfb7b1c1f507b810efd0e6ffd5b5640c4a58ec3d10b2c78721170
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18646603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9fa1724795ff480c4df555cdd5e9b00905a02e71d0b1798862bef43a7adef09`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:49:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 06:49:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 06:50:11 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 06:50:12 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 06:50:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 06:50:15 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 06:50:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 06:50:16 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 06:50:17 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 06:50:18 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 06:50:19 GMT
USER fluent
# Tue, 05 Apr 2022 06:50:20 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 06:50:21 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81503ac049ce7244d3d38dea8d6628e3a8f3686b552eaa595832e851e7b24cec`  
		Last Modified: Tue, 05 Apr 2022 06:50:56 GMT  
		Size: 15.8 MB (15823915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbeb39e9230acf9694ec1b22e134b093b296107b64469c70133d6d96925349ce`  
		Last Modified: Tue, 05 Apr 2022 06:50:54 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c386bf86331003882f38a6998054b3db51f3338d97967bf34e86bb481a6fb8b5`  
		Last Modified: Tue, 05 Apr 2022 06:50:54 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221067b38e66567afa51f469318ebf7a16ad4bc4e39538ae40f9b68ee5dde54b`  
		Last Modified: Tue, 05 Apr 2022 06:50:54 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:74396e82970758c21f00286817fc1072e3f4eddf4059b3e8a9a1399dfcbfa7d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19177382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47dc73169025ebbdee5656614778fbbc1de53028a8df347516e3898f794f91d4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:02:42 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 29 Mar 2022 07:02:48 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 29 Mar 2022 07:04:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 29 Mar 2022 07:04:57 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 29 Mar 2022 07:05:00 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 29 Mar 2022 07:05:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 29 Mar 2022 07:05:11 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 29 Mar 2022 07:05:26 GMT
ENV LD_PRELOAD=
# Tue, 29 Mar 2022 07:05:33 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 29 Mar 2022 07:05:40 GMT
EXPOSE 24224 5140
# Tue, 29 Mar 2022 07:05:47 GMT
USER fluent
# Tue, 29 Mar 2022 07:05:52 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 29 Mar 2022 07:06:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437ffd869a8c005426a744ae803dbee5ec8f9e8eeb4fde014c61bff713c7ab47`  
		Last Modified: Tue, 29 Mar 2022 07:06:47 GMT  
		Size: 16.4 MB (16360320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e2918b4bef90b68239dad4d6b5f536e1f85586531c935f7fedcacc0b9e118`  
		Last Modified: Tue, 29 Mar 2022 07:06:43 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9254a848c77f3292b5ca1ebc3438d2e530fd1375ea2461133f74127cf216547c`  
		Last Modified: Tue, 29 Mar 2022 07:06:44 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6903793bd754af57f6f05215379f86959e367647eb69b9f26422992204491a65`  
		Last Modified: Tue, 29 Mar 2022 07:06:43 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:fcf8dc973f484df1b04d6770c54b7097f210a9494760448791cd473fd8e018b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18833986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a47b04692700f8d50356c0605419b39a0a0a3d4dd8933335802d78dc996253ea`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:56:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 03:56:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 03:57:28 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 03:57:30 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 03:57:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 03:57:30 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 03:57:30 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 03:57:30 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 03:57:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 03:57:30 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 03:57:31 GMT
USER fluent
# Tue, 05 Apr 2022 03:57:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 03:57:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80885e5fcbe2d38543d5e0902ede12aac0343ddb30a4b60bc4d78867956435ce`  
		Last Modified: Tue, 05 Apr 2022 03:58:02 GMT  
		Size: 16.2 MB (16226727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37dee1aa1774c4de428bdaced201f30a775a16bb7da2c3d9a6ae31bebaed78`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da865ce216091b128ba285b8c6097d5b808474cbe95220b3d9d5e88e6a25fbd`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ad6695a5e27dd3ddaec0e5987c6384aa0eeb5374548d4e86df5137d86bd62c`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14-1`

```console
$ docker pull fluentd@sha256:58e12480b6e2c165033acecb19839aa30540011292f896f1ce7d311594b12d8c
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
$ docker pull fluentd@sha256:9624d5acdaf03449120293a1f5332154dc9c2796fddf4b1f998aeee5aaca7027
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19140452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67baae9b19cfb841cf601e71744c8ca21215ace602e9f9f19a067db195f59fe2`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:31:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 05:31:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 05:31:53 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 05:31:54 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 05:31:54 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 05:31:54 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 05:31:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 05:31:54 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 05:31:55 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 05:31:55 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 05:31:55 GMT
USER fluent
# Tue, 05 Apr 2022 05:31:55 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 05:31:55 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936d25ead3b8f27d0334b355d9b92e616d40d9cc8430663aad2f5a7dae97fe70`  
		Last Modified: Tue, 05 Apr 2022 05:32:11 GMT  
		Size: 16.3 MB (16318942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17136e407c73d69fe22c40b78d0fd8362ad64a6ee12ac86078963008ed8de6ce`  
		Last Modified: Tue, 05 Apr 2022 05:32:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc407e43b50c4b653f48a4cb801756f119be7c9578a9426dfee249b75e1c095`  
		Last Modified: Tue, 05 Apr 2022 05:32:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16866cbcbbe2b12afffe51d9bb77aaacf05a7f77fa90414cca23ccb8b42d3a7d`  
		Last Modified: Tue, 05 Apr 2022 05:32:08 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:eccd3db54f9bc90a198b634e0e6a3987b7f35bd61ae36362b73d62afe8f9868f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18418380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c900544d36a12e0801f94e8e89f1a434d311239fe52840ec45b4596417731ab`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:47:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 03:47:01 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 03:49:04 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 03:49:07 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 03:49:07 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 03:49:08 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 03:49:08 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 03:49:09 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 03:49:09 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 03:49:10 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 03:49:10 GMT
USER fluent
# Tue, 05 Apr 2022 03:49:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 03:49:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba04dedd066e85ce0deb0792036097ac770d1cb776c943190c4aaad2ceaaaed9`  
		Last Modified: Tue, 05 Apr 2022 03:49:50 GMT  
		Size: 15.8 MB (15791034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9882a5266134e1ff2c8a0f5ccbf7fbdf77b9813066d0aac67351dc607bd22f1`  
		Last Modified: Tue, 05 Apr 2022 03:49:38 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b311ddae61d7c4492bbca6f8cee231eb0a43e5db843fee98d54fd0d1a5ccef81`  
		Last Modified: Tue, 05 Apr 2022 03:49:38 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5bd91546af2bfd1dd7cc77fb8d6e9583ed5abd335c2d626f51adaa57111b3f`  
		Last Modified: Tue, 05 Apr 2022 03:49:38 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:9c0a4a84381fbbeb0395dde2fe0bee86b10175d37a709e26fd605d8f9067ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18972013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e0fbbb0f44e27ef9cc9444a08b96deccfa95b0a1ca69617abe6de2a22cdad5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:48:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 07:48:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 07:49:14 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 07:49:15 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 07:49:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 07:49:18 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 07:49:18 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 07:49:19 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 07:49:20 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 07:49:21 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 07:49:22 GMT
USER fluent
# Tue, 05 Apr 2022 07:49:23 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 07:49:24 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4d143b870226d5f39fdb8712aa4a5601a1f92e4b54f9dada0506bc3bb13b45`  
		Last Modified: Tue, 05 Apr 2022 07:49:54 GMT  
		Size: 16.2 MB (16248964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4683f09bd99f0a5d12da8c36d87c3f80cf54f591b19de3b614b1517ed3799a0d`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120b5acf02cc6a091e3e5c982d71e683eebcbfe34dc73d38a806c24cf01ab732`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f8e42a7770e420773b29e879e7fcf9d5a5c9f80bf8b6eaf7f78448964ebcf1`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; 386

```console
$ docker pull fluentd@sha256:299d9671ba5bfb7b1c1f507b810efd0e6ffd5b5640c4a58ec3d10b2c78721170
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18646603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9fa1724795ff480c4df555cdd5e9b00905a02e71d0b1798862bef43a7adef09`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:49:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 06:49:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 06:50:11 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 06:50:12 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 06:50:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 06:50:15 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 06:50:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 06:50:16 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 06:50:17 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 06:50:18 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 06:50:19 GMT
USER fluent
# Tue, 05 Apr 2022 06:50:20 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 06:50:21 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81503ac049ce7244d3d38dea8d6628e3a8f3686b552eaa595832e851e7b24cec`  
		Last Modified: Tue, 05 Apr 2022 06:50:56 GMT  
		Size: 15.8 MB (15823915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbeb39e9230acf9694ec1b22e134b093b296107b64469c70133d6d96925349ce`  
		Last Modified: Tue, 05 Apr 2022 06:50:54 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c386bf86331003882f38a6998054b3db51f3338d97967bf34e86bb481a6fb8b5`  
		Last Modified: Tue, 05 Apr 2022 06:50:54 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221067b38e66567afa51f469318ebf7a16ad4bc4e39538ae40f9b68ee5dde54b`  
		Last Modified: Tue, 05 Apr 2022 06:50:54 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:74396e82970758c21f00286817fc1072e3f4eddf4059b3e8a9a1399dfcbfa7d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19177382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47dc73169025ebbdee5656614778fbbc1de53028a8df347516e3898f794f91d4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:02:42 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 29 Mar 2022 07:02:48 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 29 Mar 2022 07:04:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 29 Mar 2022 07:04:57 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 29 Mar 2022 07:05:00 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 29 Mar 2022 07:05:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 29 Mar 2022 07:05:11 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 29 Mar 2022 07:05:26 GMT
ENV LD_PRELOAD=
# Tue, 29 Mar 2022 07:05:33 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 29 Mar 2022 07:05:40 GMT
EXPOSE 24224 5140
# Tue, 29 Mar 2022 07:05:47 GMT
USER fluent
# Tue, 29 Mar 2022 07:05:52 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 29 Mar 2022 07:06:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437ffd869a8c005426a744ae803dbee5ec8f9e8eeb4fde014c61bff713c7ab47`  
		Last Modified: Tue, 29 Mar 2022 07:06:47 GMT  
		Size: 16.4 MB (16360320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e2918b4bef90b68239dad4d6b5f536e1f85586531c935f7fedcacc0b9e118`  
		Last Modified: Tue, 29 Mar 2022 07:06:43 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9254a848c77f3292b5ca1ebc3438d2e530fd1375ea2461133f74127cf216547c`  
		Last Modified: Tue, 29 Mar 2022 07:06:44 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6903793bd754af57f6f05215379f86959e367647eb69b9f26422992204491a65`  
		Last Modified: Tue, 29 Mar 2022 07:06:43 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-1` - linux; s390x

```console
$ docker pull fluentd@sha256:fcf8dc973f484df1b04d6770c54b7097f210a9494760448791cd473fd8e018b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18833986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a47b04692700f8d50356c0605419b39a0a0a3d4dd8933335802d78dc996253ea`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:56:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 03:56:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 03:57:28 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 03:57:30 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 03:57:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 03:57:30 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 03:57:30 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 03:57:30 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 03:57:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 03:57:30 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 03:57:31 GMT
USER fluent
# Tue, 05 Apr 2022 03:57:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 03:57:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80885e5fcbe2d38543d5e0902ede12aac0343ddb30a4b60bc4d78867956435ce`  
		Last Modified: Tue, 05 Apr 2022 03:58:02 GMT  
		Size: 16.2 MB (16226727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37dee1aa1774c4de428bdaced201f30a775a16bb7da2c3d9a6ae31bebaed78`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da865ce216091b128ba285b8c6097d5b808474cbe95220b3d9d5e88e6a25fbd`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ad6695a5e27dd3ddaec0e5987c6384aa0eeb5374548d4e86df5137d86bd62c`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14-debian-1`

```console
$ docker pull fluentd@sha256:b34ba5f961a3d3d73c3377492b3982c03d35449f7557f8499b061515d723b7c5
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
$ docker pull fluentd@sha256:041991c4d3b39999aeaef9218733abf056418e0529fbd2dd77cab8d12169906c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83283167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2bd6365a693f4134d00b581f27947b7f805af5cca9d0591737357a8312d02d3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:32:17 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 10:32:17 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:09:10 GMT
ENV RUBY_MAJOR=2.6
# Tue, 29 Mar 2022 11:09:10 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 29 Mar 2022 11:09:10 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 29 Mar 2022 11:11:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 29 Mar 2022 11:11:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 29 Mar 2022 11:11:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 29 Mar 2022 11:11:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 11:11:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 29 Mar 2022 11:11:35 GMT
CMD ["irb"]
# Tue, 29 Mar 2022 12:08:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 29 Mar 2022 12:08:00 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 29 Mar 2022 12:08:00 GMT
ENV TINI_VERSION=0.18.0
# Tue, 29 Mar 2022 12:09:16 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 29 Mar 2022 12:09:16 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 29 Mar 2022 12:09:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 29 Mar 2022 12:09:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 29 Mar 2022 12:09:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 29 Mar 2022 12:09:17 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 29 Mar 2022 12:09:17 GMT
EXPOSE 24224 5140
# Tue, 29 Mar 2022 12:09:17 GMT
USER fluent
# Tue, 29 Mar 2022 12:09:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 29 Mar 2022 12:09:17 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f50025d0672279ac92c03f9450d7acd8865318daf73a2ac10dcc574ce8597b`  
		Last Modified: Tue, 29 Mar 2022 11:19:28 GMT  
		Size: 12.6 MB (12581277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5812fdc56bb069b5ee346cc2335a2233b171cbec31ff56d4c2fb7fd7727b4d9`  
		Last Modified: Tue, 29 Mar 2022 11:19:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f5df3ee9a9220264a3aa410db4a01b41b3e0befad894ef873563594ba8a734`  
		Last Modified: Tue, 29 Mar 2022 11:22:56 GMT  
		Size: 21.5 MB (21499670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef0095d54b23f7af992ebce05d5f546ea45fbfc670091847512877ac7174f94`  
		Last Modified: Tue, 29 Mar 2022 11:22:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29518ca34abcc93c9fef21db6613b211ec11193b61e67be6df6aa55dd8340f29`  
		Last Modified: Tue, 29 Mar 2022 12:09:49 GMT  
		Size: 22.0 MB (22047166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96a85a812f7d5e364a30421d559e2c63e7518e353ab1cbc2cd2c86a9408401c`  
		Last Modified: Tue, 29 Mar 2022 12:09:46 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753f0f47910fb78876b6407c11f32a5fd2504a06a22f081cd89276d832e35335`  
		Last Modified: Tue, 29 Mar 2022 12:09:46 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a625a1d7557ee9d61fb8799f9eae75d262e9342bdee13cdeba04b5a820a725b4`  
		Last Modified: Tue, 29 Mar 2022 12:09:46 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:d656fe1f8a7f1e23ec873cc4f25ba7c4f030178b3ac9fd4ed2f9a42b4212c08f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77208381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f317e2626a67fa267fc87201a354c517485c889270b1e47492501f623d8f6d36`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:36 GMT
ADD file:7ac5498e2c44686d7eb272ef7645a0a64486cf942610f6754aa4a932f5b1a4be in / 
# Tue, 29 Mar 2022 00:51:37 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 23:55:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 23:55:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 23:55:22 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 00:50:53 GMT
ENV RUBY_MAJOR=2.6
# Wed, 30 Mar 2022 00:50:53 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 30 Mar 2022 00:50:54 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 30 Mar 2022 00:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 30 Mar 2022 00:55:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 30 Mar 2022 00:55:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 30 Mar 2022 00:55:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 00:55:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 30 Mar 2022 00:55:18 GMT
CMD ["irb"]
# Wed, 30 Mar 2022 16:12:15 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 30 Mar 2022 16:12:15 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 30 Mar 2022 16:12:16 GMT
ENV TINI_VERSION=0.18.0
# Wed, 30 Mar 2022 16:15:53 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 30 Mar 2022 16:15:55 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 30 Mar 2022 16:15:55 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 30 Mar 2022 16:15:56 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 30 Mar 2022 16:15:56 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 30 Mar 2022 16:15:57 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 30 Mar 2022 16:15:57 GMT
EXPOSE 24224 5140
# Wed, 30 Mar 2022 16:15:57 GMT
USER fluent
# Wed, 30 Mar 2022 16:15:58 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 30 Mar 2022 16:15:58 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:8f10b1b67f0119a2dd5f838a3e98ab2c412e4b51fb1e4841e2b79fd4cae86105`  
		Last Modified: Tue, 29 Mar 2022 01:06:51 GMT  
		Size: 24.9 MB (24887495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d61cee00ab1594084e741b9bc23ddac1a53d682cf9002f20009b3954f152f4`  
		Last Modified: Wed, 30 Mar 2022 01:02:28 GMT  
		Size: 10.4 MB (10360014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771b0d8ac0e9af8ec47a4e53390a9ea93d2f590387ef3585cfd09f151cdfe5ac`  
		Last Modified: Wed, 30 Mar 2022 01:02:21 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d66a5d4bacf9d15c5dc3df764141e1f36dccfa0781ed31a25989baa49d633`  
		Last Modified: Wed, 30 Mar 2022 01:08:06 GMT  
		Size: 20.8 MB (20761443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fa0e2a74fa04306284d775fd22b1e83d9baee0a88d059c0638849877de142e`  
		Last Modified: Wed, 30 Mar 2022 01:07:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c000066185c53f4dca76b4a836bff6b26fdb5a5ef4c703d9e44a3d466bf7fd4`  
		Last Modified: Wed, 30 Mar 2022 16:16:46 GMT  
		Size: 21.2 MB (21196354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5780bed88d4c137e104f1d1300d915614928dcdb07b5e314ea2c4bf9e81aa144`  
		Last Modified: Wed, 30 Mar 2022 16:16:33 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a99a970331d421d4adf1cb56ec8d52ffe0feed64830a6a176d4d106dc7533d`  
		Last Modified: Wed, 30 Mar 2022 16:16:33 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39e7941e79a1621b84aa2be11aee400bf647f21009a1d6e92648c0ee30773b6`  
		Last Modified: Wed, 30 Mar 2022 16:16:33 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:82293fc5d265522625d006ff0ed1ca570b6ce9014c7356eb95a679397245755f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74391319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c23d95fccf6b10a4a9158baecbb01e4258a31c9113f4fd7b8a0c522abfc3913`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 02:19:40 GMT
ADD file:8d54e000817531229c35a32eee074105c7b4d3c08b7ca56b1abdd80571687f28 in / 
# Tue, 29 Mar 2022 02:19:41 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 15:13:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 15:13:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 30 Mar 2022 15:13:30 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 16:07:43 GMT
ENV RUBY_MAJOR=2.6
# Wed, 30 Mar 2022 16:07:43 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 30 Mar 2022 16:07:44 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 30 Mar 2022 16:11:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 30 Mar 2022 16:11:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 30 Mar 2022 16:11:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 30 Mar 2022 16:11:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 16:11:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 30 Mar 2022 16:12:00 GMT
CMD ["irb"]
# Thu, 31 Mar 2022 16:35:19 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 31 Mar 2022 16:35:19 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 31 Mar 2022 16:35:19 GMT
ENV TINI_VERSION=0.18.0
# Thu, 31 Mar 2022 16:38:37 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 31 Mar 2022 16:38:39 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 31 Mar 2022 16:38:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 31 Mar 2022 16:38:40 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 31 Mar 2022 16:38:40 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 31 Mar 2022 16:38:41 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 31 Mar 2022 16:38:41 GMT
EXPOSE 24224 5140
# Thu, 31 Mar 2022 16:38:42 GMT
USER fluent
# Thu, 31 Mar 2022 16:38:42 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 31 Mar 2022 16:38:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:d4bf0b27c669e589de33695047d638174fc2ca819a4366d5f80d1ad6b01c0c0e`  
		Last Modified: Tue, 29 Mar 2022 02:35:26 GMT  
		Size: 22.8 MB (22753045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04862a4df372593524d65e6b7c2365699b0398767c88c0fab28bf6a99781d104`  
		Last Modified: Wed, 30 Mar 2022 16:28:04 GMT  
		Size: 9.9 MB (9878660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548be5969b8b14b8d1bcf6dc49c6a130fe52b692a652b5b24817fea6db90f73b`  
		Last Modified: Wed, 30 Mar 2022 16:27:57 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535dc7086445db768e5a623cf5303dff117dba87a81cd70059f39eaa3ef22f9`  
		Last Modified: Wed, 30 Mar 2022 16:34:44 GMT  
		Size: 20.7 MB (20671983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13f47a1b3ec5c506273dff8f4b89b39ff2339f6d695550f6ff60f42ad03a3c7`  
		Last Modified: Wed, 30 Mar 2022 16:34:34 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c19fe6d4f2b6209daddc32a1f379c0045a6c307e2bde6b81955cf77fdc732af`  
		Last Modified: Thu, 31 Mar 2022 16:39:18 GMT  
		Size: 21.1 MB (21084552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b39fc07bc42171bd64966151cd545c2a187996c11bb6205885a9259c1e3b03`  
		Last Modified: Thu, 31 Mar 2022 16:39:06 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0af2ce697fb9556a4c47d0066c4057c621e3f6156f2be0c1c4502c5db457c5c`  
		Last Modified: Thu, 31 Mar 2022 16:39:06 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006922c578bafa59a4207873cd8581036ea9094e88d5583814c927d34364bb75`  
		Last Modified: Thu, 31 Mar 2022 16:39:05 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:3c03d769cd552de56cae1ff606efb5fe5f9aa7d1e1cfa3bcf772f8b8e88912ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.2 MB (80158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c14cb51be2632876fdaa98bc5c00f87e773403a181a2a6857758b82e7dc984a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:42 GMT
ADD file:fdc8a5391a75cbf8c121f8f799ca08e94d2b3967b2546b36231c9297f7ce2151 in / 
# Tue, 29 Mar 2022 00:43:43 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:07:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 01:07:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 30 Mar 2022 01:07:59 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 01:51:03 GMT
ENV RUBY_MAJOR=2.6
# Wed, 30 Mar 2022 01:51:03 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 30 Mar 2022 01:51:04 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 30 Mar 2022 01:53:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 30 Mar 2022 01:53:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 30 Mar 2022 01:53:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 30 Mar 2022 01:53:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 01:53:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 30 Mar 2022 01:53:33 GMT
CMD ["irb"]
# Wed, 30 Mar 2022 21:54:37 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 30 Mar 2022 21:54:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 30 Mar 2022 21:54:39 GMT
ENV TINI_VERSION=0.18.0
# Wed, 30 Mar 2022 21:56:04 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 30 Mar 2022 21:56:05 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 30 Mar 2022 21:56:06 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 30 Mar 2022 21:56:07 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 30 Mar 2022 21:56:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 30 Mar 2022 21:56:08 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 30 Mar 2022 21:56:09 GMT
EXPOSE 24224 5140
# Wed, 30 Mar 2022 21:56:10 GMT
USER fluent
# Wed, 30 Mar 2022 21:56:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 30 Mar 2022 21:56:12 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:5022906f515a0d4ec6bc1d0e5e7a01f47b1fbbb912e7e3f1ace27987169a9a21`  
		Last Modified: Tue, 29 Mar 2022 00:50:58 GMT  
		Size: 25.9 MB (25919777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e3b5e34538914ef987dcf4cb0510a9cfe8a87fc125a5becc70001d361c786`  
		Last Modified: Wed, 30 Mar 2022 02:05:21 GMT  
		Size: 11.3 MB (11280384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba948d1a3c98e143c52c978123573078325be9c0af31e4058612687efebfdfb`  
		Last Modified: Wed, 30 Mar 2022 02:05:19 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414161481edc6a6f4a4d19d73e0fa8e2ba2bf981112d1c6b6bf5d3329349faf6`  
		Last Modified: Wed, 30 Mar 2022 02:09:41 GMT  
		Size: 21.1 MB (21124676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d389668796fa88725fc723e8c5a7361c09107cdfd208b3f661ae40b97a01c5bf`  
		Last Modified: Wed, 30 Mar 2022 02:09:39 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6a34d7c0ed01b9e91283ab03f0ef765b68d26210e09e6a8242fa801e93fc5c`  
		Last Modified: Wed, 30 Mar 2022 21:56:41 GMT  
		Size: 21.8 MB (21831211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c11206bd4e004af2dd88de35b32fedc4d2680e2fdcc560a750536c0e3b9708`  
		Last Modified: Wed, 30 Mar 2022 21:56:32 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e2bd26c0d4ef2282b8cf39a6566bf34f07786dc6a67748d0835328d8d5caed`  
		Last Modified: Wed, 30 Mar 2022 21:56:32 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b0f9eadbb41ce520dee402100c04dd2f5fe77b7ad47c1d7286aaa929bc0ee4`  
		Last Modified: Wed, 30 Mar 2022 21:56:32 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:955b28154bebf5baddcca0dac8bf05c1f0d304627b5481f6b6d6f66f531797fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86784032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d24ad15f2d5f74bcd9796873a3237716d60a6794583edf9e67e2d87419c036`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:26 GMT
ADD file:bcf3d504dc285de8b639c7f4017c41a4593a6c2aa6f046c9be79e587d05b5120 in / 
# Tue, 29 Mar 2022 00:42:27 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:00:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:00:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 10:00:17 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 10:28:16 GMT
ENV RUBY_MAJOR=2.6
# Tue, 29 Mar 2022 10:28:17 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 29 Mar 2022 10:28:18 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 29 Mar 2022 10:30:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 29 Mar 2022 10:30:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 29 Mar 2022 10:30:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 29 Mar 2022 10:30:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:30:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 29 Mar 2022 10:30:09 GMT
CMD ["irb"]
# Tue, 29 Mar 2022 23:11:13 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 29 Mar 2022 23:11:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 29 Mar 2022 23:11:15 GMT
ENV TINI_VERSION=0.18.0
# Tue, 29 Mar 2022 23:12:34 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 29 Mar 2022 23:12:35 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 29 Mar 2022 23:12:36 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 29 Mar 2022 23:12:37 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 29 Mar 2022 23:12:37 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 29 Mar 2022 23:12:38 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 29 Mar 2022 23:12:39 GMT
EXPOSE 24224 5140
# Tue, 29 Mar 2022 23:12:40 GMT
USER fluent
# Tue, 29 Mar 2022 23:12:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 29 Mar 2022 23:12:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:65b92490caa5e2c0588fab60d39315a2a8c09aa8ea0fe208d23f6984a47ecc03`  
		Last Modified: Tue, 29 Mar 2022 00:50:02 GMT  
		Size: 27.8 MB (27801252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a237049b615c6378412074b43b9be2a006a39ce2774924350cb13cf964196eb`  
		Last Modified: Tue, 29 Mar 2022 10:38:43 GMT  
		Size: 17.2 MB (17235396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b347ed75fb0e86c7dc48ba6f435bc768d9dab571bbb43ab3c59fcf217720b0`  
		Last Modified: Tue, 29 Mar 2022 10:38:40 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52dd970f365dfc71f0cccf5cc4adfbc501ccb8877f528a2a4feae8ccc08f773`  
		Last Modified: Tue, 29 Mar 2022 10:43:12 GMT  
		Size: 20.7 MB (20730521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d7b627bbbe90bf1a6c1b760ed7ff39aae1df765a0601ae0b57579d7dc1e0c2`  
		Last Modified: Tue, 29 Mar 2022 10:43:09 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6817082f2ab1e2a255768a5a2648b42cb55dc9138a7ee3f09bb7d25955b26da4`  
		Last Modified: Tue, 29 Mar 2022 23:13:15 GMT  
		Size: 21.0 MB (21013969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5969a0bc2ee2d318ca6106c0741f0c3f35c5431e61834530f6cf96d8c0d5d8`  
		Last Modified: Tue, 29 Mar 2022 23:13:11 GMT  
		Size: 1.7 KB (1690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e0ace038547457d89125ff75a379351aea8e108cdc0a47f5f2656295cf986e`  
		Last Modified: Tue, 29 Mar 2022 23:13:11 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b784f3c1ba79d2304637bb7d1a5eca89ca779d9b0027b7ef7ebf0c7ddb8e344`  
		Last Modified: Tue, 29 Mar 2022 23:13:11 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:989d8f1bfe768a97f6e2ea16a84b925d99b6edcf0c400091992590377a38ecc6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87935114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaac4e68e8fe3ba61ec4557da59ed02ff29400c455b59c8782be010dec0841df`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:59 GMT
ADD file:7271d778d432a07f57fedf8d50d83699ef545acc9db9346f6fe75b0054af4cd1 in / 
# Tue, 29 Mar 2022 00:23:00 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 20:23:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 20:23:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 20:23:19 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 21:30:34 GMT
ENV RUBY_MAJOR=2.6
# Tue, 29 Mar 2022 21:30:38 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 29 Mar 2022 21:30:41 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 29 Mar 2022 21:39:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 29 Mar 2022 21:39:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 29 Mar 2022 21:39:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 29 Mar 2022 21:39:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 21:39:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 29 Mar 2022 21:39:41 GMT
CMD ["irb"]
# Thu, 31 Mar 2022 07:43:21 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 31 Mar 2022 07:43:32 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 31 Mar 2022 07:43:43 GMT
ENV TINI_VERSION=0.18.0
# Thu, 31 Mar 2022 07:51:34 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 31 Mar 2022 07:51:53 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 31 Mar 2022 07:51:55 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 31 Mar 2022 07:51:57 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 31 Mar 2022 07:52:02 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 31 Mar 2022 07:52:05 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 31 Mar 2022 07:52:10 GMT
EXPOSE 24224 5140
# Thu, 31 Mar 2022 07:52:14 GMT
USER fluent
# Thu, 31 Mar 2022 07:52:19 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 31 Mar 2022 07:52:29 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7db831386ce67ac1cf2b4f1513fe3746c9ea2b8d4c82efca75be638eaf533614`  
		Last Modified: Tue, 29 Mar 2022 00:34:41 GMT  
		Size: 30.6 MB (30560163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308b496e1e95a5feaf264a7cc31e6b3c3374fe5e96c73fe9189627bc50dc558`  
		Last Modified: Tue, 29 Mar 2022 21:51:39 GMT  
		Size: 12.7 MB (12724933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2deab05a4a7c0b5c756150a843ec69322aa059b31c6b469fae6c15e5e74aaa25`  
		Last Modified: Tue, 29 Mar 2022 21:51:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f0a35ca2769ec55d71f410f5d08ac7e45b1bf18dfa5a17d50f8f05152c194a`  
		Last Modified: Tue, 29 Mar 2022 21:56:22 GMT  
		Size: 22.0 MB (22023986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f97273e93ae2fe876a65e78747af44593b94b399040a171bac17bdbbb6acb6`  
		Last Modified: Tue, 29 Mar 2022 21:56:19 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b003f751454321978e44824a15ab720c39002e3ffb65661fc30f89189890f51`  
		Last Modified: Thu, 31 Mar 2022 07:53:06 GMT  
		Size: 22.6 MB (22622942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5eedff3ff03861cb4381102a43056a352a2358e161624d34d6bacea87a4411`  
		Last Modified: Thu, 31 Mar 2022 07:53:00 GMT  
		Size: 1.8 KB (1848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522fa6af9c82b8dfb969d4b73131b20d01df1eec8e7af2f8087ad272e82f88b4`  
		Last Modified: Thu, 31 Mar 2022 07:53:00 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e078a3e517d50e9b364620e7bb02e5686903af0d0f7239b37bb4df6372540354`  
		Last Modified: Thu, 31 Mar 2022 07:53:00 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:ac330e0e0b3071afc3eef56901d8707e620cb972ae9ce7f63f2f71d8b27f9e69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80465601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc664b4e73304827a754cb1671a9d480672a41c41cd62497ea9d21b77d812f7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:52:27 GMT
ADD file:dbf01085079906b34f3ec9db0b9ce31aa1466b935a47e8e30772a5488f76fec0 in / 
# Tue, 29 Mar 2022 00:52:29 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 23:33:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 23:33:42 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 23:33:43 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 23:59:48 GMT
ENV RUBY_MAJOR=2.6
# Tue, 29 Mar 2022 23:59:48 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 29 Mar 2022 23:59:48 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 30 Mar 2022 00:01:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 30 Mar 2022 00:01:26 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 30 Mar 2022 00:01:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 30 Mar 2022 00:01:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 00:01:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 30 Mar 2022 00:01:27 GMT
CMD ["irb"]
# Wed, 30 Mar 2022 15:02:38 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 30 Mar 2022 15:02:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 30 Mar 2022 15:02:38 GMT
ENV TINI_VERSION=0.18.0
# Wed, 30 Mar 2022 15:03:59 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 30 Mar 2022 15:04:01 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 30 Mar 2022 15:04:01 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 30 Mar 2022 15:04:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 30 Mar 2022 15:04:01 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 30 Mar 2022 15:04:01 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 30 Mar 2022 15:04:01 GMT
EXPOSE 24224 5140
# Wed, 30 Mar 2022 15:04:01 GMT
USER fluent
# Wed, 30 Mar 2022 15:04:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 30 Mar 2022 15:04:01 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:66ccc81b275f683f44a0f40ddce6992117eefe92dca84fadf6d2e51c22d11a64`  
		Last Modified: Tue, 29 Mar 2022 01:10:22 GMT  
		Size: 25.8 MB (25765916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c7fef25a0104760352e9846edcca0599e6167969de298ead38bb9f0845ae59`  
		Last Modified: Wed, 30 Mar 2022 00:13:23 GMT  
		Size: 10.8 MB (10826282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb216b7b703c4afd0ec4fdc5ab770e98ddc5e4ab72b12f1a48dc83b985c39ee2`  
		Last Modified: Wed, 30 Mar 2022 00:13:23 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acd651cf7f219b34108b8e0c2723d3b52a15ef3bc3fcb42c8c49336e6178f9`  
		Last Modified: Wed, 30 Mar 2022 00:40:14 GMT  
		Size: 21.6 MB (21644993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bfe1468da328f616766642f208547bc2f50d0a4931e852e368334e0710c16d`  
		Last Modified: Wed, 30 Mar 2022 00:40:14 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22500aea0e2398dc904dd288938eab5fdc6c0d7fe6a8de3423788a25bcced254`  
		Last Modified: Wed, 30 Mar 2022 15:04:30 GMT  
		Size: 22.2 MB (22225325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab2bafe9863bae31aed4a3944d8aa130db3c148ab64ab2fbee83d730279bd19`  
		Last Modified: Wed, 30 Mar 2022 15:04:28 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39180924d7042649a3a1e10e38444e0b22aa47aa6f1d0f2b8eae9941aaa8cf7f`  
		Last Modified: Wed, 30 Mar 2022 15:04:28 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8012fea02cbea16fbda10b38eacf74efe04b8759f5fc72d9743c7ad47960a069`  
		Last Modified: Wed, 30 Mar 2022 15:04:28 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14.0-1.0`

```console
$ docker pull fluentd@sha256:58e12480b6e2c165033acecb19839aa30540011292f896f1ce7d311594b12d8c
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
$ docker pull fluentd@sha256:9624d5acdaf03449120293a1f5332154dc9c2796fddf4b1f998aeee5aaca7027
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19140452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67baae9b19cfb841cf601e71744c8ca21215ace602e9f9f19a067db195f59fe2`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:31:10 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 05:31:10 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 05:31:53 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 05:31:54 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 05:31:54 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 05:31:54 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 05:31:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 05:31:54 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 05:31:55 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 05:31:55 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 05:31:55 GMT
USER fluent
# Tue, 05 Apr 2022 05:31:55 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 05:31:55 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936d25ead3b8f27d0334b355d9b92e616d40d9cc8430663aad2f5a7dae97fe70`  
		Last Modified: Tue, 05 Apr 2022 05:32:11 GMT  
		Size: 16.3 MB (16318942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17136e407c73d69fe22c40b78d0fd8362ad64a6ee12ac86078963008ed8de6ce`  
		Last Modified: Tue, 05 Apr 2022 05:32:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc407e43b50c4b653f48a4cb801756f119be7c9578a9426dfee249b75e1c095`  
		Last Modified: Tue, 05 Apr 2022 05:32:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16866cbcbbe2b12afffe51d9bb77aaacf05a7f77fa90414cca23ccb8b42d3a7d`  
		Last Modified: Tue, 05 Apr 2022 05:32:08 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:eccd3db54f9bc90a198b634e0e6a3987b7f35bd61ae36362b73d62afe8f9868f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18418380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c900544d36a12e0801f94e8e89f1a434d311239fe52840ec45b4596417731ab`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:47:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 03:47:01 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 03:49:04 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 03:49:07 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 03:49:07 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 03:49:08 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 03:49:08 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 03:49:09 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 03:49:09 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 03:49:10 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 03:49:10 GMT
USER fluent
# Tue, 05 Apr 2022 03:49:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 03:49:11 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba04dedd066e85ce0deb0792036097ac770d1cb776c943190c4aaad2ceaaaed9`  
		Last Modified: Tue, 05 Apr 2022 03:49:50 GMT  
		Size: 15.8 MB (15791034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9882a5266134e1ff2c8a0f5ccbf7fbdf77b9813066d0aac67351dc607bd22f1`  
		Last Modified: Tue, 05 Apr 2022 03:49:38 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b311ddae61d7c4492bbca6f8cee231eb0a43e5db843fee98d54fd0d1a5ccef81`  
		Last Modified: Tue, 05 Apr 2022 03:49:38 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5bd91546af2bfd1dd7cc77fb8d6e9583ed5abd335c2d626f51adaa57111b3f`  
		Last Modified: Tue, 05 Apr 2022 03:49:38 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:9c0a4a84381fbbeb0395dde2fe0bee86b10175d37a709e26fd605d8f9067ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18972013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e0fbbb0f44e27ef9cc9444a08b96deccfa95b0a1ca69617abe6de2a22cdad5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:48:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 07:48:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 07:49:14 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 07:49:15 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 07:49:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 07:49:18 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 07:49:18 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 07:49:19 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 07:49:20 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 07:49:21 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 07:49:22 GMT
USER fluent
# Tue, 05 Apr 2022 07:49:23 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 07:49:24 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4d143b870226d5f39fdb8712aa4a5601a1f92e4b54f9dada0506bc3bb13b45`  
		Last Modified: Tue, 05 Apr 2022 07:49:54 GMT  
		Size: 16.2 MB (16248964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4683f09bd99f0a5d12da8c36d87c3f80cf54f591b19de3b614b1517ed3799a0d`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120b5acf02cc6a091e3e5c982d71e683eebcbfe34dc73d38a806c24cf01ab732`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f8e42a7770e420773b29e879e7fcf9d5a5c9f80bf8b6eaf7f78448964ebcf1`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:299d9671ba5bfb7b1c1f507b810efd0e6ffd5b5640c4a58ec3d10b2c78721170
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18646603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9fa1724795ff480c4df555cdd5e9b00905a02e71d0b1798862bef43a7adef09`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:49:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 06:49:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 06:50:11 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 06:50:12 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 06:50:14 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 06:50:15 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 06:50:15 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 06:50:16 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 06:50:17 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 06:50:18 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 06:50:19 GMT
USER fluent
# Tue, 05 Apr 2022 06:50:20 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 06:50:21 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81503ac049ce7244d3d38dea8d6628e3a8f3686b552eaa595832e851e7b24cec`  
		Last Modified: Tue, 05 Apr 2022 06:50:56 GMT  
		Size: 15.8 MB (15823915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbeb39e9230acf9694ec1b22e134b093b296107b64469c70133d6d96925349ce`  
		Last Modified: Tue, 05 Apr 2022 06:50:54 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c386bf86331003882f38a6998054b3db51f3338d97967bf34e86bb481a6fb8b5`  
		Last Modified: Tue, 05 Apr 2022 06:50:54 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221067b38e66567afa51f469318ebf7a16ad4bc4e39538ae40f9b68ee5dde54b`  
		Last Modified: Tue, 05 Apr 2022 06:50:54 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:74396e82970758c21f00286817fc1072e3f4eddf4059b3e8a9a1399dfcbfa7d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19177382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47dc73169025ebbdee5656614778fbbc1de53028a8df347516e3898f794f91d4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:02:42 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 29 Mar 2022 07:02:48 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 29 Mar 2022 07:04:39 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 29 Mar 2022 07:04:57 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 29 Mar 2022 07:05:00 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 29 Mar 2022 07:05:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 29 Mar 2022 07:05:11 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 29 Mar 2022 07:05:26 GMT
ENV LD_PRELOAD=
# Tue, 29 Mar 2022 07:05:33 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 29 Mar 2022 07:05:40 GMT
EXPOSE 24224 5140
# Tue, 29 Mar 2022 07:05:47 GMT
USER fluent
# Tue, 29 Mar 2022 07:05:52 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 29 Mar 2022 07:06:02 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437ffd869a8c005426a744ae803dbee5ec8f9e8eeb4fde014c61bff713c7ab47`  
		Last Modified: Tue, 29 Mar 2022 07:06:47 GMT  
		Size: 16.4 MB (16360320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2e2918b4bef90b68239dad4d6b5f536e1f85586531c935f7fedcacc0b9e118`  
		Last Modified: Tue, 29 Mar 2022 07:06:43 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9254a848c77f3292b5ca1ebc3438d2e530fd1375ea2461133f74127cf216547c`  
		Last Modified: Tue, 29 Mar 2022 07:06:44 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6903793bd754af57f6f05215379f86959e367647eb69b9f26422992204491a65`  
		Last Modified: Tue, 29 Mar 2022 07:06:43 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:fcf8dc973f484df1b04d6770c54b7097f210a9494760448791cd473fd8e018b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18833986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a47b04692700f8d50356c0605419b39a0a0a3d4dd8933335802d78dc996253ea`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:56:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 03:56:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 03:57:28 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 03:57:30 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 03:57:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 03:57:30 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 03:57:30 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 03:57:30 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 03:57:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 03:57:30 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 03:57:31 GMT
USER fluent
# Tue, 05 Apr 2022 03:57:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 03:57:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80885e5fcbe2d38543d5e0902ede12aac0343ddb30a4b60bc4d78867956435ce`  
		Last Modified: Tue, 05 Apr 2022 03:58:02 GMT  
		Size: 16.2 MB (16226727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37dee1aa1774c4de428bdaced201f30a775a16bb7da2c3d9a6ae31bebaed78`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da865ce216091b128ba285b8c6097d5b808474cbe95220b3d9d5e88e6a25fbd`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ad6695a5e27dd3ddaec0e5987c6384aa0eeb5374548d4e86df5137d86bd62c`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.14.0-debian-1.0`

```console
$ docker pull fluentd@sha256:b34ba5f961a3d3d73c3377492b3982c03d35449f7557f8499b061515d723b7c5
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
$ docker pull fluentd@sha256:041991c4d3b39999aeaef9218733abf056418e0529fbd2dd77cab8d12169906c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83283167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2bd6365a693f4134d00b581f27947b7f805af5cca9d0591737357a8312d02d3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:32:17 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 10:32:17 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:09:10 GMT
ENV RUBY_MAJOR=2.6
# Tue, 29 Mar 2022 11:09:10 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 29 Mar 2022 11:09:10 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 29 Mar 2022 11:11:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 29 Mar 2022 11:11:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 29 Mar 2022 11:11:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 29 Mar 2022 11:11:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 11:11:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 29 Mar 2022 11:11:35 GMT
CMD ["irb"]
# Tue, 29 Mar 2022 12:08:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 29 Mar 2022 12:08:00 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 29 Mar 2022 12:08:00 GMT
ENV TINI_VERSION=0.18.0
# Tue, 29 Mar 2022 12:09:16 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 29 Mar 2022 12:09:16 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 29 Mar 2022 12:09:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 29 Mar 2022 12:09:17 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 29 Mar 2022 12:09:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 29 Mar 2022 12:09:17 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 29 Mar 2022 12:09:17 GMT
EXPOSE 24224 5140
# Tue, 29 Mar 2022 12:09:17 GMT
USER fluent
# Tue, 29 Mar 2022 12:09:17 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 29 Mar 2022 12:09:17 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f50025d0672279ac92c03f9450d7acd8865318daf73a2ac10dcc574ce8597b`  
		Last Modified: Tue, 29 Mar 2022 11:19:28 GMT  
		Size: 12.6 MB (12581277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5812fdc56bb069b5ee346cc2335a2233b171cbec31ff56d4c2fb7fd7727b4d9`  
		Last Modified: Tue, 29 Mar 2022 11:19:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f5df3ee9a9220264a3aa410db4a01b41b3e0befad894ef873563594ba8a734`  
		Last Modified: Tue, 29 Mar 2022 11:22:56 GMT  
		Size: 21.5 MB (21499670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef0095d54b23f7af992ebce05d5f546ea45fbfc670091847512877ac7174f94`  
		Last Modified: Tue, 29 Mar 2022 11:22:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29518ca34abcc93c9fef21db6613b211ec11193b61e67be6df6aa55dd8340f29`  
		Last Modified: Tue, 29 Mar 2022 12:09:49 GMT  
		Size: 22.0 MB (22047166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96a85a812f7d5e364a30421d559e2c63e7518e353ab1cbc2cd2c86a9408401c`  
		Last Modified: Tue, 29 Mar 2022 12:09:46 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753f0f47910fb78876b6407c11f32a5fd2504a06a22f081cd89276d832e35335`  
		Last Modified: Tue, 29 Mar 2022 12:09:46 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a625a1d7557ee9d61fb8799f9eae75d262e9342bdee13cdeba04b5a820a725b4`  
		Last Modified: Tue, 29 Mar 2022 12:09:46 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:d656fe1f8a7f1e23ec873cc4f25ba7c4f030178b3ac9fd4ed2f9a42b4212c08f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77208381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f317e2626a67fa267fc87201a354c517485c889270b1e47492501f623d8f6d36`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:36 GMT
ADD file:7ac5498e2c44686d7eb272ef7645a0a64486cf942610f6754aa4a932f5b1a4be in / 
# Tue, 29 Mar 2022 00:51:37 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 23:55:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 23:55:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 23:55:22 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 00:50:53 GMT
ENV RUBY_MAJOR=2.6
# Wed, 30 Mar 2022 00:50:53 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 30 Mar 2022 00:50:54 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 30 Mar 2022 00:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 30 Mar 2022 00:55:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 30 Mar 2022 00:55:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 30 Mar 2022 00:55:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 00:55:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 30 Mar 2022 00:55:18 GMT
CMD ["irb"]
# Wed, 30 Mar 2022 16:12:15 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 30 Mar 2022 16:12:15 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 30 Mar 2022 16:12:16 GMT
ENV TINI_VERSION=0.18.0
# Wed, 30 Mar 2022 16:15:53 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 30 Mar 2022 16:15:55 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 30 Mar 2022 16:15:55 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 30 Mar 2022 16:15:56 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 30 Mar 2022 16:15:56 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 30 Mar 2022 16:15:57 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 30 Mar 2022 16:15:57 GMT
EXPOSE 24224 5140
# Wed, 30 Mar 2022 16:15:57 GMT
USER fluent
# Wed, 30 Mar 2022 16:15:58 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 30 Mar 2022 16:15:58 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:8f10b1b67f0119a2dd5f838a3e98ab2c412e4b51fb1e4841e2b79fd4cae86105`  
		Last Modified: Tue, 29 Mar 2022 01:06:51 GMT  
		Size: 24.9 MB (24887495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d61cee00ab1594084e741b9bc23ddac1a53d682cf9002f20009b3954f152f4`  
		Last Modified: Wed, 30 Mar 2022 01:02:28 GMT  
		Size: 10.4 MB (10360014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771b0d8ac0e9af8ec47a4e53390a9ea93d2f590387ef3585cfd09f151cdfe5ac`  
		Last Modified: Wed, 30 Mar 2022 01:02:21 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d66a5d4bacf9d15c5dc3df764141e1f36dccfa0781ed31a25989baa49d633`  
		Last Modified: Wed, 30 Mar 2022 01:08:06 GMT  
		Size: 20.8 MB (20761443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fa0e2a74fa04306284d775fd22b1e83d9baee0a88d059c0638849877de142e`  
		Last Modified: Wed, 30 Mar 2022 01:07:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c000066185c53f4dca76b4a836bff6b26fdb5a5ef4c703d9e44a3d466bf7fd4`  
		Last Modified: Wed, 30 Mar 2022 16:16:46 GMT  
		Size: 21.2 MB (21196354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5780bed88d4c137e104f1d1300d915614928dcdb07b5e314ea2c4bf9e81aa144`  
		Last Modified: Wed, 30 Mar 2022 16:16:33 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a99a970331d421d4adf1cb56ec8d52ffe0feed64830a6a176d4d106dc7533d`  
		Last Modified: Wed, 30 Mar 2022 16:16:33 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39e7941e79a1621b84aa2be11aee400bf647f21009a1d6e92648c0ee30773b6`  
		Last Modified: Wed, 30 Mar 2022 16:16:33 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:82293fc5d265522625d006ff0ed1ca570b6ce9014c7356eb95a679397245755f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74391319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c23d95fccf6b10a4a9158baecbb01e4258a31c9113f4fd7b8a0c522abfc3913`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 02:19:40 GMT
ADD file:8d54e000817531229c35a32eee074105c7b4d3c08b7ca56b1abdd80571687f28 in / 
# Tue, 29 Mar 2022 02:19:41 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 15:13:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 15:13:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 30 Mar 2022 15:13:30 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 16:07:43 GMT
ENV RUBY_MAJOR=2.6
# Wed, 30 Mar 2022 16:07:43 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 30 Mar 2022 16:07:44 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 30 Mar 2022 16:11:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 30 Mar 2022 16:11:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 30 Mar 2022 16:11:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 30 Mar 2022 16:11:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 16:11:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 30 Mar 2022 16:12:00 GMT
CMD ["irb"]
# Thu, 31 Mar 2022 16:35:19 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 31 Mar 2022 16:35:19 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 31 Mar 2022 16:35:19 GMT
ENV TINI_VERSION=0.18.0
# Thu, 31 Mar 2022 16:38:37 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 31 Mar 2022 16:38:39 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 31 Mar 2022 16:38:40 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 31 Mar 2022 16:38:40 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 31 Mar 2022 16:38:40 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 31 Mar 2022 16:38:41 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 31 Mar 2022 16:38:41 GMT
EXPOSE 24224 5140
# Thu, 31 Mar 2022 16:38:42 GMT
USER fluent
# Thu, 31 Mar 2022 16:38:42 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 31 Mar 2022 16:38:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:d4bf0b27c669e589de33695047d638174fc2ca819a4366d5f80d1ad6b01c0c0e`  
		Last Modified: Tue, 29 Mar 2022 02:35:26 GMT  
		Size: 22.8 MB (22753045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04862a4df372593524d65e6b7c2365699b0398767c88c0fab28bf6a99781d104`  
		Last Modified: Wed, 30 Mar 2022 16:28:04 GMT  
		Size: 9.9 MB (9878660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548be5969b8b14b8d1bcf6dc49c6a130fe52b692a652b5b24817fea6db90f73b`  
		Last Modified: Wed, 30 Mar 2022 16:27:57 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535dc7086445db768e5a623cf5303dff117dba87a81cd70059f39eaa3ef22f9`  
		Last Modified: Wed, 30 Mar 2022 16:34:44 GMT  
		Size: 20.7 MB (20671983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13f47a1b3ec5c506273dff8f4b89b39ff2339f6d695550f6ff60f42ad03a3c7`  
		Last Modified: Wed, 30 Mar 2022 16:34:34 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c19fe6d4f2b6209daddc32a1f379c0045a6c307e2bde6b81955cf77fdc732af`  
		Last Modified: Thu, 31 Mar 2022 16:39:18 GMT  
		Size: 21.1 MB (21084552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b39fc07bc42171bd64966151cd545c2a187996c11bb6205885a9259c1e3b03`  
		Last Modified: Thu, 31 Mar 2022 16:39:06 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0af2ce697fb9556a4c47d0066c4057c621e3f6156f2be0c1c4502c5db457c5c`  
		Last Modified: Thu, 31 Mar 2022 16:39:06 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006922c578bafa59a4207873cd8581036ea9094e88d5583814c927d34364bb75`  
		Last Modified: Thu, 31 Mar 2022 16:39:05 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:3c03d769cd552de56cae1ff606efb5fe5f9aa7d1e1cfa3bcf772f8b8e88912ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.2 MB (80158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c14cb51be2632876fdaa98bc5c00f87e773403a181a2a6857758b82e7dc984a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:42 GMT
ADD file:fdc8a5391a75cbf8c121f8f799ca08e94d2b3967b2546b36231c9297f7ce2151 in / 
# Tue, 29 Mar 2022 00:43:43 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:07:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 01:07:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 30 Mar 2022 01:07:59 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 01:51:03 GMT
ENV RUBY_MAJOR=2.6
# Wed, 30 Mar 2022 01:51:03 GMT
ENV RUBY_VERSION=2.6.9
# Wed, 30 Mar 2022 01:51:04 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 30 Mar 2022 01:53:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 30 Mar 2022 01:53:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 30 Mar 2022 01:53:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 30 Mar 2022 01:53:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 01:53:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 30 Mar 2022 01:53:33 GMT
CMD ["irb"]
# Wed, 30 Mar 2022 21:54:37 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 30 Mar 2022 21:54:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 30 Mar 2022 21:54:39 GMT
ENV TINI_VERSION=0.18.0
# Wed, 30 Mar 2022 21:56:04 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 30 Mar 2022 21:56:05 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 30 Mar 2022 21:56:06 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 30 Mar 2022 21:56:07 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 30 Mar 2022 21:56:07 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 30 Mar 2022 21:56:08 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 30 Mar 2022 21:56:09 GMT
EXPOSE 24224 5140
# Wed, 30 Mar 2022 21:56:10 GMT
USER fluent
# Wed, 30 Mar 2022 21:56:11 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 30 Mar 2022 21:56:12 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:5022906f515a0d4ec6bc1d0e5e7a01f47b1fbbb912e7e3f1ace27987169a9a21`  
		Last Modified: Tue, 29 Mar 2022 00:50:58 GMT  
		Size: 25.9 MB (25919777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e3b5e34538914ef987dcf4cb0510a9cfe8a87fc125a5becc70001d361c786`  
		Last Modified: Wed, 30 Mar 2022 02:05:21 GMT  
		Size: 11.3 MB (11280384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba948d1a3c98e143c52c978123573078325be9c0af31e4058612687efebfdfb`  
		Last Modified: Wed, 30 Mar 2022 02:05:19 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414161481edc6a6f4a4d19d73e0fa8e2ba2bf981112d1c6b6bf5d3329349faf6`  
		Last Modified: Wed, 30 Mar 2022 02:09:41 GMT  
		Size: 21.1 MB (21124676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d389668796fa88725fc723e8c5a7361c09107cdfd208b3f661ae40b97a01c5bf`  
		Last Modified: Wed, 30 Mar 2022 02:09:39 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6a34d7c0ed01b9e91283ab03f0ef765b68d26210e09e6a8242fa801e93fc5c`  
		Last Modified: Wed, 30 Mar 2022 21:56:41 GMT  
		Size: 21.8 MB (21831211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c11206bd4e004af2dd88de35b32fedc4d2680e2fdcc560a750536c0e3b9708`  
		Last Modified: Wed, 30 Mar 2022 21:56:32 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e2bd26c0d4ef2282b8cf39a6566bf34f07786dc6a67748d0835328d8d5caed`  
		Last Modified: Wed, 30 Mar 2022 21:56:32 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b0f9eadbb41ce520dee402100c04dd2f5fe77b7ad47c1d7286aaa929bc0ee4`  
		Last Modified: Wed, 30 Mar 2022 21:56:32 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; 386

```console
$ docker pull fluentd@sha256:955b28154bebf5baddcca0dac8bf05c1f0d304627b5481f6b6d6f66f531797fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86784032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d24ad15f2d5f74bcd9796873a3237716d60a6794583edf9e67e2d87419c036`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:26 GMT
ADD file:bcf3d504dc285de8b639c7f4017c41a4593a6c2aa6f046c9be79e587d05b5120 in / 
# Tue, 29 Mar 2022 00:42:27 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:00:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:00:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 10:00:17 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 10:28:16 GMT
ENV RUBY_MAJOR=2.6
# Tue, 29 Mar 2022 10:28:17 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 29 Mar 2022 10:28:18 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 29 Mar 2022 10:30:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 29 Mar 2022 10:30:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 29 Mar 2022 10:30:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 29 Mar 2022 10:30:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:30:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 29 Mar 2022 10:30:09 GMT
CMD ["irb"]
# Tue, 29 Mar 2022 23:11:13 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 29 Mar 2022 23:11:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 29 Mar 2022 23:11:15 GMT
ENV TINI_VERSION=0.18.0
# Tue, 29 Mar 2022 23:12:34 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 29 Mar 2022 23:12:35 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 29 Mar 2022 23:12:36 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 29 Mar 2022 23:12:37 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 29 Mar 2022 23:12:37 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 29 Mar 2022 23:12:38 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 29 Mar 2022 23:12:39 GMT
EXPOSE 24224 5140
# Tue, 29 Mar 2022 23:12:40 GMT
USER fluent
# Tue, 29 Mar 2022 23:12:41 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 29 Mar 2022 23:12:42 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:65b92490caa5e2c0588fab60d39315a2a8c09aa8ea0fe208d23f6984a47ecc03`  
		Last Modified: Tue, 29 Mar 2022 00:50:02 GMT  
		Size: 27.8 MB (27801252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a237049b615c6378412074b43b9be2a006a39ce2774924350cb13cf964196eb`  
		Last Modified: Tue, 29 Mar 2022 10:38:43 GMT  
		Size: 17.2 MB (17235396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b347ed75fb0e86c7dc48ba6f435bc768d9dab571bbb43ab3c59fcf217720b0`  
		Last Modified: Tue, 29 Mar 2022 10:38:40 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52dd970f365dfc71f0cccf5cc4adfbc501ccb8877f528a2a4feae8ccc08f773`  
		Last Modified: Tue, 29 Mar 2022 10:43:12 GMT  
		Size: 20.7 MB (20730521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d7b627bbbe90bf1a6c1b760ed7ff39aae1df765a0601ae0b57579d7dc1e0c2`  
		Last Modified: Tue, 29 Mar 2022 10:43:09 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6817082f2ab1e2a255768a5a2648b42cb55dc9138a7ee3f09bb7d25955b26da4`  
		Last Modified: Tue, 29 Mar 2022 23:13:15 GMT  
		Size: 21.0 MB (21013969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5969a0bc2ee2d318ca6106c0741f0c3f35c5431e61834530f6cf96d8c0d5d8`  
		Last Modified: Tue, 29 Mar 2022 23:13:11 GMT  
		Size: 1.7 KB (1690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e0ace038547457d89125ff75a379351aea8e108cdc0a47f5f2656295cf986e`  
		Last Modified: Tue, 29 Mar 2022 23:13:11 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b784f3c1ba79d2304637bb7d1a5eca89ca779d9b0027b7ef7ebf0c7ddb8e344`  
		Last Modified: Tue, 29 Mar 2022 23:13:11 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; ppc64le

```console
$ docker pull fluentd@sha256:989d8f1bfe768a97f6e2ea16a84b925d99b6edcf0c400091992590377a38ecc6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87935114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaac4e68e8fe3ba61ec4557da59ed02ff29400c455b59c8782be010dec0841df`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:59 GMT
ADD file:7271d778d432a07f57fedf8d50d83699ef545acc9db9346f6fe75b0054af4cd1 in / 
# Tue, 29 Mar 2022 00:23:00 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 20:23:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 20:23:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 20:23:19 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 21:30:34 GMT
ENV RUBY_MAJOR=2.6
# Tue, 29 Mar 2022 21:30:38 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 29 Mar 2022 21:30:41 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Tue, 29 Mar 2022 21:39:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 29 Mar 2022 21:39:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 29 Mar 2022 21:39:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 29 Mar 2022 21:39:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 21:39:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 29 Mar 2022 21:39:41 GMT
CMD ["irb"]
# Thu, 31 Mar 2022 07:43:21 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 31 Mar 2022 07:43:32 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Thu, 31 Mar 2022 07:43:43 GMT
ENV TINI_VERSION=0.18.0
# Thu, 31 Mar 2022 07:51:34 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Thu, 31 Mar 2022 07:51:53 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 31 Mar 2022 07:51:55 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 31 Mar 2022 07:51:57 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 31 Mar 2022 07:52:02 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 31 Mar 2022 07:52:05 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 31 Mar 2022 07:52:10 GMT
EXPOSE 24224 5140
# Thu, 31 Mar 2022 07:52:14 GMT
USER fluent
# Thu, 31 Mar 2022 07:52:19 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 31 Mar 2022 07:52:29 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7db831386ce67ac1cf2b4f1513fe3746c9ea2b8d4c82efca75be638eaf533614`  
		Last Modified: Tue, 29 Mar 2022 00:34:41 GMT  
		Size: 30.6 MB (30560163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308b496e1e95a5feaf264a7cc31e6b3c3374fe5e96c73fe9189627bc50dc558`  
		Last Modified: Tue, 29 Mar 2022 21:51:39 GMT  
		Size: 12.7 MB (12724933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2deab05a4a7c0b5c756150a843ec69322aa059b31c6b469fae6c15e5e74aaa25`  
		Last Modified: Tue, 29 Mar 2022 21:51:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f0a35ca2769ec55d71f410f5d08ac7e45b1bf18dfa5a17d50f8f05152c194a`  
		Last Modified: Tue, 29 Mar 2022 21:56:22 GMT  
		Size: 22.0 MB (22023986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f97273e93ae2fe876a65e78747af44593b94b399040a171bac17bdbbb6acb6`  
		Last Modified: Tue, 29 Mar 2022 21:56:19 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b003f751454321978e44824a15ab720c39002e3ffb65661fc30f89189890f51`  
		Last Modified: Thu, 31 Mar 2022 07:53:06 GMT  
		Size: 22.6 MB (22622942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5eedff3ff03861cb4381102a43056a352a2358e161624d34d6bacea87a4411`  
		Last Modified: Thu, 31 Mar 2022 07:53:00 GMT  
		Size: 1.8 KB (1848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522fa6af9c82b8dfb969d4b73131b20d01df1eec8e7af2f8087ad272e82f88b4`  
		Last Modified: Thu, 31 Mar 2022 07:53:00 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e078a3e517d50e9b364620e7bb02e5686903af0d0f7239b37bb4df6372540354`  
		Last Modified: Thu, 31 Mar 2022 07:53:00 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.14.0-debian-1.0` - linux; s390x

```console
$ docker pull fluentd@sha256:ac330e0e0b3071afc3eef56901d8707e620cb972ae9ce7f63f2f71d8b27f9e69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80465601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc664b4e73304827a754cb1671a9d480672a41c41cd62497ea9d21b77d812f7`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 29 Mar 2022 00:52:27 GMT
ADD file:dbf01085079906b34f3ec9db0b9ce31aa1466b935a47e8e30772a5488f76fec0 in / 
# Tue, 29 Mar 2022 00:52:29 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 23:33:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 23:33:42 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 23:33:43 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 23:59:48 GMT
ENV RUBY_MAJOR=2.6
# Tue, 29 Mar 2022 23:59:48 GMT
ENV RUBY_VERSION=2.6.9
# Tue, 29 Mar 2022 23:59:48 GMT
ENV RUBY_DOWNLOAD_SHA256=6a041d82ae6e0f02ccb1465e620d94a7196489d8a13d6018a160da42ebc1eece
# Wed, 30 Mar 2022 00:01:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 30 Mar 2022 00:01:26 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 30 Mar 2022 00:01:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 30 Mar 2022 00:01:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 00:01:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 30 Mar 2022 00:01:27 GMT
CMD ["irb"]
# Wed, 30 Mar 2022 15:02:38 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 30 Mar 2022 15:02:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 30 Mar 2022 15:02:38 GMT
ENV TINI_VERSION=0.18.0
# Wed, 30 Mar 2022 15:03:59 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-4.5.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/4.5.0/jemalloc-4.5.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-4.5.0.tar.bz2 && cd jemalloc-4.5.0/  && ./configure && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 30 Mar 2022 15:04:01 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 30 Mar 2022 15:04:01 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 30 Mar 2022 15:04:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 30 Mar 2022 15:04:01 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 30 Mar 2022 15:04:01 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Wed, 30 Mar 2022 15:04:01 GMT
EXPOSE 24224 5140
# Wed, 30 Mar 2022 15:04:01 GMT
USER fluent
# Wed, 30 Mar 2022 15:04:01 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 30 Mar 2022 15:04:01 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:66ccc81b275f683f44a0f40ddce6992117eefe92dca84fadf6d2e51c22d11a64`  
		Last Modified: Tue, 29 Mar 2022 01:10:22 GMT  
		Size: 25.8 MB (25765916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c7fef25a0104760352e9846edcca0599e6167969de298ead38bb9f0845ae59`  
		Last Modified: Wed, 30 Mar 2022 00:13:23 GMT  
		Size: 10.8 MB (10826282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb216b7b703c4afd0ec4fdc5ab770e98ddc5e4ab72b12f1a48dc83b985c39ee2`  
		Last Modified: Wed, 30 Mar 2022 00:13:23 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acd651cf7f219b34108b8e0c2723d3b52a15ef3bc3fcb42c8c49336e6178f9`  
		Last Modified: Wed, 30 Mar 2022 00:40:14 GMT  
		Size: 21.6 MB (21644993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bfe1468da328f616766642f208547bc2f50d0a4931e852e368334e0710c16d`  
		Last Modified: Wed, 30 Mar 2022 00:40:14 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22500aea0e2398dc904dd288938eab5fdc6c0d7fe6a8de3423788a25bcced254`  
		Last Modified: Wed, 30 Mar 2022 15:04:30 GMT  
		Size: 22.2 MB (22225325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab2bafe9863bae31aed4a3944d8aa130db3c148ab64ab2fbee83d730279bd19`  
		Last Modified: Wed, 30 Mar 2022 15:04:28 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39180924d7042649a3a1e10e38444e0b22aa47aa6f1d0f2b8eae9941aaa8cf7f`  
		Last Modified: Wed, 30 Mar 2022 15:04:28 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8012fea02cbea16fbda10b38eacf74efe04b8759f5fc72d9743c7ad47960a069`  
		Last Modified: Wed, 30 Mar 2022 15:04:28 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
