<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kong`

-	[`kong:1`](#kong1)
-	[`kong:1.5`](#kong15)
-	[`kong:1.5.1`](#kong151)
-	[`kong:1.5.1-alpine`](#kong151-alpine)
-	[`kong:1.5.1-centos`](#kong151-centos)
-	[`kong:1.5.1-ubuntu`](#kong151-ubuntu)
-	[`kong:1.5-centos`](#kong15-centos)
-	[`kong:1.5-ubuntu`](#kong15-ubuntu)
-	[`kong:2`](#kong2)
-	[`kong:2.0`](#kong20)
-	[`kong:2.0.4`](#kong204)
-	[`kong:2.0.4-alpine`](#kong204-alpine)
-	[`kong:2.0.4-centos`](#kong204-centos)
-	[`kong:2.0.4-ubuntu`](#kong204-ubuntu)
-	[`kong:2.0-centos`](#kong20-centos)
-	[`kong:2.0-ubuntu`](#kong20-ubuntu)
-	[`kong:2.1`](#kong21)
-	[`kong:2.1.0-beta.1`](#kong210-beta1)
-	[`kong:2.1.0-beta.1-alpine`](#kong210-beta1-alpine)
-	[`kong:2.1.0-beta.1-centos`](#kong210-beta1-centos)
-	[`kong:2.1.0-beta.1-ubuntu`](#kong210-beta1-ubuntu)
-	[`kong:2.1-alpine`](#kong21-alpine)
-	[`kong:2.1-centos`](#kong21-centos)
-	[`kong:2.1-ubuntu`](#kong21-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:centos`](#kongcentos)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:1`

**does not exist** (yet?)

## `kong:1.5`

```console
$ docker pull kong@sha256:d394801bcfdfd7ffb00416baab1d5a0152a698320a72c3ad5eccb8b78b3767eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5` - linux; amd64

```console
$ docker pull kong@sha256:5d9044488b2587b9e06376a35cb8e48bce8789821794b932735f93ca74256882
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44122107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb43d1ffc3b7166fbb62df75fe40fd74ddf32ecc6a7f02e67040f83a0f6ab4d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:01:31 GMT
ENV KONG_VERSION=1.5.1
# Fri, 24 Apr 2020 14:01:31 GMT
ENV KONG_SHA256=ae31a80d82642ef485a59c832cc91beda7403617cb79384d47b5fbdb2b6f7224
# Fri, 24 Apr 2020 14:01:40 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:01:40 GMT
USER kong
# Fri, 24 Apr 2020 14:01:40 GMT
COPY file:a3a704d6fb65fcd83b4f8be540ad321c86550844ad700b6ca4833afbd65c04a2 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:01:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:01:41 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:01:41 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:01:41 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877f5d653a9ebb1ffa8146c3d0adb444848a636343eb69dd1e60599fe0a2a94d`  
		Last Modified: Fri, 24 Apr 2020 14:05:29 GMT  
		Size: 41.3 MB (41325960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed14408bcf7d87cab0dda9795262fadaf39a4d65221d26f8128bc8b6ff3ae88`  
		Last Modified: Fri, 24 Apr 2020 14:05:21 GMT  
		Size: 567.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.1`

```console
$ docker pull kong@sha256:d394801bcfdfd7ffb00416baab1d5a0152a698320a72c3ad5eccb8b78b3767eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5.1` - linux; amd64

```console
$ docker pull kong@sha256:5d9044488b2587b9e06376a35cb8e48bce8789821794b932735f93ca74256882
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44122107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb43d1ffc3b7166fbb62df75fe40fd74ddf32ecc6a7f02e67040f83a0f6ab4d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:01:31 GMT
ENV KONG_VERSION=1.5.1
# Fri, 24 Apr 2020 14:01:31 GMT
ENV KONG_SHA256=ae31a80d82642ef485a59c832cc91beda7403617cb79384d47b5fbdb2b6f7224
# Fri, 24 Apr 2020 14:01:40 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:01:40 GMT
USER kong
# Fri, 24 Apr 2020 14:01:40 GMT
COPY file:a3a704d6fb65fcd83b4f8be540ad321c86550844ad700b6ca4833afbd65c04a2 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:01:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:01:41 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:01:41 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:01:41 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877f5d653a9ebb1ffa8146c3d0adb444848a636343eb69dd1e60599fe0a2a94d`  
		Last Modified: Fri, 24 Apr 2020 14:05:29 GMT  
		Size: 41.3 MB (41325960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed14408bcf7d87cab0dda9795262fadaf39a4d65221d26f8128bc8b6ff3ae88`  
		Last Modified: Fri, 24 Apr 2020 14:05:21 GMT  
		Size: 567.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.1-alpine`

```console
$ docker pull kong@sha256:d394801bcfdfd7ffb00416baab1d5a0152a698320a72c3ad5eccb8b78b3767eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:5d9044488b2587b9e06376a35cb8e48bce8789821794b932735f93ca74256882
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44122107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb43d1ffc3b7166fbb62df75fe40fd74ddf32ecc6a7f02e67040f83a0f6ab4d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:01:31 GMT
ENV KONG_VERSION=1.5.1
# Fri, 24 Apr 2020 14:01:31 GMT
ENV KONG_SHA256=ae31a80d82642ef485a59c832cc91beda7403617cb79384d47b5fbdb2b6f7224
# Fri, 24 Apr 2020 14:01:40 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:01:40 GMT
USER kong
# Fri, 24 Apr 2020 14:01:40 GMT
COPY file:a3a704d6fb65fcd83b4f8be540ad321c86550844ad700b6ca4833afbd65c04a2 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:01:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:01:41 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:01:41 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:01:41 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877f5d653a9ebb1ffa8146c3d0adb444848a636343eb69dd1e60599fe0a2a94d`  
		Last Modified: Fri, 24 Apr 2020 14:05:29 GMT  
		Size: 41.3 MB (41325960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed14408bcf7d87cab0dda9795262fadaf39a4d65221d26f8128bc8b6ff3ae88`  
		Last Modified: Fri, 24 Apr 2020 14:05:21 GMT  
		Size: 567.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.1-centos`

```console
$ docker pull kong@sha256:1e5daef6de28a3cf07fdfe0a388dd8afb7323b3024d265a6ecaca50ebafa44d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:25e4f468d3406fc0b11878c6237393ad8efb322632a23bfc7acec0bed685f472
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151295984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4713522c8c9ce6a6f6412f8a5edb89417a714fe844f5a3aeb919e4f466e59a38`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:54:58 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 05 May 2020 21:54:58 GMT
ENV KONG_VERSION=1.5.1
# Tue, 05 May 2020 21:54:58 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 21:54:58 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 21:55:35 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 21:55:52 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 21:55:52 GMT
USER kong
# Tue, 05 May 2020 21:55:52 GMT
COPY file:53261f3826b37731452f0b663f02629669c2338dfa058cd1a4d6be45db56e5a6 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:55:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:55:53 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 21:55:53 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 21:55:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe1df8626656e70284e03cc075b524446a3eed089992705f3ae8ba0aa5411b7`  
		Last Modified: Tue, 05 May 2020 22:03:02 GMT  
		Size: 6.6 MB (6605212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54720925d19a1b0ac8043b74835533b91584b9affb8daf2c87856438fe9b158f`  
		Last Modified: Tue, 05 May 2020 22:03:17 GMT  
		Size: 68.8 MB (68810065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652852c5b39726a80091ad85a93689d862800f1ecfdbc0cd727cdd21fb6ec114`  
		Last Modified: Tue, 05 May 2020 22:03:01 GMT  
		Size: 566.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.1-ubuntu`

```console
$ docker pull kong@sha256:a82a8a9384c63c488f1b83575f08ec3e72fbb963f2a10099c0d3e60b70452d12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.5.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:bb20355370665e67fb35c994175f646c91760b6b3c88e8d1be6c3823cd7a6613
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81296098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1769533790190be37265cc4ae87cbb92b012b633398cea92c7d6b9dedbc975bd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:42:09 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 17 Jun 2020 03:42:09 GMT
ENV KONG_VERSION=1.5.1
# Wed, 17 Jun 2020 03:42:26 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong"     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb     && chown -R kong:0 /usr/local/kong     && chmod -R g=u /usr/local/kong
# Wed, 17 Jun 2020 03:42:26 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 17 Jun 2020 03:42:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:42:27 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 17 Jun 2020 03:42:27 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Jun 2020 03:42:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf3c737e169fad205ed349d8a146a5ad4379a4cdd62b78315fbe25cc4cb577d`  
		Last Modified: Wed, 17 Jun 2020 03:44:40 GMT  
		Size: 37.0 MB (36973962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde4daff2ebf22165a55aa5a0b204c493fa0a1d9f5676132111e4742aca5c445`  
		Last Modified: Wed, 17 Jun 2020 03:44:32 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.5.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:12272814aed876ed502e4242bec933d833fa6c095ef322b4db0ef11f234da518
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75977427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f9e357b388c1e529eee74c40813fd9adf21a75c40453faf96896d8122f6685`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:46:36 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 17 Jun 2020 02:46:38 GMT
ENV KONG_VERSION=1.5.1
# Wed, 17 Jun 2020 02:47:26 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong"     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb     && chown -R kong:0 /usr/local/kong     && chmod -R g=u /usr/local/kong
# Wed, 17 Jun 2020 02:47:29 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 17 Jun 2020 02:47:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 17 Jun 2020 02:47:32 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 17 Jun 2020 02:47:32 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Jun 2020 02:47:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071a9d8f76fae18e566e6e1f7bdf8af4816b3819ae078b6355479db1ec3ea502`  
		Last Modified: Wed, 17 Jun 2020 02:51:08 GMT  
		Size: 36.0 MB (35971689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45dc5cf1ab767a3baf2c27445783c33083e93b0c2bb8ac964d521ba614294ec`  
		Last Modified: Wed, 17 Jun 2020 02:50:54 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5-centos`

```console
$ docker pull kong@sha256:1e5daef6de28a3cf07fdfe0a388dd8afb7323b3024d265a6ecaca50ebafa44d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5-centos` - linux; amd64

```console
$ docker pull kong@sha256:25e4f468d3406fc0b11878c6237393ad8efb322632a23bfc7acec0bed685f472
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151295984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4713522c8c9ce6a6f6412f8a5edb89417a714fe844f5a3aeb919e4f466e59a38`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:54:58 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 05 May 2020 21:54:58 GMT
ENV KONG_VERSION=1.5.1
# Tue, 05 May 2020 21:54:58 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 21:54:58 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 21:55:35 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 21:55:52 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 21:55:52 GMT
USER kong
# Tue, 05 May 2020 21:55:52 GMT
COPY file:53261f3826b37731452f0b663f02629669c2338dfa058cd1a4d6be45db56e5a6 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:55:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:55:53 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 21:55:53 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 21:55:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe1df8626656e70284e03cc075b524446a3eed089992705f3ae8ba0aa5411b7`  
		Last Modified: Tue, 05 May 2020 22:03:02 GMT  
		Size: 6.6 MB (6605212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54720925d19a1b0ac8043b74835533b91584b9affb8daf2c87856438fe9b158f`  
		Last Modified: Tue, 05 May 2020 22:03:17 GMT  
		Size: 68.8 MB (68810065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652852c5b39726a80091ad85a93689d862800f1ecfdbc0cd727cdd21fb6ec114`  
		Last Modified: Tue, 05 May 2020 22:03:01 GMT  
		Size: 566.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5-ubuntu`

```console
$ docker pull kong@sha256:a82a8a9384c63c488f1b83575f08ec3e72fbb963f2a10099c0d3e60b70452d12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:bb20355370665e67fb35c994175f646c91760b6b3c88e8d1be6c3823cd7a6613
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81296098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1769533790190be37265cc4ae87cbb92b012b633398cea92c7d6b9dedbc975bd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:42:09 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 17 Jun 2020 03:42:09 GMT
ENV KONG_VERSION=1.5.1
# Wed, 17 Jun 2020 03:42:26 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong"     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb     && chown -R kong:0 /usr/local/kong     && chmod -R g=u /usr/local/kong
# Wed, 17 Jun 2020 03:42:26 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 17 Jun 2020 03:42:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:42:27 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 17 Jun 2020 03:42:27 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Jun 2020 03:42:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf3c737e169fad205ed349d8a146a5ad4379a4cdd62b78315fbe25cc4cb577d`  
		Last Modified: Wed, 17 Jun 2020 03:44:40 GMT  
		Size: 37.0 MB (36973962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde4daff2ebf22165a55aa5a0b204c493fa0a1d9f5676132111e4742aca5c445`  
		Last Modified: Wed, 17 Jun 2020 03:44:32 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:12272814aed876ed502e4242bec933d833fa6c095ef322b4db0ef11f234da518
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75977427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f9e357b388c1e529eee74c40813fd9adf21a75c40453faf96896d8122f6685`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:46:36 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 17 Jun 2020 02:46:38 GMT
ENV KONG_VERSION=1.5.1
# Wed, 17 Jun 2020 02:47:26 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong"     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb     && chown -R kong:0 /usr/local/kong     && chmod -R g=u /usr/local/kong
# Wed, 17 Jun 2020 02:47:29 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 17 Jun 2020 02:47:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 17 Jun 2020 02:47:32 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 17 Jun 2020 02:47:32 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Jun 2020 02:47:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071a9d8f76fae18e566e6e1f7bdf8af4816b3819ae078b6355479db1ec3ea502`  
		Last Modified: Wed, 17 Jun 2020 02:51:08 GMT  
		Size: 36.0 MB (35971689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45dc5cf1ab767a3baf2c27445783c33083e93b0c2bb8ac964d521ba614294ec`  
		Last Modified: Wed, 17 Jun 2020 02:50:54 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2`

**does not exist** (yet?)

## `kong:2.0`

```console
$ docker pull kong@sha256:32a09516a4fad6a7d42a90f7f754970555027a73e349b980a72c7120e00488b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0` - linux; amd64

```console
$ docker pull kong@sha256:dc302feb438b82d99d70e7e140df748654b53341bde9725c7d663baa8fb9b5e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.0 MB (89025900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a800e1cef72354e6e0f6549c23e47d8622aed285f35e7ec340cd19dce577d01`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Tue, 05 May 2020 00:19:57 GMT
COPY file:987d0472e007e4e357d96fa432bce568836a2259b787227f9a9e1c369d9efc37 in /tmp/kong.tar.gz 
# Tue, 05 May 2020 00:19:57 GMT
ARG KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:19:57 GMT
ENV KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:19:57 GMT
ARG KONG_SHA256=457dd0172ae2de2e0b71ce625f78e06449faf38fd734dd6825eb7782d74cb77e
# Tue, 05 May 2020 00:19:57 GMT
ENV KONG_SHA256=457dd0172ae2de2e0b71ce625f78e06449faf38fd734dd6825eb7782d74cb77e
# Tue, 05 May 2020 00:20:09 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libgcc openssl pcre perl tzdata libcap zip bash && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 00:20:10 GMT
COPY file:c7c95ad9b95e03a404039e7ee878ca4bb52cbcb965cd2d12c91037eb7a3b7e65 in /docker-entrypoint.sh 
# Tue, 05 May 2020 00:20:10 GMT
USER kong
# Tue, 05 May 2020 00:20:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 00:20:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 00:20:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 00:20:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79162f4c09617b6148c79941fef29989fd4efaf75afb688429147db76f1c1937`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362c162bd1100f98c75c4f57997da5b9e28cd6ed876bf245131f63971c73f7aa`  
		Last Modified: Tue, 05 May 2020 00:22:58 GMT  
		Size: 86.2 MB (86211770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4da51840b66cea01c99f6efb58af2ac5bee97ac78b11d937f7bc2dca9ac4de`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.4`

```console
$ docker pull kong@sha256:32a09516a4fad6a7d42a90f7f754970555027a73e349b980a72c7120e00488b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.4` - linux; amd64

```console
$ docker pull kong@sha256:dc302feb438b82d99d70e7e140df748654b53341bde9725c7d663baa8fb9b5e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.0 MB (89025900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a800e1cef72354e6e0f6549c23e47d8622aed285f35e7ec340cd19dce577d01`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Tue, 05 May 2020 00:19:57 GMT
COPY file:987d0472e007e4e357d96fa432bce568836a2259b787227f9a9e1c369d9efc37 in /tmp/kong.tar.gz 
# Tue, 05 May 2020 00:19:57 GMT
ARG KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:19:57 GMT
ENV KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:19:57 GMT
ARG KONG_SHA256=457dd0172ae2de2e0b71ce625f78e06449faf38fd734dd6825eb7782d74cb77e
# Tue, 05 May 2020 00:19:57 GMT
ENV KONG_SHA256=457dd0172ae2de2e0b71ce625f78e06449faf38fd734dd6825eb7782d74cb77e
# Tue, 05 May 2020 00:20:09 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libgcc openssl pcre perl tzdata libcap zip bash && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 00:20:10 GMT
COPY file:c7c95ad9b95e03a404039e7ee878ca4bb52cbcb965cd2d12c91037eb7a3b7e65 in /docker-entrypoint.sh 
# Tue, 05 May 2020 00:20:10 GMT
USER kong
# Tue, 05 May 2020 00:20:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 00:20:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 00:20:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 00:20:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79162f4c09617b6148c79941fef29989fd4efaf75afb688429147db76f1c1937`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362c162bd1100f98c75c4f57997da5b9e28cd6ed876bf245131f63971c73f7aa`  
		Last Modified: Tue, 05 May 2020 00:22:58 GMT  
		Size: 86.2 MB (86211770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4da51840b66cea01c99f6efb58af2ac5bee97ac78b11d937f7bc2dca9ac4de`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.4-alpine`

```console
$ docker pull kong@sha256:32a09516a4fad6a7d42a90f7f754970555027a73e349b980a72c7120e00488b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.4-alpine` - linux; amd64

```console
$ docker pull kong@sha256:dc302feb438b82d99d70e7e140df748654b53341bde9725c7d663baa8fb9b5e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.0 MB (89025900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a800e1cef72354e6e0f6549c23e47d8622aed285f35e7ec340cd19dce577d01`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Tue, 05 May 2020 00:19:57 GMT
COPY file:987d0472e007e4e357d96fa432bce568836a2259b787227f9a9e1c369d9efc37 in /tmp/kong.tar.gz 
# Tue, 05 May 2020 00:19:57 GMT
ARG KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:19:57 GMT
ENV KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:19:57 GMT
ARG KONG_SHA256=457dd0172ae2de2e0b71ce625f78e06449faf38fd734dd6825eb7782d74cb77e
# Tue, 05 May 2020 00:19:57 GMT
ENV KONG_SHA256=457dd0172ae2de2e0b71ce625f78e06449faf38fd734dd6825eb7782d74cb77e
# Tue, 05 May 2020 00:20:09 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libgcc openssl pcre perl tzdata libcap zip bash && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 00:20:10 GMT
COPY file:c7c95ad9b95e03a404039e7ee878ca4bb52cbcb965cd2d12c91037eb7a3b7e65 in /docker-entrypoint.sh 
# Tue, 05 May 2020 00:20:10 GMT
USER kong
# Tue, 05 May 2020 00:20:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 00:20:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 00:20:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 00:20:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79162f4c09617b6148c79941fef29989fd4efaf75afb688429147db76f1c1937`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362c162bd1100f98c75c4f57997da5b9e28cd6ed876bf245131f63971c73f7aa`  
		Last Modified: Tue, 05 May 2020 00:22:58 GMT  
		Size: 86.2 MB (86211770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4da51840b66cea01c99f6efb58af2ac5bee97ac78b11d937f7bc2dca9ac4de`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.4-centos`

```console
$ docker pull kong@sha256:26b695f46f0401152bb06730abff6966a06a35c75d151ede1859b450a213df40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.4-centos` - linux; amd64

```console
$ docker pull kong@sha256:0770a2caadebe3516c2b2e3a89f03f0b5ebe5ded765d4b9d89cc9e9107496ab2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125876109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33606e3edaee945be23e4e4e9a8afbc416da3421b00be80f861dec3045b53b2a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:54:26 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 21:54:26 GMT
ARG ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
ENV ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
COPY file:73044b225363e2703a176f55b132687ead4bab30398788756be18d2965fac2cd in /tmp/kong.rpm 
# Tue, 05 May 2020 21:54:27 GMT
ARG KONG_VERSION=2.0.4
# Tue, 05 May 2020 21:54:27 GMT
ENV KONG_VERSION=2.0.4
# Tue, 05 May 2020 21:54:27 GMT
ARG KONG_SHA256=16a934a7bc2e182f00f03bd75b67f4bdb483150b3820d33cab9b0c95539dd353
# Tue, 05 May 2020 21:54:27 GMT
ENV KONG_SHA256=16a934a7bc2e182f00f03bd75b67f4bdb483150b3820d33cab9b0c95539dd353
# Tue, 05 May 2020 21:54:46 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm &&         echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 21:54:47 GMT
COPY file:c7c95ad9b95e03a404039e7ee878ca4bb52cbcb965cd2d12c91037eb7a3b7e65 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:54:47 GMT
USER kong
# Tue, 05 May 2020 21:54:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:54:47 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 21:54:47 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 21:54:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce7701dd3817fcacdc04d8abfd7cd6ea61fe7f4d909903260a2ebe43fce007f`  
		Last Modified: Tue, 05 May 2020 22:02:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c09eae848c2b3842c2e1b6863034e9fb2ca603d8438ae1ffa8d1f1dbd3d1593`  
		Last Modified: Tue, 05 May 2020 22:02:55 GMT  
		Size: 50.0 MB (49995157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a8e1c9ddcadf4475ac984587a95973290b72baed79445bbec7bddea3e7d3ad`  
		Last Modified: Tue, 05 May 2020 22:02:16 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.4-ubuntu`

```console
$ docker pull kong@sha256:6222f8cb4f3dec2ad85cf009b6b730a7f9fd709cd767d103996b02d8a9c9f67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:6e7fc280432b51237a21c97dd07c51109d33ee3bbfbd1853d6311118ee05503d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94258837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b976ee092dd39308988372a5f626dc0e1cbac717718540d7ec5de2e140ce543`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:41:23 GMT
ARG ASSET=ce
# Wed, 17 Jun 2020 03:41:23 GMT
ENV ASSET=ce
# Wed, 17 Jun 2020 03:41:23 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 17 Jun 2020 03:41:23 GMT
ARG KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 03:41:23 GMT
ENV KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 03:41:56 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb &&         apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 17 Jun 2020 03:41:57 GMT
COPY file:7cd3b30326ffeaddc1253699208f97fb54711d4ae930aeeeff1e19ebf51cb561 in /docker-entrypoint.sh 
# Wed, 17 Jun 2020 03:41:57 GMT
USER kong
# Wed, 17 Jun 2020 03:41:58 GMT
RUN kong version
# Wed, 17 Jun 2020 03:41:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:41:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 17 Jun 2020 03:41:58 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Jun 2020 03:41:58 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4343b29744d103aba382b3e0d1bb877f9ecd481767e889ab6c86d1875c6bad99`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c77d810dd3c12a2c32a82bc3979848e8ffe74d88da00a775d5973e2e2303d18`  
		Last Modified: Wed, 17 Jun 2020 03:44:24 GMT  
		Size: 49.9 MB (49936157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c17c931a333f8e16904735f731b63e0b725c77ac98f4cb169e71a903211d53`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad02e74085ded36213dfb17ff4f178ddef933eaed8d1cdda2638546c6946a638`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0.4-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:bfe55a1154736a2511706bf70738456beb92347076e4d77da757dea9dcc95b13
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87924719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd516ef147e5aaaf5b7bec7f6936d10ee29cbba55ed74531d95eeffbc2b11297`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:45:16 GMT
ARG ASSET=ce
# Wed, 17 Jun 2020 02:45:17 GMT
ENV ASSET=ce
# Wed, 17 Jun 2020 02:45:18 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 17 Jun 2020 02:45:19 GMT
ARG KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 02:45:20 GMT
ENV KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 02:46:17 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb &&         apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 17 Jun 2020 02:46:19 GMT
COPY file:7cd3b30326ffeaddc1253699208f97fb54711d4ae930aeeeff1e19ebf51cb561 in /docker-entrypoint.sh 
# Wed, 17 Jun 2020 02:46:20 GMT
USER kong
# Wed, 17 Jun 2020 02:46:23 GMT
RUN kong version
# Wed, 17 Jun 2020 02:46:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 17 Jun 2020 02:46:26 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 17 Jun 2020 02:46:27 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Jun 2020 02:46:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbc29ff205b221c87f413da3a2f3e77b0a8bd55423a1c457fa93d22615eaed3`  
		Last Modified: Wed, 17 Jun 2020 02:50:30 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0275674bb4421e953a1033181662ff0f986471cb8558a0a315ef33de0279d5f`  
		Last Modified: Wed, 17 Jun 2020 02:50:46 GMT  
		Size: 47.9 MB (47918437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81881d2e67473789d504c5467b5f509af8732e4972e825165e6735f065ca001d`  
		Last Modified: Wed, 17 Jun 2020 02:50:30 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99478ac15ba0dbc59c297073e133ea73e0459eb3b290ccaab1d5b0c61fa4bf7b`  
		Last Modified: Wed, 17 Jun 2020 02:50:31 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-centos`

```console
$ docker pull kong@sha256:26b695f46f0401152bb06730abff6966a06a35c75d151ede1859b450a213df40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:0770a2caadebe3516c2b2e3a89f03f0b5ebe5ded765d4b9d89cc9e9107496ab2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125876109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33606e3edaee945be23e4e4e9a8afbc416da3421b00be80f861dec3045b53b2a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:54:26 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 21:54:26 GMT
ARG ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
ENV ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
COPY file:73044b225363e2703a176f55b132687ead4bab30398788756be18d2965fac2cd in /tmp/kong.rpm 
# Tue, 05 May 2020 21:54:27 GMT
ARG KONG_VERSION=2.0.4
# Tue, 05 May 2020 21:54:27 GMT
ENV KONG_VERSION=2.0.4
# Tue, 05 May 2020 21:54:27 GMT
ARG KONG_SHA256=16a934a7bc2e182f00f03bd75b67f4bdb483150b3820d33cab9b0c95539dd353
# Tue, 05 May 2020 21:54:27 GMT
ENV KONG_SHA256=16a934a7bc2e182f00f03bd75b67f4bdb483150b3820d33cab9b0c95539dd353
# Tue, 05 May 2020 21:54:46 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm &&         echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 21:54:47 GMT
COPY file:c7c95ad9b95e03a404039e7ee878ca4bb52cbcb965cd2d12c91037eb7a3b7e65 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:54:47 GMT
USER kong
# Tue, 05 May 2020 21:54:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:54:47 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 21:54:47 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 21:54:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce7701dd3817fcacdc04d8abfd7cd6ea61fe7f4d909903260a2ebe43fce007f`  
		Last Modified: Tue, 05 May 2020 22:02:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c09eae848c2b3842c2e1b6863034e9fb2ca603d8438ae1ffa8d1f1dbd3d1593`  
		Last Modified: Tue, 05 May 2020 22:02:55 GMT  
		Size: 50.0 MB (49995157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a8e1c9ddcadf4475ac984587a95973290b72baed79445bbec7bddea3e7d3ad`  
		Last Modified: Tue, 05 May 2020 22:02:16 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-ubuntu`

```console
$ docker pull kong@sha256:6222f8cb4f3dec2ad85cf009b6b730a7f9fd709cd767d103996b02d8a9c9f67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:6e7fc280432b51237a21c97dd07c51109d33ee3bbfbd1853d6311118ee05503d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94258837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b976ee092dd39308988372a5f626dc0e1cbac717718540d7ec5de2e140ce543`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:41:23 GMT
ARG ASSET=ce
# Wed, 17 Jun 2020 03:41:23 GMT
ENV ASSET=ce
# Wed, 17 Jun 2020 03:41:23 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 17 Jun 2020 03:41:23 GMT
ARG KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 03:41:23 GMT
ENV KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 03:41:56 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb &&         apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 17 Jun 2020 03:41:57 GMT
COPY file:7cd3b30326ffeaddc1253699208f97fb54711d4ae930aeeeff1e19ebf51cb561 in /docker-entrypoint.sh 
# Wed, 17 Jun 2020 03:41:57 GMT
USER kong
# Wed, 17 Jun 2020 03:41:58 GMT
RUN kong version
# Wed, 17 Jun 2020 03:41:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:41:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 17 Jun 2020 03:41:58 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Jun 2020 03:41:58 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4343b29744d103aba382b3e0d1bb877f9ecd481767e889ab6c86d1875c6bad99`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c77d810dd3c12a2c32a82bc3979848e8ffe74d88da00a775d5973e2e2303d18`  
		Last Modified: Wed, 17 Jun 2020 03:44:24 GMT  
		Size: 49.9 MB (49936157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c17c931a333f8e16904735f731b63e0b725c77ac98f4cb169e71a903211d53`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad02e74085ded36213dfb17ff4f178ddef933eaed8d1cdda2638546c6946a638`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:bfe55a1154736a2511706bf70738456beb92347076e4d77da757dea9dcc95b13
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87924719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd516ef147e5aaaf5b7bec7f6936d10ee29cbba55ed74531d95eeffbc2b11297`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:45:16 GMT
ARG ASSET=ce
# Wed, 17 Jun 2020 02:45:17 GMT
ENV ASSET=ce
# Wed, 17 Jun 2020 02:45:18 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 17 Jun 2020 02:45:19 GMT
ARG KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 02:45:20 GMT
ENV KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 02:46:17 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb &&         apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 17 Jun 2020 02:46:19 GMT
COPY file:7cd3b30326ffeaddc1253699208f97fb54711d4ae930aeeeff1e19ebf51cb561 in /docker-entrypoint.sh 
# Wed, 17 Jun 2020 02:46:20 GMT
USER kong
# Wed, 17 Jun 2020 02:46:23 GMT
RUN kong version
# Wed, 17 Jun 2020 02:46:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 17 Jun 2020 02:46:26 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 17 Jun 2020 02:46:27 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Jun 2020 02:46:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbc29ff205b221c87f413da3a2f3e77b0a8bd55423a1c457fa93d22615eaed3`  
		Last Modified: Wed, 17 Jun 2020 02:50:30 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0275674bb4421e953a1033181662ff0f986471cb8558a0a315ef33de0279d5f`  
		Last Modified: Wed, 17 Jun 2020 02:50:46 GMT  
		Size: 47.9 MB (47918437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81881d2e67473789d504c5467b5f509af8732e4972e825165e6735f065ca001d`  
		Last Modified: Wed, 17 Jun 2020 02:50:30 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99478ac15ba0dbc59c297073e133ea73e0459eb3b290ccaab1d5b0c61fa4bf7b`  
		Last Modified: Wed, 17 Jun 2020 02:50:31 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1`

**does not exist** (yet?)

## `kong:2.1.0-beta.1`

**does not exist** (yet?)

## `kong:2.1.0-beta.1-alpine`

**does not exist** (yet?)

## `kong:2.1.0-beta.1-centos`

**does not exist** (yet?)

## `kong:2.1.0-beta.1-ubuntu`

**does not exist** (yet?)

## `kong:2.1-alpine`

**does not exist** (yet?)

## `kong:2.1-centos`

**does not exist** (yet?)

## `kong:2.1-ubuntu`

**does not exist** (yet?)

## `kong:alpine`

```console
$ docker pull kong@sha256:32a09516a4fad6a7d42a90f7f754970555027a73e349b980a72c7120e00488b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:dc302feb438b82d99d70e7e140df748654b53341bde9725c7d663baa8fb9b5e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.0 MB (89025900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a800e1cef72354e6e0f6549c23e47d8622aed285f35e7ec340cd19dce577d01`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Tue, 05 May 2020 00:19:57 GMT
COPY file:987d0472e007e4e357d96fa432bce568836a2259b787227f9a9e1c369d9efc37 in /tmp/kong.tar.gz 
# Tue, 05 May 2020 00:19:57 GMT
ARG KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:19:57 GMT
ENV KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:19:57 GMT
ARG KONG_SHA256=457dd0172ae2de2e0b71ce625f78e06449faf38fd734dd6825eb7782d74cb77e
# Tue, 05 May 2020 00:19:57 GMT
ENV KONG_SHA256=457dd0172ae2de2e0b71ce625f78e06449faf38fd734dd6825eb7782d74cb77e
# Tue, 05 May 2020 00:20:09 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libgcc openssl pcre perl tzdata libcap zip bash && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 00:20:10 GMT
COPY file:c7c95ad9b95e03a404039e7ee878ca4bb52cbcb965cd2d12c91037eb7a3b7e65 in /docker-entrypoint.sh 
# Tue, 05 May 2020 00:20:10 GMT
USER kong
# Tue, 05 May 2020 00:20:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 00:20:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 00:20:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 00:20:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79162f4c09617b6148c79941fef29989fd4efaf75afb688429147db76f1c1937`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362c162bd1100f98c75c4f57997da5b9e28cd6ed876bf245131f63971c73f7aa`  
		Last Modified: Tue, 05 May 2020 00:22:58 GMT  
		Size: 86.2 MB (86211770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4da51840b66cea01c99f6efb58af2ac5bee97ac78b11d937f7bc2dca9ac4de`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:26b695f46f0401152bb06730abff6966a06a35c75d151ede1859b450a213df40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:0770a2caadebe3516c2b2e3a89f03f0b5ebe5ded765d4b9d89cc9e9107496ab2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125876109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33606e3edaee945be23e4e4e9a8afbc416da3421b00be80f861dec3045b53b2a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:54:26 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 21:54:26 GMT
ARG ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
ENV ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
COPY file:73044b225363e2703a176f55b132687ead4bab30398788756be18d2965fac2cd in /tmp/kong.rpm 
# Tue, 05 May 2020 21:54:27 GMT
ARG KONG_VERSION=2.0.4
# Tue, 05 May 2020 21:54:27 GMT
ENV KONG_VERSION=2.0.4
# Tue, 05 May 2020 21:54:27 GMT
ARG KONG_SHA256=16a934a7bc2e182f00f03bd75b67f4bdb483150b3820d33cab9b0c95539dd353
# Tue, 05 May 2020 21:54:27 GMT
ENV KONG_SHA256=16a934a7bc2e182f00f03bd75b67f4bdb483150b3820d33cab9b0c95539dd353
# Tue, 05 May 2020 21:54:46 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm &&         echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 21:54:47 GMT
COPY file:c7c95ad9b95e03a404039e7ee878ca4bb52cbcb965cd2d12c91037eb7a3b7e65 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:54:47 GMT
USER kong
# Tue, 05 May 2020 21:54:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:54:47 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 21:54:47 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 21:54:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce7701dd3817fcacdc04d8abfd7cd6ea61fe7f4d909903260a2ebe43fce007f`  
		Last Modified: Tue, 05 May 2020 22:02:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c09eae848c2b3842c2e1b6863034e9fb2ca603d8438ae1ffa8d1f1dbd3d1593`  
		Last Modified: Tue, 05 May 2020 22:02:55 GMT  
		Size: 50.0 MB (49995157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a8e1c9ddcadf4475ac984587a95973290b72baed79445bbec7bddea3e7d3ad`  
		Last Modified: Tue, 05 May 2020 22:02:16 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:32a09516a4fad6a7d42a90f7f754970555027a73e349b980a72c7120e00488b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:dc302feb438b82d99d70e7e140df748654b53341bde9725c7d663baa8fb9b5e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.0 MB (89025900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a800e1cef72354e6e0f6549c23e47d8622aed285f35e7ec340cd19dce577d01`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Tue, 05 May 2020 00:19:57 GMT
COPY file:987d0472e007e4e357d96fa432bce568836a2259b787227f9a9e1c369d9efc37 in /tmp/kong.tar.gz 
# Tue, 05 May 2020 00:19:57 GMT
ARG KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:19:57 GMT
ENV KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:19:57 GMT
ARG KONG_SHA256=457dd0172ae2de2e0b71ce625f78e06449faf38fd734dd6825eb7782d74cb77e
# Tue, 05 May 2020 00:19:57 GMT
ENV KONG_SHA256=457dd0172ae2de2e0b71ce625f78e06449faf38fd734dd6825eb7782d74cb77e
# Tue, 05 May 2020 00:20:09 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libgcc openssl pcre perl tzdata libcap zip bash && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 00:20:10 GMT
COPY file:c7c95ad9b95e03a404039e7ee878ca4bb52cbcb965cd2d12c91037eb7a3b7e65 in /docker-entrypoint.sh 
# Tue, 05 May 2020 00:20:10 GMT
USER kong
# Tue, 05 May 2020 00:20:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 00:20:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 00:20:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 00:20:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79162f4c09617b6148c79941fef29989fd4efaf75afb688429147db76f1c1937`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362c162bd1100f98c75c4f57997da5b9e28cd6ed876bf245131f63971c73f7aa`  
		Last Modified: Tue, 05 May 2020 00:22:58 GMT  
		Size: 86.2 MB (86211770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4da51840b66cea01c99f6efb58af2ac5bee97ac78b11d937f7bc2dca9ac4de`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:6222f8cb4f3dec2ad85cf009b6b730a7f9fd709cd767d103996b02d8a9c9f67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:6e7fc280432b51237a21c97dd07c51109d33ee3bbfbd1853d6311118ee05503d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94258837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b976ee092dd39308988372a5f626dc0e1cbac717718540d7ec5de2e140ce543`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:41:23 GMT
ARG ASSET=ce
# Wed, 17 Jun 2020 03:41:23 GMT
ENV ASSET=ce
# Wed, 17 Jun 2020 03:41:23 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 17 Jun 2020 03:41:23 GMT
ARG KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 03:41:23 GMT
ENV KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 03:41:56 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb &&         apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 17 Jun 2020 03:41:57 GMT
COPY file:7cd3b30326ffeaddc1253699208f97fb54711d4ae930aeeeff1e19ebf51cb561 in /docker-entrypoint.sh 
# Wed, 17 Jun 2020 03:41:57 GMT
USER kong
# Wed, 17 Jun 2020 03:41:58 GMT
RUN kong version
# Wed, 17 Jun 2020 03:41:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:41:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 17 Jun 2020 03:41:58 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Jun 2020 03:41:58 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4343b29744d103aba382b3e0d1bb877f9ecd481767e889ab6c86d1875c6bad99`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c77d810dd3c12a2c32a82bc3979848e8ffe74d88da00a775d5973e2e2303d18`  
		Last Modified: Wed, 17 Jun 2020 03:44:24 GMT  
		Size: 49.9 MB (49936157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c17c931a333f8e16904735f731b63e0b725c77ac98f4cb169e71a903211d53`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad02e74085ded36213dfb17ff4f178ddef933eaed8d1cdda2638546c6946a638`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:bfe55a1154736a2511706bf70738456beb92347076e4d77da757dea9dcc95b13
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87924719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd516ef147e5aaaf5b7bec7f6936d10ee29cbba55ed74531d95eeffbc2b11297`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 17 Jun 2020 01:44:20 GMT
ADD file:e359a3b06531f763adba716802e252fa49b2e6126f0d3dae1451fc94f5617a13 in / 
# Wed, 17 Jun 2020 01:44:24 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:44:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:44:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:45:16 GMT
ARG ASSET=ce
# Wed, 17 Jun 2020 02:45:17 GMT
ENV ASSET=ce
# Wed, 17 Jun 2020 02:45:18 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 17 Jun 2020 02:45:19 GMT
ARG KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 02:45:20 GMT
ENV KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 02:46:17 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb &&         apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 17 Jun 2020 02:46:19 GMT
COPY file:7cd3b30326ffeaddc1253699208f97fb54711d4ae930aeeeff1e19ebf51cb561 in /docker-entrypoint.sh 
# Wed, 17 Jun 2020 02:46:20 GMT
USER kong
# Wed, 17 Jun 2020 02:46:23 GMT
RUN kong version
# Wed, 17 Jun 2020 02:46:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 17 Jun 2020 02:46:26 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 17 Jun 2020 02:46:27 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Jun 2020 02:46:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:13340090a20bfb81868e7119dc439546fe30dcfccce42509f0fb4d998a1d1fee`  
		Last Modified: Fri, 15 May 2020 16:25:35 GMT  
		Size: 40.0 MB (40003935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eea8c54eb3d5e45521f4ba5c57ede8436f58690cb8a37da90cfcda5efc25f7`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f69e728f2821d6dce88bd1c73ebda9481628a80b563e677ec423b08fdba87`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b20459bfc0dfbc19d643cff0a457a117336e167bb8051554fb88aee48feff`  
		Last Modified: Wed, 17 Jun 2020 01:45:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbc29ff205b221c87f413da3a2f3e77b0a8bd55423a1c457fa93d22615eaed3`  
		Last Modified: Wed, 17 Jun 2020 02:50:30 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0275674bb4421e953a1033181662ff0f986471cb8558a0a315ef33de0279d5f`  
		Last Modified: Wed, 17 Jun 2020 02:50:46 GMT  
		Size: 47.9 MB (47918437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81881d2e67473789d504c5467b5f509af8732e4972e825165e6735f065ca001d`  
		Last Modified: Wed, 17 Jun 2020 02:50:30 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99478ac15ba0dbc59c297073e133ea73e0459eb3b290ccaab1d5b0c61fa4bf7b`  
		Last Modified: Wed, 17 Jun 2020 02:50:31 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
