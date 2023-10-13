<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fluentd`

-	[`fluentd:latest`](#fluentdlatest)
-	[`fluentd:v1.16-1`](#fluentdv116-1)
-	[`fluentd:v1.16-debian-1`](#fluentdv116-debian-1)
-	[`fluentd:v1.16.2-1.1`](#fluentdv1162-11)
-	[`fluentd:v1.16.2-debian-1.1`](#fluentdv1162-debian-11)

## `fluentd:latest`

```console
$ docker pull fluentd@sha256:0e1090ed3901b0f4a5a4faabb10f91c4fa680da2e2a6503c23832ade8212bfc5
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
$ docker pull fluentd@sha256:13ee83b11a86c4e6593b5acb8e647c22cf1b9feef123612b9dd586465ed05254
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25155206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6e2964bb824f2aacb86d0ca3170997802f000be1eff97299b1188ec8611aa4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 10:08:31 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:19:32 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:20:26 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:20:27 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:20:27 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:20:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:20:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:20:27 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:20:27 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:20:28 GMT
USER fluent
# Wed, 04 Oct 2023 21:20:28 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:20:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8827fca176be13b72bd568162360ca80ecd8eef45b5ef68c80b3a000f503183`  
		Last Modified: Wed, 04 Oct 2023 21:24:01 GMT  
		Size: 21.8 MB (21774385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6515ca36e5cdb6a7919ba7b37f2dd0f2d248776d1f9485d6447a039b1ed9452`  
		Last Modified: Wed, 04 Oct 2023 21:23:58 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3543c7841d7564df2c94d78f0afdedb172e4b82c8677f5b5ad85136ac57a1dd3`  
		Last Modified: Wed, 04 Oct 2023 21:23:58 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57e8a5d5c2f2b9f7e226a62461f9a68d3c8ffaa5b73c8a92b05fa8bcc8d1d96`  
		Last Modified: Wed, 04 Oct 2023 21:23:58 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:059df7f5071014b62e8cd4b3d56609cecbf887753011d04bb0a3b0e017a60f72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23848199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f827678b99b7f0450b51a46ea4bbded99d2af7bc05d42292069f7ac5157f0b4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 22:13:50 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 20:49:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 20:50:18 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 20:50:18 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 20:50:18 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 20:50:19 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 20:50:19 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 20:50:19 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 20:50:19 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 20:50:19 GMT
USER fluent
# Wed, 04 Oct 2023 20:50:19 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 20:50:19 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553532437e6782bb598563089e5c9712ae1d947bcc0e062ecde36c20a8de5397`  
		Last Modified: Wed, 04 Oct 2023 20:50:32 GMT  
		Size: 20.7 MB (20733532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d15a3c0a2634f3d4b2d360f2e9ef8cf7e467483d959c924d4ce1b9de09ff85`  
		Last Modified: Wed, 04 Oct 2023 20:50:29 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b8122aae986d2ea394888a2a35bdfe989c9aff09557fab2b7a3a40c97ca077`  
		Last Modified: Wed, 04 Oct 2023 20:50:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff8c6799857457a342c810fea84380b9f681c2db904dff6caef780d7e0671d3`  
		Last Modified: Wed, 04 Oct 2023 20:50:29 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:8197de0448a2f17bf11f791952b47dada2db36420039a914517dd8fdb9576cd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24629281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b9bbe3c7c4f2dc30c2ce5307d8fe088a8d1b645f876b2f86ab83f0c04d8ec45`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 10:36:07 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:39:29 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:40:19 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:40:19 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:40:20 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:40:20 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:40:20 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:40:20 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:40:20 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:40:20 GMT
USER fluent
# Wed, 04 Oct 2023 21:40:20 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:40:20 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e3f59536119d5781bb641b631d26d36f17086051a8b4afd4683c39e225bb4`  
		Last Modified: Wed, 04 Oct 2023 21:43:15 GMT  
		Size: 21.4 MB (21368773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf0687a8f3c9c7bc2628fceef6bc75e8642ea202b985274313ddd137d5bde2f`  
		Last Modified: Wed, 04 Oct 2023 21:43:12 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f3742a3460d54456ef66da27bcb397c738c7a99e48ee599835c2d5d935c0ca`  
		Last Modified: Wed, 04 Oct 2023 21:43:12 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3629019f4be74a2ec436a05f010c0abc28d5060bf37a9e2874366f5210daf2`  
		Last Modified: Wed, 04 Oct 2023 21:43:12 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; 386

```console
$ docker pull fluentd@sha256:b83b7e92a71b743f967b5288f16a4df4305653819cdb9aaf2d900d46f42909fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24437573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a376d83aefcf980ab1d54ab6eaa54cfe7efd64178c391d35d5dd01828a219566`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:24:48 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:38:20 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:39:32 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:39:33 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:39:33 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:39:33 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:39:33 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:39:33 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:39:33 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:39:33 GMT
USER fluent
# Wed, 04 Oct 2023 21:39:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:39:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eeb7c7b7c8cf58216ccf047891a51db52037f8d73338c44bda2aade1939af3`  
		Last Modified: Wed, 04 Oct 2023 21:43:33 GMT  
		Size: 21.0 MB (21021575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfff789f4260eb9a35837ba5b55a3132024fc07f657c0a7a36b4c537c93e532`  
		Last Modified: Wed, 04 Oct 2023 21:43:28 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3634708fd9e50993123edc881d3b612bd7abd118c86c10ae821d153c32627d6c`  
		Last Modified: Wed, 04 Oct 2023 21:43:28 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecb450aa2b0fc245622f769a3b887b13b78e60ea9541bfea6ff5c6ec88b683f`  
		Last Modified: Wed, 04 Oct 2023 21:43:28 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:00ec95a9165ad95d580fdd03e9ac2168cbb48c84e783c0d256d2ff2e2c012649
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (25008964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc2fe004ba2fc07cbd3ae7d50e767842934d907a6ed122619d1e28e110d0efec`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:06:25 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:16:46 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:18:54 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:18:58 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:19:00 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:19:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:19:02 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:19:02 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:19:03 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:19:04 GMT
USER fluent
# Wed, 04 Oct 2023 21:19:05 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:19:06 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686c1faa62490a3123a764ff1f9eb8f56b2d2370ca4c57a0df250c27b5f8c567`  
		Last Modified: Wed, 04 Oct 2023 21:27:05 GMT  
		Size: 21.6 MB (21615400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f05d8caa8bd28ac8b74de327805f02bd7541b08a3ff76a90a8edd0ec3be3a8`  
		Last Modified: Wed, 04 Oct 2023 21:26:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74498b595a258f3d58d08ebcd2d0594e2b0954606ac5dce53681b96fa90a9fb6`  
		Last Modified: Wed, 04 Oct 2023 21:26:59 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3e2fa1f46398cb0c1fce47f3a1dbbe71e2ec584d77c560feebc765d18af209`  
		Last Modified: Wed, 04 Oct 2023 21:26:59 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:4bf9c8b8442eecc11953268bb67197327b4dcd7dfd3c362260c96a431e13fe04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (29998860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7f6f610b30aa0140b9f9276b6b90fa1f395f17501f7fcdb7a94c3614ef43a3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:17:28 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:41:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:47:54 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:48:02 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:48:02 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:48:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:48:03 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:48:04 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:48:05 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:48:05 GMT
USER fluent
# Wed, 04 Oct 2023 21:48:05 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:48:06 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a7cda602ceb77b991077268ddf9794e50138b46af24af519f72acbdec17298`  
		Last Modified: Wed, 04 Oct 2023 21:54:17 GMT  
		Size: 26.8 MB (26820669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977fa9f658a1932ce284e4498f48f661f20e5b5bf01569236217ff0fcc0ea6cc`  
		Last Modified: Wed, 04 Oct 2023 21:54:12 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a7282d352e8cc5052eaaf24c4c0a054b8e7ed3b58082b373ae53b18b4c2eab`  
		Last Modified: Wed, 04 Oct 2023 21:54:12 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b8e091f38fa0c967d062af79901add256471c87f62cbe5b767a12554086282`  
		Last Modified: Wed, 04 Oct 2023 21:54:12 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16-1`

```console
$ docker pull fluentd@sha256:0e1090ed3901b0f4a5a4faabb10f91c4fa680da2e2a6503c23832ade8212bfc5
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
$ docker pull fluentd@sha256:13ee83b11a86c4e6593b5acb8e647c22cf1b9feef123612b9dd586465ed05254
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25155206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6e2964bb824f2aacb86d0ca3170997802f000be1eff97299b1188ec8611aa4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 10:08:31 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:19:32 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:20:26 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:20:27 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:20:27 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:20:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:20:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:20:27 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:20:27 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:20:28 GMT
USER fluent
# Wed, 04 Oct 2023 21:20:28 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:20:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8827fca176be13b72bd568162360ca80ecd8eef45b5ef68c80b3a000f503183`  
		Last Modified: Wed, 04 Oct 2023 21:24:01 GMT  
		Size: 21.8 MB (21774385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6515ca36e5cdb6a7919ba7b37f2dd0f2d248776d1f9485d6447a039b1ed9452`  
		Last Modified: Wed, 04 Oct 2023 21:23:58 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3543c7841d7564df2c94d78f0afdedb172e4b82c8677f5b5ad85136ac57a1dd3`  
		Last Modified: Wed, 04 Oct 2023 21:23:58 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57e8a5d5c2f2b9f7e226a62461f9a68d3c8ffaa5b73c8a92b05fa8bcc8d1d96`  
		Last Modified: Wed, 04 Oct 2023 21:23:58 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:059df7f5071014b62e8cd4b3d56609cecbf887753011d04bb0a3b0e017a60f72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23848199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f827678b99b7f0450b51a46ea4bbded99d2af7bc05d42292069f7ac5157f0b4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 22:13:50 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 20:49:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 20:50:18 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 20:50:18 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 20:50:18 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 20:50:19 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 20:50:19 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 20:50:19 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 20:50:19 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 20:50:19 GMT
USER fluent
# Wed, 04 Oct 2023 20:50:19 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 20:50:19 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553532437e6782bb598563089e5c9712ae1d947bcc0e062ecde36c20a8de5397`  
		Last Modified: Wed, 04 Oct 2023 20:50:32 GMT  
		Size: 20.7 MB (20733532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d15a3c0a2634f3d4b2d360f2e9ef8cf7e467483d959c924d4ce1b9de09ff85`  
		Last Modified: Wed, 04 Oct 2023 20:50:29 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b8122aae986d2ea394888a2a35bdfe989c9aff09557fab2b7a3a40c97ca077`  
		Last Modified: Wed, 04 Oct 2023 20:50:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff8c6799857457a342c810fea84380b9f681c2db904dff6caef780d7e0671d3`  
		Last Modified: Wed, 04 Oct 2023 20:50:29 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:8197de0448a2f17bf11f791952b47dada2db36420039a914517dd8fdb9576cd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24629281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b9bbe3c7c4f2dc30c2ce5307d8fe088a8d1b645f876b2f86ab83f0c04d8ec45`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 10:36:07 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:39:29 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:40:19 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:40:19 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:40:20 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:40:20 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:40:20 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:40:20 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:40:20 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:40:20 GMT
USER fluent
# Wed, 04 Oct 2023 21:40:20 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:40:20 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e3f59536119d5781bb641b631d26d36f17086051a8b4afd4683c39e225bb4`  
		Last Modified: Wed, 04 Oct 2023 21:43:15 GMT  
		Size: 21.4 MB (21368773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf0687a8f3c9c7bc2628fceef6bc75e8642ea202b985274313ddd137d5bde2f`  
		Last Modified: Wed, 04 Oct 2023 21:43:12 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f3742a3460d54456ef66da27bcb397c738c7a99e48ee599835c2d5d935c0ca`  
		Last Modified: Wed, 04 Oct 2023 21:43:12 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3629019f4be74a2ec436a05f010c0abc28d5060bf37a9e2874366f5210daf2`  
		Last Modified: Wed, 04 Oct 2023 21:43:12 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; 386

```console
$ docker pull fluentd@sha256:b83b7e92a71b743f967b5288f16a4df4305653819cdb9aaf2d900d46f42909fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24437573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a376d83aefcf980ab1d54ab6eaa54cfe7efd64178c391d35d5dd01828a219566`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:24:48 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:38:20 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:39:32 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:39:33 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:39:33 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:39:33 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:39:33 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:39:33 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:39:33 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:39:33 GMT
USER fluent
# Wed, 04 Oct 2023 21:39:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:39:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eeb7c7b7c8cf58216ccf047891a51db52037f8d73338c44bda2aade1939af3`  
		Last Modified: Wed, 04 Oct 2023 21:43:33 GMT  
		Size: 21.0 MB (21021575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfff789f4260eb9a35837ba5b55a3132024fc07f657c0a7a36b4c537c93e532`  
		Last Modified: Wed, 04 Oct 2023 21:43:28 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3634708fd9e50993123edc881d3b612bd7abd118c86c10ae821d153c32627d6c`  
		Last Modified: Wed, 04 Oct 2023 21:43:28 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecb450aa2b0fc245622f769a3b887b13b78e60ea9541bfea6ff5c6ec88b683f`  
		Last Modified: Wed, 04 Oct 2023 21:43:28 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:00ec95a9165ad95d580fdd03e9ac2168cbb48c84e783c0d256d2ff2e2c012649
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (25008964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc2fe004ba2fc07cbd3ae7d50e767842934d907a6ed122619d1e28e110d0efec`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:06:25 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:16:46 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:18:54 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:18:58 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:19:00 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:19:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:19:02 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:19:02 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:19:03 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:19:04 GMT
USER fluent
# Wed, 04 Oct 2023 21:19:05 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:19:06 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686c1faa62490a3123a764ff1f9eb8f56b2d2370ca4c57a0df250c27b5f8c567`  
		Last Modified: Wed, 04 Oct 2023 21:27:05 GMT  
		Size: 21.6 MB (21615400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f05d8caa8bd28ac8b74de327805f02bd7541b08a3ff76a90a8edd0ec3be3a8`  
		Last Modified: Wed, 04 Oct 2023 21:26:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74498b595a258f3d58d08ebcd2d0594e2b0954606ac5dce53681b96fa90a9fb6`  
		Last Modified: Wed, 04 Oct 2023 21:26:59 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3e2fa1f46398cb0c1fce47f3a1dbbe71e2ec584d77c560feebc765d18af209`  
		Last Modified: Wed, 04 Oct 2023 21:26:59 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-1` - linux; s390x

```console
$ docker pull fluentd@sha256:4bf9c8b8442eecc11953268bb67197327b4dcd7dfd3c362260c96a431e13fe04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (29998860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7f6f610b30aa0140b9f9276b6b90fa1f395f17501f7fcdb7a94c3614ef43a3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:17:28 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:41:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:47:54 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:48:02 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:48:02 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:48:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:48:03 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:48:04 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:48:05 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:48:05 GMT
USER fluent
# Wed, 04 Oct 2023 21:48:05 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:48:06 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a7cda602ceb77b991077268ddf9794e50138b46af24af519f72acbdec17298`  
		Last Modified: Wed, 04 Oct 2023 21:54:17 GMT  
		Size: 26.8 MB (26820669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977fa9f658a1932ce284e4498f48f661f20e5b5bf01569236217ff0fcc0ea6cc`  
		Last Modified: Wed, 04 Oct 2023 21:54:12 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a7282d352e8cc5052eaaf24c4c0a054b8e7ed3b58082b373ae53b18b4c2eab`  
		Last Modified: Wed, 04 Oct 2023 21:54:12 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b8e091f38fa0c967d062af79901add256471c87f62cbe5b767a12554086282`  
		Last Modified: Wed, 04 Oct 2023 21:54:12 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16-debian-1`

```console
$ docker pull fluentd@sha256:befea572f2daeba921c28672296fe0694b556b0622964e647d1d479d8921a7c4
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
$ docker pull fluentd@sha256:1d35b62d38ac4862b12d5a46d0ab6a6977f25a55c67714e754a1fd75f623dc8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101942094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aacad0b7deb5aea838b3ead852533866f015887813d35c708e49f16713c8f151`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:40:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 11 Oct 2023 20:40:06 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:53:51 GMT
ENV RUBY_MAJOR=3.1
# Wed, 11 Oct 2023 20:53:51 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 11 Oct 2023 20:53:51 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 11 Oct 2023 20:56:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 11 Oct 2023 20:56:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 11 Oct 2023 20:56:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 11 Oct 2023 20:56:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 20:56:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 11 Oct 2023 20:56:15 GMT
CMD ["irb"]
# Thu, 12 Oct 2023 06:01:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 12 Oct 2023 06:01:00 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Thu, 12 Oct 2023 06:01:00 GMT
ENV TINI_VERSION=0.18.0
# Thu, 12 Oct 2023 06:03:43 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 12 Oct 2023 06:03:43 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 12 Oct 2023 06:03:43 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 12 Oct 2023 06:03:43 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 12 Oct 2023 06:03:44 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 12 Oct 2023 06:03:44 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 12 Oct 2023 06:03:44 GMT
EXPOSE 24224 5140
# Thu, 12 Oct 2023 06:03:44 GMT
USER fluent
# Thu, 12 Oct 2023 06:03:44 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 12 Oct 2023 06:03:44 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cada58eb07f29ef1071239308b2b20caad81f8e70a2e078b9c3942432a24748a`  
		Last Modified: Wed, 11 Oct 2023 21:02:56 GMT  
		Size: 10.0 MB (10021717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f1f2bc41fecf9f6996acb6131616bcda56b2d1ee86e8caf908b0cf4baee0fa`  
		Last Modified: Wed, 11 Oct 2023 21:02:54 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bd3d484b43fb5b7ca12bbfa678a88f48219ce775b9f8152dc51a43b849dcea`  
		Last Modified: Wed, 11 Oct 2023 21:04:16 GMT  
		Size: 32.6 MB (32626510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3247685206df6aabd82f42e588449f6ed42988d1739536dc1f1949b8246b2ea`  
		Last Modified: Wed, 11 Oct 2023 21:04:13 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5988d3bce7f6edd02460183bb7036f40e34bfd2715492c9453d66256388277b`  
		Last Modified: Thu, 12 Oct 2023 06:04:06 GMT  
		Size: 27.9 MB (27872924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904e2dc8488bac9a65f778c936fbe1b94c2953f7289b91a2a1faa23a14e86f2f`  
		Last Modified: Thu, 12 Oct 2023 06:04:02 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e394af679a8fcd7c18d7cf3f46698dea21eaa47105b29fae6373de4f1f035ff`  
		Last Modified: Thu, 12 Oct 2023 06:04:02 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1baaef83ca20941d0622841736a497746421e78e4ae5c23c015ee5b4c7479`  
		Last Modified: Thu, 12 Oct 2023 06:04:02 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:30277a6b225a3ca190caf35d4ddac9107134c3138418f8263d109b24ed589c6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.4 MB (95424469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9f0fe4d727d55de639cfcd83ea58d4332b6165ae9147de1ddc129ab57d3c0e`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:59 GMT
ADD file:01d6efe5a08019fcf00cfd0af4d6d61c6d4e43fd98cbb0054e82e8a78275573f in / 
# Wed, 11 Oct 2023 17:37:59 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:49:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 03:49:21 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 04:09:59 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 04:09:59 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 04:09:59 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 04:12:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 04:12:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 04:12:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 04:12:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 04:12:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 04:12:16 GMT
CMD ["irb"]
# Thu, 12 Oct 2023 11:02:36 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 12 Oct 2023 11:02:36 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Thu, 12 Oct 2023 11:02:36 GMT
ENV TINI_VERSION=0.18.0
# Thu, 12 Oct 2023 11:05:32 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 12 Oct 2023 11:05:33 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 12 Oct 2023 11:05:33 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 12 Oct 2023 11:05:33 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 12 Oct 2023 11:05:33 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 12 Oct 2023 11:05:33 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 12 Oct 2023 11:05:33 GMT
EXPOSE 24224 5140
# Thu, 12 Oct 2023 11:05:33 GMT
USER fluent
# Thu, 12 Oct 2023 11:05:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 12 Oct 2023 11:05:33 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:5419c984dacdb9784c03bde904accd013b4e056c627102949c262726f4cae135`  
		Last Modified: Wed, 11 Oct 2023 17:41:31 GMT  
		Size: 28.9 MB (28921245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ead933bc941cea2ffb6c4d6fe4e20f52c37f3845e5bd3adf65401c074b30405`  
		Last Modified: Thu, 12 Oct 2023 04:18:02 GMT  
		Size: 8.6 MB (8635095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e413e1de044985e68b1c11111564a51671f6d424adceac0c66f2bd9e6324c0cd`  
		Last Modified: Thu, 12 Oct 2023 04:18:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3db94c0b0266a6fd06599342cd2f2e32e6c11e549ef29cfff77cf3a9bc322ea`  
		Last Modified: Thu, 12 Oct 2023 04:20:25 GMT  
		Size: 31.2 MB (31166661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048eb6c35fccd60db10de5cee780548e084553fce2fde38316d922c764cfd3ea`  
		Last Modified: Thu, 12 Oct 2023 04:20:21 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77959d857f8643a9f4a201606b38019ef2e94fe2b4b158d0457e04bfee76fee6`  
		Last Modified: Thu, 12 Oct 2023 11:05:54 GMT  
		Size: 26.7 MB (26698391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4460e94d5e6e45182a9ef199438d7520199c6af8e34c06e797917ce171d6e5f`  
		Last Modified: Thu, 12 Oct 2023 11:05:50 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfa600877995d2d370f53cc781ba8fdfbc0263c2ff0b93629d24c56d51c204e`  
		Last Modified: Thu, 12 Oct 2023 11:05:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091d056ca4fa3d21d3f1a28a4fd2a11fa3b85fea32b7d9db21adbb88a3bb0d4`  
		Last Modified: Thu, 12 Oct 2023 11:05:50 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:0746522c0d2f70c4a7fc2623b10969d0fc68e3f8ea22711bb5169edef52a7309
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92298190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21a8f0c2ab7ecacf0cce1dd67e1ca0648f21b7fb6fa05231feedd6686a87fccd`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:01:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:01:55 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 03:01:55 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 03:14:16 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 03:14:16 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 03:14:16 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 03:16:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 03:16:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 03:16:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 03:16:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 03:16:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 03:16:22 GMT
CMD ["irb"]
# Thu, 12 Oct 2023 08:29:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 12 Oct 2023 08:29:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Thu, 12 Oct 2023 08:29:55 GMT
ENV TINI_VERSION=0.18.0
# Thu, 12 Oct 2023 08:32:35 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 12 Oct 2023 08:32:36 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 12 Oct 2023 08:32:36 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 12 Oct 2023 08:32:36 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 12 Oct 2023 08:32:36 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 12 Oct 2023 08:32:36 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 12 Oct 2023 08:32:36 GMT
EXPOSE 24224 5140
# Thu, 12 Oct 2023 08:32:36 GMT
USER fluent
# Thu, 12 Oct 2023 08:32:37 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 12 Oct 2023 08:32:37 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f9636c03e22ba9071724f871360aae36c539df2faafdf58a3c131bd60038d`  
		Last Modified: Thu, 12 Oct 2023 03:22:54 GMT  
		Size: 8.1 MB (8143351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86d4eac531a88957762c8a3d6e3711aa7a8a06b1cf89ad341f35f8ac693e45f`  
		Last Modified: Thu, 12 Oct 2023 03:22:52 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3990b56ab59221f567f9388458451b5c82db38375f8662d1fe2f6fdd5b4d51e`  
		Last Modified: Thu, 12 Oct 2023 03:24:16 GMT  
		Size: 31.0 MB (31037064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960dc7bfd5da030f6a2484c01db2d4deee02218224bf90f6b34605c4a35a3d21`  
		Last Modified: Thu, 12 Oct 2023 03:24:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4354999af8623328b657659a4ff7a9c7f011927faafa321cd319a630c805b`  
		Last Modified: Thu, 12 Oct 2023 08:32:57 GMT  
		Size: 26.5 MB (26535691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b442a5f30cbd88ee7e337892b040ed719a3d0e90d4a410477bc2cdf3d6eb1`  
		Last Modified: Thu, 12 Oct 2023 08:32:53 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0e39a56ba14f787a0d8523c8e4accc580ef7a7eeb013c954d6ba667b46e4e9`  
		Last Modified: Thu, 12 Oct 2023 08:32:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af9cddf002a17d0395cb9b8949987082d3182519c341dfbcf655af9f88535ce`  
		Last Modified: Thu, 12 Oct 2023 08:32:53 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:da3426e00fd909f0bc2c8cf495fe2cb49fed112ce92e484e20966103d3cf0e78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98934000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf6062cb43c15cdf8c4e7bcb580fbb938b0e273c0751b7704d2488849af2cef`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 04:11:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 04:11:09 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 04:29:41 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 04:29:41 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 04:29:41 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 04:31:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 04:31:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 04:31:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 04:31:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 04:31:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 04:31:28 GMT
CMD ["irb"]
# Thu, 12 Oct 2023 16:49:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 12 Oct 2023 16:49:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Thu, 12 Oct 2023 16:49:47 GMT
ENV TINI_VERSION=0.18.0
# Thu, 12 Oct 2023 16:52:08 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 12 Oct 2023 16:52:09 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 12 Oct 2023 16:52:09 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 12 Oct 2023 16:52:09 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 12 Oct 2023 16:52:09 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 12 Oct 2023 16:52:09 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 12 Oct 2023 16:52:10 GMT
EXPOSE 24224 5140
# Thu, 12 Oct 2023 16:52:10 GMT
USER fluent
# Thu, 12 Oct 2023 16:52:10 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 12 Oct 2023 16:52:10 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bca149b06cc0822e464b97deb3f0e1765c7c343855686fa86fc6ad21eef09`  
		Last Modified: Thu, 12 Oct 2023 04:40:09 GMT  
		Size: 9.2 MB (9242842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:929d9dba3329c59299ffae40f3755aa9eaf86094a0ac13ceb2ae223b930fcb6e`  
		Last Modified: Thu, 12 Oct 2023 04:40:07 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a1bd4bca37a9899d12797ef0bd2cc43fffa42f9db9d5475fd020c72acc09b0`  
		Last Modified: Thu, 12 Oct 2023 04:42:30 GMT  
		Size: 32.0 MB (31988170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabd83ec237a83e722494c12d85ff805ada5a0b34af683c6c4d1b7fd3d7ba0ec`  
		Last Modified: Thu, 12 Oct 2023 04:42:28 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222dfd299961582307faf55eb1ed91d185ee7d154f5177fafe4a1d1f710db39`  
		Last Modified: Thu, 12 Oct 2023 16:52:36 GMT  
		Size: 27.6 MB (27635816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323915812ea3703835be97713e18811679a4ad0ad1ebe4be343ccdc6b0e86e3d`  
		Last Modified: Thu, 12 Oct 2023 16:52:32 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0218b5f3403920751cd622262b5c4dda4b329d2e2d8867083412d139b5c87`  
		Last Modified: Thu, 12 Oct 2023 16:52:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f152efba4ec8ac4612ab1fc8d8690edb6bd3d39c6f12bd73f1f855c655b379c5`  
		Last Modified: Thu, 12 Oct 2023 16:52:32 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; 386

```console
$ docker pull fluentd@sha256:fb8868a9cabcd24f58d456ad24969a26e1a4ba655e7e03431cb47ae22b1131f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102334316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9514f5f768714327e5f39b4c70f81f02eb564b75df21a00aa43c154a80c4757e`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:03 GMT
ADD file:ec6d51df021532be6c52d882f60a33d5cce8c3bff039efe8b98e923f2658ba45 in / 
# Wed, 11 Oct 2023 17:41:03 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 13:54:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 13:54:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 13:54:10 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 14:28:24 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 14:28:25 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 14:28:25 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 14:32:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 14:32:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 14:32:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 14:32:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 14:32:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 14:32:20 GMT
CMD ["irb"]
# Thu, 12 Oct 2023 19:50:12 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 12 Oct 2023 19:50:12 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Thu, 12 Oct 2023 19:50:13 GMT
ENV TINI_VERSION=0.18.0
# Thu, 12 Oct 2023 19:53:29 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 12 Oct 2023 19:53:30 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 12 Oct 2023 19:53:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 12 Oct 2023 19:53:30 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 12 Oct 2023 19:53:30 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 12 Oct 2023 19:53:31 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 12 Oct 2023 19:53:31 GMT
EXPOSE 24224 5140
# Thu, 12 Oct 2023 19:53:31 GMT
USER fluent
# Thu, 12 Oct 2023 19:53:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 12 Oct 2023 19:53:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f088164df28359c53d5766709e069e084073984ecf4688687b4c7c529a8926a5`  
		Last Modified: Wed, 11 Oct 2023 17:46:21 GMT  
		Size: 32.4 MB (32402649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e045311c545b9c6a36c38d190ed0c7a1b9e53f8a464211fe2b76a26a31b28561`  
		Last Modified: Thu, 12 Oct 2023 14:48:52 GMT  
		Size: 12.0 MB (11996853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124ad071b0b247992c848286a2b552573bc810f23965ff5acc606553c8bff2b7`  
		Last Modified: Thu, 12 Oct 2023 14:48:48 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3092bd268cf7e12aa9a43fa056edeff95a32db47593c6740f8aa4348513e85`  
		Last Modified: Thu, 12 Oct 2023 14:51:31 GMT  
		Size: 31.2 MB (31182869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a048f68c77b8f3a3150c1a2f7ed34cfceeebb5837058861df1f274385672d2f`  
		Last Modified: Thu, 12 Oct 2023 14:51:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416e10adc149ce79435c2d35fdfddcb4f79f69fa9280a1a991b81f2dcd422999`  
		Last Modified: Thu, 12 Oct 2023 19:53:52 GMT  
		Size: 26.7 MB (26748870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f535ff54e9ff41078958550a0f0c6c3a34a47656df15538905504253287ac5`  
		Last Modified: Thu, 12 Oct 2023 19:53:46 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2874e6fe8a129a9afde710ac19995e267dc44f4490ba65d0ed53f1c00b4a8113`  
		Last Modified: Thu, 12 Oct 2023 19:53:47 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8621a5a59af207a51cf15e19ed78d3758560c13a3babbcc8848808bca768acfd`  
		Last Modified: Thu, 12 Oct 2023 19:53:46 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:58af8b1a07fa62380725ea999fadcd433fea5800ea767502b7fa8ec9074a6eb5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106928332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:874c8c715eaa088724508702be39ad03722a3afea4bbaaeb20270405bdbd0d2a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:53 GMT
ADD file:96450fb62af4cd68105cbbf612cb5d2f79139cc9416835b6c2fdf40727635939 in / 
# Wed, 11 Oct 2023 17:44:55 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 06:09:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 06:09:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 06:09:21 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 06:50:24 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 06:50:25 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 06:50:25 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 06:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 06:55:17 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 06:55:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 06:55:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 06:55:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 06:55:23 GMT
CMD ["irb"]
# Fri, 13 Oct 2023 00:39:01 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 13 Oct 2023 00:39:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 13 Oct 2023 00:39:02 GMT
ENV TINI_VERSION=0.18.0
# Fri, 13 Oct 2023 00:43:10 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 13 Oct 2023 00:43:15 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 13 Oct 2023 00:43:16 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 13 Oct 2023 00:43:16 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 13 Oct 2023 00:43:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 13 Oct 2023 00:43:17 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 13 Oct 2023 00:43:18 GMT
EXPOSE 24224 5140
# Fri, 13 Oct 2023 00:43:19 GMT
USER fluent
# Fri, 13 Oct 2023 00:43:19 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 13 Oct 2023 00:43:20 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:cde4df93466f96fbb1bbc513d09d354ea1e58d3e619c19fcf9120dbba87405ea`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 35.3 MB (35293715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a339ef030d6cbd0678fb5b755061c2364eebea3fd313ba6a16446a838798c4`  
		Last Modified: Thu, 12 Oct 2023 07:06:01 GMT  
		Size: 10.5 MB (10482000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8215dcad534ea438a0485b3f584082b5a6c1bd7654a5044cef8e996e6f638d`  
		Last Modified: Thu, 12 Oct 2023 07:05:57 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f89b0f5dbb5d17bd9bca0220770d50516d37e64e516188b07bc60bf4094925`  
		Last Modified: Thu, 12 Oct 2023 07:08:48 GMT  
		Size: 32.8 MB (32792476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3a8c04aebcf152942430d6ab4d3c381b15fce7d4e441b679caa35de3887e0e`  
		Last Modified: Thu, 12 Oct 2023 07:08:43 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf073a0f31b07ca404fe0971a99f156b98d7ec3b1fa0c9f3ba4f5d5ad0296c3`  
		Last Modified: Fri, 13 Oct 2023 00:43:37 GMT  
		Size: 28.4 MB (28357061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6f81aa2c585f6812a98bf94a95e1ccd4b54aeb05f0a69017d96ba50a33cad7`  
		Last Modified: Fri, 13 Oct 2023 00:43:33 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b66d55ea6382055a39b7b479206f4009ccf2b7f616ce16724bc958e3559a6e`  
		Last Modified: Fri, 13 Oct 2023 00:43:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52658ecfea3c402612eb784d95e147d7239f4671d8176de030ed9eaa033a324`  
		Last Modified: Fri, 13 Oct 2023 00:43:34 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16-debian-1` - linux; s390x

```console
$ docker pull fluentd@sha256:42e8719313de5cb68981482d24232892df063ccf34412c8013d6959fc2745ecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99076678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af8d85d4906f5185b49303e96f2124520e47c3f828795e67b03c652d8cf086d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:58 GMT
ADD file:0cfc89fea6da8404b2bccfb0c408dde9e7497e8a93304c4ced9e51bd2b3a319a in / 
# Wed, 11 Oct 2023 17:51:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 11:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 11:54:03 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 11:54:03 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 12:14:40 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 12:14:40 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 12:14:40 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 12:16:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 12:16:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 12:16:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 12:16:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 12:16:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 12:16:50 GMT
CMD ["irb"]
# Fri, 13 Oct 2023 05:15:37 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 13 Oct 2023 05:15:37 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 13 Oct 2023 05:15:38 GMT
ENV TINI_VERSION=0.18.0
# Fri, 13 Oct 2023 05:17:57 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 13 Oct 2023 05:18:02 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 13 Oct 2023 05:18:02 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 13 Oct 2023 05:18:02 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 13 Oct 2023 05:18:02 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 13 Oct 2023 05:18:02 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 13 Oct 2023 05:18:03 GMT
EXPOSE 24224 5140
# Fri, 13 Oct 2023 05:18:03 GMT
USER fluent
# Fri, 13 Oct 2023 05:18:03 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 13 Oct 2023 05:18:03 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a12df18f4c86c0f825c6b30eb023dc9f30ba0de34f6b97dca708a7247f4f6c49`  
		Last Modified: Wed, 11 Oct 2023 17:57:36 GMT  
		Size: 29.7 MB (29656917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88bf7eca8131e729ed68be7d20715f838c60bbd70ecd694daafbb18f5c024fb`  
		Last Modified: Thu, 12 Oct 2023 12:24:31 GMT  
		Size: 8.9 MB (8863483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa8aa7a11bd587f6a3d11dad38338bc0ea6244ab9fd025418d672d507720d5c`  
		Last Modified: Thu, 12 Oct 2023 12:24:29 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1e2625770a9412e9d16facf0693a7548c7db170616b8d2b9f2b5e5a234c3da`  
		Last Modified: Thu, 12 Oct 2023 12:31:39 GMT  
		Size: 32.4 MB (32445871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4217c616a268964d4460dbc4e159272f5e1201596dbc48e7a6f1f3ee96274d4`  
		Last Modified: Thu, 12 Oct 2023 12:31:36 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bd006d86925e9abaac41a252e34f3f754994d0bc78f0b8ed72ec33f4ff2493`  
		Last Modified: Fri, 13 Oct 2023 05:18:28 GMT  
		Size: 28.1 MB (28107316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dac9b67dda63d3f1cf254e6275535f656d449b7cfff885f0a5b38adc30617f`  
		Last Modified: Fri, 13 Oct 2023 05:18:24 GMT  
		Size: 1.8 KB (1849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5f36efc254ffbead802bef684da0856f6abf30ea5292b4c7be709b95d61e13`  
		Last Modified: Fri, 13 Oct 2023 05:18:24 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff35552b5a60f9933900226a53c3fff29bd8d92abcda771eaec152ddc7a65d1e`  
		Last Modified: Fri, 13 Oct 2023 05:18:24 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16.2-1.1`

```console
$ docker pull fluentd@sha256:0e1090ed3901b0f4a5a4faabb10f91c4fa680da2e2a6503c23832ade8212bfc5
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
$ docker pull fluentd@sha256:13ee83b11a86c4e6593b5acb8e647c22cf1b9feef123612b9dd586465ed05254
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25155206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6e2964bb824f2aacb86d0ca3170997802f000be1eff97299b1188ec8611aa4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 10:08:31 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:19:32 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:20:26 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:20:27 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:20:27 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:20:27 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:20:27 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:20:27 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:20:27 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:20:28 GMT
USER fluent
# Wed, 04 Oct 2023 21:20:28 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:20:28 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8827fca176be13b72bd568162360ca80ecd8eef45b5ef68c80b3a000f503183`  
		Last Modified: Wed, 04 Oct 2023 21:24:01 GMT  
		Size: 21.8 MB (21774385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6515ca36e5cdb6a7919ba7b37f2dd0f2d248776d1f9485d6447a039b1ed9452`  
		Last Modified: Wed, 04 Oct 2023 21:23:58 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3543c7841d7564df2c94d78f0afdedb172e4b82c8677f5b5ad85136ac57a1dd3`  
		Last Modified: Wed, 04 Oct 2023 21:23:58 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57e8a5d5c2f2b9f7e226a62461f9a68d3c8ffaa5b73c8a92b05fa8bcc8d1d96`  
		Last Modified: Wed, 04 Oct 2023 21:23:58 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:059df7f5071014b62e8cd4b3d56609cecbf887753011d04bb0a3b0e017a60f72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23848199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f827678b99b7f0450b51a46ea4bbded99d2af7bc05d42292069f7ac5157f0b4`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 22:13:50 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 20:49:14 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 20:50:18 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 20:50:18 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 20:50:18 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 20:50:19 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 20:50:19 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 20:50:19 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 20:50:19 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 20:50:19 GMT
USER fluent
# Wed, 04 Oct 2023 20:50:19 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 20:50:19 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553532437e6782bb598563089e5c9712ae1d947bcc0e062ecde36c20a8de5397`  
		Last Modified: Wed, 04 Oct 2023 20:50:32 GMT  
		Size: 20.7 MB (20733532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d15a3c0a2634f3d4b2d360f2e9ef8cf7e467483d959c924d4ce1b9de09ff85`  
		Last Modified: Wed, 04 Oct 2023 20:50:29 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b8122aae986d2ea394888a2a35bdfe989c9aff09557fab2b7a3a40c97ca077`  
		Last Modified: Wed, 04 Oct 2023 20:50:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff8c6799857457a342c810fea84380b9f681c2db904dff6caef780d7e0671d3`  
		Last Modified: Wed, 04 Oct 2023 20:50:29 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:8197de0448a2f17bf11f791952b47dada2db36420039a914517dd8fdb9576cd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24629281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b9bbe3c7c4f2dc30c2ce5307d8fe088a8d1b645f876b2f86ab83f0c04d8ec45`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 10:36:07 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:39:29 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:40:19 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:40:19 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:40:20 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:40:20 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:40:20 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:40:20 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:40:20 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:40:20 GMT
USER fluent
# Wed, 04 Oct 2023 21:40:20 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:40:20 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e3f59536119d5781bb641b631d26d36f17086051a8b4afd4683c39e225bb4`  
		Last Modified: Wed, 04 Oct 2023 21:43:15 GMT  
		Size: 21.4 MB (21368773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf0687a8f3c9c7bc2628fceef6bc75e8642ea202b985274313ddd137d5bde2f`  
		Last Modified: Wed, 04 Oct 2023 21:43:12 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f3742a3460d54456ef66da27bcb397c738c7a99e48ee599835c2d5d935c0ca`  
		Last Modified: Wed, 04 Oct 2023 21:43:12 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3629019f4be74a2ec436a05f010c0abc28d5060bf37a9e2874366f5210daf2`  
		Last Modified: Wed, 04 Oct 2023 21:43:12 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; 386

```console
$ docker pull fluentd@sha256:b83b7e92a71b743f967b5288f16a4df4305653819cdb9aaf2d900d46f42909fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24437573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a376d83aefcf980ab1d54ab6eaa54cfe7efd64178c391d35d5dd01828a219566`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:24:48 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:38:20 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:39:32 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:39:33 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:39:33 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:39:33 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:39:33 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:39:33 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:39:33 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:39:33 GMT
USER fluent
# Wed, 04 Oct 2023 21:39:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:39:34 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eeb7c7b7c8cf58216ccf047891a51db52037f8d73338c44bda2aade1939af3`  
		Last Modified: Wed, 04 Oct 2023 21:43:33 GMT  
		Size: 21.0 MB (21021575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfff789f4260eb9a35837ba5b55a3132024fc07f657c0a7a36b4c537c93e532`  
		Last Modified: Wed, 04 Oct 2023 21:43:28 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3634708fd9e50993123edc881d3b612bd7abd118c86c10ae821d153c32627d6c`  
		Last Modified: Wed, 04 Oct 2023 21:43:28 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecb450aa2b0fc245622f769a3b887b13b78e60ea9541bfea6ff5c6ec88b683f`  
		Last Modified: Wed, 04 Oct 2023 21:43:28 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:00ec95a9165ad95d580fdd03e9ac2168cbb48c84e783c0d256d2ff2e2c012649
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.0 MB (25008964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc2fe004ba2fc07cbd3ae7d50e767842934d907a6ed122619d1e28e110d0efec`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:06:25 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:16:46 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:18:54 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:18:58 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:19:00 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:19:01 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:19:02 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:19:02 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:19:03 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:19:04 GMT
USER fluent
# Wed, 04 Oct 2023 21:19:05 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:19:06 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686c1faa62490a3123a764ff1f9eb8f56b2d2370ca4c57a0df250c27b5f8c567`  
		Last Modified: Wed, 04 Oct 2023 21:27:05 GMT  
		Size: 21.6 MB (21615400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f05d8caa8bd28ac8b74de327805f02bd7541b08a3ff76a90a8edd0ec3be3a8`  
		Last Modified: Wed, 04 Oct 2023 21:26:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74498b595a258f3d58d08ebcd2d0594e2b0954606ac5dce53681b96fa90a9fb6`  
		Last Modified: Wed, 04 Oct 2023 21:26:59 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3e2fa1f46398cb0c1fce47f3a1dbbe71e2ec584d77c560feebc765d18af209`  
		Last Modified: Wed, 04 Oct 2023 21:26:59 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-1.1` - linux; s390x

```console
$ docker pull fluentd@sha256:4bf9c8b8442eecc11953268bb67197327b4dcd7dfd3c362260c96a431e13fe04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (29998860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7f6f610b30aa0140b9f9276b6b90fa1f395f17501f7fcdb7a94c3614ef43a3`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:17:28 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 04 Oct 2023 21:41:57 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Wed, 04 Oct 2023 21:47:54 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && gem install bigdecimal -v 1.4.4  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Wed, 04 Oct 2023 21:48:02 GMT
RUN addgroup -S fluent && adduser -S -G fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 04 Oct 2023 21:48:02 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 04 Oct 2023 21:48:03 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 04 Oct 2023 21:48:03 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 04 Oct 2023 21:48:04 GMT
ENV LD_PRELOAD=
# Wed, 04 Oct 2023 21:48:05 GMT
EXPOSE 24224 5140
# Wed, 04 Oct 2023 21:48:05 GMT
USER fluent
# Wed, 04 Oct 2023 21:48:05 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 04 Oct 2023 21:48:06 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a7cda602ceb77b991077268ddf9794e50138b46af24af519f72acbdec17298`  
		Last Modified: Wed, 04 Oct 2023 21:54:17 GMT  
		Size: 26.8 MB (26820669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977fa9f658a1932ce284e4498f48f661f20e5b5bf01569236217ff0fcc0ea6cc`  
		Last Modified: Wed, 04 Oct 2023 21:54:12 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a7282d352e8cc5052eaaf24c4c0a054b8e7ed3b58082b373ae53b18b4c2eab`  
		Last Modified: Wed, 04 Oct 2023 21:54:12 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b8e091f38fa0c967d062af79901add256471c87f62cbe5b767a12554086282`  
		Last Modified: Wed, 04 Oct 2023 21:54:12 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fluentd:v1.16.2-debian-1.1`

```console
$ docker pull fluentd@sha256:befea572f2daeba921c28672296fe0694b556b0622964e647d1d479d8921a7c4
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
$ docker pull fluentd@sha256:1d35b62d38ac4862b12d5a46d0ab6a6977f25a55c67714e754a1fd75f623dc8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101942094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aacad0b7deb5aea838b3ead852533866f015887813d35c708e49f16713c8f151`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:40:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 11 Oct 2023 20:40:06 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:53:51 GMT
ENV RUBY_MAJOR=3.1
# Wed, 11 Oct 2023 20:53:51 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 11 Oct 2023 20:53:51 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 11 Oct 2023 20:56:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 11 Oct 2023 20:56:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 11 Oct 2023 20:56:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 11 Oct 2023 20:56:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 20:56:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 11 Oct 2023 20:56:15 GMT
CMD ["irb"]
# Thu, 12 Oct 2023 06:01:00 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 12 Oct 2023 06:01:00 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Thu, 12 Oct 2023 06:01:00 GMT
ENV TINI_VERSION=0.18.0
# Thu, 12 Oct 2023 06:03:43 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 12 Oct 2023 06:03:43 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 12 Oct 2023 06:03:43 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 12 Oct 2023 06:03:43 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 12 Oct 2023 06:03:44 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 12 Oct 2023 06:03:44 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 12 Oct 2023 06:03:44 GMT
EXPOSE 24224 5140
# Thu, 12 Oct 2023 06:03:44 GMT
USER fluent
# Thu, 12 Oct 2023 06:03:44 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 12 Oct 2023 06:03:44 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cada58eb07f29ef1071239308b2b20caad81f8e70a2e078b9c3942432a24748a`  
		Last Modified: Wed, 11 Oct 2023 21:02:56 GMT  
		Size: 10.0 MB (10021717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f1f2bc41fecf9f6996acb6131616bcda56b2d1ee86e8caf908b0cf4baee0fa`  
		Last Modified: Wed, 11 Oct 2023 21:02:54 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bd3d484b43fb5b7ca12bbfa678a88f48219ce775b9f8152dc51a43b849dcea`  
		Last Modified: Wed, 11 Oct 2023 21:04:16 GMT  
		Size: 32.6 MB (32626510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3247685206df6aabd82f42e588449f6ed42988d1739536dc1f1949b8246b2ea`  
		Last Modified: Wed, 11 Oct 2023 21:04:13 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5988d3bce7f6edd02460183bb7036f40e34bfd2715492c9453d66256388277b`  
		Last Modified: Thu, 12 Oct 2023 06:04:06 GMT  
		Size: 27.9 MB (27872924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904e2dc8488bac9a65f778c936fbe1b94c2953f7289b91a2a1faa23a14e86f2f`  
		Last Modified: Thu, 12 Oct 2023 06:04:02 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e394af679a8fcd7c18d7cf3f46698dea21eaa47105b29fae6373de4f1f035ff`  
		Last Modified: Thu, 12 Oct 2023 06:04:02 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1baaef83ca20941d0622841736a497746421e78e4ae5c23c015ee5b4c7479`  
		Last Modified: Thu, 12 Oct 2023 06:04:02 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; arm variant v5

```console
$ docker pull fluentd@sha256:30277a6b225a3ca190caf35d4ddac9107134c3138418f8263d109b24ed589c6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.4 MB (95424469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9f0fe4d727d55de639cfcd83ea58d4332b6165ae9147de1ddc129ab57d3c0e`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:59 GMT
ADD file:01d6efe5a08019fcf00cfd0af4d6d61c6d4e43fd98cbb0054e82e8a78275573f in / 
# Wed, 11 Oct 2023 17:37:59 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:49:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 03:49:21 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 04:09:59 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 04:09:59 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 04:09:59 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 04:12:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 04:12:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 04:12:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 04:12:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 04:12:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 04:12:16 GMT
CMD ["irb"]
# Thu, 12 Oct 2023 11:02:36 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 12 Oct 2023 11:02:36 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Thu, 12 Oct 2023 11:02:36 GMT
ENV TINI_VERSION=0.18.0
# Thu, 12 Oct 2023 11:05:32 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 12 Oct 2023 11:05:33 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 12 Oct 2023 11:05:33 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 12 Oct 2023 11:05:33 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 12 Oct 2023 11:05:33 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 12 Oct 2023 11:05:33 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 12 Oct 2023 11:05:33 GMT
EXPOSE 24224 5140
# Thu, 12 Oct 2023 11:05:33 GMT
USER fluent
# Thu, 12 Oct 2023 11:05:33 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 12 Oct 2023 11:05:33 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:5419c984dacdb9784c03bde904accd013b4e056c627102949c262726f4cae135`  
		Last Modified: Wed, 11 Oct 2023 17:41:31 GMT  
		Size: 28.9 MB (28921245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ead933bc941cea2ffb6c4d6fe4e20f52c37f3845e5bd3adf65401c074b30405`  
		Last Modified: Thu, 12 Oct 2023 04:18:02 GMT  
		Size: 8.6 MB (8635095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e413e1de044985e68b1c11111564a51671f6d424adceac0c66f2bd9e6324c0cd`  
		Last Modified: Thu, 12 Oct 2023 04:18:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3db94c0b0266a6fd06599342cd2f2e32e6c11e549ef29cfff77cf3a9bc322ea`  
		Last Modified: Thu, 12 Oct 2023 04:20:25 GMT  
		Size: 31.2 MB (31166661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048eb6c35fccd60db10de5cee780548e084553fce2fde38316d922c764cfd3ea`  
		Last Modified: Thu, 12 Oct 2023 04:20:21 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77959d857f8643a9f4a201606b38019ef2e94fe2b4b158d0457e04bfee76fee6`  
		Last Modified: Thu, 12 Oct 2023 11:05:54 GMT  
		Size: 26.7 MB (26698391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4460e94d5e6e45182a9ef199438d7520199c6af8e34c06e797917ce171d6e5f`  
		Last Modified: Thu, 12 Oct 2023 11:05:50 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfa600877995d2d370f53cc781ba8fdfbc0263c2ff0b93629d24c56d51c204e`  
		Last Modified: Thu, 12 Oct 2023 11:05:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091d056ca4fa3d21d3f1a28a4fd2a11fa3b85fea32b7d9db21adbb88a3bb0d4`  
		Last Modified: Thu, 12 Oct 2023 11:05:50 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; arm variant v7

```console
$ docker pull fluentd@sha256:0746522c0d2f70c4a7fc2623b10969d0fc68e3f8ea22711bb5169edef52a7309
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92298190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21a8f0c2ab7ecacf0cce1dd67e1ca0648f21b7fb6fa05231feedd6686a87fccd`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:01:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:01:55 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 03:01:55 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 03:14:16 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 03:14:16 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 03:14:16 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 03:16:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 03:16:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 03:16:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 03:16:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 03:16:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 03:16:22 GMT
CMD ["irb"]
# Thu, 12 Oct 2023 08:29:54 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 12 Oct 2023 08:29:54 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Thu, 12 Oct 2023 08:29:55 GMT
ENV TINI_VERSION=0.18.0
# Thu, 12 Oct 2023 08:32:35 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 12 Oct 2023 08:32:36 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 12 Oct 2023 08:32:36 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 12 Oct 2023 08:32:36 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 12 Oct 2023 08:32:36 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 12 Oct 2023 08:32:36 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 12 Oct 2023 08:32:36 GMT
EXPOSE 24224 5140
# Thu, 12 Oct 2023 08:32:36 GMT
USER fluent
# Thu, 12 Oct 2023 08:32:37 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 12 Oct 2023 08:32:37 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f9636c03e22ba9071724f871360aae36c539df2faafdf58a3c131bd60038d`  
		Last Modified: Thu, 12 Oct 2023 03:22:54 GMT  
		Size: 8.1 MB (8143351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86d4eac531a88957762c8a3d6e3711aa7a8a06b1cf89ad341f35f8ac693e45f`  
		Last Modified: Thu, 12 Oct 2023 03:22:52 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3990b56ab59221f567f9388458451b5c82db38375f8662d1fe2f6fdd5b4d51e`  
		Last Modified: Thu, 12 Oct 2023 03:24:16 GMT  
		Size: 31.0 MB (31037064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960dc7bfd5da030f6a2484c01db2d4deee02218224bf90f6b34605c4a35a3d21`  
		Last Modified: Thu, 12 Oct 2023 03:24:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f4354999af8623328b657659a4ff7a9c7f011927faafa321cd319a630c805b`  
		Last Modified: Thu, 12 Oct 2023 08:32:57 GMT  
		Size: 26.5 MB (26535691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b442a5f30cbd88ee7e337892b040ed719a3d0e90d4a410477bc2cdf3d6eb1`  
		Last Modified: Thu, 12 Oct 2023 08:32:53 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0e39a56ba14f787a0d8523c8e4accc580ef7a7eeb013c954d6ba667b46e4e9`  
		Last Modified: Thu, 12 Oct 2023 08:32:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af9cddf002a17d0395cb9b8949987082d3182519c341dfbcf655af9f88535ce`  
		Last Modified: Thu, 12 Oct 2023 08:32:53 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:da3426e00fd909f0bc2c8cf495fe2cb49fed112ce92e484e20966103d3cf0e78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98934000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf6062cb43c15cdf8c4e7bcb580fbb938b0e273c0751b7704d2488849af2cef`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 04:11:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 04:11:09 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 04:29:41 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 04:29:41 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 04:29:41 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 04:31:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 04:31:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 04:31:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 04:31:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 04:31:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 04:31:28 GMT
CMD ["irb"]
# Thu, 12 Oct 2023 16:49:47 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 12 Oct 2023 16:49:47 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Thu, 12 Oct 2023 16:49:47 GMT
ENV TINI_VERSION=0.18.0
# Thu, 12 Oct 2023 16:52:08 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 12 Oct 2023 16:52:09 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 12 Oct 2023 16:52:09 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 12 Oct 2023 16:52:09 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 12 Oct 2023 16:52:09 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 12 Oct 2023 16:52:09 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 12 Oct 2023 16:52:10 GMT
EXPOSE 24224 5140
# Thu, 12 Oct 2023 16:52:10 GMT
USER fluent
# Thu, 12 Oct 2023 16:52:10 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 12 Oct 2023 16:52:10 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bca149b06cc0822e464b97deb3f0e1765c7c343855686fa86fc6ad21eef09`  
		Last Modified: Thu, 12 Oct 2023 04:40:09 GMT  
		Size: 9.2 MB (9242842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:929d9dba3329c59299ffae40f3755aa9eaf86094a0ac13ceb2ae223b930fcb6e`  
		Last Modified: Thu, 12 Oct 2023 04:40:07 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a1bd4bca37a9899d12797ef0bd2cc43fffa42f9db9d5475fd020c72acc09b0`  
		Last Modified: Thu, 12 Oct 2023 04:42:30 GMT  
		Size: 32.0 MB (31988170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabd83ec237a83e722494c12d85ff805ada5a0b34af683c6c4d1b7fd3d7ba0ec`  
		Last Modified: Thu, 12 Oct 2023 04:42:28 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222dfd299961582307faf55eb1ed91d185ee7d154f5177fafe4a1d1f710db39`  
		Last Modified: Thu, 12 Oct 2023 16:52:36 GMT  
		Size: 27.6 MB (27635816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323915812ea3703835be97713e18811679a4ad0ad1ebe4be343ccdc6b0e86e3d`  
		Last Modified: Thu, 12 Oct 2023 16:52:32 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0218b5f3403920751cd622262b5c4dda4b329d2e2d8867083412d139b5c87`  
		Last Modified: Thu, 12 Oct 2023 16:52:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f152efba4ec8ac4612ab1fc8d8690edb6bd3d39c6f12bd73f1f855c655b379c5`  
		Last Modified: Thu, 12 Oct 2023 16:52:32 GMT  
		Size: 459.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; 386

```console
$ docker pull fluentd@sha256:fb8868a9cabcd24f58d456ad24969a26e1a4ba655e7e03431cb47ae22b1131f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102334316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9514f5f768714327e5f39b4c70f81f02eb564b75df21a00aa43c154a80c4757e`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:03 GMT
ADD file:ec6d51df021532be6c52d882f60a33d5cce8c3bff039efe8b98e923f2658ba45 in / 
# Wed, 11 Oct 2023 17:41:03 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 13:54:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 13:54:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 13:54:10 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 14:28:24 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 14:28:25 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 14:28:25 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 14:32:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 14:32:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 14:32:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 14:32:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 14:32:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 14:32:20 GMT
CMD ["irb"]
# Thu, 12 Oct 2023 19:50:12 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Thu, 12 Oct 2023 19:50:12 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Thu, 12 Oct 2023 19:50:13 GMT
ENV TINI_VERSION=0.18.0
# Thu, 12 Oct 2023 19:53:29 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Thu, 12 Oct 2023 19:53:30 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Thu, 12 Oct 2023 19:53:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Thu, 12 Oct 2023 19:53:30 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Thu, 12 Oct 2023 19:53:30 GMT
ENV FLUENTD_CONF=fluent.conf
# Thu, 12 Oct 2023 19:53:31 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Thu, 12 Oct 2023 19:53:31 GMT
EXPOSE 24224 5140
# Thu, 12 Oct 2023 19:53:31 GMT
USER fluent
# Thu, 12 Oct 2023 19:53:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Thu, 12 Oct 2023 19:53:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:f088164df28359c53d5766709e069e084073984ecf4688687b4c7c529a8926a5`  
		Last Modified: Wed, 11 Oct 2023 17:46:21 GMT  
		Size: 32.4 MB (32402649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e045311c545b9c6a36c38d190ed0c7a1b9e53f8a464211fe2b76a26a31b28561`  
		Last Modified: Thu, 12 Oct 2023 14:48:52 GMT  
		Size: 12.0 MB (11996853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124ad071b0b247992c848286a2b552573bc810f23965ff5acc606553c8bff2b7`  
		Last Modified: Thu, 12 Oct 2023 14:48:48 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3092bd268cf7e12aa9a43fa056edeff95a32db47593c6740f8aa4348513e85`  
		Last Modified: Thu, 12 Oct 2023 14:51:31 GMT  
		Size: 31.2 MB (31182869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a048f68c77b8f3a3150c1a2f7ed34cfceeebb5837058861df1f274385672d2f`  
		Last Modified: Thu, 12 Oct 2023 14:51:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416e10adc149ce79435c2d35fdfddcb4f79f69fa9280a1a991b81f2dcd422999`  
		Last Modified: Thu, 12 Oct 2023 19:53:52 GMT  
		Size: 26.7 MB (26748870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f535ff54e9ff41078958550a0f0c6c3a34a47656df15538905504253287ac5`  
		Last Modified: Thu, 12 Oct 2023 19:53:46 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2874e6fe8a129a9afde710ac19995e267dc44f4490ba65d0ed53f1c00b4a8113`  
		Last Modified: Thu, 12 Oct 2023 19:53:47 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8621a5a59af207a51cf15e19ed78d3758560c13a3babbcc8848808bca768acfd`  
		Last Modified: Thu, 12 Oct 2023 19:53:46 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; ppc64le

```console
$ docker pull fluentd@sha256:58af8b1a07fa62380725ea999fadcd433fea5800ea767502b7fa8ec9074a6eb5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106928332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:874c8c715eaa088724508702be39ad03722a3afea4bbaaeb20270405bdbd0d2a`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:53 GMT
ADD file:96450fb62af4cd68105cbbf612cb5d2f79139cc9416835b6c2fdf40727635939 in / 
# Wed, 11 Oct 2023 17:44:55 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 06:09:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 06:09:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 06:09:21 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 06:50:24 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 06:50:25 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 06:50:25 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 06:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 06:55:17 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 06:55:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 06:55:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 06:55:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 06:55:23 GMT
CMD ["irb"]
# Fri, 13 Oct 2023 00:39:01 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 13 Oct 2023 00:39:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 13 Oct 2023 00:39:02 GMT
ENV TINI_VERSION=0.18.0
# Fri, 13 Oct 2023 00:43:10 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 13 Oct 2023 00:43:15 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 13 Oct 2023 00:43:16 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 13 Oct 2023 00:43:16 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 13 Oct 2023 00:43:17 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 13 Oct 2023 00:43:17 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 13 Oct 2023 00:43:18 GMT
EXPOSE 24224 5140
# Fri, 13 Oct 2023 00:43:19 GMT
USER fluent
# Fri, 13 Oct 2023 00:43:19 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 13 Oct 2023 00:43:20 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:cde4df93466f96fbb1bbc513d09d354ea1e58d3e619c19fcf9120dbba87405ea`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 35.3 MB (35293715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a339ef030d6cbd0678fb5b755061c2364eebea3fd313ba6a16446a838798c4`  
		Last Modified: Thu, 12 Oct 2023 07:06:01 GMT  
		Size: 10.5 MB (10482000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8215dcad534ea438a0485b3f584082b5a6c1bd7654a5044cef8e996e6f638d`  
		Last Modified: Thu, 12 Oct 2023 07:05:57 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f89b0f5dbb5d17bd9bca0220770d50516d37e64e516188b07bc60bf4094925`  
		Last Modified: Thu, 12 Oct 2023 07:08:48 GMT  
		Size: 32.8 MB (32792476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3a8c04aebcf152942430d6ab4d3c381b15fce7d4e441b679caa35de3887e0e`  
		Last Modified: Thu, 12 Oct 2023 07:08:43 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf073a0f31b07ca404fe0971a99f156b98d7ec3b1fa0c9f3ba4f5d5ad0296c3`  
		Last Modified: Fri, 13 Oct 2023 00:43:37 GMT  
		Size: 28.4 MB (28357061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6f81aa2c585f6812a98bf94a95e1ccd4b54aeb05f0a69017d96ba50a33cad7`  
		Last Modified: Fri, 13 Oct 2023 00:43:33 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b66d55ea6382055a39b7b479206f4009ccf2b7f616ce16724bc958e3559a6e`  
		Last Modified: Fri, 13 Oct 2023 00:43:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52658ecfea3c402612eb784d95e147d7239f4671d8176de030ed9eaa033a324`  
		Last Modified: Fri, 13 Oct 2023 00:43:34 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:v1.16.2-debian-1.1` - linux; s390x

```console
$ docker pull fluentd@sha256:42e8719313de5cb68981482d24232892df063ccf34412c8013d6959fc2745ecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99076678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af8d85d4906f5185b49303e96f2124520e47c3f828795e67b03c652d8cf086d`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:58 GMT
ADD file:0cfc89fea6da8404b2bccfb0c408dde9e7497e8a93304c4ced9e51bd2b3a319a in / 
# Wed, 11 Oct 2023 17:51:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 11:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 11:54:03 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 Oct 2023 11:54:03 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 12:14:40 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 Oct 2023 12:14:40 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 12 Oct 2023 12:14:40 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 12 Oct 2023 12:16:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 Oct 2023 12:16:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 Oct 2023 12:16:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 Oct 2023 12:16:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 12:16:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 12 Oct 2023 12:16:50 GMT
CMD ["irb"]
# Fri, 13 Oct 2023 05:15:37 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Fri, 13 Oct 2023 05:15:37 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.16.2
# Fri, 13 Oct 2023 05:15:38 GMT
ENV TINI_VERSION=0.18.0
# Fri, 13 Oct 2023 05:17:57 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends             ca-certificates  && buildDeps="       make gcc g++ libc-dev       wget bzip2 gnupg dirmngr     "  && apt-get install -y --no-install-recommends $buildDeps  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.16.1  && gem install json -v 2.6.3  && gem install rexml -v 3.2.6  && gem install async -v 1.31.0  && gem install async-http -v 0.60.2 && gem install uri -v 0.12.2  && gem install fluentd -v 1.16.2  && dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"  && wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"  && wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"  && export GNUPGHOME="$(mktemp -d)"  && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5  && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini  && rm -r /usr/local/bin/tini.asc  && chmod +x /usr/local/bin/tini  && tini -h  && wget -O /tmp/jemalloc-5.3.0.tar.bz2 https://github.com/jemalloc/jemalloc/releases/download/5.3.0/jemalloc-5.3.0.tar.bz2  && cd /tmp && tar -xjf jemalloc-5.3.0.tar.bz2 && cd jemalloc-5.3.0/  && (echo "je_cv_madv_free=no" > config.cache) && ./configure -C && make  && mv lib/libjemalloc.so.2 /usr/lib  && apt-get purge -y --auto-remove                   -o APT::AutoRemove::RecommendsImportant=false                   $buildDeps  && rm -rf /var/lib/apt/lists/*  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/3.*/gems/fluentd-*/test
# Fri, 13 Oct 2023 05:18:02 GMT
RUN groupadd -r fluent && useradd -r -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Fri, 13 Oct 2023 05:18:02 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Fri, 13 Oct 2023 05:18:02 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Fri, 13 Oct 2023 05:18:02 GMT
ENV FLUENTD_CONF=fluent.conf
# Fri, 13 Oct 2023 05:18:02 GMT
ENV LD_PRELOAD=/usr/lib/libjemalloc.so.2
# Fri, 13 Oct 2023 05:18:03 GMT
EXPOSE 24224 5140
# Fri, 13 Oct 2023 05:18:03 GMT
USER fluent
# Fri, 13 Oct 2023 05:18:03 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Fri, 13 Oct 2023 05:18:03 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:a12df18f4c86c0f825c6b30eb023dc9f30ba0de34f6b97dca708a7247f4f6c49`  
		Last Modified: Wed, 11 Oct 2023 17:57:36 GMT  
		Size: 29.7 MB (29656917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88bf7eca8131e729ed68be7d20715f838c60bbd70ecd694daafbb18f5c024fb`  
		Last Modified: Thu, 12 Oct 2023 12:24:31 GMT  
		Size: 8.9 MB (8863483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa8aa7a11bd587f6a3d11dad38338bc0ea6244ab9fd025418d672d507720d5c`  
		Last Modified: Thu, 12 Oct 2023 12:24:29 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1e2625770a9412e9d16facf0693a7548c7db170616b8d2b9f2b5e5a234c3da`  
		Last Modified: Thu, 12 Oct 2023 12:31:39 GMT  
		Size: 32.4 MB (32445871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4217c616a268964d4460dbc4e159272f5e1201596dbc48e7a6f1f3ee96274d4`  
		Last Modified: Thu, 12 Oct 2023 12:31:36 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bd006d86925e9abaac41a252e34f3f754994d0bc78f0b8ed72ec33f4ff2493`  
		Last Modified: Fri, 13 Oct 2023 05:18:28 GMT  
		Size: 28.1 MB (28107316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dac9b67dda63d3f1cf254e6275535f656d449b7cfff885f0a5b38adc30617f`  
		Last Modified: Fri, 13 Oct 2023 05:18:24 GMT  
		Size: 1.8 KB (1849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5f36efc254ffbead802bef684da0856f6abf30ea5292b4c7be709b95d61e13`  
		Last Modified: Fri, 13 Oct 2023 05:18:24 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff35552b5a60f9933900226a53c3fff29bd8d92abcda771eaec152ddc7a65d1e`  
		Last Modified: Fri, 13 Oct 2023 05:18:24 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
