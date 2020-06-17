<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kong`

-	[`kong:1.0`](#kong10)
-	[`kong:1.0.4`](#kong104)
-	[`kong:1.0.4-alpine`](#kong104-alpine)
-	[`kong:1.0.4-centos`](#kong104-centos)
-	[`kong:1.0-centos`](#kong10-centos)
-	[`kong:1.1`](#kong11)
-	[`kong:1.1.3`](#kong113)
-	[`kong:1.1.3-alpine`](#kong113-alpine)
-	[`kong:1.1.3-centos`](#kong113-centos)
-	[`kong:1.1-centos`](#kong11-centos)
-	[`kong:1.2`](#kong12)
-	[`kong:1.2.3`](#kong123)
-	[`kong:1.2.3-alpine`](#kong123-alpine)
-	[`kong:1.2.3-centos`](#kong123-centos)
-	[`kong:1.2-centos`](#kong12-centos)
-	[`kong:1.3`](#kong13)
-	[`kong:1.3.1`](#kong131)
-	[`kong:1.3.1-alpine`](#kong131-alpine)
-	[`kong:1.3.1-centos`](#kong131-centos)
-	[`kong:1.3.1-ubuntu`](#kong131-ubuntu)
-	[`kong:1.3-centos`](#kong13-centos)
-	[`kong:1.3-ubuntu`](#kong13-ubuntu)
-	[`kong:1.4`](#kong14)
-	[`kong:1.4.3`](#kong143)
-	[`kong:1.4.3-alpine`](#kong143-alpine)
-	[`kong:1.4.3-centos`](#kong143-centos)
-	[`kong:1.4.3-ubuntu`](#kong143-ubuntu)
-	[`kong:1.4-centos`](#kong14-centos)
-	[`kong:1.4-ubuntu`](#kong14-ubuntu)
-	[`kong:1.5`](#kong15)
-	[`kong:1.5.1`](#kong151)
-	[`kong:1.5.1-alpine`](#kong151-alpine)
-	[`kong:1.5.1-centos`](#kong151-centos)
-	[`kong:1.5.1-ubuntu`](#kong151-ubuntu)
-	[`kong:1.5-centos`](#kong15-centos)
-	[`kong:1.5-ubuntu`](#kong15-ubuntu)
-	[`kong:2.0`](#kong20)
-	[`kong:2.0.4`](#kong204)
-	[`kong:2.0.4-alpine`](#kong204-alpine)
-	[`kong:2.0.4-centos`](#kong204-centos)
-	[`kong:2.0.4-ubuntu`](#kong204-ubuntu)
-	[`kong:2.0-centos`](#kong20-centos)
-	[`kong:2.0-ubuntu`](#kong20-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:centos`](#kongcentos)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:1.0`

```console
$ docker pull kong@sha256:49ba0401edf7bf6d2170fc8c272bba4cce5bd91a79a2cb2a1b73294d066ed711
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0` - linux; amd64

```console
$ docker pull kong@sha256:8aac8407146a5b0ab93345e3a64a3677278950aec19a877d4ab2d9d31e7686a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43676224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f949b09952dcf8cf3415a8c8d4bf6d6450948daaf901841499e823bebab1e756`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 29 May 2020 21:43:24 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 29 May 2020 21:43:25 GMT
ENV KONG_VERSION=1.0.4
# Fri, 29 May 2020 21:43:25 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Fri, 29 May 2020 21:43:33 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 29 May 2020 21:43:34 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 29 May 2020 21:43:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 May 2020 21:43:34 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 29 May 2020 21:43:34 GMT
STOPSIGNAL SIGTERM
# Fri, 29 May 2020 21:43:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ebb43b5e78acd88ac9a5ee2c74c36f193227222fe08aa746133f4fe4083936`  
		Last Modified: Fri, 29 May 2020 21:44:09 GMT  
		Size: 40.9 MB (40878088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889efb21ee89a2c48ec4a532258b3278a110515f86aa46d20a4c3ea95e1e77be`  
		Last Modified: Fri, 29 May 2020 21:43:58 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0.4`

```console
$ docker pull kong@sha256:49ba0401edf7bf6d2170fc8c272bba4cce5bd91a79a2cb2a1b73294d066ed711
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0.4` - linux; amd64

```console
$ docker pull kong@sha256:8aac8407146a5b0ab93345e3a64a3677278950aec19a877d4ab2d9d31e7686a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43676224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f949b09952dcf8cf3415a8c8d4bf6d6450948daaf901841499e823bebab1e756`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 29 May 2020 21:43:24 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 29 May 2020 21:43:25 GMT
ENV KONG_VERSION=1.0.4
# Fri, 29 May 2020 21:43:25 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Fri, 29 May 2020 21:43:33 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 29 May 2020 21:43:34 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 29 May 2020 21:43:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 May 2020 21:43:34 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 29 May 2020 21:43:34 GMT
STOPSIGNAL SIGTERM
# Fri, 29 May 2020 21:43:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ebb43b5e78acd88ac9a5ee2c74c36f193227222fe08aa746133f4fe4083936`  
		Last Modified: Fri, 29 May 2020 21:44:09 GMT  
		Size: 40.9 MB (40878088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889efb21ee89a2c48ec4a532258b3278a110515f86aa46d20a4c3ea95e1e77be`  
		Last Modified: Fri, 29 May 2020 21:43:58 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0.4-alpine`

```console
$ docker pull kong@sha256:49ba0401edf7bf6d2170fc8c272bba4cce5bd91a79a2cb2a1b73294d066ed711
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0.4-alpine` - linux; amd64

```console
$ docker pull kong@sha256:8aac8407146a5b0ab93345e3a64a3677278950aec19a877d4ab2d9d31e7686a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43676224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f949b09952dcf8cf3415a8c8d4bf6d6450948daaf901841499e823bebab1e756`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 29 May 2020 21:43:24 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 29 May 2020 21:43:25 GMT
ENV KONG_VERSION=1.0.4
# Fri, 29 May 2020 21:43:25 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Fri, 29 May 2020 21:43:33 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 29 May 2020 21:43:34 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 29 May 2020 21:43:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 May 2020 21:43:34 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 29 May 2020 21:43:34 GMT
STOPSIGNAL SIGTERM
# Fri, 29 May 2020 21:43:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ebb43b5e78acd88ac9a5ee2c74c36f193227222fe08aa746133f4fe4083936`  
		Last Modified: Fri, 29 May 2020 21:44:09 GMT  
		Size: 40.9 MB (40878088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889efb21ee89a2c48ec4a532258b3278a110515f86aa46d20a4c3ea95e1e77be`  
		Last Modified: Fri, 29 May 2020 21:43:58 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0.4-centos`

```console
$ docker pull kong@sha256:6b8262cbafa0da3409757e0f93895b2562cc8d0b019d795923e704daff56a4f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0.4-centos` - linux; amd64

```console
$ docker pull kong@sha256:56dac83357e0880b693fd919a13d87b4d9b55cca04f7cf55b8cd9d24bbe346de
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150405950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30ee883d9ec345ab41e5383ea35f12635be56ec443823689346eeb85e5f4850d`
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
# Tue, 05 May 2020 22:00:44 GMT
ENV KONG_VERSION=1.0.4
# Tue, 05 May 2020 22:00:44 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 22:00:44 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 22:01:31 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 22:01:46 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 22:01:47 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 05 May 2020 22:01:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 22:01:47 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 22:01:47 GMT
STOPSIGNAL SIGTERM
# Tue, 05 May 2020 22:01:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180c3c3037c92349687610ddf07ba05aaede38b32597f8200c49c66c1f062601`  
		Last Modified: Tue, 05 May 2020 22:04:38 GMT  
		Size: 6.6 MB (6605092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b078203132d52e4d8400e354ab41c5f7b2debf9928a4a881df2dc96a5bd40`  
		Last Modified: Tue, 05 May 2020 22:04:48 GMT  
		Size: 67.9 MB (67920122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51371cdb13ff5e3084b41c17086370cd4b28b88f233124994479ee12d9f104e`  
		Last Modified: Tue, 05 May 2020 22:04:36 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0-centos`

```console
$ docker pull kong@sha256:6b8262cbafa0da3409757e0f93895b2562cc8d0b019d795923e704daff56a4f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:56dac83357e0880b693fd919a13d87b4d9b55cca04f7cf55b8cd9d24bbe346de
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150405950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30ee883d9ec345ab41e5383ea35f12635be56ec443823689346eeb85e5f4850d`
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
# Tue, 05 May 2020 22:00:44 GMT
ENV KONG_VERSION=1.0.4
# Tue, 05 May 2020 22:00:44 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 22:00:44 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 22:01:31 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 22:01:46 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 22:01:47 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 05 May 2020 22:01:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 22:01:47 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 22:01:47 GMT
STOPSIGNAL SIGTERM
# Tue, 05 May 2020 22:01:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180c3c3037c92349687610ddf07ba05aaede38b32597f8200c49c66c1f062601`  
		Last Modified: Tue, 05 May 2020 22:04:38 GMT  
		Size: 6.6 MB (6605092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b078203132d52e4d8400e354ab41c5f7b2debf9928a4a881df2dc96a5bd40`  
		Last Modified: Tue, 05 May 2020 22:04:48 GMT  
		Size: 67.9 MB (67920122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51371cdb13ff5e3084b41c17086370cd4b28b88f233124994479ee12d9f104e`  
		Last Modified: Tue, 05 May 2020 22:04:36 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.1`

```console
$ docker pull kong@sha256:a70fdb9985072cee9067d63f26bdc9073e5db4476dd41d049ba3e1d17cddeaea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1` - linux; amd64

```console
$ docker pull kong@sha256:e5eab11634c6b2684c18565c69bf3f88dff35925342cca5353ffdc3ada87244e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43997829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b281b0020211988f6b9787fbbd132dd35ad47c81a7f35f7798f6db3cce87b428`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:03:55 GMT
ENV KONG_VERSION=1.1.3
# Fri, 24 Apr 2020 14:03:55 GMT
ENV KONG_SHA256=834fc83540d77a0ea934ad2c7b59d7f50f9cf8750347ef0ffc572e1b508abbd4
# Fri, 24 Apr 2020 14:04:04 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:04:04 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:04:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:04:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:04:05 GMT
STOPSIGNAL SIGTERM
# Fri, 24 Apr 2020 14:04:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90cdf278884cd9e0ea384833990a604cc5b31842f7b709336673cf88c43592e`  
		Last Modified: Fri, 24 Apr 2020 14:07:34 GMT  
		Size: 41.2 MB (41201651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ad140e7cc05450bbd54986485868179b5fbe971509d6a59793795752b88697`  
		Last Modified: Fri, 24 Apr 2020 14:07:09 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.1.3`

```console
$ docker pull kong@sha256:a70fdb9985072cee9067d63f26bdc9073e5db4476dd41d049ba3e1d17cddeaea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1.3` - linux; amd64

```console
$ docker pull kong@sha256:e5eab11634c6b2684c18565c69bf3f88dff35925342cca5353ffdc3ada87244e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43997829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b281b0020211988f6b9787fbbd132dd35ad47c81a7f35f7798f6db3cce87b428`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:03:55 GMT
ENV KONG_VERSION=1.1.3
# Fri, 24 Apr 2020 14:03:55 GMT
ENV KONG_SHA256=834fc83540d77a0ea934ad2c7b59d7f50f9cf8750347ef0ffc572e1b508abbd4
# Fri, 24 Apr 2020 14:04:04 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:04:04 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:04:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:04:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:04:05 GMT
STOPSIGNAL SIGTERM
# Fri, 24 Apr 2020 14:04:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90cdf278884cd9e0ea384833990a604cc5b31842f7b709336673cf88c43592e`  
		Last Modified: Fri, 24 Apr 2020 14:07:34 GMT  
		Size: 41.2 MB (41201651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ad140e7cc05450bbd54986485868179b5fbe971509d6a59793795752b88697`  
		Last Modified: Fri, 24 Apr 2020 14:07:09 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.1.3-alpine`

```console
$ docker pull kong@sha256:a70fdb9985072cee9067d63f26bdc9073e5db4476dd41d049ba3e1d17cddeaea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:e5eab11634c6b2684c18565c69bf3f88dff35925342cca5353ffdc3ada87244e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43997829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b281b0020211988f6b9787fbbd132dd35ad47c81a7f35f7798f6db3cce87b428`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:03:55 GMT
ENV KONG_VERSION=1.1.3
# Fri, 24 Apr 2020 14:03:55 GMT
ENV KONG_SHA256=834fc83540d77a0ea934ad2c7b59d7f50f9cf8750347ef0ffc572e1b508abbd4
# Fri, 24 Apr 2020 14:04:04 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:04:04 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:04:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:04:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:04:05 GMT
STOPSIGNAL SIGTERM
# Fri, 24 Apr 2020 14:04:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90cdf278884cd9e0ea384833990a604cc5b31842f7b709336673cf88c43592e`  
		Last Modified: Fri, 24 Apr 2020 14:07:34 GMT  
		Size: 41.2 MB (41201651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ad140e7cc05450bbd54986485868179b5fbe971509d6a59793795752b88697`  
		Last Modified: Fri, 24 Apr 2020 14:07:09 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.1.3-centos`

```console
$ docker pull kong@sha256:93c55f96f94045cda9b0c2969f1b44784a469423bcb7d0cd408f6bcc17d33d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1.3-centos` - linux; amd64

```console
$ docker pull kong@sha256:fda791db1f702e27817594802b5a8121daf5529a70410468bacb931283399306
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150610367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ece9d1b3d8f162ff091c5a514529e26854e3f50b7d7cd6e052a6e37b3b15fbe`
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
# Tue, 05 May 2020 21:59:36 GMT
ENV KONG_VERSION=1.1.3
# Tue, 05 May 2020 21:59:36 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 21:59:37 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 22:00:13 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 22:00:33 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 22:00:34 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 05 May 2020 22:00:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 22:00:34 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 22:00:34 GMT
STOPSIGNAL SIGTERM
# Tue, 05 May 2020 22:00:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55adf4f87e4bd87dac07bc3f0ae2d00b0e8bac1cd901146c8eeca6631f2cb7a2`  
		Last Modified: Tue, 05 May 2020 22:04:20 GMT  
		Size: 6.6 MB (6605157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06efc1985939b9987f835de840d5421ac7e6ab770187799a54f2fe82ffdf8e5`  
		Last Modified: Tue, 05 May 2020 22:04:31 GMT  
		Size: 68.1 MB (68124474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c01cfd2e7838a378fd52f6f305eac5117b269671ded0a6ec2fbb2163688525d`  
		Last Modified: Tue, 05 May 2020 22:04:19 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.1-centos`

```console
$ docker pull kong@sha256:93c55f96f94045cda9b0c2969f1b44784a469423bcb7d0cd408f6bcc17d33d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:fda791db1f702e27817594802b5a8121daf5529a70410468bacb931283399306
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150610367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ece9d1b3d8f162ff091c5a514529e26854e3f50b7d7cd6e052a6e37b3b15fbe`
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
# Tue, 05 May 2020 21:59:36 GMT
ENV KONG_VERSION=1.1.3
# Tue, 05 May 2020 21:59:36 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 21:59:37 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 22:00:13 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 22:00:33 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 22:00:34 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 05 May 2020 22:00:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 22:00:34 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 22:00:34 GMT
STOPSIGNAL SIGTERM
# Tue, 05 May 2020 22:00:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55adf4f87e4bd87dac07bc3f0ae2d00b0e8bac1cd901146c8eeca6631f2cb7a2`  
		Last Modified: Tue, 05 May 2020 22:04:20 GMT  
		Size: 6.6 MB (6605157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06efc1985939b9987f835de840d5421ac7e6ab770187799a54f2fe82ffdf8e5`  
		Last Modified: Tue, 05 May 2020 22:04:31 GMT  
		Size: 68.1 MB (68124474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c01cfd2e7838a378fd52f6f305eac5117b269671ded0a6ec2fbb2163688525d`  
		Last Modified: Tue, 05 May 2020 22:04:19 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2`

```console
$ docker pull kong@sha256:0a220de753e707dde302abaf3cac565f60630ecee18135188790f4c161097fe4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2` - linux; amd64

```console
$ docker pull kong@sha256:88eda39b24a31e609c1e3f51b7d64bec94d8da6875a27f049b309959a1696ba2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44491889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c0554b08bd184aec9565dc3368a69bc97efd8e000ea7749e6ef4906468d111f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:03:38 GMT
ENV KONG_VERSION=1.2.3
# Fri, 24 Apr 2020 14:03:38 GMT
ENV KONG_SHA256=4633380fdf5cc3706f53f8697e9789b57aaf06c6bdc67d31bc0dd043453947c3
# Fri, 24 Apr 2020 14:03:46 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:03:47 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:03:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:03:47 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:03:47 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:03:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4cceb88dc774ada5ebe0156eebeb87a02c100ddd375f56668cea38d9cd50bd`  
		Last Modified: Fri, 24 Apr 2020 14:07:04 GMT  
		Size: 41.7 MB (41695711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cb758513301bb3145ef8bb703c7a1a7de3b96048be4f9b8bfedc89226da537`  
		Last Modified: Fri, 24 Apr 2020 14:06:56 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2.3`

```console
$ docker pull kong@sha256:0a220de753e707dde302abaf3cac565f60630ecee18135188790f4c161097fe4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2.3` - linux; amd64

```console
$ docker pull kong@sha256:88eda39b24a31e609c1e3f51b7d64bec94d8da6875a27f049b309959a1696ba2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44491889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c0554b08bd184aec9565dc3368a69bc97efd8e000ea7749e6ef4906468d111f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:03:38 GMT
ENV KONG_VERSION=1.2.3
# Fri, 24 Apr 2020 14:03:38 GMT
ENV KONG_SHA256=4633380fdf5cc3706f53f8697e9789b57aaf06c6bdc67d31bc0dd043453947c3
# Fri, 24 Apr 2020 14:03:46 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:03:47 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:03:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:03:47 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:03:47 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:03:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4cceb88dc774ada5ebe0156eebeb87a02c100ddd375f56668cea38d9cd50bd`  
		Last Modified: Fri, 24 Apr 2020 14:07:04 GMT  
		Size: 41.7 MB (41695711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cb758513301bb3145ef8bb703c7a1a7de3b96048be4f9b8bfedc89226da537`  
		Last Modified: Fri, 24 Apr 2020 14:06:56 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2.3-alpine`

```console
$ docker pull kong@sha256:0a220de753e707dde302abaf3cac565f60630ecee18135188790f4c161097fe4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:88eda39b24a31e609c1e3f51b7d64bec94d8da6875a27f049b309959a1696ba2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44491889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c0554b08bd184aec9565dc3368a69bc97efd8e000ea7749e6ef4906468d111f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:03:38 GMT
ENV KONG_VERSION=1.2.3
# Fri, 24 Apr 2020 14:03:38 GMT
ENV KONG_SHA256=4633380fdf5cc3706f53f8697e9789b57aaf06c6bdc67d31bc0dd043453947c3
# Fri, 24 Apr 2020 14:03:46 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:03:47 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:03:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:03:47 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:03:47 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:03:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4cceb88dc774ada5ebe0156eebeb87a02c100ddd375f56668cea38d9cd50bd`  
		Last Modified: Fri, 24 Apr 2020 14:07:04 GMT  
		Size: 41.7 MB (41695711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cb758513301bb3145ef8bb703c7a1a7de3b96048be4f9b8bfedc89226da537`  
		Last Modified: Fri, 24 Apr 2020 14:06:56 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2.3-centos`

```console
$ docker pull kong@sha256:ecfe6ea3a501d4c7cfd2f9d1b23c2b26c00cc2a460a63c754567d824d943a873
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2.3-centos` - linux; amd64

```console
$ docker pull kong@sha256:b4aa17d4a12ae515e4c0b0d61d535f919ee3b0b880a5c0de0aaf85a7835f7e3f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.8 MB (150822806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24ba27435ac8a5f78cef289134bcbacee2d7c74d985258d9bde111f032f1c466`
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
# Tue, 05 May 2020 21:58:29 GMT
ENV KONG_VERSION=1.2.3
# Tue, 05 May 2020 21:58:29 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 21:58:29 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 21:59:05 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 21:59:22 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 21:59:23 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:59:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:59:23 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 21:59:23 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 21:59:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055676567108ef0d63aa927aac38dd80a0910b61cd50ebc6aaedf2deb6bb055e`  
		Last Modified: Tue, 05 May 2020 22:04:03 GMT  
		Size: 6.6 MB (6605142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a3e674b41a4d1081271d58d3483ff220d9498b98b55e0ddecaf87e7277a0a7`  
		Last Modified: Tue, 05 May 2020 22:04:14 GMT  
		Size: 68.3 MB (68336926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cad7e8f6a1e16b04e739858f554378aee1f49a968d1b346e28f4f5334c8654`  
		Last Modified: Tue, 05 May 2020 22:04:01 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2-centos`

```console
$ docker pull kong@sha256:ecfe6ea3a501d4c7cfd2f9d1b23c2b26c00cc2a460a63c754567d824d943a873
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2-centos` - linux; amd64

```console
$ docker pull kong@sha256:b4aa17d4a12ae515e4c0b0d61d535f919ee3b0b880a5c0de0aaf85a7835f7e3f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.8 MB (150822806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24ba27435ac8a5f78cef289134bcbacee2d7c74d985258d9bde111f032f1c466`
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
# Tue, 05 May 2020 21:58:29 GMT
ENV KONG_VERSION=1.2.3
# Tue, 05 May 2020 21:58:29 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 21:58:29 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 21:59:05 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 21:59:22 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 21:59:23 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:59:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:59:23 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 21:59:23 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 21:59:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055676567108ef0d63aa927aac38dd80a0910b61cd50ebc6aaedf2deb6bb055e`  
		Last Modified: Tue, 05 May 2020 22:04:03 GMT  
		Size: 6.6 MB (6605142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a3e674b41a4d1081271d58d3483ff220d9498b98b55e0ddecaf87e7277a0a7`  
		Last Modified: Tue, 05 May 2020 22:04:14 GMT  
		Size: 68.3 MB (68336926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cad7e8f6a1e16b04e739858f554378aee1f49a968d1b346e28f4f5334c8654`  
		Last Modified: Tue, 05 May 2020 22:04:01 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3`

```console
$ docker pull kong@sha256:0cd1b682f10211c387757ba0e3520c1d25905da5e086735e5744edde249df55b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3` - linux; amd64

```console
$ docker pull kong@sha256:f59c5f3ef2f1e4d9123320914701d43ed3e1031ddcd806a53f707a642f4a0ae5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44814763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a7ddaa9f805973fb53604814900d9abeeee4f946ee89dc7560a4419efc27be3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:02:56 GMT
ENV KONG_VERSION=1.3.1
# Fri, 24 Apr 2020 14:02:56 GMT
ENV KONG_SHA256=61754e884ab7fb62e55ca3547736e14b9b603268f05d33927c17483458c89ddc
# Fri, 24 Apr 2020 14:03:04 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:03:05 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:03:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:03:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:03:05 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:03:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28afcb7677c6d925a67b4c17aa78d35dd746bbd950e31b4bbb7084c02e88f79`  
		Last Modified: Fri, 24 Apr 2020 14:06:38 GMT  
		Size: 42.0 MB (42018585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c2708df13f478f0de9265e1dc36c8468a62b8a5d20ab32fc806c5f4708c9a3`  
		Last Modified: Fri, 24 Apr 2020 14:06:28 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.1`

```console
$ docker pull kong@sha256:0cd1b682f10211c387757ba0e3520c1d25905da5e086735e5744edde249df55b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.1` - linux; amd64

```console
$ docker pull kong@sha256:f59c5f3ef2f1e4d9123320914701d43ed3e1031ddcd806a53f707a642f4a0ae5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44814763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a7ddaa9f805973fb53604814900d9abeeee4f946ee89dc7560a4419efc27be3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:02:56 GMT
ENV KONG_VERSION=1.3.1
# Fri, 24 Apr 2020 14:02:56 GMT
ENV KONG_SHA256=61754e884ab7fb62e55ca3547736e14b9b603268f05d33927c17483458c89ddc
# Fri, 24 Apr 2020 14:03:04 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:03:05 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:03:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:03:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:03:05 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:03:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28afcb7677c6d925a67b4c17aa78d35dd746bbd950e31b4bbb7084c02e88f79`  
		Last Modified: Fri, 24 Apr 2020 14:06:38 GMT  
		Size: 42.0 MB (42018585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c2708df13f478f0de9265e1dc36c8468a62b8a5d20ab32fc806c5f4708c9a3`  
		Last Modified: Fri, 24 Apr 2020 14:06:28 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.1-alpine`

```console
$ docker pull kong@sha256:0cd1b682f10211c387757ba0e3520c1d25905da5e086735e5744edde249df55b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:f59c5f3ef2f1e4d9123320914701d43ed3e1031ddcd806a53f707a642f4a0ae5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44814763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a7ddaa9f805973fb53604814900d9abeeee4f946ee89dc7560a4419efc27be3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:02:56 GMT
ENV KONG_VERSION=1.3.1
# Fri, 24 Apr 2020 14:02:56 GMT
ENV KONG_SHA256=61754e884ab7fb62e55ca3547736e14b9b603268f05d33927c17483458c89ddc
# Fri, 24 Apr 2020 14:03:04 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:03:05 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:03:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:03:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:03:05 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:03:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28afcb7677c6d925a67b4c17aa78d35dd746bbd950e31b4bbb7084c02e88f79`  
		Last Modified: Fri, 24 Apr 2020 14:06:38 GMT  
		Size: 42.0 MB (42018585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c2708df13f478f0de9265e1dc36c8468a62b8a5d20ab32fc806c5f4708c9a3`  
		Last Modified: Fri, 24 Apr 2020 14:06:28 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.1-centos`

```console
$ docker pull kong@sha256:cceb862187e84664b19f1ff25fc6edb2b5b3e1b39ae82a11d818a9d32fbcba2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:4b86bb758447601d9f400edd3e3e506af7eb4fe50f6ed570684128ec59ab98ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151335181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694d8e125cff9933d1a7d385269c51d07d16b8e158d06641e3db699aa7299399`
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
# Tue, 05 May 2020 21:57:20 GMT
ENV KONG_VERSION=1.3.1
# Tue, 05 May 2020 21:57:21 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 21:57:21 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 21:57:57 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 21:58:12 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 21:58:12 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:58:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:58:13 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 21:58:13 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 21:58:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1830aeae4bfba76aba6c12257714cb94a156f45df388e2d1b73fb9a6805dd008`  
		Last Modified: Tue, 05 May 2020 22:03:46 GMT  
		Size: 6.6 MB (6605123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c98380ddd3e7005655d20e951672270eaa279676854673a869bda252c60a68`  
		Last Modified: Tue, 05 May 2020 22:03:55 GMT  
		Size: 68.8 MB (68849322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ec6e72e779d9314238f98699205b33003d26ec55a4840df5916cfc0eefb85a`  
		Last Modified: Tue, 05 May 2020 22:03:44 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.1-ubuntu`

```console
$ docker pull kong@sha256:bc243b1f57158a2747fe64f9562f205d979c8674a22d349a8f1ff6980910c8d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:7a68253f30a01475846d6f8b3f9aa4683c057ff9797baa407fe43c0b1168f191
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81268007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a993be0a4e88404bf6b76669d0ac72177cdc8f8c07560a9f51ab4e0393434a39`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 14:00:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:03:10 GMT
ENV KONG_VERSION=1.3.1
# Fri, 24 Apr 2020 14:03:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Fri, 24 Apr 2020 14:03:30 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:03:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:03:31 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:03:31 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:03:31 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7cc69fdf4ca326c2462e8bbe2905a24a9eb232b2f6b45a357ef73cd71bbc75`  
		Last Modified: Fri, 24 Apr 2020 14:06:51 GMT  
		Size: 37.0 MB (37019016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcc55aa8062d3f458a54b1e70eac4f6bfbfdcebc9232fbf1727dd39359ee277`  
		Last Modified: Fri, 24 Apr 2020 14:06:44 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3-centos`

```console
$ docker pull kong@sha256:cceb862187e84664b19f1ff25fc6edb2b5b3e1b39ae82a11d818a9d32fbcba2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3-centos` - linux; amd64

```console
$ docker pull kong@sha256:4b86bb758447601d9f400edd3e3e506af7eb4fe50f6ed570684128ec59ab98ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151335181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694d8e125cff9933d1a7d385269c51d07d16b8e158d06641e3db699aa7299399`
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
# Tue, 05 May 2020 21:57:20 GMT
ENV KONG_VERSION=1.3.1
# Tue, 05 May 2020 21:57:21 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 21:57:21 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 21:57:57 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 21:58:12 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 21:58:12 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:58:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:58:13 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 21:58:13 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 21:58:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1830aeae4bfba76aba6c12257714cb94a156f45df388e2d1b73fb9a6805dd008`  
		Last Modified: Tue, 05 May 2020 22:03:46 GMT  
		Size: 6.6 MB (6605123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c98380ddd3e7005655d20e951672270eaa279676854673a869bda252c60a68`  
		Last Modified: Tue, 05 May 2020 22:03:55 GMT  
		Size: 68.8 MB (68849322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ec6e72e779d9314238f98699205b33003d26ec55a4840df5916cfc0eefb85a`  
		Last Modified: Tue, 05 May 2020 22:03:44 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3-ubuntu`

```console
$ docker pull kong@sha256:af50c45f847c070a0c8d807c42dcd0ffa7ca12def9cd1978dfc15c96e3287419
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:7a68253f30a01475846d6f8b3f9aa4683c057ff9797baa407fe43c0b1168f191
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81268007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a993be0a4e88404bf6b76669d0ac72177cdc8f8c07560a9f51ab4e0393434a39`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 14:00:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:03:10 GMT
ENV KONG_VERSION=1.3.1
# Fri, 24 Apr 2020 14:03:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Fri, 24 Apr 2020 14:03:30 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:03:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:03:31 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:03:31 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:03:31 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7cc69fdf4ca326c2462e8bbe2905a24a9eb232b2f6b45a357ef73cd71bbc75`  
		Last Modified: Fri, 24 Apr 2020 14:06:51 GMT  
		Size: 37.0 MB (37019016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcc55aa8062d3f458a54b1e70eac4f6bfbfdcebc9232fbf1727dd39359ee277`  
		Last Modified: Fri, 24 Apr 2020 14:06:44 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:eb3454c6427783ce723203d80b0965f92c277f45cb6022cff31a730fcacc094e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75784829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e972c11c44663384ea10e5b80f493bd59155ec86a93e424e362c8fe8cfcac37`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 19 Dec 2019 03:54:56 GMT
ADD file:ef40ad352b3111bab843b916e802c7cb18aeccc96a65fe9a7a5330572431e7c7 in / 
# Thu, 19 Dec 2019 03:54:59 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 03:55:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 03:55:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 03:55:11 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:46:45 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 19 Dec 2019 07:47:39 GMT
ENV KONG_VERSION=1.3.0
# Thu, 19 Dec 2019 07:48:21 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 19 Dec 2019 07:48:24 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 19 Dec 2019 07:48:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:48:26 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 19 Dec 2019 07:48:28 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 07:48:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:b8d9a83fac1745f67aed1e924445fc9a89cd885fe70d0e1e335cbe4791f490b5`  
		Last Modified: Thu, 19 Dec 2019 03:57:28 GMT  
		Size: 39.9 MB (39875399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b9cc76ef947c73adaf3c9e2dd2f8da166e815b37d431b9baae7aebe84096fe`  
		Last Modified: Thu, 19 Dec 2019 03:57:19 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0d286195ea15592986e2820cc7366deda87cc2802b6cfe82a6f5388aceb4a4`  
		Last Modified: Thu, 19 Dec 2019 03:57:18 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120fa5dd162f3d2fa3a1452a4d909074c6ffcba06016d39e5781581ec1ec5f88`  
		Last Modified: Thu, 19 Dec 2019 03:57:18 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df99ab07fe46df2c670fdefa6329d71025b7199f43f6d8ed60ae527e197ef38`  
		Last Modified: Thu, 19 Dec 2019 07:49:17 GMT  
		Size: 35.9 MB (35907633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd759577537829c9d5631e88bf468fbf149c5b86ee845da6a5cd0e14e413092c`  
		Last Modified: Thu, 19 Dec 2019 07:49:02 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4`

```console
$ docker pull kong@sha256:b77490f37557628122ccfcdb8afae54bb081828ca464c980dadf69cafa31ff7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4` - linux; amd64

```console
$ docker pull kong@sha256:33d73a68ada9f93a9ef52d495f2b2a0e4a4775ea7d3aafe327da75c3c369d36e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44123771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ded3c6d1ba57d85525498255ad331783ae379656aadd444e2c5e3a751d1c64`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:02:13 GMT
ENV KONG_VERSION=1.4.3
# Fri, 24 Apr 2020 14:02:13 GMT
ENV KONG_SHA256=419d4e3d19f2d5c35ec6367e736b0d5509be4a7577d203008514a90f8dd5fdf1
# Fri, 24 Apr 2020 14:02:22 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:02:23 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:02:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:02:23 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:02:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:02:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eadacc9175c6c8fa6b61313eb2c46edde354d3bd76b9767a6c714b9d9b6319`  
		Last Modified: Fri, 24 Apr 2020 14:05:53 GMT  
		Size: 41.3 MB (41327594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca9d1d576bcb9baa2540912704b3314e3b7df1e20df99b94e099066049f7c91`  
		Last Modified: Fri, 24 Apr 2020 14:05:45 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.3`

```console
$ docker pull kong@sha256:b77490f37557628122ccfcdb8afae54bb081828ca464c980dadf69cafa31ff7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4.3` - linux; amd64

```console
$ docker pull kong@sha256:33d73a68ada9f93a9ef52d495f2b2a0e4a4775ea7d3aafe327da75c3c369d36e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44123771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ded3c6d1ba57d85525498255ad331783ae379656aadd444e2c5e3a751d1c64`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:02:13 GMT
ENV KONG_VERSION=1.4.3
# Fri, 24 Apr 2020 14:02:13 GMT
ENV KONG_SHA256=419d4e3d19f2d5c35ec6367e736b0d5509be4a7577d203008514a90f8dd5fdf1
# Fri, 24 Apr 2020 14:02:22 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:02:23 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:02:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:02:23 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:02:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:02:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eadacc9175c6c8fa6b61313eb2c46edde354d3bd76b9767a6c714b9d9b6319`  
		Last Modified: Fri, 24 Apr 2020 14:05:53 GMT  
		Size: 41.3 MB (41327594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca9d1d576bcb9baa2540912704b3314e3b7df1e20df99b94e099066049f7c91`  
		Last Modified: Fri, 24 Apr 2020 14:05:45 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.3-alpine`

```console
$ docker pull kong@sha256:b77490f37557628122ccfcdb8afae54bb081828ca464c980dadf69cafa31ff7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:33d73a68ada9f93a9ef52d495f2b2a0e4a4775ea7d3aafe327da75c3c369d36e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44123771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ded3c6d1ba57d85525498255ad331783ae379656aadd444e2c5e3a751d1c64`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:02:13 GMT
ENV KONG_VERSION=1.4.3
# Fri, 24 Apr 2020 14:02:13 GMT
ENV KONG_SHA256=419d4e3d19f2d5c35ec6367e736b0d5509be4a7577d203008514a90f8dd5fdf1
# Fri, 24 Apr 2020 14:02:22 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:02:23 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:02:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:02:23 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:02:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:02:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eadacc9175c6c8fa6b61313eb2c46edde354d3bd76b9767a6c714b9d9b6319`  
		Last Modified: Fri, 24 Apr 2020 14:05:53 GMT  
		Size: 41.3 MB (41327594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca9d1d576bcb9baa2540912704b3314e3b7df1e20df99b94e099066049f7c91`  
		Last Modified: Fri, 24 Apr 2020 14:05:45 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.3-centos`

```console
$ docker pull kong@sha256:a238399bea1adb3c6960171d8b0647d5acf9406b5f1c3f6e53e1a33ca314ed64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4.3-centos` - linux; amd64

```console
$ docker pull kong@sha256:8c81cd36da58552e0f97942df9c9b3b0b993d9e69934b3ffcebd018f8d112709
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151305582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de7c4d8144bea6d7d66591b2176ff6798fd1507de068111b28396598734d7646`
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
# Tue, 05 May 2020 21:56:10 GMT
ENV KONG_VERSION=1.4.3
# Tue, 05 May 2020 21:56:10 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 21:56:10 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 21:56:46 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 21:57:02 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 21:57:02 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:57:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:57:03 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 21:57:03 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 21:57:03 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e9242cd6b5c0e572b0232b9454bee479dd8758a47e73dffb0f83d5961dfa50`  
		Last Modified: Tue, 05 May 2020 22:03:24 GMT  
		Size: 6.6 MB (6605099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5787a23592612fc9da7a6a0eb267a652ac592a8c0b3db68700e2b1c9234deb`  
		Last Modified: Tue, 05 May 2020 22:03:39 GMT  
		Size: 68.8 MB (68819748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f0d2587cb74bd747b2e6f987acff041809d076126589c74f97eeb395421bc0`  
		Last Modified: Tue, 05 May 2020 22:03:22 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.3-ubuntu`

```console
$ docker pull kong@sha256:1947d4e4d6ad0d8e03bea8a539e784fbc62449a946f33a9fe027dbeceb0b75a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.4.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:aa2faf4417184fe81e5d62aaf928ecf9ac771da54a317de412de257af1d758c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81234406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a2a026120b41781573d42390e80efaabfc84fa5b5970c2b7f7bdda6099a124`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 14:00:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:02:27 GMT
ENV KONG_VERSION=1.4.3
# Fri, 24 Apr 2020 14:02:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) KONG_SHA256='d5e8debfd0c3a56a447a0613df1ebc8626eb262dc7af80ac7a5df4df329849c8' ;; 		arm64) KONG_SHA256='87f2328f40754e3ca849cdaac1883de1a0da7c780f3a4f913d5ae906e33d7dce' ;; 	esac; 	echo "$KONG_SHA256 kong.deb" | sha256sum -c - 	&& rm -rf kong.deb
# Fri, 24 Apr 2020 14:02:47 GMT
RUN kong version
# Fri, 24 Apr 2020 14:02:47 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:02:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:02:47 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:02:47 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:02:48 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca07fa0c6368909b4b2d55f8ac0e5e8333cc8359f37d88b7195bcdfd0e6b910b`  
		Last Modified: Fri, 24 Apr 2020 14:06:23 GMT  
		Size: 37.0 MB (36985323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86371219f57f51668e2129601bdd59bb0d2a9a1115d21dae6f02a9cfe9c640d0`  
		Last Modified: Fri, 24 Apr 2020 14:05:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3a12629a04e7c55df751f11ca729601d23078e57cf98b315f0d443eef6f957`  
		Last Modified: Fri, 24 Apr 2020 14:05:58 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.4.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:43aa9efc44df64eb7ca4ab98851b63bd84aa5482a53bb8abab4fe625dcea93d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75935017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ebda6449e7d24943c48327dbb7946c92dbffee8ad1379f045f378f195d8873`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:01:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 15:03:03 GMT
ENV KONG_VERSION=1.4.3
# Fri, 24 Apr 2020 15:03:43 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) KONG_SHA256='d5e8debfd0c3a56a447a0613df1ebc8626eb262dc7af80ac7a5df4df329849c8' ;; 		arm64) KONG_SHA256='87f2328f40754e3ca849cdaac1883de1a0da7c780f3a4f913d5ae906e33d7dce' ;; 	esac; 	echo "$KONG_SHA256 kong.deb" | sha256sum -c - 	&& rm -rf kong.deb
# Fri, 24 Apr 2020 15:03:47 GMT
RUN kong version
# Fri, 24 Apr 2020 15:03:48 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 15:03:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 15:03:49 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 15:03:50 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 15:03:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657e49e338488bc5e7f1094c4c82fbc746ef045f73df125663e539d546ae604b`  
		Last Modified: Fri, 24 Apr 2020 15:06:28 GMT  
		Size: 36.0 MB (35964328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fe4ceae85866c07c838f22f19887b72f257b543d8f8eb5710eaf0ee3f00433`  
		Last Modified: Fri, 24 Apr 2020 15:06:15 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbe79164650de57cf0ef2e48a1b75ba226937d0c9d42b4385f57069f2eba601`  
		Last Modified: Fri, 24 Apr 2020 15:06:15 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4-centos`

```console
$ docker pull kong@sha256:a238399bea1adb3c6960171d8b0647d5acf9406b5f1c3f6e53e1a33ca314ed64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4-centos` - linux; amd64

```console
$ docker pull kong@sha256:8c81cd36da58552e0f97942df9c9b3b0b993d9e69934b3ffcebd018f8d112709
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151305582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de7c4d8144bea6d7d66591b2176ff6798fd1507de068111b28396598734d7646`
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
# Tue, 05 May 2020 21:56:10 GMT
ENV KONG_VERSION=1.4.3
# Tue, 05 May 2020 21:56:10 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 05 May 2020 21:56:10 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 05 May 2020 21:56:46 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 05 May 2020 21:57:02 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 21:57:02 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 05 May 2020 21:57:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:57:03 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 21:57:03 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 21:57:03 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e9242cd6b5c0e572b0232b9454bee479dd8758a47e73dffb0f83d5961dfa50`  
		Last Modified: Tue, 05 May 2020 22:03:24 GMT  
		Size: 6.6 MB (6605099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5787a23592612fc9da7a6a0eb267a652ac592a8c0b3db68700e2b1c9234deb`  
		Last Modified: Tue, 05 May 2020 22:03:39 GMT  
		Size: 68.8 MB (68819748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f0d2587cb74bd747b2e6f987acff041809d076126589c74f97eeb395421bc0`  
		Last Modified: Tue, 05 May 2020 22:03:22 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4-ubuntu`

```console
$ docker pull kong@sha256:1947d4e4d6ad0d8e03bea8a539e784fbc62449a946f33a9fe027dbeceb0b75a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:aa2faf4417184fe81e5d62aaf928ecf9ac771da54a317de412de257af1d758c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81234406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a2a026120b41781573d42390e80efaabfc84fa5b5970c2b7f7bdda6099a124`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 14:00:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:02:27 GMT
ENV KONG_VERSION=1.4.3
# Fri, 24 Apr 2020 14:02:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) KONG_SHA256='d5e8debfd0c3a56a447a0613df1ebc8626eb262dc7af80ac7a5df4df329849c8' ;; 		arm64) KONG_SHA256='87f2328f40754e3ca849cdaac1883de1a0da7c780f3a4f913d5ae906e33d7dce' ;; 	esac; 	echo "$KONG_SHA256 kong.deb" | sha256sum -c - 	&& rm -rf kong.deb
# Fri, 24 Apr 2020 14:02:47 GMT
RUN kong version
# Fri, 24 Apr 2020 14:02:47 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:02:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:02:47 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:02:47 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:02:48 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca07fa0c6368909b4b2d55f8ac0e5e8333cc8359f37d88b7195bcdfd0e6b910b`  
		Last Modified: Fri, 24 Apr 2020 14:06:23 GMT  
		Size: 37.0 MB (36985323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86371219f57f51668e2129601bdd59bb0d2a9a1115d21dae6f02a9cfe9c640d0`  
		Last Modified: Fri, 24 Apr 2020 14:05:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3a12629a04e7c55df751f11ca729601d23078e57cf98b315f0d443eef6f957`  
		Last Modified: Fri, 24 Apr 2020 14:05:58 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.4-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:43aa9efc44df64eb7ca4ab98851b63bd84aa5482a53bb8abab4fe625dcea93d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75935017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ebda6449e7d24943c48327dbb7946c92dbffee8ad1379f045f378f195d8873`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:01:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 15:03:03 GMT
ENV KONG_VERSION=1.4.3
# Fri, 24 Apr 2020 15:03:43 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) KONG_SHA256='d5e8debfd0c3a56a447a0613df1ebc8626eb262dc7af80ac7a5df4df329849c8' ;; 		arm64) KONG_SHA256='87f2328f40754e3ca849cdaac1883de1a0da7c780f3a4f913d5ae906e33d7dce' ;; 	esac; 	echo "$KONG_SHA256 kong.deb" | sha256sum -c - 	&& rm -rf kong.deb
# Fri, 24 Apr 2020 15:03:47 GMT
RUN kong version
# Fri, 24 Apr 2020 15:03:48 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 15:03:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 15:03:49 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 15:03:50 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 15:03:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657e49e338488bc5e7f1094c4c82fbc746ef045f73df125663e539d546ae604b`  
		Last Modified: Fri, 24 Apr 2020 15:06:28 GMT  
		Size: 36.0 MB (35964328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fe4ceae85866c07c838f22f19887b72f257b543d8f8eb5710eaf0ee3f00433`  
		Last Modified: Fri, 24 Apr 2020 15:06:15 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbe79164650de57cf0ef2e48a1b75ba226937d0c9d42b4385f57069f2eba601`  
		Last Modified: Fri, 24 Apr 2020 15:06:15 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull kong@sha256:d3a8c5df99a10751a8530c129e0107be20641d4eb553dd8449d785a02760c975
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.5.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:773ad0aca96f173c1d53b88a4f82ef3104d35291e1c204c7897bee5225d4e92e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81222974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68d9d917c3ac30dc3f62aaeab3702c895a31373f03920d512c6582167259bd0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 14:00:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:01:45 GMT
ENV KONG_VERSION=1.5.1
# Fri, 24 Apr 2020 14:02:05 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong"     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb     && chown -R kong:0 /usr/local/kong     && chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:02:05 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:02:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:02:06 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:02:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:02:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f057fbda42043d24ac437698c3db2e8b61ea40da37e3b55cbf955372db8e4b7`  
		Last Modified: Fri, 24 Apr 2020 14:05:41 GMT  
		Size: 37.0 MB (36973983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36987e0504cc3722909cf5764bee765bec9c9a3341516ba79015972542f829f9`  
		Last Modified: Fri, 24 Apr 2020 14:05:34 GMT  
		Size: 310.0 B  
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
$ docker pull kong@sha256:d3a8c5df99a10751a8530c129e0107be20641d4eb553dd8449d785a02760c975
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:773ad0aca96f173c1d53b88a4f82ef3104d35291e1c204c7897bee5225d4e92e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81222974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68d9d917c3ac30dc3f62aaeab3702c895a31373f03920d512c6582167259bd0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 14:00:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:01:45 GMT
ENV KONG_VERSION=1.5.1
# Fri, 24 Apr 2020 14:02:05 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong"     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb     && chown -R kong:0 /usr/local/kong     && chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:02:05 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:02:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:02:06 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:02:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:02:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f057fbda42043d24ac437698c3db2e8b61ea40da37e3b55cbf955372db8e4b7`  
		Last Modified: Fri, 24 Apr 2020 14:05:41 GMT  
		Size: 37.0 MB (36973983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36987e0504cc3722909cf5764bee765bec9c9a3341516ba79015972542f829f9`  
		Last Modified: Fri, 24 Apr 2020 14:05:34 GMT  
		Size: 310.0 B  
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
$ docker pull kong@sha256:30f6a852c52885d5224a9a11909cd71cdf49c00c80a115e645d0dcac352e5826
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:04b888bc8fd9cfc1516f49afb1a23d9358eefa73644f93ca032b47ff8e4b9244
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94226502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db63c39030e9f1d7d4b3389835db430eaf61cde681e2e735e1ee05fa61eeea1f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 00:20:15 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:20:15 GMT
ENV ASSET=ce
# Tue, 05 May 2020 00:20:15 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Tue, 05 May 2020 00:20:15 GMT
ARG KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:20:15 GMT
ENV KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:20:52 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb &&         apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 00:20:52 GMT
COPY file:7cd3b30326ffeaddc1253699208f97fb54711d4ae930aeeeff1e19ebf51cb561 in /docker-entrypoint.sh 
# Tue, 05 May 2020 00:20:53 GMT
USER kong
# Tue, 05 May 2020 00:20:53 GMT
RUN kong version
# Tue, 05 May 2020 00:20:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 00:20:54 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 00:20:54 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 00:20:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbbe2a18126b8c44901d32f83ce9cd42aff6cae600d10916c4100151495a717`  
		Last Modified: Tue, 05 May 2020 00:23:04 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4759db0bac7c33f04375f76464db29faf6f14050dd64118ea19fac69e58955`  
		Last Modified: Tue, 05 May 2020 00:23:14 GMT  
		Size: 50.0 MB (49976972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26935d63d3595a8f0bb3c04d40c83e6bb2d9d66157dbf5fe4b13039d1eb8d424`  
		Last Modified: Tue, 05 May 2020 00:23:04 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba60a69b0762aec9563a55fec7fe8f55178757f44a352e9ba34ccb48eba23faa`  
		Last Modified: Tue, 05 May 2020 00:23:04 GMT  
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
$ docker pull kong@sha256:30f6a852c52885d5224a9a11909cd71cdf49c00c80a115e645d0dcac352e5826
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:04b888bc8fd9cfc1516f49afb1a23d9358eefa73644f93ca032b47ff8e4b9244
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94226502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db63c39030e9f1d7d4b3389835db430eaf61cde681e2e735e1ee05fa61eeea1f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 00:20:15 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:20:15 GMT
ENV ASSET=ce
# Tue, 05 May 2020 00:20:15 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Tue, 05 May 2020 00:20:15 GMT
ARG KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:20:15 GMT
ENV KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:20:52 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb &&         apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 00:20:52 GMT
COPY file:7cd3b30326ffeaddc1253699208f97fb54711d4ae930aeeeff1e19ebf51cb561 in /docker-entrypoint.sh 
# Tue, 05 May 2020 00:20:53 GMT
USER kong
# Tue, 05 May 2020 00:20:53 GMT
RUN kong version
# Tue, 05 May 2020 00:20:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 00:20:54 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 00:20:54 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 00:20:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbbe2a18126b8c44901d32f83ce9cd42aff6cae600d10916c4100151495a717`  
		Last Modified: Tue, 05 May 2020 00:23:04 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4759db0bac7c33f04375f76464db29faf6f14050dd64118ea19fac69e58955`  
		Last Modified: Tue, 05 May 2020 00:23:14 GMT  
		Size: 50.0 MB (49976972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26935d63d3595a8f0bb3c04d40c83e6bb2d9d66157dbf5fe4b13039d1eb8d424`  
		Last Modified: Tue, 05 May 2020 00:23:04 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba60a69b0762aec9563a55fec7fe8f55178757f44a352e9ba34ccb48eba23faa`  
		Last Modified: Tue, 05 May 2020 00:23:04 GMT  
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
$ docker pull kong@sha256:30f6a852c52885d5224a9a11909cd71cdf49c00c80a115e645d0dcac352e5826
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:04b888bc8fd9cfc1516f49afb1a23d9358eefa73644f93ca032b47ff8e4b9244
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94226502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db63c39030e9f1d7d4b3389835db430eaf61cde681e2e735e1ee05fa61eeea1f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 00:20:15 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:20:15 GMT
ENV ASSET=ce
# Tue, 05 May 2020 00:20:15 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Tue, 05 May 2020 00:20:15 GMT
ARG KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:20:15 GMT
ENV KONG_VERSION=2.0.4
# Tue, 05 May 2020 00:20:52 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb &&         apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 05 May 2020 00:20:52 GMT
COPY file:7cd3b30326ffeaddc1253699208f97fb54711d4ae930aeeeff1e19ebf51cb561 in /docker-entrypoint.sh 
# Tue, 05 May 2020 00:20:53 GMT
USER kong
# Tue, 05 May 2020 00:20:53 GMT
RUN kong version
# Tue, 05 May 2020 00:20:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 00:20:54 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 May 2020 00:20:54 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 May 2020 00:20:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbbe2a18126b8c44901d32f83ce9cd42aff6cae600d10916c4100151495a717`  
		Last Modified: Tue, 05 May 2020 00:23:04 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4759db0bac7c33f04375f76464db29faf6f14050dd64118ea19fac69e58955`  
		Last Modified: Tue, 05 May 2020 00:23:14 GMT  
		Size: 50.0 MB (49976972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26935d63d3595a8f0bb3c04d40c83e6bb2d9d66157dbf5fe4b13039d1eb8d424`  
		Last Modified: Tue, 05 May 2020 00:23:04 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba60a69b0762aec9563a55fec7fe8f55178757f44a352e9ba34ccb48eba23faa`  
		Last Modified: Tue, 05 May 2020 00:23:04 GMT  
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
