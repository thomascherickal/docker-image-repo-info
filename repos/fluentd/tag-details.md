<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.16-1`](#fluentdv116-1)
-	[`fluentd:v1.16-debian-1`](#fluentdv116-debian-1)
-	[`fluentd:v1.16.2-1.1`](#fluentdv1162-11)
-	[`fluentd:v1.16.2-debian-1.1`](#fluentdv1162-debian-11)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:f9ed4ab7e75b6369fff2daf0096a612f893b6e8bc5c3747f6494578401ad2c98
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
$ docker pull fluentd@sha256:3c2fd3f02143a97f88563a709f587fc5b1fc474abb81d658514f9fbe18419298
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24389978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54a9d681e718662df831981f5747b863531b7e75df8e24759db842996f8e1198`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:50 GMT
ADD file:4ad1e09b0030ebbf09adcc7c616502a079dc61aff7c6edce2f2ea248cd85b2df in / 
# Fri, 01 Dec 2023 02:03:50 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:36:41 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 08:36:41 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 08:37:53 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 08:37:54 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 08:37:54 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 08:37:54 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 08:37:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 08:37:54 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 08:37:54 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 08:37:54 GMT
USER fluent
# Fri, 01 Dec 2023 08:37:54 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 08:37:54 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7583c43471b6e056e4cc98119de7f0921ba6ad8cd2645554165c3d9869b344dc`  
		Last Modified: Fri, 01 Dec 2023 02:04:31 GMT  
		Size: 3.4 MB (3414867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1841979fc88966e3d89a480d1e0eadda7c1ceaffccbfab4f68fa6f71627e5672`  
		Last Modified: Fri, 01 Dec 2023 08:38:15 GMT  
		Size: 21.0 MB (20972893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f17165846b5ae5c8f7ad15c5c13a35a138fd9c7c1c35ec1e9e8232f7a53669c`  
		Last Modified: Fri, 01 Dec 2023 08:38:11 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f020a48b3033b877edf033d1e74005e935e4d7ea3147419398848f5df1d467d7`  
		Last Modified: Fri, 01 Dec 2023 08:38:11 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6983e2e098f9c510bf0c0881cfd9f81e79e0af37ee4329b324ec706202dda9`  
		Last Modified: Fri, 01 Dec 2023 08:38:11 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:06064cb53f42f805b1946a31d34c34647d5611673c1c7113d73b5c9d0b21bb2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (24980550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60659ee3aa15aa7965e9c25008437c0e05b4509b1e50708d94ff6a9fb84eed9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:15 GMT
ADD file:e3eb0ea4f652282ad08228d0d146f33998b9e93641756d780ac0205aa828c070 in / 
# Thu, 30 Nov 2023 23:19:17 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:15:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 09:15:05 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 09:16:19 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 09:16:23 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 09:16:23 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 09:16:23 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 09:16:24 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 09:16:24 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 09:16:25 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 09:16:25 GMT
USER fluent
# Fri, 01 Dec 2023 09:16:27 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 09:16:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c7d387f1f267ea360529df8d70b246f949e1afdb2317cdf84b028cda80a093d1`  
		Last Modified: Thu, 30 Nov 2023 23:20:17 GMT  
		Size: 3.4 MB (3391875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7a80b7ff08da16f05f6a776231ac45b6368ac8053aa51af84edd843f23f6d7`  
		Last Modified: Fri, 01 Dec 2023 09:16:55 GMT  
		Size: 21.6 MB (21586460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2cde9c35b90aae2d2c5cd3b0b903870bfef416decef9de5b104688bfe8e4cd`  
		Last Modified: Fri, 01 Dec 2023 09:16:51 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e24ecf7f6b2ce5667036c99af4a10d40816a3b1cbcc37a77e7f1057e567a4`  
		Last Modified: Fri, 01 Dec 2023 09:16:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf294ce4920cd3b5572caf811776d3ede284e4030cd46d9fbb119539e1bea55`  
		Last Modified: Fri, 01 Dec 2023 09:16:51 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:8dc6fe66dd204bb1a8ddb578cfc7d884d3b4e941e9364b8b45768a8c7251866d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 MB (24344676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da789c11c913e7a14818b1e01ffe2097ee34f9ea34ddb69489ed4b324f1a30a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:16 GMT
ADD file:bf416048d22b9a0deecb508385355d79b8d5d12b655c600dbdc0948f7dcbb2c2 in / 
# Thu, 30 Nov 2023 22:42:17 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:33:05 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 07:33:05 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 07:33:55 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 07:33:57 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 07:33:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 07:33:58 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 07:33:58 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 07:33:58 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 07:33:58 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 07:33:58 GMT
USER fluent
# Fri, 01 Dec 2023 07:33:58 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 07:33:58 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7e9e7e53b618240d2e82e8cab6b677eab6786c4210dcc2b1a35bfd4cb492757e`  
		Last Modified: Thu, 30 Nov 2023 22:43:01 GMT  
		Size: 3.2 MB (3176332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe327a2544c4e778f522fb67a1b812ba1c7ed59dfc75a92135bc3fa8f5be4c`  
		Last Modified: Fri, 01 Dec 2023 07:34:28 GMT  
		Size: 21.2 MB (21166130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7473f89df1730fec4a115cf646581a8512461c3b81203dbf46f7a2c320735baf`  
		Last Modified: Fri, 01 Dec 2023 07:34:24 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71f50240810f589308561c891b6a1a6220ea11f6a9212e66859e52fbd9decf5`  
		Last Modified: Fri, 01 Dec 2023 07:34:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13deb526ac0a28952c08e5f3b033fa5c47d7069d1ebffe011f2a7e5a650531ea`  
		Last Modified: Fri, 01 Dec 2023 07:34:24 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16-1`

```console
$ docker pull fluentd@sha256:f9ed4ab7e75b6369fff2daf0096a612f893b6e8bc5c3747f6494578401ad2c98
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
$ docker pull fluentd@sha256:3c2fd3f02143a97f88563a709f587fc5b1fc474abb81d658514f9fbe18419298
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24389978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54a9d681e718662df831981f5747b863531b7e75df8e24759db842996f8e1198`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:50 GMT
ADD file:4ad1e09b0030ebbf09adcc7c616502a079dc61aff7c6edce2f2ea248cd85b2df in / 
# Fri, 01 Dec 2023 02:03:50 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:36:41 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 08:36:41 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 08:37:53 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 08:37:54 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 08:37:54 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 08:37:54 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 08:37:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 08:37:54 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 08:37:54 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 08:37:54 GMT
USER fluent
# Fri, 01 Dec 2023 08:37:54 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 08:37:54 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7583c43471b6e056e4cc98119de7f0921ba6ad8cd2645554165c3d9869b344dc`  
		Last Modified: Fri, 01 Dec 2023 02:04:31 GMT  
		Size: 3.4 MB (3414867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1841979fc88966e3d89a480d1e0eadda7c1ceaffccbfab4f68fa6f71627e5672`  
		Last Modified: Fri, 01 Dec 2023 08:38:15 GMT  
		Size: 21.0 MB (20972893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f17165846b5ae5c8f7ad15c5c13a35a138fd9c7c1c35ec1e9e8232f7a53669c`  
		Last Modified: Fri, 01 Dec 2023 08:38:11 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f020a48b3033b877edf033d1e74005e935e4d7ea3147419398848f5df1d467d7`  
		Last Modified: Fri, 01 Dec 2023 08:38:11 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6983e2e098f9c510bf0c0881cfd9f81e79e0af37ee4329b324ec706202dda9`  
		Last Modified: Fri, 01 Dec 2023 08:38:11 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:06064cb53f42f805b1946a31d34c34647d5611673c1c7113d73b5c9d0b21bb2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (24980550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60659ee3aa15aa7965e9c25008437c0e05b4509b1e50708d94ff6a9fb84eed9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:15 GMT
ADD file:e3eb0ea4f652282ad08228d0d146f33998b9e93641756d780ac0205aa828c070 in / 
# Thu, 30 Nov 2023 23:19:17 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:15:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 09:15:05 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 09:16:19 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 09:16:23 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 09:16:23 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 09:16:23 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 09:16:24 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 09:16:24 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 09:16:25 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 09:16:25 GMT
USER fluent
# Fri, 01 Dec 2023 09:16:27 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 09:16:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c7d387f1f267ea360529df8d70b246f949e1afdb2317cdf84b028cda80a093d1`  
		Last Modified: Thu, 30 Nov 2023 23:20:17 GMT  
		Size: 3.4 MB (3391875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7a80b7ff08da16f05f6a776231ac45b6368ac8053aa51af84edd843f23f6d7`  
		Last Modified: Fri, 01 Dec 2023 09:16:55 GMT  
		Size: 21.6 MB (21586460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2cde9c35b90aae2d2c5cd3b0b903870bfef416decef9de5b104688bfe8e4cd`  
		Last Modified: Fri, 01 Dec 2023 09:16:51 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e24ecf7f6b2ce5667036c99af4a10d40816a3b1cbcc37a77e7f1057e567a4`  
		Last Modified: Fri, 01 Dec 2023 09:16:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf294ce4920cd3b5572caf811776d3ede284e4030cd46d9fbb119539e1bea55`  
		Last Modified: Fri, 01 Dec 2023 09:16:51 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; s390x

```console
$ docker pull fluentd@sha256:8dc6fe66dd204bb1a8ddb578cfc7d884d3b4e941e9364b8b45768a8c7251866d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 MB (24344676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da789c11c913e7a14818b1e01ffe2097ee34f9ea34ddb69489ed4b324f1a30a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:16 GMT
ADD file:bf416048d22b9a0deecb508385355d79b8d5d12b655c600dbdc0948f7dcbb2c2 in / 
# Thu, 30 Nov 2023 22:42:17 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:33:05 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 07:33:05 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 07:33:55 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 07:33:57 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 07:33:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 07:33:58 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 07:33:58 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 07:33:58 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 07:33:58 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 07:33:58 GMT
USER fluent
# Fri, 01 Dec 2023 07:33:58 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 07:33:58 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7e9e7e53b618240d2e82e8cab6b677eab6786c4210dcc2b1a35bfd4cb492757e`  
		Last Modified: Thu, 30 Nov 2023 22:43:01 GMT  
		Size: 3.2 MB (3176332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe327a2544c4e778f522fb67a1b812ba1c7ed59dfc75a92135bc3fa8f5be4c`  
		Last Modified: Fri, 01 Dec 2023 07:34:28 GMT  
		Size: 21.2 MB (21166130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7473f89df1730fec4a115cf646581a8512461c3b81203dbf46f7a2c320735baf`  
		Last Modified: Fri, 01 Dec 2023 07:34:24 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71f50240810f589308561c891b6a1a6220ea11f6a9212e66859e52fbd9decf5`  
		Last Modified: Fri, 01 Dec 2023 07:34:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13deb526ac0a28952c08e5f3b033fa5c47d7069d1ebffe011f2a7e5a650531ea`  
		Last Modified: Fri, 01 Dec 2023 07:34:24 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16-debian-1`

```console
$ docker pull fluentd@sha256:a4bb0739a01bceed040037d0a0281da2a130d0fe23edd77616ccb77210f5477f
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
$ docker pull fluentd@sha256:de6b08c0722e3258d7184fefceda232e647db09bb375539c3ef1817f92da3f1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.4 MB (95375635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b21789fb7d84733cb8bbca983fd31df57a71484a19054a326109506c7f4b67c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:38 GMT
ADD file:831966ecbc1ad85566dda1f3580cd9306cc099069cd418506e8befd03c296d1c in / 
# Tue, 19 Dec 2023 01:55:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 12:59:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 12:59:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 12:59:15 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 13:18:32 GMT
ENV RUBY_MAJOR=3.1
# Tue, 19 Dec 2023 13:18:32 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 19 Dec 2023 13:18:32 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 19 Dec 2023 13:20:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 13:20:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 13:20:48 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 13:20:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 13:20:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 13:20:49 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 15:55:38 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 19 Dec 2023 15:55:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 19 Dec 2023 15:55:38 GMT
ENV TINI_VERSION=0.18.0
# Tue, 19 Dec 2023 15:58:29 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 19 Dec 2023 15:58:30 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 19 Dec 2023 15:58:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 19 Dec 2023 15:58:30 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 19 Dec 2023 15:58:30 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 19 Dec 2023 15:58:30 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 19 Dec 2023 15:58:30 GMT
EXPOSE 24224 5140
# Tue, 19 Dec 2023 15:58:30 GMT
USER fluent
# Tue, 19 Dec 2023 15:58:30 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 19 Dec 2023 15:58:30 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:fdebea600ba5b47ddd94c41d9d687679a030fdad563a3490945a5433dae01d54`  
		Last Modified: Tue, 19 Dec 2023 01:59:22 GMT  
		Size: 28.9 MB (28921283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd586bc00be11904ae65ff66105b2bd18c84bc0751b2d67b643b4c7965fb429`  
		Last Modified: Tue, 19 Dec 2023 13:26:50 GMT  
		Size: 8.6 MB (8635144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406bdd32ba707754193dce642fb1cdc2a0da0ac8632f45d32e15fa40413e4a04`  
		Last Modified: Tue, 19 Dec 2023 13:26:47 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c37bee31292cceef580e1c4d913a1b951a077ecf58ddc6d562ed5b7978e07`  
		Last Modified: Tue, 19 Dec 2023 13:29:08 GMT  
		Size: 31.2 MB (31166773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504c66c7935394139254fb2124d33d98bbe52997b709afb01f7dfd994db9d83c`  
		Last Modified: Tue, 19 Dec 2023 13:29:05 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7395b41a8b266bc5cbbdee4866b5f5198b9e17ac0caa42fc0bf464fa61297c72`  
		Last Modified: Tue, 19 Dec 2023 15:58:55 GMT  
		Size: 26.6 MB (26649355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa072139a946213b52eddaf360a6a2d954d3b0e2beac64fca6ba34f60d7a34b`  
		Last Modified: Tue, 19 Dec 2023 15:58:51 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275bb04183c34e13479a063d7957a17ae67965a23942efef53744f3c85d2a974`  
		Last Modified: Tue, 19 Dec 2023 15:58:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d08426512c5387b54212f1dd220a81afbb43d645ce7fef493339d3fee50f34f`  
		Last Modified: Tue, 19 Dec 2023 15:58:51 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:ccbe0bc83019e4b0174e5c08415591408a86c93efca82e89f5a074757dc278f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92249880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:080ee4e16564a3f99b3983c76b6eb0bf4d988e907af13250553595567df60398`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:09 GMT
ADD file:496e70a34ff4dabb4eefdf40e4e2f0563bea0c120bb43206f8f52ab5a887b637 in / 
# Tue, 19 Dec 2023 02:08:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 14:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 14:07:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 14:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 14:24:43 GMT
ENV RUBY_MAJOR=3.1
# Tue, 19 Dec 2023 14:24:43 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 19 Dec 2023 14:24:43 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 19 Dec 2023 14:26:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 14:26:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 14:26:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 14:26:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 14:26:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 14:26:50 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 20:56:30 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 19 Dec 2023 20:56:30 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 19 Dec 2023 20:56:30 GMT
ENV TINI_VERSION=0.18.0
# Tue, 19 Dec 2023 20:59:42 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 19 Dec 2023 20:59:43 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 19 Dec 2023 20:59:44 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 19 Dec 2023 20:59:44 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 19 Dec 2023 20:59:44 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 19 Dec 2023 20:59:45 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 19 Dec 2023 20:59:45 GMT
EXPOSE 24224 5140
# Tue, 19 Dec 2023 20:59:45 GMT
USER fluent
# Tue, 19 Dec 2023 20:59:46 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 19 Dec 2023 20:59:46 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:19ccf4d6cc6956e4a5522352be94632923aa376a9939a4f45428a4f304c73bc8`  
		Last Modified: Tue, 19 Dec 2023 02:12:33 GMT  
		Size: 26.6 MB (26578972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe750af02298ab490e5712e33031353765ea4101f5cd4bff3310a126a3ed736d`  
		Last Modified: Tue, 19 Dec 2023 14:36:51 GMT  
		Size: 8.1 MB (8143347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32ed8f74a3d55e1928321d48f47f358a2ab355338bff2f5bf074b6d62352cf5`  
		Last Modified: Tue, 19 Dec 2023 14:36:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0091f712c5229a4d6741239f4001fb0f94e4cb7e085171c89f8961ea0bdb60`  
		Last Modified: Tue, 19 Dec 2023 14:39:06 GMT  
		Size: 31.0 MB (31036989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26daf12e039ba59bb8c3460b4fada2b17e04c40bff68e408eb386f8c0d81d484`  
		Last Modified: Tue, 19 Dec 2023 14:39:03 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac0b6d42f7707f15327ffeac83454ad7ef7529297e29bc5e3d2f3e9640b415e`  
		Last Modified: Tue, 19 Dec 2023 21:00:05 GMT  
		Size: 26.5 MB (26487492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4342625675da8d2baaf505266707e53b2994c4f0186bc6b54b4cc7f848c17601`  
		Last Modified: Tue, 19 Dec 2023 20:59:58 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce6aaa3b499831c29fb3eb7e1fc01c247e2966edc3eff8437b1cea511db9fad`  
		Last Modified: Tue, 19 Dec 2023 20:59:59 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b557daf1d7d45de2448b2cdfd8a0f3e0fb6a26c95a15b0e5d9430736c4f4b3d`  
		Last Modified: Tue, 19 Dec 2023 20:59:59 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:b87753a79681149df09f70d9fa430f8c4a4eabe441f0db14dc641a9a7157826b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98888635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77f00ec74d44e458b1928eb2cd12512c5e85cf4babc2a167473a51a8e7692340`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:25 GMT
ADD file:4dd1c5e17a5e57644787f37e8ad290baef6c93f4f112b976f19136480a293713 in / 
# Tue, 19 Dec 2023 01:41:25 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:26:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:26:56 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 06:26:56 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 06:35:32 GMT
ENV RUBY_MAJOR=3.1
# Tue, 19 Dec 2023 06:35:32 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 19 Dec 2023 06:35:32 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 19 Dec 2023 06:37:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 06:37:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 06:37:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 06:37:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 06:37:14 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 06:37:14 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 13:37:16 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 19 Dec 2023 13:37:16 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 19 Dec 2023 13:37:16 GMT
ENV TINI_VERSION=0.18.0
# Tue, 19 Dec 2023 13:39:34 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 19 Dec 2023 13:39:34 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 19 Dec 2023 13:39:34 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 19 Dec 2023 13:39:34 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 19 Dec 2023 13:39:35 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 19 Dec 2023 13:39:35 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 19 Dec 2023 13:39:35 GMT
EXPOSE 24224 5140
# Tue, 19 Dec 2023 13:39:35 GMT
USER fluent
# Tue, 19 Dec 2023 13:39:35 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 19 Dec 2023 13:39:35 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2244706f264b35566276550fbc21ada79613ddfff850e372b8f5113110a67c93`  
		Last Modified: Tue, 19 Dec 2023 01:45:22 GMT  
		Size: 30.1 MB (30064052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3779e90ad31f2a1360b80abe1848a969c0d6161a8aadf54f49d8c59ed5bdab5`  
		Last Modified: Tue, 19 Dec 2023 06:41:55 GMT  
		Size: 9.2 MB (9242697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b6a20da9f2a64c3300db60255c5f44d6014efcb96d3b857d92e8d6901537e3`  
		Last Modified: Tue, 19 Dec 2023 06:41:54 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4ec57c8ec90c40345b8a1c36768e413d0a5f640901eb0e3a2ce0c0542328fa`  
		Last Modified: Tue, 19 Dec 2023 06:43:07 GMT  
		Size: 32.0 MB (31988125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e72ee3befaf51f54539ffa57d13c9678d9dc4d9ef3b7f070f295ddc7c3065e`  
		Last Modified: Tue, 19 Dec 2023 06:43:05 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b02cf20175eb12fd5f41bd377e6cd1cb53410f83ed6113ca69258638865ee6`  
		Last Modified: Tue, 19 Dec 2023 13:39:51 GMT  
		Size: 27.6 MB (27590671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b46cc0962fab11f7a1cb0f559932365fb36192beb81000bb5ed690343f88d2`  
		Last Modified: Tue, 19 Dec 2023 13:39:48 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fc8b414094947b06a6d53be1cef084267bc6a85f01140f8fe326bc42e60075`  
		Last Modified: Tue, 19 Dec 2023 13:39:48 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b61510de22fa034dfe75cc55d98b8810210dfbcb125a2511995e499e4a26c13`  
		Last Modified: Tue, 19 Dec 2023 13:39:48 GMT  
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
$ docker pull fluentd@sha256:ff09ae55bbcbe91bbba79049d5f67d7e4aede694c46d3df22cd8539021ce1d98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (99011556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6ccaa5c71ab640c5ed836c6495ab943bdced303a2bd28b77aa16f65b70fd85b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 19 Dec 2023 01:43:11 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
# Tue, 19 Dec 2023 01:43:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 09:20:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 09:20:17 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 09:20:17 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 09:40:34 GMT
ENV RUBY_MAJOR=3.1
# Tue, 19 Dec 2023 09:40:34 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 19 Dec 2023 09:40:34 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 19 Dec 2023 09:42:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 09:42:47 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 09:42:48 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 09:42:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 09:42:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 09:42:48 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 15:01:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 19 Dec 2023 15:01:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 19 Dec 2023 15:01:51 GMT
ENV TINI_VERSION=0.18.0
# Tue, 19 Dec 2023 15:03:57 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 19 Dec 2023 15:03:59 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 19 Dec 2023 15:03:59 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 19 Dec 2023 15:03:59 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 19 Dec 2023 15:03:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 19 Dec 2023 15:03:59 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 19 Dec 2023 15:03:59 GMT
EXPOSE 24224 5140
# Tue, 19 Dec 2023 15:04:00 GMT
USER fluent
# Tue, 19 Dec 2023 15:04:00 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 19 Dec 2023 15:04:00 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4feb70f84c58e43e54d6f658d8f8e71f2d6711ffe1072343b0c056590d3966a8`  
		Last Modified: Tue, 19 Dec 2023 09:49:05 GMT  
		Size: 8.9 MB (8863457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992e91c00e0c624b76d9e40e50731dec6f57716b084a24c6f124b59621bda864`  
		Last Modified: Tue, 19 Dec 2023 09:49:04 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a4a1f5dfc98bfb66b2b1b3a172b995aadc69d2e52b1ee2480340f10ebb3928`  
		Last Modified: Tue, 19 Dec 2023 09:50:43 GMT  
		Size: 32.4 MB (32445735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da2f37aae1c1694d032c60c503b2b93fd96c73b65edc2999b06723ad844c6a6`  
		Last Modified: Tue, 19 Dec 2023 09:50:41 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e26ab2dde4cd7412f5f5247753e5a1381e04952787a25c7de8073c9dcb6b8`  
		Last Modified: Tue, 19 Dec 2023 15:04:26 GMT  
		Size: 28.0 MB (28042273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991b484b07aa4d356c6fc9fbe551e19323b47b81f34c739c7ce659b73b4bf231`  
		Last Modified: Tue, 19 Dec 2023 15:04:22 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c364001a84123f4ec0b08d2c57802a03e2c67696ca65485b90064169973babda`  
		Last Modified: Tue, 19 Dec 2023 15:04:22 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8e9d252e09d6b7432a14a9befa6df557504c56b1fee488fb9e59317be6f983`  
		Last Modified: Tue, 19 Dec 2023 15:04:22 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16.2-1.1`

```console
$ docker pull fluentd@sha256:f9ed4ab7e75b6369fff2daf0096a612f893b6e8bc5c3747f6494578401ad2c98
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
$ docker pull fluentd@sha256:3c2fd3f02143a97f88563a709f587fc5b1fc474abb81d658514f9fbe18419298
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24389978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54a9d681e718662df831981f5747b863531b7e75df8e24759db842996f8e1198`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:50 GMT
ADD file:4ad1e09b0030ebbf09adcc7c616502a079dc61aff7c6edce2f2ea248cd85b2df in / 
# Fri, 01 Dec 2023 02:03:50 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:36:41 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 08:36:41 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 08:37:53 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 08:37:54 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 08:37:54 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 08:37:54 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 08:37:54 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 08:37:54 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 08:37:54 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 08:37:54 GMT
USER fluent
# Fri, 01 Dec 2023 08:37:54 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 08:37:54 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7583c43471b6e056e4cc98119de7f0921ba6ad8cd2645554165c3d9869b344dc`  
		Last Modified: Fri, 01 Dec 2023 02:04:31 GMT  
		Size: 3.4 MB (3414867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1841979fc88966e3d89a480d1e0eadda7c1ceaffccbfab4f68fa6f71627e5672`  
		Last Modified: Fri, 01 Dec 2023 08:38:15 GMT  
		Size: 21.0 MB (20972893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f17165846b5ae5c8f7ad15c5c13a35a138fd9c7c1c35ec1e9e8232f7a53669c`  
		Last Modified: Fri, 01 Dec 2023 08:38:11 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f020a48b3033b877edf033d1e74005e935e4d7ea3147419398848f5df1d467d7`  
		Last Modified: Fri, 01 Dec 2023 08:38:11 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6983e2e098f9c510bf0c0881cfd9f81e79e0af37ee4329b324ec706202dda9`  
		Last Modified: Fri, 01 Dec 2023 08:38:11 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:06064cb53f42f805b1946a31d34c34647d5611673c1c7113d73b5c9d0b21bb2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (24980550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60659ee3aa15aa7965e9c25008437c0e05b4509b1e50708d94ff6a9fb84eed9`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:15 GMT
ADD file:e3eb0ea4f652282ad08228d0d146f33998b9e93641756d780ac0205aa828c070 in / 
# Thu, 30 Nov 2023 23:19:17 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:15:04 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 09:15:05 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 09:16:19 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 09:16:23 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 09:16:23 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 09:16:23 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 09:16:24 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 09:16:24 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 09:16:25 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 09:16:25 GMT
USER fluent
# Fri, 01 Dec 2023 09:16:27 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 09:16:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:c7d387f1f267ea360529df8d70b246f949e1afdb2317cdf84b028cda80a093d1`  
		Last Modified: Thu, 30 Nov 2023 23:20:17 GMT  
		Size: 3.4 MB (3391875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7a80b7ff08da16f05f6a776231ac45b6368ac8053aa51af84edd843f23f6d7`  
		Last Modified: Fri, 01 Dec 2023 09:16:55 GMT  
		Size: 21.6 MB (21586460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2cde9c35b90aae2d2c5cd3b0b903870bfef416decef9de5b104688bfe8e4cd`  
		Last Modified: Fri, 01 Dec 2023 09:16:51 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e24ecf7f6b2ce5667036c99af4a10d40816a3b1cbcc37a77e7f1057e567a4`  
		Last Modified: Fri, 01 Dec 2023 09:16:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf294ce4920cd3b5572caf811776d3ede284e4030cd46d9fbb119539e1bea55`  
		Last Modified: Fri, 01 Dec 2023 09:16:51 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; s390x

```console
$ docker pull fluentd@sha256:8dc6fe66dd204bb1a8ddb578cfc7d884d3b4e941e9364b8b45768a8c7251866d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 MB (24344676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da789c11c913e7a14818b1e01ffe2097ee34f9ea34ddb69489ed4b324f1a30a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:16 GMT
ADD file:bf416048d22b9a0deecb508385355d79b8d5d12b655c600dbdc0948f7dcbb2c2 in / 
# Thu, 30 Nov 2023 22:42:17 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:33:05 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 01 Dec 2023 07:33:05 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 01 Dec 2023 07:33:55 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 01 Dec 2023 07:33:57 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 01 Dec 2023 07:33:58 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 01 Dec 2023 07:33:58 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 01 Dec 2023 07:33:58 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 01 Dec 2023 07:33:58 GMT
ENV LD_PRELOAD=
# Fri, 01 Dec 2023 07:33:58 GMT
EXPOSE 24224 5140
# Fri, 01 Dec 2023 07:33:58 GMT
USER fluent
# Fri, 01 Dec 2023 07:33:58 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 01 Dec 2023 07:33:58 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:7e9e7e53b618240d2e82e8cab6b677eab6786c4210dcc2b1a35bfd4cb492757e`  
		Last Modified: Thu, 30 Nov 2023 22:43:01 GMT  
		Size: 3.2 MB (3176332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe327a2544c4e778f522fb67a1b812ba1c7ed59dfc75a92135bc3fa8f5be4c`  
		Last Modified: Fri, 01 Dec 2023 07:34:28 GMT  
		Size: 21.2 MB (21166130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7473f89df1730fec4a115cf646581a8512461c3b81203dbf46f7a2c320735baf`  
		Last Modified: Fri, 01 Dec 2023 07:34:24 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71f50240810f589308561c891b6a1a6220ea11f6a9212e66859e52fbd9decf5`  
		Last Modified: Fri, 01 Dec 2023 07:34:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13deb526ac0a28952c08e5f3b033fa5c47d7069d1ebffe011f2a7e5a650531ea`  
		Last Modified: Fri, 01 Dec 2023 07:34:24 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16.2-debian-1.1`

```console
$ docker pull fluentd@sha256:a4bb0739a01bceed040037d0a0281da2a130d0fe23edd77616ccb77210f5477f
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
$ docker pull fluentd@sha256:de6b08c0722e3258d7184fefceda232e647db09bb375539c3ef1817f92da3f1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.4 MB (95375635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b21789fb7d84733cb8bbca983fd31df57a71484a19054a326109506c7f4b67c`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:38 GMT
ADD file:831966ecbc1ad85566dda1f3580cd9306cc099069cd418506e8befd03c296d1c in / 
# Tue, 19 Dec 2023 01:55:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 12:59:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 12:59:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 12:59:15 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 13:18:32 GMT
ENV RUBY_MAJOR=3.1
# Tue, 19 Dec 2023 13:18:32 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 19 Dec 2023 13:18:32 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 19 Dec 2023 13:20:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 13:20:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 13:20:48 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 13:20:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 13:20:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 13:20:49 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 15:55:38 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 19 Dec 2023 15:55:38 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 19 Dec 2023 15:55:38 GMT
ENV TINI_VERSION=0.18.0
# Tue, 19 Dec 2023 15:58:29 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 19 Dec 2023 15:58:30 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 19 Dec 2023 15:58:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 19 Dec 2023 15:58:30 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 19 Dec 2023 15:58:30 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 19 Dec 2023 15:58:30 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 19 Dec 2023 15:58:30 GMT
EXPOSE 24224 5140
# Tue, 19 Dec 2023 15:58:30 GMT
USER fluent
# Tue, 19 Dec 2023 15:58:30 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 19 Dec 2023 15:58:30 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:fdebea600ba5b47ddd94c41d9d687679a030fdad563a3490945a5433dae01d54`  
		Last Modified: Tue, 19 Dec 2023 01:59:22 GMT  
		Size: 28.9 MB (28921283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd586bc00be11904ae65ff66105b2bd18c84bc0751b2d67b643b4c7965fb429`  
		Last Modified: Tue, 19 Dec 2023 13:26:50 GMT  
		Size: 8.6 MB (8635144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406bdd32ba707754193dce642fb1cdc2a0da0ac8632f45d32e15fa40413e4a04`  
		Last Modified: Tue, 19 Dec 2023 13:26:47 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c37bee31292cceef580e1c4d913a1b951a077ecf58ddc6d562ed5b7978e07`  
		Last Modified: Tue, 19 Dec 2023 13:29:08 GMT  
		Size: 31.2 MB (31166773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504c66c7935394139254fb2124d33d98bbe52997b709afb01f7dfd994db9d83c`  
		Last Modified: Tue, 19 Dec 2023 13:29:05 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7395b41a8b266bc5cbbdee4866b5f5198b9e17ac0caa42fc0bf464fa61297c72`  
		Last Modified: Tue, 19 Dec 2023 15:58:55 GMT  
		Size: 26.6 MB (26649355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa072139a946213b52eddaf360a6a2d954d3b0e2beac64fca6ba34f60d7a34b`  
		Last Modified: Tue, 19 Dec 2023 15:58:51 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275bb04183c34e13479a063d7957a17ae67965a23942efef53744f3c85d2a974`  
		Last Modified: Tue, 19 Dec 2023 15:58:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d08426512c5387b54212f1dd220a81afbb43d645ce7fef493339d3fee50f34f`  
		Last Modified: Tue, 19 Dec 2023 15:58:51 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:ccbe0bc83019e4b0174e5c08415591408a86c93efca82e89f5a074757dc278f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92249880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:080ee4e16564a3f99b3983c76b6eb0bf4d988e907af13250553595567df60398`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:09 GMT
ADD file:496e70a34ff4dabb4eefdf40e4e2f0563bea0c120bb43206f8f52ab5a887b637 in / 
# Tue, 19 Dec 2023 02:08:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 14:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 14:07:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 14:07:28 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 14:24:43 GMT
ENV RUBY_MAJOR=3.1
# Tue, 19 Dec 2023 14:24:43 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 19 Dec 2023 14:24:43 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 19 Dec 2023 14:26:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 14:26:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 14:26:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 14:26:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 14:26:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 14:26:50 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 20:56:30 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 19 Dec 2023 20:56:30 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 19 Dec 2023 20:56:30 GMT
ENV TINI_VERSION=0.18.0
# Tue, 19 Dec 2023 20:59:42 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 19 Dec 2023 20:59:43 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 19 Dec 2023 20:59:44 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 19 Dec 2023 20:59:44 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 19 Dec 2023 20:59:44 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 19 Dec 2023 20:59:45 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 19 Dec 2023 20:59:45 GMT
EXPOSE 24224 5140
# Tue, 19 Dec 2023 20:59:45 GMT
USER fluent
# Tue, 19 Dec 2023 20:59:46 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 19 Dec 2023 20:59:46 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:19ccf4d6cc6956e4a5522352be94632923aa376a9939a4f45428a4f304c73bc8`  
		Last Modified: Tue, 19 Dec 2023 02:12:33 GMT  
		Size: 26.6 MB (26578972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe750af02298ab490e5712e33031353765ea4101f5cd4bff3310a126a3ed736d`  
		Last Modified: Tue, 19 Dec 2023 14:36:51 GMT  
		Size: 8.1 MB (8143347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32ed8f74a3d55e1928321d48f47f358a2ab355338bff2f5bf074b6d62352cf5`  
		Last Modified: Tue, 19 Dec 2023 14:36:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0091f712c5229a4d6741239f4001fb0f94e4cb7e085171c89f8961ea0bdb60`  
		Last Modified: Tue, 19 Dec 2023 14:39:06 GMT  
		Size: 31.0 MB (31036989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26daf12e039ba59bb8c3460b4fada2b17e04c40bff68e408eb386f8c0d81d484`  
		Last Modified: Tue, 19 Dec 2023 14:39:03 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac0b6d42f7707f15327ffeac83454ad7ef7529297e29bc5e3d2f3e9640b415e`  
		Last Modified: Tue, 19 Dec 2023 21:00:05 GMT  
		Size: 26.5 MB (26487492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4342625675da8d2baaf505266707e53b2994c4f0186bc6b54b4cc7f848c17601`  
		Last Modified: Tue, 19 Dec 2023 20:59:58 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce6aaa3b499831c29fb3eb7e1fc01c247e2966edc3eff8437b1cea511db9fad`  
		Last Modified: Tue, 19 Dec 2023 20:59:59 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b557daf1d7d45de2448b2cdfd8a0f3e0fb6a26c95a15b0e5d9430736c4f4b3d`  
		Last Modified: Tue, 19 Dec 2023 20:59:59 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:b87753a79681149df09f70d9fa430f8c4a4eabe441f0db14dc641a9a7157826b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98888635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77f00ec74d44e458b1928eb2cd12512c5e85cf4babc2a167473a51a8e7692340`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:25 GMT
ADD file:4dd1c5e17a5e57644787f37e8ad290baef6c93f4f112b976f19136480a293713 in / 
# Tue, 19 Dec 2023 01:41:25 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:26:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:26:56 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 06:26:56 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 06:35:32 GMT
ENV RUBY_MAJOR=3.1
# Tue, 19 Dec 2023 06:35:32 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 19 Dec 2023 06:35:32 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 19 Dec 2023 06:37:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 06:37:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 06:37:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 06:37:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 06:37:14 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 06:37:14 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 13:37:16 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 19 Dec 2023 13:37:16 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 19 Dec 2023 13:37:16 GMT
ENV TINI_VERSION=0.18.0
# Tue, 19 Dec 2023 13:39:34 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 19 Dec 2023 13:39:34 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 19 Dec 2023 13:39:34 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 19 Dec 2023 13:39:34 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 19 Dec 2023 13:39:35 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 19 Dec 2023 13:39:35 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 19 Dec 2023 13:39:35 GMT
EXPOSE 24224 5140
# Tue, 19 Dec 2023 13:39:35 GMT
USER fluent
# Tue, 19 Dec 2023 13:39:35 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 19 Dec 2023 13:39:35 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:2244706f264b35566276550fbc21ada79613ddfff850e372b8f5113110a67c93`  
		Last Modified: Tue, 19 Dec 2023 01:45:22 GMT  
		Size: 30.1 MB (30064052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3779e90ad31f2a1360b80abe1848a969c0d6161a8aadf54f49d8c59ed5bdab5`  
		Last Modified: Tue, 19 Dec 2023 06:41:55 GMT  
		Size: 9.2 MB (9242697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b6a20da9f2a64c3300db60255c5f44d6014efcb96d3b857d92e8d6901537e3`  
		Last Modified: Tue, 19 Dec 2023 06:41:54 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4ec57c8ec90c40345b8a1c36768e413d0a5f640901eb0e3a2ce0c0542328fa`  
		Last Modified: Tue, 19 Dec 2023 06:43:07 GMT  
		Size: 32.0 MB (31988125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e72ee3befaf51f54539ffa57d13c9678d9dc4d9ef3b7f070f295ddc7c3065e`  
		Last Modified: Tue, 19 Dec 2023 06:43:05 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b02cf20175eb12fd5f41bd377e6cd1cb53410f83ed6113ca69258638865ee6`  
		Last Modified: Tue, 19 Dec 2023 13:39:51 GMT  
		Size: 27.6 MB (27590671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b46cc0962fab11f7a1cb0f559932365fb36192beb81000bb5ed690343f88d2`  
		Last Modified: Tue, 19 Dec 2023 13:39:48 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fc8b414094947b06a6d53be1cef084267bc6a85f01140f8fe326bc42e60075`  
		Last Modified: Tue, 19 Dec 2023 13:39:48 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b61510de22fa034dfe75cc55d98b8810210dfbcb125a2511995e499e4a26c13`  
		Last Modified: Tue, 19 Dec 2023 13:39:48 GMT  
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
$ docker pull fluentd@sha256:ff09ae55bbcbe91bbba79049d5f67d7e4aede694c46d3df22cd8539021ce1d98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (99011556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6ccaa5c71ab640c5ed836c6495ab943bdced303a2bd28b77aa16f65b70fd85b`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 19 Dec 2023 01:43:11 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
# Tue, 19 Dec 2023 01:43:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 09:20:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 09:20:17 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 09:20:17 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 09:40:34 GMT
ENV RUBY_MAJOR=3.1
# Tue, 19 Dec 2023 09:40:34 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 19 Dec 2023 09:40:34 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 19 Dec 2023 09:42:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 09:42:47 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 09:42:48 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 09:42:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 09:42:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 09:42:48 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 15:01:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 19 Dec 2023 15:01:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Tue, 19 Dec 2023 15:01:51 GMT
ENV TINI_VERSION=0.18.0
# Tue, 19 Dec 2023 15:03:57 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Tue, 19 Dec 2023 15:03:59 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 19 Dec 2023 15:03:59 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 19 Dec 2023 15:03:59 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 19 Dec 2023 15:03:59 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 19 Dec 2023 15:03:59 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Tue, 19 Dec 2023 15:03:59 GMT
EXPOSE 24224 5140
# Tue, 19 Dec 2023 15:04:00 GMT
USER fluent
# Tue, 19 Dec 2023 15:04:00 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 19 Dec 2023 15:04:00 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4feb70f84c58e43e54d6f658d8f8e71f2d6711ffe1072343b0c056590d3966a8`  
		Last Modified: Tue, 19 Dec 2023 09:49:05 GMT  
		Size: 8.9 MB (8863457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992e91c00e0c624b76d9e40e50731dec6f57716b084a24c6f124b59621bda864`  
		Last Modified: Tue, 19 Dec 2023 09:49:04 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a4a1f5dfc98bfb66b2b1b3a172b995aadc69d2e52b1ee2480340f10ebb3928`  
		Last Modified: Tue, 19 Dec 2023 09:50:43 GMT  
		Size: 32.4 MB (32445735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da2f37aae1c1694d032c60c503b2b93fd96c73b65edc2999b06723ad844c6a6`  
		Last Modified: Tue, 19 Dec 2023 09:50:41 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e26ab2dde4cd7412f5f5247753e5a1381e04952787a25c7de8073c9dcb6b8`  
		Last Modified: Tue, 19 Dec 2023 15:04:26 GMT  
		Size: 28.0 MB (28042273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991b484b07aa4d356c6fc9fbe551e19323b47b81f34c739c7ce659b73b4bf231`  
		Last Modified: Tue, 19 Dec 2023 15:04:22 GMT  
		Size: 1.8 KB (1847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c364001a84123f4ec0b08d2c57802a03e2c67696ca65485b90064169973babda`  
		Last Modified: Tue, 19 Dec 2023 15:04:22 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8e9d252e09d6b7432a14a9befa6df557504c56b1fee488fb9e59317be6f983`  
		Last Modified: Tue, 19 Dec 2023 15:04:22 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
