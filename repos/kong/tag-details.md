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
$ docker pull kong@sha256:e8b74b4b016c37e6fd05e670aa27edd0090ca5d6166220c50a2c2bc58ca24015
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0` - linux; amd64

```console
$ docker pull kong@sha256:10cb9c66f645611caec1a6c0da627715c49041aafe851a7a196535a0eb107e65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43713472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc61b1e593bd75dee2e0f69ec55447f9fe309437776ad3988849ff7d35319b04`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:04:12 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:04:13 GMT
ENV KONG_VERSION=1.0.4
# Fri, 24 Apr 2020 14:04:13 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Fri, 24 Apr 2020 14:04:25 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:04:25 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:04:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:04:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:04:26 GMT
STOPSIGNAL SIGTERM
# Fri, 24 Apr 2020 14:04:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5896e635bdb2f7c0480ffb2da79e5f0c984589fd4a9ae124b232318a35c632`  
		Last Modified: Fri, 24 Apr 2020 14:07:47 GMT  
		Size: 40.9 MB (40899558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aba3afa0845beb68987692ccaed1f44c9b5a7e14dce542df83f851d5bcb9d9`  
		Last Modified: Fri, 24 Apr 2020 14:07:39 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0.4`

```console
$ docker pull kong@sha256:e8b74b4b016c37e6fd05e670aa27edd0090ca5d6166220c50a2c2bc58ca24015
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0.4` - linux; amd64

```console
$ docker pull kong@sha256:10cb9c66f645611caec1a6c0da627715c49041aafe851a7a196535a0eb107e65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43713472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc61b1e593bd75dee2e0f69ec55447f9fe309437776ad3988849ff7d35319b04`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:04:12 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:04:13 GMT
ENV KONG_VERSION=1.0.4
# Fri, 24 Apr 2020 14:04:13 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Fri, 24 Apr 2020 14:04:25 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:04:25 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:04:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:04:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:04:26 GMT
STOPSIGNAL SIGTERM
# Fri, 24 Apr 2020 14:04:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5896e635bdb2f7c0480ffb2da79e5f0c984589fd4a9ae124b232318a35c632`  
		Last Modified: Fri, 24 Apr 2020 14:07:47 GMT  
		Size: 40.9 MB (40899558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aba3afa0845beb68987692ccaed1f44c9b5a7e14dce542df83f851d5bcb9d9`  
		Last Modified: Fri, 24 Apr 2020 14:07:39 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0.4-alpine`

```console
$ docker pull kong@sha256:e8b74b4b016c37e6fd05e670aa27edd0090ca5d6166220c50a2c2bc58ca24015
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0.4-alpine` - linux; amd64

```console
$ docker pull kong@sha256:10cb9c66f645611caec1a6c0da627715c49041aafe851a7a196535a0eb107e65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43713472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc61b1e593bd75dee2e0f69ec55447f9fe309437776ad3988849ff7d35319b04`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:04:12 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:04:13 GMT
ENV KONG_VERSION=1.0.4
# Fri, 24 Apr 2020 14:04:13 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Fri, 24 Apr 2020 14:04:25 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:04:25 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:04:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:04:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:04:26 GMT
STOPSIGNAL SIGTERM
# Fri, 24 Apr 2020 14:04:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5896e635bdb2f7c0480ffb2da79e5f0c984589fd4a9ae124b232318a35c632`  
		Last Modified: Fri, 24 Apr 2020 14:07:47 GMT  
		Size: 40.9 MB (40899558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aba3afa0845beb68987692ccaed1f44c9b5a7e14dce542df83f851d5bcb9d9`  
		Last Modified: Fri, 24 Apr 2020 14:07:39 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0.4-centos`

```console
$ docker pull kong@sha256:77e5f7773c23e470f94191b28a8b56236df7f9fa9cc9de66751cf0473bc6dc20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0.4-centos` - linux; amd64

```console
$ docker pull kong@sha256:9e6460328b9d3ae8f8bcf79fb522f13a1c842dbf9e0370f2ab082a9b40d748b2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150121223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b38ae75379b04f42504ffcb60a49b85392fec9bd01a71eed634780745438b4e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 12 Nov 2019 02:36:31 GMT
ENV KONG_VERSION=1.0.4
# Tue, 12 Nov 2019 02:36:32 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 12 Nov 2019 02:36:32 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 12 Nov 2019 02:37:08 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 12 Nov 2019 02:37:25 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 12 Nov 2019 02:37:25 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 12 Nov 2019 02:37:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Nov 2019 02:37:26 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 12 Nov 2019 02:37:26 GMT
STOPSIGNAL SIGTERM
# Tue, 12 Nov 2019 02:37:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b1c6d4b52980911e9e22741afa6a78a7878864b2fa5a27e6df89998fc4ec03`  
		Last Modified: Tue, 12 Nov 2019 02:38:58 GMT  
		Size: 6.5 MB (6513662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621c59962ec0e5d3595bd5e270fd6490a17ea12c74c89fe2188c5e07be2ddc26`  
		Last Modified: Tue, 12 Nov 2019 02:39:11 GMT  
		Size: 67.8 MB (67826253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e87031ba2eeddd34af50108b52563b396acfdf24880a73c7eec127bab6dfc9`  
		Last Modified: Tue, 12 Nov 2019 02:38:56 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0-centos`

```console
$ docker pull kong@sha256:77e5f7773c23e470f94191b28a8b56236df7f9fa9cc9de66751cf0473bc6dc20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:9e6460328b9d3ae8f8bcf79fb522f13a1c842dbf9e0370f2ab082a9b40d748b2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150121223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b38ae75379b04f42504ffcb60a49b85392fec9bd01a71eed634780745438b4e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 12 Nov 2019 02:36:31 GMT
ENV KONG_VERSION=1.0.4
# Tue, 12 Nov 2019 02:36:32 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 12 Nov 2019 02:36:32 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 12 Nov 2019 02:37:08 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 12 Nov 2019 02:37:25 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 12 Nov 2019 02:37:25 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 12 Nov 2019 02:37:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Nov 2019 02:37:26 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 12 Nov 2019 02:37:26 GMT
STOPSIGNAL SIGTERM
# Tue, 12 Nov 2019 02:37:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b1c6d4b52980911e9e22741afa6a78a7878864b2fa5a27e6df89998fc4ec03`  
		Last Modified: Tue, 12 Nov 2019 02:38:58 GMT  
		Size: 6.5 MB (6513662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621c59962ec0e5d3595bd5e270fd6490a17ea12c74c89fe2188c5e07be2ddc26`  
		Last Modified: Tue, 12 Nov 2019 02:39:11 GMT  
		Size: 67.8 MB (67826253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e87031ba2eeddd34af50108b52563b396acfdf24880a73c7eec127bab6dfc9`  
		Last Modified: Tue, 12 Nov 2019 02:38:56 GMT  
		Size: 596.0 B  
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
$ docker pull kong@sha256:dba6b7cc0893194eeee3fd0b3445681cfb6f3d3962dde24c8da50243ab5104f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1.3-centos` - linux; amd64

```console
$ docker pull kong@sha256:d9b355f7ba41e4a9c3b3c65c612ba19900baa6d3e9bccec7bbb8ef54abbeb970
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.3 MB (150321368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:308d4d4ac92a1ac8ec31550ebbfc573ffb446e83581387edff55aeb335b4e170`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 12 Nov 2019 02:35:25 GMT
ENV KONG_VERSION=1.1.3
# Tue, 12 Nov 2019 02:35:25 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 12 Nov 2019 02:35:25 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 12 Nov 2019 02:36:02 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 12 Nov 2019 02:36:18 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 12 Nov 2019 02:36:18 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 12 Nov 2019 02:36:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Nov 2019 02:36:18 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 12 Nov 2019 02:36:18 GMT
STOPSIGNAL SIGTERM
# Tue, 12 Nov 2019 02:36:19 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0e70613548fdb3460a003fd27f550f754d37c987f3ab5b000dfb963e1bdf7c`  
		Last Modified: Tue, 12 Nov 2019 02:38:40 GMT  
		Size: 6.5 MB (6513650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d091cacdcf91d22eca96fc761ee90af005c50fc83fba621e25c9edeefeef0dc0`  
		Last Modified: Tue, 12 Nov 2019 02:38:51 GMT  
		Size: 68.0 MB (68026409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f888d6299ad53b0e43827bdd8013a76650ce8189cd01a90c8fdc8dfa1f6817`  
		Last Modified: Tue, 12 Nov 2019 02:38:37 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.1-centos`

```console
$ docker pull kong@sha256:dba6b7cc0893194eeee3fd0b3445681cfb6f3d3962dde24c8da50243ab5104f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:d9b355f7ba41e4a9c3b3c65c612ba19900baa6d3e9bccec7bbb8ef54abbeb970
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.3 MB (150321368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:308d4d4ac92a1ac8ec31550ebbfc573ffb446e83581387edff55aeb335b4e170`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 12 Nov 2019 02:35:25 GMT
ENV KONG_VERSION=1.1.3
# Tue, 12 Nov 2019 02:35:25 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 12 Nov 2019 02:35:25 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 12 Nov 2019 02:36:02 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 12 Nov 2019 02:36:18 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 12 Nov 2019 02:36:18 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 12 Nov 2019 02:36:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Nov 2019 02:36:18 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 12 Nov 2019 02:36:18 GMT
STOPSIGNAL SIGTERM
# Tue, 12 Nov 2019 02:36:19 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0e70613548fdb3460a003fd27f550f754d37c987f3ab5b000dfb963e1bdf7c`  
		Last Modified: Tue, 12 Nov 2019 02:38:40 GMT  
		Size: 6.5 MB (6513650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d091cacdcf91d22eca96fc761ee90af005c50fc83fba621e25c9edeefeef0dc0`  
		Last Modified: Tue, 12 Nov 2019 02:38:51 GMT  
		Size: 68.0 MB (68026409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f888d6299ad53b0e43827bdd8013a76650ce8189cd01a90c8fdc8dfa1f6817`  
		Last Modified: Tue, 12 Nov 2019 02:38:37 GMT  
		Size: 597.0 B  
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
$ docker pull kong@sha256:35e90d094395d28a4fa21beb37c1fa7f31d5d7e2350e8ee7db86159ecea19876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2.3-centos` - linux; amd64

```console
$ docker pull kong@sha256:9fbe2dcafb4d4587ac3644caf7b0e8a12382c656575c8b0b1f483cc331e790cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150529184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4f48a350f29f77cd006fa37cb3c197a87a4da3e6ec7a3d3ce8b3927f627e5b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 01:25:22 GMT
ENV KONG_VERSION=1.2.3
# Tue, 14 Jan 2020 01:25:22 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 14 Jan 2020 01:25:22 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 14 Jan 2020 01:26:08 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 14 Jan 2020 01:26:29 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 01:26:30 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 01:26:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 01:26:30 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 01:26:31 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 01:26:31 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da74f69b2b613d1d7fdc7003ff0e60ea281bbb2d3040295d20db649b5fae130a`  
		Last Modified: Tue, 14 Jan 2020 01:28:37 GMT  
		Size: 6.5 MB (6509482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9b50a96728cd2bbc68096c87fcade81ae10f7f29df20b14a4635921d049973`  
		Last Modified: Tue, 14 Jan 2020 01:28:54 GMT  
		Size: 68.2 MB (68238395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1764843998abefc7e6097ec1a381531feb27213c68f32414758a5eb0eaf73e1c`  
		Last Modified: Tue, 14 Jan 2020 01:28:35 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2-centos`

```console
$ docker pull kong@sha256:35e90d094395d28a4fa21beb37c1fa7f31d5d7e2350e8ee7db86159ecea19876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2-centos` - linux; amd64

```console
$ docker pull kong@sha256:9fbe2dcafb4d4587ac3644caf7b0e8a12382c656575c8b0b1f483cc331e790cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150529184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4f48a350f29f77cd006fa37cb3c197a87a4da3e6ec7a3d3ce8b3927f627e5b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 01:25:22 GMT
ENV KONG_VERSION=1.2.3
# Tue, 14 Jan 2020 01:25:22 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 14 Jan 2020 01:25:22 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 14 Jan 2020 01:26:08 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 14 Jan 2020 01:26:29 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 01:26:30 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 01:26:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 01:26:30 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 01:26:31 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 01:26:31 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da74f69b2b613d1d7fdc7003ff0e60ea281bbb2d3040295d20db649b5fae130a`  
		Last Modified: Tue, 14 Jan 2020 01:28:37 GMT  
		Size: 6.5 MB (6509482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9b50a96728cd2bbc68096c87fcade81ae10f7f29df20b14a4635921d049973`  
		Last Modified: Tue, 14 Jan 2020 01:28:54 GMT  
		Size: 68.2 MB (68238395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1764843998abefc7e6097ec1a381531feb27213c68f32414758a5eb0eaf73e1c`  
		Last Modified: Tue, 14 Jan 2020 01:28:35 GMT  
		Size: 595.0 B  
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
$ docker pull kong@sha256:0ba172cdf82b54eaf7739c61db4eb0c47ae7554a506924071457cad60d6a6906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:d22db75ef9031126a6e4cbbb3cd94662072bab380c3e516b6135c4199959bd29
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151044740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8c8720ab4d79bdb907cdecd71bba23803e39a9be3fe146438ece8d202ea760`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 22:22:29 GMT
ENV KONG_VERSION=1.3.1
# Tue, 14 Jan 2020 22:22:29 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 14 Jan 2020 22:22:29 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 14 Jan 2020 22:23:05 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 14 Jan 2020 22:23:21 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 22:23:22 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 22:23:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 22:23:22 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 22:23:22 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 22:23:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02049c55e2837f3c70aead0921f1db5a4872025c607d3dc5116d1ba859b51f9`  
		Last Modified: Tue, 14 Jan 2020 22:25:16 GMT  
		Size: 6.5 MB (6509442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4d0b7a116382c5564d2c5c880c5c3d9bf7b7c5092d2fc61bec08e040fd2aa0`  
		Last Modified: Tue, 14 Jan 2020 22:25:25 GMT  
		Size: 68.8 MB (68753989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9946c97e98d93e7c75f1a69d736cca74c0ef5c84eb49e82aa05aff26fa5299b5`  
		Last Modified: Tue, 14 Jan 2020 22:25:14 GMT  
		Size: 597.0 B  
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
$ docker pull kong@sha256:0ba172cdf82b54eaf7739c61db4eb0c47ae7554a506924071457cad60d6a6906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3-centos` - linux; amd64

```console
$ docker pull kong@sha256:d22db75ef9031126a6e4cbbb3cd94662072bab380c3e516b6135c4199959bd29
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151044740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8c8720ab4d79bdb907cdecd71bba23803e39a9be3fe146438ece8d202ea760`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 22:22:29 GMT
ENV KONG_VERSION=1.3.1
# Tue, 14 Jan 2020 22:22:29 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 14 Jan 2020 22:22:29 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 14 Jan 2020 22:23:05 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 14 Jan 2020 22:23:21 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 22:23:22 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 22:23:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 22:23:22 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 22:23:22 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 22:23:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02049c55e2837f3c70aead0921f1db5a4872025c607d3dc5116d1ba859b51f9`  
		Last Modified: Tue, 14 Jan 2020 22:25:16 GMT  
		Size: 6.5 MB (6509442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4d0b7a116382c5564d2c5c880c5c3d9bf7b7c5092d2fc61bec08e040fd2aa0`  
		Last Modified: Tue, 14 Jan 2020 22:25:25 GMT  
		Size: 68.8 MB (68753989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9946c97e98d93e7c75f1a69d736cca74c0ef5c84eb49e82aa05aff26fa5299b5`  
		Last Modified: Tue, 14 Jan 2020 22:25:14 GMT  
		Size: 597.0 B  
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
$ docker pull kong@sha256:7a3d24cc151c71a3e6b21a0ce1d9abb02319310e27cba574d589fdd9bbe01b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4.3-centos` - linux; amd64

```console
$ docker pull kong@sha256:14d8790ce741f3eff735585bc0d5d9d50987c005dcf36798696d9878781ceda2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151015480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb6fd2dfc9a9bb23217d4a96a11150478cb6405b50501065a2940ea27530da8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 22:20:48 GMT
ENV KONG_VERSION=1.4.3
# Tue, 14 Jan 2020 22:20:48 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 14 Jan 2020 22:20:49 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 14 Jan 2020 22:21:30 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 14 Jan 2020 22:21:45 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 22:21:46 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 22:21:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 22:21:46 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 22:21:46 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 22:21:46 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86b7d4e4b1d66e8816a702601f75950ada5658756a23c92889be69c88f782ac`  
		Last Modified: Tue, 14 Jan 2020 22:24:33 GMT  
		Size: 6.5 MB (6509459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b25dc7b909ebc0a174d6c5b5d0649f384105961713922fd66f679805077fc9`  
		Last Modified: Tue, 14 Jan 2020 22:24:46 GMT  
		Size: 68.7 MB (68724713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61970c4ef7ea78a93c722ae1546c466f6f15e5b699170c3777dd9e5dd1e9a7c9`  
		Last Modified: Tue, 14 Jan 2020 22:24:31 GMT  
		Size: 596.0 B  
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
$ docker pull kong@sha256:7a3d24cc151c71a3e6b21a0ce1d9abb02319310e27cba574d589fdd9bbe01b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4-centos` - linux; amd64

```console
$ docker pull kong@sha256:14d8790ce741f3eff735585bc0d5d9d50987c005dcf36798696d9878781ceda2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151015480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb6fd2dfc9a9bb23217d4a96a11150478cb6405b50501065a2940ea27530da8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 22:20:48 GMT
ENV KONG_VERSION=1.4.3
# Tue, 14 Jan 2020 22:20:48 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 14 Jan 2020 22:20:49 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 14 Jan 2020 22:21:30 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 14 Jan 2020 22:21:45 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 22:21:46 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 22:21:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 22:21:46 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 22:21:46 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 22:21:46 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86b7d4e4b1d66e8816a702601f75950ada5658756a23c92889be69c88f782ac`  
		Last Modified: Tue, 14 Jan 2020 22:24:33 GMT  
		Size: 6.5 MB (6509459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b25dc7b909ebc0a174d6c5b5d0649f384105961713922fd66f679805077fc9`  
		Last Modified: Tue, 14 Jan 2020 22:24:46 GMT  
		Size: 68.7 MB (68724713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61970c4ef7ea78a93c722ae1546c466f6f15e5b699170c3777dd9e5dd1e9a7c9`  
		Last Modified: Tue, 14 Jan 2020 22:24:31 GMT  
		Size: 596.0 B  
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
$ docker pull kong@sha256:8387cf5156f9b0dd15eb8535861b87e31f430582f48734d4c4c8c44aec3e8595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:bd1baaaeb1f72e06fc5d86c3ee0d7317b62ebf66917701c2d37dc2fc148d2a20
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151015552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5270b2fe8bd4fd692070376a391bb56160b45b85e03c3a1bc1557e763caea119`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 02:46:12 GMT
ENV KONG_VERSION=1.5.1
# Fri, 21 Feb 2020 02:46:12 GMT
ARG SU_EXEC_VERSION=0.2
# Fri, 21 Feb 2020 02:46:12 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Fri, 21 Feb 2020 02:46:51 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Fri, 21 Feb 2020 02:47:11 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Sat, 28 Mar 2020 00:21:33 GMT
USER kong
# Sat, 28 Mar 2020 00:21:33 GMT
COPY file:53261f3826b37731452f0b663f02629669c2338dfa058cd1a4d6be45db56e5a6 in /docker-entrypoint.sh 
# Sat, 28 Mar 2020 00:21:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 28 Mar 2020 00:21:33 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 28 Mar 2020 00:21:33 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Mar 2020 00:21:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6292abf50ad2723c1adfe121106d3855de2bbbbb0479db36c7b4430328e89969`  
		Last Modified: Fri, 21 Feb 2020 02:49:14 GMT  
		Size: 6.5 MB (6513076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75d410a46302a1f26ae2e6618e34fafa46b445222a1a45432dd35f2c639be41`  
		Last Modified: Fri, 21 Feb 2020 02:49:28 GMT  
		Size: 68.7 MB (68721196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ed1ba07032dad4ab9891023c0c24c708d6125754501d9ea8b4cb2d8f6c8843`  
		Last Modified: Sat, 28 Mar 2020 00:22:49 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.1-ubuntu`

```console
$ docker pull kong@sha256:d8f5ea602296269c81eee45ee668b6b21db1434becd0ee217a5c2ee424453fd7
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
$ docker pull kong@sha256:52c5cd4493111f90e4b3aac1601e26b6b5be6a99f1dd7c94b3e4a27e66e59fb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75942346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f854930558de9b7c6b868545e87707b85dd16633d30ecb1b1b14cb084b3cf9`
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
# Fri, 24 Apr 2020 15:02:14 GMT
ENV KONG_VERSION=1.5.1
# Fri, 24 Apr 2020 15:02:53 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong"     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb     && chown -R kong:0 /usr/local/kong     && chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 15:02:55 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 15:02:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 15:02:56 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 15:02:57 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 15:02:57 GMT
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
	-	`sha256:2663054c3f17e59c590ef347d2cdd25a8aee8720ca29040284d560c6d9f590cd`  
		Last Modified: Fri, 24 Apr 2020 15:06:10 GMT  
		Size: 36.0 MB (35971750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe13085350e0c5d55790dee125c670e925e351bfe732bfdeaec9285514acb8f`  
		Last Modified: Fri, 24 Apr 2020 15:05:57 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5-centos`

```console
$ docker pull kong@sha256:8387cf5156f9b0dd15eb8535861b87e31f430582f48734d4c4c8c44aec3e8595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5-centos` - linux; amd64

```console
$ docker pull kong@sha256:bd1baaaeb1f72e06fc5d86c3ee0d7317b62ebf66917701c2d37dc2fc148d2a20
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151015552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5270b2fe8bd4fd692070376a391bb56160b45b85e03c3a1bc1557e763caea119`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 02:46:12 GMT
ENV KONG_VERSION=1.5.1
# Fri, 21 Feb 2020 02:46:12 GMT
ARG SU_EXEC_VERSION=0.2
# Fri, 21 Feb 2020 02:46:12 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Fri, 21 Feb 2020 02:46:51 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Fri, 21 Feb 2020 02:47:11 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Sat, 28 Mar 2020 00:21:33 GMT
USER kong
# Sat, 28 Mar 2020 00:21:33 GMT
COPY file:53261f3826b37731452f0b663f02629669c2338dfa058cd1a4d6be45db56e5a6 in /docker-entrypoint.sh 
# Sat, 28 Mar 2020 00:21:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 28 Mar 2020 00:21:33 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 28 Mar 2020 00:21:33 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Mar 2020 00:21:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6292abf50ad2723c1adfe121106d3855de2bbbbb0479db36c7b4430328e89969`  
		Last Modified: Fri, 21 Feb 2020 02:49:14 GMT  
		Size: 6.5 MB (6513076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75d410a46302a1f26ae2e6618e34fafa46b445222a1a45432dd35f2c639be41`  
		Last Modified: Fri, 21 Feb 2020 02:49:28 GMT  
		Size: 68.7 MB (68721196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ed1ba07032dad4ab9891023c0c24c708d6125754501d9ea8b4cb2d8f6c8843`  
		Last Modified: Sat, 28 Mar 2020 00:22:49 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5-ubuntu`

```console
$ docker pull kong@sha256:d8f5ea602296269c81eee45ee668b6b21db1434becd0ee217a5c2ee424453fd7
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
$ docker pull kong@sha256:52c5cd4493111f90e4b3aac1601e26b6b5be6a99f1dd7c94b3e4a27e66e59fb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75942346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f854930558de9b7c6b868545e87707b85dd16633d30ecb1b1b14cb084b3cf9`
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
# Fri, 24 Apr 2020 15:02:14 GMT
ENV KONG_VERSION=1.5.1
# Fri, 24 Apr 2020 15:02:53 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong"     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb     && chown -R kong:0 /usr/local/kong     && chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 15:02:55 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 15:02:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 15:02:56 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 15:02:57 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 15:02:57 GMT
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
	-	`sha256:2663054c3f17e59c590ef347d2cdd25a8aee8720ca29040284d560c6d9f590cd`  
		Last Modified: Fri, 24 Apr 2020 15:06:10 GMT  
		Size: 36.0 MB (35971750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe13085350e0c5d55790dee125c670e925e351bfe732bfdeaec9285514acb8f`  
		Last Modified: Fri, 24 Apr 2020 15:05:57 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0`

```console
$ docker pull kong@sha256:91090b440c2b5fc5eac5cb0be5338cc694d3916ec36ae0820e82564c8768408a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0` - linux; amd64

```console
$ docker pull kong@sha256:f011e06bcd405b709597899cfe4c4c87c2d969719aa7e069fb7606b8846bc70e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49441887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fc5f4a6339b5ab03e19928dd064599d48accad8e9d72ee49f8d47d59683e03f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:00:32 GMT
ENV KONG_VERSION=2.0.3
# Fri, 24 Apr 2020 14:00:32 GMT
ENV KONG_SHA256=db6a8ac847c347fb4d49c4763181c529bb9584187cdccdcc657ce00d605c99ac
# Fri, 24 Apr 2020 14:00:42 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:00:42 GMT
USER kong
# Fri, 24 Apr 2020 14:00:43 GMT
COPY file:d4cc11e4d968fd7df92b7b157746b27dc40d08cd20ca769e15cffc687cea9b5c in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:00:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:00:43 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:00:43 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:00:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22d7adb1f0d5fc98aab8c49b6bcfcca26cb93e8960e1abdf19a0a3bb1f95cc4`  
		Last Modified: Fri, 24 Apr 2020 14:04:59 GMT  
		Size: 46.6 MB (46645952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e622e03b921a6f2a639d5199d656b2b5c26a96dde09596479d5c19af7c7bef`  
		Last Modified: Fri, 24 Apr 2020 14:04:48 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.4`

**does not exist** (yet?)

## `kong:2.0.4-alpine`

**does not exist** (yet?)

## `kong:2.0.4-centos`

**does not exist** (yet?)

## `kong:2.0.4-ubuntu`

**does not exist** (yet?)

## `kong:2.0-centos`

```console
$ docker pull kong@sha256:cf0db57a429d75d14999631ca5ad7e8aba99074f35c8a2485c24ebccb4958904
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:043ee61b7269a392c48ed05afbda8657a732043e51555afe2ac555c5aa5b4476
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.4 MB (158442645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c21f6b284f01143bf3d326e78ffc3531ea53f2a7e5fab166077537a57896dcc6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 08 Apr 2020 21:29:04 GMT
ENV KONG_VERSION=2.0.3
# Wed, 08 Apr 2020 21:29:10 GMT
RUN yum install -y -q unzip 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Wed, 08 Apr 2020 21:29:26 GMT
RUN useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 08 Apr 2020 21:29:27 GMT
USER kong
# Wed, 08 Apr 2020 21:29:27 GMT
COPY file:d4cc11e4d968fd7df92b7b157746b27dc40d08cd20ca769e15cffc687cea9b5c in /docker-entrypoint.sh 
# Wed, 08 Apr 2020 21:29:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 08 Apr 2020 21:29:27 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 08 Apr 2020 21:29:28 GMT
STOPSIGNAL SIGQUIT
# Wed, 08 Apr 2020 21:29:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118a283d15f0b8d28c667ecaef11f9bcc20eb99542c2ac4f45189d8f715999df`  
		Last Modified: Wed, 08 Apr 2020 21:31:06 GMT  
		Size: 6.6 MB (6569066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ef44249d4c775f4d4c1c347cab01973bee052579c36db601bcbd7fa8eaba28`  
		Last Modified: Wed, 08 Apr 2020 21:31:19 GMT  
		Size: 76.1 MB (76092511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ebd767dcb9e711030da712324b59839e3602a4e6a4812d4dd4dfcf07f1ca4f`  
		Last Modified: Wed, 08 Apr 2020 21:31:04 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-ubuntu`

```console
$ docker pull kong@sha256:23cf1861b1a335ab6cb4834e42525e4ded2fd8e8ae12b36e43d1851c5444bdf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:3af4f7265c010362747ebc66fe38ea7f47d282e74d16f8c211f77767335e928d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87658876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf6f9ec4da9ba9e9cfed606337e38af60018dae39679beef3b94c8b99a1367a`
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
# Fri, 24 Apr 2020 14:00:48 GMT
ENV KONG_VERSION=2.0.3
# Fri, 24 Apr 2020 14:01:19 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Fri, 24 Apr 2020 14:01:19 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:01:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:01:20 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:01:20 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:01:20 GMT
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
	-	`sha256:c5e9dac2419c8adb8feb12ea037b6519842d75ff8c7764a6ac05ca669bf12a2a`  
		Last Modified: Fri, 24 Apr 2020 14:05:15 GMT  
		Size: 43.4 MB (43409885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6625257153606153fb694003dde07dacde024461c85e1017f5c96e21e15d523a`  
		Last Modified: Fri, 24 Apr 2020 14:05:06 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d6e10b48436ec3184bf2961e34f61f6958e67fe0b73c82e94a9712fd7fd5c5b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82086343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be75df7f0ba9985ea3490fe4410d45369842f90cbb53349d4b08172448085491`
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
# Fri, 24 Apr 2020 15:01:08 GMT
ENV KONG_VERSION=2.0.3
# Fri, 24 Apr 2020 15:01:58 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Fri, 24 Apr 2020 15:02:00 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 15:02:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 15:02:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 15:02:02 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 15:02:03 GMT
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
	-	`sha256:944df7dd3a6ed7fafa6529b4611d6364b80745a02611d67fa97b6f00cb406254`  
		Last Modified: Fri, 24 Apr 2020 15:05:49 GMT  
		Size: 42.1 MB (42115745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eed3ec499601a2baed60c11fb5b92824c4e58f480571d83a64893f1997d2a30`  
		Last Modified: Fri, 24 Apr 2020 15:05:34 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:91090b440c2b5fc5eac5cb0be5338cc694d3916ec36ae0820e82564c8768408a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:f011e06bcd405b709597899cfe4c4c87c2d969719aa7e069fb7606b8846bc70e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49441887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fc5f4a6339b5ab03e19928dd064599d48accad8e9d72ee49f8d47d59683e03f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:00:32 GMT
ENV KONG_VERSION=2.0.3
# Fri, 24 Apr 2020 14:00:32 GMT
ENV KONG_SHA256=db6a8ac847c347fb4d49c4763181c529bb9584187cdccdcc657ce00d605c99ac
# Fri, 24 Apr 2020 14:00:42 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:00:42 GMT
USER kong
# Fri, 24 Apr 2020 14:00:43 GMT
COPY file:d4cc11e4d968fd7df92b7b157746b27dc40d08cd20ca769e15cffc687cea9b5c in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:00:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:00:43 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:00:43 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:00:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22d7adb1f0d5fc98aab8c49b6bcfcca26cb93e8960e1abdf19a0a3bb1f95cc4`  
		Last Modified: Fri, 24 Apr 2020 14:04:59 GMT  
		Size: 46.6 MB (46645952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e622e03b921a6f2a639d5199d656b2b5c26a96dde09596479d5c19af7c7bef`  
		Last Modified: Fri, 24 Apr 2020 14:04:48 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:cf0db57a429d75d14999631ca5ad7e8aba99074f35c8a2485c24ebccb4958904
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:043ee61b7269a392c48ed05afbda8657a732043e51555afe2ac555c5aa5b4476
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.4 MB (158442645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c21f6b284f01143bf3d326e78ffc3531ea53f2a7e5fab166077537a57896dcc6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:32:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 08 Apr 2020 21:29:04 GMT
ENV KONG_VERSION=2.0.3
# Wed, 08 Apr 2020 21:29:10 GMT
RUN yum install -y -q unzip 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Wed, 08 Apr 2020 21:29:26 GMT
RUN useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 08 Apr 2020 21:29:27 GMT
USER kong
# Wed, 08 Apr 2020 21:29:27 GMT
COPY file:d4cc11e4d968fd7df92b7b157746b27dc40d08cd20ca769e15cffc687cea9b5c in /docker-entrypoint.sh 
# Wed, 08 Apr 2020 21:29:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 08 Apr 2020 21:29:27 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 08 Apr 2020 21:29:28 GMT
STOPSIGNAL SIGQUIT
# Wed, 08 Apr 2020 21:29:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118a283d15f0b8d28c667ecaef11f9bcc20eb99542c2ac4f45189d8f715999df`  
		Last Modified: Wed, 08 Apr 2020 21:31:06 GMT  
		Size: 6.6 MB (6569066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ef44249d4c775f4d4c1c347cab01973bee052579c36db601bcbd7fa8eaba28`  
		Last Modified: Wed, 08 Apr 2020 21:31:19 GMT  
		Size: 76.1 MB (76092511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ebd767dcb9e711030da712324b59839e3602a4e6a4812d4dd4dfcf07f1ca4f`  
		Last Modified: Wed, 08 Apr 2020 21:31:04 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:91090b440c2b5fc5eac5cb0be5338cc694d3916ec36ae0820e82564c8768408a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:f011e06bcd405b709597899cfe4c4c87c2d969719aa7e069fb7606b8846bc70e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49441887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fc5f4a6339b5ab03e19928dd064599d48accad8e9d72ee49f8d47d59683e03f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:00:32 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 24 Apr 2020 14:00:32 GMT
ENV KONG_VERSION=2.0.3
# Fri, 24 Apr 2020 14:00:32 GMT
ENV KONG_SHA256=db6a8ac847c347fb4d49c4763181c529bb9584187cdccdcc657ce00d605c99ac
# Fri, 24 Apr 2020 14:00:42 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 24 Apr 2020 14:00:42 GMT
USER kong
# Fri, 24 Apr 2020 14:00:43 GMT
COPY file:d4cc11e4d968fd7df92b7b157746b27dc40d08cd20ca769e15cffc687cea9b5c in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:00:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:00:43 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:00:43 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:00:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22d7adb1f0d5fc98aab8c49b6bcfcca26cb93e8960e1abdf19a0a3bb1f95cc4`  
		Last Modified: Fri, 24 Apr 2020 14:04:59 GMT  
		Size: 46.6 MB (46645952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e622e03b921a6f2a639d5199d656b2b5c26a96dde09596479d5c19af7c7bef`  
		Last Modified: Fri, 24 Apr 2020 14:04:48 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:23cf1861b1a335ab6cb4834e42525e4ded2fd8e8ae12b36e43d1851c5444bdf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:3af4f7265c010362747ebc66fe38ea7f47d282e74d16f8c211f77767335e928d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87658876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf6f9ec4da9ba9e9cfed606337e38af60018dae39679beef3b94c8b99a1367a`
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
# Fri, 24 Apr 2020 14:00:48 GMT
ENV KONG_VERSION=2.0.3
# Fri, 24 Apr 2020 14:01:19 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Fri, 24 Apr 2020 14:01:19 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 14:01:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 14:01:20 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 14:01:20 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 14:01:20 GMT
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
	-	`sha256:c5e9dac2419c8adb8feb12ea037b6519842d75ff8c7764a6ac05ca669bf12a2a`  
		Last Modified: Fri, 24 Apr 2020 14:05:15 GMT  
		Size: 43.4 MB (43409885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6625257153606153fb694003dde07dacde024461c85e1017f5c96e21e15d523a`  
		Last Modified: Fri, 24 Apr 2020 14:05:06 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d6e10b48436ec3184bf2961e34f61f6958e67fe0b73c82e94a9712fd7fd5c5b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82086343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be75df7f0ba9985ea3490fe4410d45369842f90cbb53349d4b08172448085491`
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
# Fri, 24 Apr 2020 15:01:08 GMT
ENV KONG_VERSION=2.0.3
# Fri, 24 Apr 2020 15:01:58 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Fri, 24 Apr 2020 15:02:00 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 24 Apr 2020 15:02:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 15:02:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Apr 2020 15:02:02 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 15:02:03 GMT
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
	-	`sha256:944df7dd3a6ed7fafa6529b4611d6364b80745a02611d67fa97b6f00cb406254`  
		Last Modified: Fri, 24 Apr 2020 15:05:49 GMT  
		Size: 42.1 MB (42115745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eed3ec499601a2baed60c11fb5b92824c4e58f480571d83a64893f1997d2a30`  
		Last Modified: Fri, 24 Apr 2020 15:05:34 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
