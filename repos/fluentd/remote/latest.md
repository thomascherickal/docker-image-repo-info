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
