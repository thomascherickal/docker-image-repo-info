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
-	[`kong:2.0.1`](#kong201)
-	[`kong:2.0.1-alpine`](#kong201-alpine)
-	[`kong:2.0.1-centos`](#kong201-centos)
-	[`kong:2.0.1-ubuntu`](#kong201-ubuntu)
-	[`kong:2.0-centos`](#kong20-centos)
-	[`kong:2.0-ubuntu`](#kong20-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:centos`](#kongcentos)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:1.0`

```console
$ docker pull kong@sha256:3697c8822df2d5c8a0768c478a7132e210162a1bf1911a6acc1843ec7493612e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0` - linux; amd64

```console
$ docker pull kong@sha256:665a671d7ca1892405c07adeacbff4bb2c8388dae97af327e0a6457cecee4ace
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43705943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53f1fbbc5aeb21feda899b5f2f9f79470c70d9c008cd61b42dbadffbdaf6907`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:35:37 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Sat, 18 Jan 2020 02:35:37 GMT
ENV KONG_VERSION=1.0.4
# Sat, 18 Jan 2020 02:35:37 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Sat, 18 Jan 2020 02:35:47 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Sat, 18 Jan 2020 02:35:47 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Sat, 18 Jan 2020 02:35:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:35:47 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 18 Jan 2020 02:35:47 GMT
STOPSIGNAL SIGTERM
# Sat, 18 Jan 2020 02:35:48 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1dfebd31975deb26ec15ada908eda99b3d143de694dbd5a8cfa346acdc4358`  
		Last Modified: Sat, 18 Jan 2020 02:36:17 GMT  
		Size: 40.9 MB (40902390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349c666893cca08eaf35fd5ef34e47a55525aa053304bb95ccc6489e75549013`  
		Last Modified: Sat, 18 Jan 2020 02:36:08 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0.4`

```console
$ docker pull kong@sha256:3697c8822df2d5c8a0768c478a7132e210162a1bf1911a6acc1843ec7493612e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0.4` - linux; amd64

```console
$ docker pull kong@sha256:665a671d7ca1892405c07adeacbff4bb2c8388dae97af327e0a6457cecee4ace
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43705943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53f1fbbc5aeb21feda899b5f2f9f79470c70d9c008cd61b42dbadffbdaf6907`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:35:37 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Sat, 18 Jan 2020 02:35:37 GMT
ENV KONG_VERSION=1.0.4
# Sat, 18 Jan 2020 02:35:37 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Sat, 18 Jan 2020 02:35:47 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Sat, 18 Jan 2020 02:35:47 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Sat, 18 Jan 2020 02:35:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:35:47 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 18 Jan 2020 02:35:47 GMT
STOPSIGNAL SIGTERM
# Sat, 18 Jan 2020 02:35:48 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1dfebd31975deb26ec15ada908eda99b3d143de694dbd5a8cfa346acdc4358`  
		Last Modified: Sat, 18 Jan 2020 02:36:17 GMT  
		Size: 40.9 MB (40902390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349c666893cca08eaf35fd5ef34e47a55525aa053304bb95ccc6489e75549013`  
		Last Modified: Sat, 18 Jan 2020 02:36:08 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0.4-alpine`

```console
$ docker pull kong@sha256:3697c8822df2d5c8a0768c478a7132e210162a1bf1911a6acc1843ec7493612e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0.4-alpine` - linux; amd64

```console
$ docker pull kong@sha256:665a671d7ca1892405c07adeacbff4bb2c8388dae97af327e0a6457cecee4ace
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43705943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53f1fbbc5aeb21feda899b5f2f9f79470c70d9c008cd61b42dbadffbdaf6907`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:35:37 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Sat, 18 Jan 2020 02:35:37 GMT
ENV KONG_VERSION=1.0.4
# Sat, 18 Jan 2020 02:35:37 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Sat, 18 Jan 2020 02:35:47 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Sat, 18 Jan 2020 02:35:47 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Sat, 18 Jan 2020 02:35:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:35:47 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 18 Jan 2020 02:35:47 GMT
STOPSIGNAL SIGTERM
# Sat, 18 Jan 2020 02:35:48 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1dfebd31975deb26ec15ada908eda99b3d143de694dbd5a8cfa346acdc4358`  
		Last Modified: Sat, 18 Jan 2020 02:36:17 GMT  
		Size: 40.9 MB (40902390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349c666893cca08eaf35fd5ef34e47a55525aa053304bb95ccc6489e75549013`  
		Last Modified: Sat, 18 Jan 2020 02:36:08 GMT  
		Size: 596.0 B  
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
$ docker pull kong@sha256:22c630a308fccac656d1ac35d34a2cf26df1804348ca8851e03952f365e6c532
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1` - linux; amd64

```console
$ docker pull kong@sha256:8697bae23c49594577ba957f19c632d6f41a9b66f265370391203bacc30acdad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43989672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3792dbc151658cd798ed6abd5c79488e77a466ae976c0661e6e72abff49c6847`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:23:40 GMT
ENV KONG_VERSION=1.1.3
# Thu, 23 Jan 2020 19:23:40 GMT
ENV KONG_SHA256=834fc83540d77a0ea934ad2c7b59d7f50f9cf8750347ef0ffc572e1b508abbd4
# Thu, 23 Jan 2020 19:23:55 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:23:55 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:23:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:23:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:23:56 GMT
STOPSIGNAL SIGTERM
# Thu, 23 Jan 2020 19:23:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d5049dd39151b5c187a6941f60abf5a21cea1cc649e835db2eaf06176bbcd4`  
		Last Modified: Thu, 23 Jan 2020 19:27:57 GMT  
		Size: 41.2 MB (41202114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed205b7bc839c3be442cf36f96e471be175a2f027f1dd8e6105c70b2ab6ed79`  
		Last Modified: Thu, 23 Jan 2020 19:27:21 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.1.3`

```console
$ docker pull kong@sha256:22c630a308fccac656d1ac35d34a2cf26df1804348ca8851e03952f365e6c532
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1.3` - linux; amd64

```console
$ docker pull kong@sha256:8697bae23c49594577ba957f19c632d6f41a9b66f265370391203bacc30acdad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43989672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3792dbc151658cd798ed6abd5c79488e77a466ae976c0661e6e72abff49c6847`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:23:40 GMT
ENV KONG_VERSION=1.1.3
# Thu, 23 Jan 2020 19:23:40 GMT
ENV KONG_SHA256=834fc83540d77a0ea934ad2c7b59d7f50f9cf8750347ef0ffc572e1b508abbd4
# Thu, 23 Jan 2020 19:23:55 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:23:55 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:23:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:23:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:23:56 GMT
STOPSIGNAL SIGTERM
# Thu, 23 Jan 2020 19:23:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d5049dd39151b5c187a6941f60abf5a21cea1cc649e835db2eaf06176bbcd4`  
		Last Modified: Thu, 23 Jan 2020 19:27:57 GMT  
		Size: 41.2 MB (41202114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed205b7bc839c3be442cf36f96e471be175a2f027f1dd8e6105c70b2ab6ed79`  
		Last Modified: Thu, 23 Jan 2020 19:27:21 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.1.3-alpine`

```console
$ docker pull kong@sha256:22c630a308fccac656d1ac35d34a2cf26df1804348ca8851e03952f365e6c532
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:8697bae23c49594577ba957f19c632d6f41a9b66f265370391203bacc30acdad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43989672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3792dbc151658cd798ed6abd5c79488e77a466ae976c0661e6e72abff49c6847`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:23:40 GMT
ENV KONG_VERSION=1.1.3
# Thu, 23 Jan 2020 19:23:40 GMT
ENV KONG_SHA256=834fc83540d77a0ea934ad2c7b59d7f50f9cf8750347ef0ffc572e1b508abbd4
# Thu, 23 Jan 2020 19:23:55 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:23:55 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:23:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:23:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:23:56 GMT
STOPSIGNAL SIGTERM
# Thu, 23 Jan 2020 19:23:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d5049dd39151b5c187a6941f60abf5a21cea1cc649e835db2eaf06176bbcd4`  
		Last Modified: Thu, 23 Jan 2020 19:27:57 GMT  
		Size: 41.2 MB (41202114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed205b7bc839c3be442cf36f96e471be175a2f027f1dd8e6105c70b2ab6ed79`  
		Last Modified: Thu, 23 Jan 2020 19:27:21 GMT  
		Size: 596.0 B  
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
$ docker pull kong@sha256:f557b04074728012e858eb24fb9f6a388517a5f09e5f05aeaf07c9f045e479fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2` - linux; amd64

```console
$ docker pull kong@sha256:55f52ecd8eedf0c8b3e0d92d98e5f1f1b39fa3ab7f8d525b5fccdce801bbc27c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44478870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb957aafd7c0189d5e7642dc6be6e34f022d3473a36937cd5a4b4ce7c2fd571`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:23:10 GMT
ENV KONG_VERSION=1.2.3
# Thu, 23 Jan 2020 19:23:10 GMT
ENV KONG_SHA256=4633380fdf5cc3706f53f8697e9789b57aaf06c6bdc67d31bc0dd043453947c3
# Thu, 23 Jan 2020 19:23:28 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:23:28 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:23:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:23:29 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:23:29 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jan 2020 19:23:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831e85993e0d145e520ebfd4de1df3794997d80f06a4916fbb8556d95b35dfc0`  
		Last Modified: Thu, 23 Jan 2020 19:27:06 GMT  
		Size: 41.7 MB (41691311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef71e3bd700178431f87500b96aeb04b2752d4c4d62bbc0417ed96f814701a`  
		Last Modified: Thu, 23 Jan 2020 19:26:53 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2.3`

```console
$ docker pull kong@sha256:f557b04074728012e858eb24fb9f6a388517a5f09e5f05aeaf07c9f045e479fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2.3` - linux; amd64

```console
$ docker pull kong@sha256:55f52ecd8eedf0c8b3e0d92d98e5f1f1b39fa3ab7f8d525b5fccdce801bbc27c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44478870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb957aafd7c0189d5e7642dc6be6e34f022d3473a36937cd5a4b4ce7c2fd571`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:23:10 GMT
ENV KONG_VERSION=1.2.3
# Thu, 23 Jan 2020 19:23:10 GMT
ENV KONG_SHA256=4633380fdf5cc3706f53f8697e9789b57aaf06c6bdc67d31bc0dd043453947c3
# Thu, 23 Jan 2020 19:23:28 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:23:28 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:23:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:23:29 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:23:29 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jan 2020 19:23:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831e85993e0d145e520ebfd4de1df3794997d80f06a4916fbb8556d95b35dfc0`  
		Last Modified: Thu, 23 Jan 2020 19:27:06 GMT  
		Size: 41.7 MB (41691311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef71e3bd700178431f87500b96aeb04b2752d4c4d62bbc0417ed96f814701a`  
		Last Modified: Thu, 23 Jan 2020 19:26:53 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2.3-alpine`

```console
$ docker pull kong@sha256:f557b04074728012e858eb24fb9f6a388517a5f09e5f05aeaf07c9f045e479fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:55f52ecd8eedf0c8b3e0d92d98e5f1f1b39fa3ab7f8d525b5fccdce801bbc27c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44478870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb957aafd7c0189d5e7642dc6be6e34f022d3473a36937cd5a4b4ce7c2fd571`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:23:10 GMT
ENV KONG_VERSION=1.2.3
# Thu, 23 Jan 2020 19:23:10 GMT
ENV KONG_SHA256=4633380fdf5cc3706f53f8697e9789b57aaf06c6bdc67d31bc0dd043453947c3
# Thu, 23 Jan 2020 19:23:28 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:23:28 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:23:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:23:29 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:23:29 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jan 2020 19:23:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831e85993e0d145e520ebfd4de1df3794997d80f06a4916fbb8556d95b35dfc0`  
		Last Modified: Thu, 23 Jan 2020 19:27:06 GMT  
		Size: 41.7 MB (41691311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef71e3bd700178431f87500b96aeb04b2752d4c4d62bbc0417ed96f814701a`  
		Last Modified: Thu, 23 Jan 2020 19:26:53 GMT  
		Size: 597.0 B  
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
$ docker pull kong@sha256:7db2c2714db50c22e925bc651bf6b81029d949f7e739f0e8a97fc200e34c592c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3` - linux; amd64

```console
$ docker pull kong@sha256:ff3c8865bff15a37e206dbf3f77855be03dbb805d9caa4b3772e038ae9c1cd70
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44809669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca339f51160f9f7345c38e79703a88e3883401ead4e96eeef6db4ecaf9206120`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:22:40 GMT
ENV KONG_VERSION=1.3.1
# Thu, 23 Jan 2020 19:22:40 GMT
ENV KONG_SHA256=61754e884ab7fb62e55ca3547736e14b9b603268f05d33927c17483458c89ddc
# Thu, 23 Jan 2020 19:22:54 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:22:55 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:22:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:22:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:22:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jan 2020 19:22:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452b2ea6fa1e5a4234f26411f35bc42e5cfa8d2f7fd89f38f2d8092bd30048e3`  
		Last Modified: Thu, 23 Jan 2020 19:26:45 GMT  
		Size: 42.0 MB (42022110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fc5abd9d51cfc560f86a45bc6053369aa8f9a12c5b4bc0fe723e8df5e26dce`  
		Last Modified: Thu, 23 Jan 2020 19:26:21 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.1`

```console
$ docker pull kong@sha256:7db2c2714db50c22e925bc651bf6b81029d949f7e739f0e8a97fc200e34c592c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.1` - linux; amd64

```console
$ docker pull kong@sha256:ff3c8865bff15a37e206dbf3f77855be03dbb805d9caa4b3772e038ae9c1cd70
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44809669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca339f51160f9f7345c38e79703a88e3883401ead4e96eeef6db4ecaf9206120`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:22:40 GMT
ENV KONG_VERSION=1.3.1
# Thu, 23 Jan 2020 19:22:40 GMT
ENV KONG_SHA256=61754e884ab7fb62e55ca3547736e14b9b603268f05d33927c17483458c89ddc
# Thu, 23 Jan 2020 19:22:54 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:22:55 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:22:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:22:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:22:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jan 2020 19:22:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452b2ea6fa1e5a4234f26411f35bc42e5cfa8d2f7fd89f38f2d8092bd30048e3`  
		Last Modified: Thu, 23 Jan 2020 19:26:45 GMT  
		Size: 42.0 MB (42022110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fc5abd9d51cfc560f86a45bc6053369aa8f9a12c5b4bc0fe723e8df5e26dce`  
		Last Modified: Thu, 23 Jan 2020 19:26:21 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.1-alpine`

```console
$ docker pull kong@sha256:7db2c2714db50c22e925bc651bf6b81029d949f7e739f0e8a97fc200e34c592c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:ff3c8865bff15a37e206dbf3f77855be03dbb805d9caa4b3772e038ae9c1cd70
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44809669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca339f51160f9f7345c38e79703a88e3883401ead4e96eeef6db4ecaf9206120`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:22:40 GMT
ENV KONG_VERSION=1.3.1
# Thu, 23 Jan 2020 19:22:40 GMT
ENV KONG_SHA256=61754e884ab7fb62e55ca3547736e14b9b603268f05d33927c17483458c89ddc
# Thu, 23 Jan 2020 19:22:54 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:22:55 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:22:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:22:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:22:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jan 2020 19:22:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452b2ea6fa1e5a4234f26411f35bc42e5cfa8d2f7fd89f38f2d8092bd30048e3`  
		Last Modified: Thu, 23 Jan 2020 19:26:45 GMT  
		Size: 42.0 MB (42022110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fc5abd9d51cfc560f86a45bc6053369aa8f9a12c5b4bc0fe723e8df5e26dce`  
		Last Modified: Thu, 23 Jan 2020 19:26:21 GMT  
		Size: 597.0 B  
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
$ docker pull kong@sha256:8a307ef9ef898573528713c566d43fe5852b732347159e15126bba5ba3fe695a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:88bc72724bbf64deb8ae1fe3edad1479d973eaa3078b9386d8aed3d043041980
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81212241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3fc5340f9b41f376a90e0881699c2a99d3a7b5f0f31eaa4020b6ef901e6b745`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:58:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Sat, 22 Feb 2020 00:00:23 GMT
ENV KONG_VERSION=1.3.1
# Sat, 22 Feb 2020 00:00:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Sat, 22 Feb 2020 00:00:47 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:00:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:00:48 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 22 Feb 2020 00:00:48 GMT
STOPSIGNAL SIGQUIT
# Sat, 22 Feb 2020 00:00:48 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1205089fe8ec790807b06be4b6519d258f5ee780b50412caa1b71b8a163e25`  
		Last Modified: Sat, 22 Feb 2020 00:02:24 GMT  
		Size: 37.0 MB (37018660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1924870f928b4f7d77b2143a960c0e516ed192ceb74271e3f3eb2ec974e851`  
		Last Modified: Sat, 22 Feb 2020 00:02:15 GMT  
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
$ docker pull kong@sha256:9289c4463e35bd2d578cc61fe2ac6a2e02999d625aa6b85c34a68f281ee84b2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:88bc72724bbf64deb8ae1fe3edad1479d973eaa3078b9386d8aed3d043041980
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81212241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3fc5340f9b41f376a90e0881699c2a99d3a7b5f0f31eaa4020b6ef901e6b745`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:58:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Sat, 22 Feb 2020 00:00:23 GMT
ENV KONG_VERSION=1.3.1
# Sat, 22 Feb 2020 00:00:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Sat, 22 Feb 2020 00:00:47 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:00:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:00:48 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 22 Feb 2020 00:00:48 GMT
STOPSIGNAL SIGQUIT
# Sat, 22 Feb 2020 00:00:48 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1205089fe8ec790807b06be4b6519d258f5ee780b50412caa1b71b8a163e25`  
		Last Modified: Sat, 22 Feb 2020 00:02:24 GMT  
		Size: 37.0 MB (37018660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1924870f928b4f7d77b2143a960c0e516ed192ceb74271e3f3eb2ec974e851`  
		Last Modified: Sat, 22 Feb 2020 00:02:15 GMT  
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
$ docker pull kong@sha256:ca379f86977ee342a4e3056c2427898ebb040cb56e7ee22d6196b988d79b37b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4` - linux; amd64

```console
$ docker pull kong@sha256:bfc307e1e6ce69b8ac4e30f560005d0a9fc26427e0a44898f8892508113c229b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44115935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3341b21bcafe79da28bf06bb9400b8f3401182efab139f6faefd165a60037d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:22:08 GMT
ENV KONG_VERSION=1.4.3
# Thu, 23 Jan 2020 19:22:09 GMT
ENV KONG_SHA256=419d4e3d19f2d5c35ec6367e736b0d5509be4a7577d203008514a90f8dd5fdf1
# Thu, 23 Jan 2020 19:22:23 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:22:24 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:22:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:22:24 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:22:25 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jan 2020 19:22:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddeaace0d1ab284a481db48cbe9b36cc15b174232d415f6965b358e4b921380`  
		Last Modified: Thu, 23 Jan 2020 19:26:12 GMT  
		Size: 41.3 MB (41328375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb74c3f8fe611cc3a95c5a63bf24322e2b44ca616d30ed985bfd6546e7b002e2`  
		Last Modified: Thu, 23 Jan 2020 19:25:44 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.3`

```console
$ docker pull kong@sha256:ca379f86977ee342a4e3056c2427898ebb040cb56e7ee22d6196b988d79b37b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4.3` - linux; amd64

```console
$ docker pull kong@sha256:bfc307e1e6ce69b8ac4e30f560005d0a9fc26427e0a44898f8892508113c229b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44115935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3341b21bcafe79da28bf06bb9400b8f3401182efab139f6faefd165a60037d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:22:08 GMT
ENV KONG_VERSION=1.4.3
# Thu, 23 Jan 2020 19:22:09 GMT
ENV KONG_SHA256=419d4e3d19f2d5c35ec6367e736b0d5509be4a7577d203008514a90f8dd5fdf1
# Thu, 23 Jan 2020 19:22:23 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:22:24 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:22:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:22:24 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:22:25 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jan 2020 19:22:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddeaace0d1ab284a481db48cbe9b36cc15b174232d415f6965b358e4b921380`  
		Last Modified: Thu, 23 Jan 2020 19:26:12 GMT  
		Size: 41.3 MB (41328375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb74c3f8fe611cc3a95c5a63bf24322e2b44ca616d30ed985bfd6546e7b002e2`  
		Last Modified: Thu, 23 Jan 2020 19:25:44 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.3-alpine`

```console
$ docker pull kong@sha256:ca379f86977ee342a4e3056c2427898ebb040cb56e7ee22d6196b988d79b37b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:bfc307e1e6ce69b8ac4e30f560005d0a9fc26427e0a44898f8892508113c229b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44115935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3341b21bcafe79da28bf06bb9400b8f3401182efab139f6faefd165a60037d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 23 Jan 2020 19:22:08 GMT
ENV KONG_VERSION=1.4.3
# Thu, 23 Jan 2020 19:22:09 GMT
ENV KONG_SHA256=419d4e3d19f2d5c35ec6367e736b0d5509be4a7577d203008514a90f8dd5fdf1
# Thu, 23 Jan 2020 19:22:23 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Thu, 23 Jan 2020 19:22:24 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Thu, 23 Jan 2020 19:22:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:22:24 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 23 Jan 2020 19:22:25 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jan 2020 19:22:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddeaace0d1ab284a481db48cbe9b36cc15b174232d415f6965b358e4b921380`  
		Last Modified: Thu, 23 Jan 2020 19:26:12 GMT  
		Size: 41.3 MB (41328375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb74c3f8fe611cc3a95c5a63bf24322e2b44ca616d30ed985bfd6546e7b002e2`  
		Last Modified: Thu, 23 Jan 2020 19:25:44 GMT  
		Size: 598.0 B  
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
$ docker pull kong@sha256:91631f3c392171cafecaa7c58c72afc9e6fe0bf6a1248a503f936c55ed4a3041
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.4.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:9d67f831d06299592d1d7cf4c578f49fc5748aa412245961c221aeb266a75e18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81179136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a79c72c1333c22dfefe0d1dc93df46f2930ddd79c1d2360685a92f9fbd38952`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:58:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:59:53 GMT
ENV KONG_VERSION=1.4.3
# Sat, 22 Feb 2020 00:00:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) KONG_SHA256='d5e8debfd0c3a56a447a0613df1ebc8626eb262dc7af80ac7a5df4df329849c8' ;; 		arm64) KONG_SHA256='87f2328f40754e3ca849cdaac1883de1a0da7c780f3a4f913d5ae906e33d7dce' ;; 	esac; 	echo "$KONG_SHA256 kong.deb" | sha256sum -c - 	&& rm -rf kong.deb
# Sat, 22 Feb 2020 00:00:12 GMT
RUN kong version
# Sat, 22 Feb 2020 00:00:12 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:00:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:00:13 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 22 Feb 2020 00:00:13 GMT
STOPSIGNAL SIGQUIT
# Sat, 22 Feb 2020 00:00:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b737ad445997eedc4be0ca475eda2f08183c7867f94cbce3a3728669f682c76`  
		Last Modified: Sat, 22 Feb 2020 00:02:11 GMT  
		Size: 37.0 MB (36985462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f802555bbcfdea897eaeb5b26863594383b3211c279bf8736c076c8299314f`  
		Last Modified: Sat, 22 Feb 2020 00:02:03 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a97513120f612bb2633022ec05f2e21f78ad328f5140a511d00571d91c4619`  
		Last Modified: Sat, 22 Feb 2020 00:02:03 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.4.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:e811e2f2eecf0962630fb0381340f75f0a98186f4a61213f5bb366aa515b8795
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75906576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28dc4fd5c46d267512e4cbcd97f2bf182db435034c4d73fc452f632d519fad35`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:50:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:51:53 GMT
ENV KONG_VERSION=1.4.3
# Fri, 21 Feb 2020 23:52:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) KONG_SHA256='d5e8debfd0c3a56a447a0613df1ebc8626eb262dc7af80ac7a5df4df329849c8' ;; 		arm64) KONG_SHA256='87f2328f40754e3ca849cdaac1883de1a0da7c780f3a4f913d5ae906e33d7dce' ;; 	esac; 	echo "$KONG_SHA256 kong.deb" | sha256sum -c - 	&& rm -rf kong.deb
# Fri, 21 Feb 2020 23:52:35 GMT
RUN kong version
# Fri, 21 Feb 2020 23:52:36 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:52:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:52:37 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:52:37 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:52:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9289b1a70d3bd42d55f7af438d57921c0e86517876ccbcec63cf0f3b4d409a2c`  
		Last Modified: Fri, 21 Feb 2020 23:55:12 GMT  
		Size: 36.0 MB (35964314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339938bef74d1827135edc6fe81d3ebb9dc53b305002ad56e39191642af997ed`  
		Last Modified: Fri, 21 Feb 2020 23:54:59 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7def3bafb83306828511edbac0f033aca34f861400c76c7c9c921b5fd9587fae`  
		Last Modified: Fri, 21 Feb 2020 23:54:59 GMT  
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
$ docker pull kong@sha256:91631f3c392171cafecaa7c58c72afc9e6fe0bf6a1248a503f936c55ed4a3041
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:9d67f831d06299592d1d7cf4c578f49fc5748aa412245961c221aeb266a75e18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81179136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a79c72c1333c22dfefe0d1dc93df46f2930ddd79c1d2360685a92f9fbd38952`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:58:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:59:53 GMT
ENV KONG_VERSION=1.4.3
# Sat, 22 Feb 2020 00:00:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) KONG_SHA256='d5e8debfd0c3a56a447a0613df1ebc8626eb262dc7af80ac7a5df4df329849c8' ;; 		arm64) KONG_SHA256='87f2328f40754e3ca849cdaac1883de1a0da7c780f3a4f913d5ae906e33d7dce' ;; 	esac; 	echo "$KONG_SHA256 kong.deb" | sha256sum -c - 	&& rm -rf kong.deb
# Sat, 22 Feb 2020 00:00:12 GMT
RUN kong version
# Sat, 22 Feb 2020 00:00:12 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:00:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:00:13 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 22 Feb 2020 00:00:13 GMT
STOPSIGNAL SIGQUIT
# Sat, 22 Feb 2020 00:00:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b737ad445997eedc4be0ca475eda2f08183c7867f94cbce3a3728669f682c76`  
		Last Modified: Sat, 22 Feb 2020 00:02:11 GMT  
		Size: 37.0 MB (36985462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f802555bbcfdea897eaeb5b26863594383b3211c279bf8736c076c8299314f`  
		Last Modified: Sat, 22 Feb 2020 00:02:03 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a97513120f612bb2633022ec05f2e21f78ad328f5140a511d00571d91c4619`  
		Last Modified: Sat, 22 Feb 2020 00:02:03 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.4-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:e811e2f2eecf0962630fb0381340f75f0a98186f4a61213f5bb366aa515b8795
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75906576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28dc4fd5c46d267512e4cbcd97f2bf182db435034c4d73fc452f632d519fad35`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:50:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:51:53 GMT
ENV KONG_VERSION=1.4.3
# Fri, 21 Feb 2020 23:52:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) KONG_SHA256='d5e8debfd0c3a56a447a0613df1ebc8626eb262dc7af80ac7a5df4df329849c8' ;; 		arm64) KONG_SHA256='87f2328f40754e3ca849cdaac1883de1a0da7c780f3a4f913d5ae906e33d7dce' ;; 	esac; 	echo "$KONG_SHA256 kong.deb" | sha256sum -c - 	&& rm -rf kong.deb
# Fri, 21 Feb 2020 23:52:35 GMT
RUN kong version
# Fri, 21 Feb 2020 23:52:36 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:52:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:52:37 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:52:37 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:52:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9289b1a70d3bd42d55f7af438d57921c0e86517876ccbcec63cf0f3b4d409a2c`  
		Last Modified: Fri, 21 Feb 2020 23:55:12 GMT  
		Size: 36.0 MB (35964314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339938bef74d1827135edc6fe81d3ebb9dc53b305002ad56e39191642af997ed`  
		Last Modified: Fri, 21 Feb 2020 23:54:59 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7def3bafb83306828511edbac0f033aca34f861400c76c7c9c921b5fd9587fae`  
		Last Modified: Fri, 21 Feb 2020 23:54:59 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5`

```console
$ docker pull kong@sha256:e2b5c7759487cc0b2530548ca78c370e274fbf85191e62464daa8cb2affd5988
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5` - linux; amd64

```console
$ docker pull kong@sha256:6b8c298fff7eb83b6caac60d604681e6652ca1b311d12539f038f7f09cc7f94a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44114390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96dd46761c01c09bb2d189676ec2f24b8d4aea0f221f5cd708945589fd9b168`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 02:44:49 GMT
ENV KONG_VERSION=1.5.1
# Fri, 21 Feb 2020 02:44:49 GMT
ENV KONG_SHA256=ae31a80d82642ef485a59c832cc91beda7403617cb79384d47b5fbdb2b6f7224
# Fri, 21 Feb 2020 02:45:09 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 21 Feb 2020 02:45:09 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 02:45:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 02:45:10 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 02:45:10 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 02:45:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a878a2ff777adb87b48621dd9d9cf7fbd7e01ab426c397503ee530538f8b1e1`  
		Last Modified: Fri, 21 Feb 2020 02:48:47 GMT  
		Size: 41.3 MB (41326830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79eb1a700b1a67c63f26044616700bff5eca7368169fe32b7201352f0cf20cec`  
		Last Modified: Fri, 21 Feb 2020 02:48:34 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.1`

```console
$ docker pull kong@sha256:e2b5c7759487cc0b2530548ca78c370e274fbf85191e62464daa8cb2affd5988
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5.1` - linux; amd64

```console
$ docker pull kong@sha256:6b8c298fff7eb83b6caac60d604681e6652ca1b311d12539f038f7f09cc7f94a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44114390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96dd46761c01c09bb2d189676ec2f24b8d4aea0f221f5cd708945589fd9b168`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 02:44:49 GMT
ENV KONG_VERSION=1.5.1
# Fri, 21 Feb 2020 02:44:49 GMT
ENV KONG_SHA256=ae31a80d82642ef485a59c832cc91beda7403617cb79384d47b5fbdb2b6f7224
# Fri, 21 Feb 2020 02:45:09 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 21 Feb 2020 02:45:09 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 02:45:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 02:45:10 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 02:45:10 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 02:45:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a878a2ff777adb87b48621dd9d9cf7fbd7e01ab426c397503ee530538f8b1e1`  
		Last Modified: Fri, 21 Feb 2020 02:48:47 GMT  
		Size: 41.3 MB (41326830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79eb1a700b1a67c63f26044616700bff5eca7368169fe32b7201352f0cf20cec`  
		Last Modified: Fri, 21 Feb 2020 02:48:34 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.1-alpine`

```console
$ docker pull kong@sha256:e2b5c7759487cc0b2530548ca78c370e274fbf85191e62464daa8cb2affd5988
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:6b8c298fff7eb83b6caac60d604681e6652ca1b311d12539f038f7f09cc7f94a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44114390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96dd46761c01c09bb2d189676ec2f24b8d4aea0f221f5cd708945589fd9b168`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 02:44:49 GMT
ENV KONG_VERSION=1.5.1
# Fri, 21 Feb 2020 02:44:49 GMT
ENV KONG_SHA256=ae31a80d82642ef485a59c832cc91beda7403617cb79384d47b5fbdb2b6f7224
# Fri, 21 Feb 2020 02:45:09 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 21 Feb 2020 02:45:09 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 02:45:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 02:45:10 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 02:45:10 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 02:45:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a878a2ff777adb87b48621dd9d9cf7fbd7e01ab426c397503ee530538f8b1e1`  
		Last Modified: Fri, 21 Feb 2020 02:48:47 GMT  
		Size: 41.3 MB (41326830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79eb1a700b1a67c63f26044616700bff5eca7368169fe32b7201352f0cf20cec`  
		Last Modified: Fri, 21 Feb 2020 02:48:34 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.1-centos`

```console
$ docker pull kong@sha256:4ee566dede1aec8d4f84387d7b76456d6c60879f80c51a202488893b2b0f3de5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:ff538f3dfd86f02ac9e3e8fecdc8bdad24703476c4a0fbcf9ec92483cc60526b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151015581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efdb8e05391bc52862e24625c06b9d82a4010cd198e237b30cfd6767f946fcd4`
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
# Fri, 21 Feb 2020 02:47:12 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 02:47:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 02:47:12 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 02:47:12 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 02:47:12 GMT
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
	-	`sha256:0a6ba559ab11cb7cf71f8f7ab49ada2a0f328a6901f18a694ce64e1117a0e015`  
		Last Modified: Fri, 21 Feb 2020 02:49:11 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.1-ubuntu`

```console
$ docker pull kong@sha256:975cce0257cd10448273c3f98910a933162f78eddfb354f4fab1eedb9be01867
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.5.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:b49cebcb14e2ce93ff1c3974ed1713a8aea364d35519ea30e94526a9f8c3dbe2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81166867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce8fd5e25241e3c23230507e8df107d4f731bcf7e1fdc559ab5688b4782b306`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:58:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:59:22 GMT
ENV KONG_VERSION=1.5.1
# Fri, 21 Feb 2020 23:59:42 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Fri, 21 Feb 2020 23:59:42 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:59:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:59:42 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:59:43 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:59:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e77bd0c3028c4da2649dea196b7e34248ed4f1cfc1d0200787f3c744369798`  
		Last Modified: Sat, 22 Feb 2020 00:01:55 GMT  
		Size: 37.0 MB (36973286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b463dbcce086b938ce4254ca3265de3c84e81107fa279a0c9c12b72838fe6a0a`  
		Last Modified: Sat, 22 Feb 2020 00:01:46 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.5.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f17f1df10642539f5dd0db38d89afd7c21f0698e0f81082db415f01e58e978d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75905812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684df87808070591b5c1a73b82f7028dbc2daeceb90b8346f0572fe43b83b045`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:50:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:50:58 GMT
ENV KONG_VERSION=1.5.1
# Fri, 21 Feb 2020 23:51:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Fri, 21 Feb 2020 23:51:36 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:51:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:51:37 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:51:38 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:51:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69e918880e88bbb913efab99306c0c132117058408571d563b91f54b79fece0`  
		Last Modified: Fri, 21 Feb 2020 23:54:53 GMT  
		Size: 36.0 MB (35963642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bb05322bdecf6137333f4e46846a4ba21bb420d611b69ed8413eb1a38c1f37`  
		Last Modified: Fri, 21 Feb 2020 23:54:39 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5-centos`

```console
$ docker pull kong@sha256:4ee566dede1aec8d4f84387d7b76456d6c60879f80c51a202488893b2b0f3de5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5-centos` - linux; amd64

```console
$ docker pull kong@sha256:ff538f3dfd86f02ac9e3e8fecdc8bdad24703476c4a0fbcf9ec92483cc60526b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151015581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efdb8e05391bc52862e24625c06b9d82a4010cd198e237b30cfd6767f946fcd4`
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
# Fri, 21 Feb 2020 02:47:12 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 02:47:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 02:47:12 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 02:47:12 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 02:47:12 GMT
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
	-	`sha256:0a6ba559ab11cb7cf71f8f7ab49ada2a0f328a6901f18a694ce64e1117a0e015`  
		Last Modified: Fri, 21 Feb 2020 02:49:11 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5-ubuntu`

```console
$ docker pull kong@sha256:975cce0257cd10448273c3f98910a933162f78eddfb354f4fab1eedb9be01867
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:b49cebcb14e2ce93ff1c3974ed1713a8aea364d35519ea30e94526a9f8c3dbe2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81166867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce8fd5e25241e3c23230507e8df107d4f731bcf7e1fdc559ab5688b4782b306`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:58:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:59:22 GMT
ENV KONG_VERSION=1.5.1
# Fri, 21 Feb 2020 23:59:42 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Fri, 21 Feb 2020 23:59:42 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:59:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:59:42 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:59:43 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:59:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e77bd0c3028c4da2649dea196b7e34248ed4f1cfc1d0200787f3c744369798`  
		Last Modified: Sat, 22 Feb 2020 00:01:55 GMT  
		Size: 37.0 MB (36973286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b463dbcce086b938ce4254ca3265de3c84e81107fa279a0c9c12b72838fe6a0a`  
		Last Modified: Sat, 22 Feb 2020 00:01:46 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f17f1df10642539f5dd0db38d89afd7c21f0698e0f81082db415f01e58e978d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75905812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684df87808070591b5c1a73b82f7028dbc2daeceb90b8346f0572fe43b83b045`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:50:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:50:58 GMT
ENV KONG_VERSION=1.5.1
# Fri, 21 Feb 2020 23:51:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Fri, 21 Feb 2020 23:51:36 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:51:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:51:37 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:51:38 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:51:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69e918880e88bbb913efab99306c0c132117058408571d563b91f54b79fece0`  
		Last Modified: Fri, 21 Feb 2020 23:54:53 GMT  
		Size: 36.0 MB (35963642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bb05322bdecf6137333f4e46846a4ba21bb420d611b69ed8413eb1a38c1f37`  
		Last Modified: Fri, 21 Feb 2020 23:54:39 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0`

```console
$ docker pull kong@sha256:1993bd333fdd9863eabe3589a8342ea6f346f3ce55dce8bd4a6fbd42f659206a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0` - linux; amd64

```console
$ docker pull kong@sha256:df5f1753c7b94726eb81979b87fe6eec1ffbfe57691f37d6b05e04e12095865f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49297922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0b5d6876a0302b6b0883cf04d23f14473ce610d531376b0ce99acc68edae59`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 05 Feb 2020 23:31:52 GMT
ENV KONG_VERSION=2.0.1
# Wed, 05 Feb 2020 23:31:52 GMT
ENV KONG_SHA256=170e3f230640cef9e307fd8411287b05a1ba9162b3fc1b53417f199869dcf065
# Mon, 10 Feb 2020 23:23:40 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc
# Mon, 10 Feb 2020 23:23:41 GMT
USER kong
# Mon, 10 Feb 2020 23:23:41 GMT
COPY file:4c514f433339e8232479c5f83c4abe18fa083902b64cf695d83937fc4947437c in /docker-entrypoint.sh 
# Mon, 10 Feb 2020 23:23:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Feb 2020 23:23:41 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 10 Feb 2020 23:23:41 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Feb 2020 23:23:42 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c490acaaae4f31e0ad3ea48c9943bbbb2115a6ce613cee1eae14854ca9c77830`  
		Last Modified: Mon, 10 Feb 2020 23:26:10 GMT  
		Size: 46.5 MB (46510603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0658c893621ea7e3a94be3bde316bef8e52f49fa0f878c5d9f60bd4c438374`  
		Last Modified: Mon, 10 Feb 2020 23:26:01 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.1`

```console
$ docker pull kong@sha256:1993bd333fdd9863eabe3589a8342ea6f346f3ce55dce8bd4a6fbd42f659206a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.1` - linux; amd64

```console
$ docker pull kong@sha256:df5f1753c7b94726eb81979b87fe6eec1ffbfe57691f37d6b05e04e12095865f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49297922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0b5d6876a0302b6b0883cf04d23f14473ce610d531376b0ce99acc68edae59`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 05 Feb 2020 23:31:52 GMT
ENV KONG_VERSION=2.0.1
# Wed, 05 Feb 2020 23:31:52 GMT
ENV KONG_SHA256=170e3f230640cef9e307fd8411287b05a1ba9162b3fc1b53417f199869dcf065
# Mon, 10 Feb 2020 23:23:40 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc
# Mon, 10 Feb 2020 23:23:41 GMT
USER kong
# Mon, 10 Feb 2020 23:23:41 GMT
COPY file:4c514f433339e8232479c5f83c4abe18fa083902b64cf695d83937fc4947437c in /docker-entrypoint.sh 
# Mon, 10 Feb 2020 23:23:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Feb 2020 23:23:41 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 10 Feb 2020 23:23:41 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Feb 2020 23:23:42 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c490acaaae4f31e0ad3ea48c9943bbbb2115a6ce613cee1eae14854ca9c77830`  
		Last Modified: Mon, 10 Feb 2020 23:26:10 GMT  
		Size: 46.5 MB (46510603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0658c893621ea7e3a94be3bde316bef8e52f49fa0f878c5d9f60bd4c438374`  
		Last Modified: Mon, 10 Feb 2020 23:26:01 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.1-alpine`

```console
$ docker pull kong@sha256:1993bd333fdd9863eabe3589a8342ea6f346f3ce55dce8bd4a6fbd42f659206a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:df5f1753c7b94726eb81979b87fe6eec1ffbfe57691f37d6b05e04e12095865f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49297922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0b5d6876a0302b6b0883cf04d23f14473ce610d531376b0ce99acc68edae59`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 05 Feb 2020 23:31:52 GMT
ENV KONG_VERSION=2.0.1
# Wed, 05 Feb 2020 23:31:52 GMT
ENV KONG_SHA256=170e3f230640cef9e307fd8411287b05a1ba9162b3fc1b53417f199869dcf065
# Mon, 10 Feb 2020 23:23:40 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc
# Mon, 10 Feb 2020 23:23:41 GMT
USER kong
# Mon, 10 Feb 2020 23:23:41 GMT
COPY file:4c514f433339e8232479c5f83c4abe18fa083902b64cf695d83937fc4947437c in /docker-entrypoint.sh 
# Mon, 10 Feb 2020 23:23:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Feb 2020 23:23:41 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 10 Feb 2020 23:23:41 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Feb 2020 23:23:42 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c490acaaae4f31e0ad3ea48c9943bbbb2115a6ce613cee1eae14854ca9c77830`  
		Last Modified: Mon, 10 Feb 2020 23:26:10 GMT  
		Size: 46.5 MB (46510603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0658c893621ea7e3a94be3bde316bef8e52f49fa0f878c5d9f60bd4c438374`  
		Last Modified: Mon, 10 Feb 2020 23:26:01 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.1-centos`

```console
$ docker pull kong@sha256:571c7f5baa933668359aad9802ef048fb0c522b782333248fa2f5e07595f9d6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:d241c5143fff7f234c6b2b56980979e69b6a02a8acdd4c96a4edf70a3c6688dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158228534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7078e29bd7b317f71822cded25a54899216da7ab71126a3492314f6cba57f25a`
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
# Wed, 05 Feb 2020 23:32:40 GMT
ENV KONG_VERSION=2.0.1
# Wed, 05 Feb 2020 23:32:45 GMT
RUN yum install -y -q unzip 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Mon, 10 Feb 2020 23:24:49 GMT
RUN useradd kong 	&& mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all
# Mon, 10 Feb 2020 23:24:49 GMT
USER kong
# Mon, 10 Feb 2020 23:24:49 GMT
COPY file:4c514f433339e8232479c5f83c4abe18fa083902b64cf695d83937fc4947437c in /docker-entrypoint.sh 
# Mon, 10 Feb 2020 23:24:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Feb 2020 23:24:50 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 10 Feb 2020 23:24:50 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Feb 2020 23:24:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e0519344698532b61d589f23f1f1283696c4aea5a0bc98f0723c5804873560`  
		Last Modified: Wed, 05 Feb 2020 23:35:01 GMT  
		Size: 6.6 MB (6569287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f829582a1bcfcff29fd617e62f3b45de4821e42649777d8323c27500a82be6b`  
		Last Modified: Mon, 10 Feb 2020 23:27:29 GMT  
		Size: 75.9 MB (75878180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905d795beaef376eabf9019dbfd316fae1c2c7ec3b6793aa72ab12125f6442e6`  
		Last Modified: Mon, 10 Feb 2020 23:26:30 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.1-ubuntu`

```console
$ docker pull kong@sha256:6884b1b187f62ee9c877de29ff6bfc37712b2b55951074369770664c0b918d46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:29330b524e13be5cca2ab14111305d4ca9dba90e39daaaed6c4068ee5289b1b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.8 MB (84759132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10032c0185ac4c470fbf652a91c2789a6e2316c1a5bb2fd98c52edc7dab058f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:58:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:58:48 GMT
ENV KONG_VERSION=2.0.1
# Fri, 21 Feb 2020 23:59:08 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb
# Fri, 21 Feb 2020 23:59:09 GMT
COPY file:da5de9257b8a314f62615a4ecc2736080e316da14d00bd323efd2be62c23222d in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:59:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:59:09 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:59:09 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:59:09 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bde84fdc6c62e356ce7c83a9a99b038153653abfdc0749ea975850dbc4e4db`  
		Last Modified: Sat, 22 Feb 2020 00:01:41 GMT  
		Size: 40.6 MB (40565549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53e6f859c77fafc346d3f1522a724dbbcbc031d7efbfbd3db3aca2ebd145c80`  
		Last Modified: Sat, 22 Feb 2020 00:01:32 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:b004232c06b70ec67fa73a376be87950cf8b2795495641cdd04ad58b2bd14c99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79179962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e3f50b87ada1237fa10e0f0ca9e13c372a4f227842d7d603d24c0aef6fbbaa6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:50:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:50:03 GMT
ENV KONG_VERSION=2.0.1
# Fri, 21 Feb 2020 23:50:42 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb
# Fri, 21 Feb 2020 23:50:45 GMT
COPY file:da5de9257b8a314f62615a4ecc2736080e316da14d00bd323efd2be62c23222d in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:50:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:50:48 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:50:49 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:50:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c254c68615ac69e67f51f050f2a39cf48e4249c3513d062dc57aa5fbf166a03e`  
		Last Modified: Fri, 21 Feb 2020 23:54:32 GMT  
		Size: 39.2 MB (39237789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e154dc7a5f6ff7ce51e8c36d94402558a03d22c8b7d76e27d6adb19f0d4c75ac`  
		Last Modified: Fri, 21 Feb 2020 23:54:18 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-centos`

```console
$ docker pull kong@sha256:571c7f5baa933668359aad9802ef048fb0c522b782333248fa2f5e07595f9d6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:d241c5143fff7f234c6b2b56980979e69b6a02a8acdd4c96a4edf70a3c6688dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158228534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7078e29bd7b317f71822cded25a54899216da7ab71126a3492314f6cba57f25a`
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
# Wed, 05 Feb 2020 23:32:40 GMT
ENV KONG_VERSION=2.0.1
# Wed, 05 Feb 2020 23:32:45 GMT
RUN yum install -y -q unzip 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Mon, 10 Feb 2020 23:24:49 GMT
RUN useradd kong 	&& mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all
# Mon, 10 Feb 2020 23:24:49 GMT
USER kong
# Mon, 10 Feb 2020 23:24:49 GMT
COPY file:4c514f433339e8232479c5f83c4abe18fa083902b64cf695d83937fc4947437c in /docker-entrypoint.sh 
# Mon, 10 Feb 2020 23:24:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Feb 2020 23:24:50 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 10 Feb 2020 23:24:50 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Feb 2020 23:24:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e0519344698532b61d589f23f1f1283696c4aea5a0bc98f0723c5804873560`  
		Last Modified: Wed, 05 Feb 2020 23:35:01 GMT  
		Size: 6.6 MB (6569287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f829582a1bcfcff29fd617e62f3b45de4821e42649777d8323c27500a82be6b`  
		Last Modified: Mon, 10 Feb 2020 23:27:29 GMT  
		Size: 75.9 MB (75878180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905d795beaef376eabf9019dbfd316fae1c2c7ec3b6793aa72ab12125f6442e6`  
		Last Modified: Mon, 10 Feb 2020 23:26:30 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-ubuntu`

```console
$ docker pull kong@sha256:6884b1b187f62ee9c877de29ff6bfc37712b2b55951074369770664c0b918d46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:29330b524e13be5cca2ab14111305d4ca9dba90e39daaaed6c4068ee5289b1b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.8 MB (84759132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10032c0185ac4c470fbf652a91c2789a6e2316c1a5bb2fd98c52edc7dab058f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:58:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:58:48 GMT
ENV KONG_VERSION=2.0.1
# Fri, 21 Feb 2020 23:59:08 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb
# Fri, 21 Feb 2020 23:59:09 GMT
COPY file:da5de9257b8a314f62615a4ecc2736080e316da14d00bd323efd2be62c23222d in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:59:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:59:09 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:59:09 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:59:09 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bde84fdc6c62e356ce7c83a9a99b038153653abfdc0749ea975850dbc4e4db`  
		Last Modified: Sat, 22 Feb 2020 00:01:41 GMT  
		Size: 40.6 MB (40565549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53e6f859c77fafc346d3f1522a724dbbcbc031d7efbfbd3db3aca2ebd145c80`  
		Last Modified: Sat, 22 Feb 2020 00:01:32 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:b004232c06b70ec67fa73a376be87950cf8b2795495641cdd04ad58b2bd14c99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79179962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e3f50b87ada1237fa10e0f0ca9e13c372a4f227842d7d603d24c0aef6fbbaa6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:50:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:50:03 GMT
ENV KONG_VERSION=2.0.1
# Fri, 21 Feb 2020 23:50:42 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb
# Fri, 21 Feb 2020 23:50:45 GMT
COPY file:da5de9257b8a314f62615a4ecc2736080e316da14d00bd323efd2be62c23222d in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:50:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:50:48 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:50:49 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:50:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c254c68615ac69e67f51f050f2a39cf48e4249c3513d062dc57aa5fbf166a03e`  
		Last Modified: Fri, 21 Feb 2020 23:54:32 GMT  
		Size: 39.2 MB (39237789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e154dc7a5f6ff7ce51e8c36d94402558a03d22c8b7d76e27d6adb19f0d4c75ac`  
		Last Modified: Fri, 21 Feb 2020 23:54:18 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:1993bd333fdd9863eabe3589a8342ea6f346f3ce55dce8bd4a6fbd42f659206a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:df5f1753c7b94726eb81979b87fe6eec1ffbfe57691f37d6b05e04e12095865f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49297922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0b5d6876a0302b6b0883cf04d23f14473ce610d531376b0ce99acc68edae59`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 05 Feb 2020 23:31:52 GMT
ENV KONG_VERSION=2.0.1
# Wed, 05 Feb 2020 23:31:52 GMT
ENV KONG_SHA256=170e3f230640cef9e307fd8411287b05a1ba9162b3fc1b53417f199869dcf065
# Mon, 10 Feb 2020 23:23:40 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc
# Mon, 10 Feb 2020 23:23:41 GMT
USER kong
# Mon, 10 Feb 2020 23:23:41 GMT
COPY file:4c514f433339e8232479c5f83c4abe18fa083902b64cf695d83937fc4947437c in /docker-entrypoint.sh 
# Mon, 10 Feb 2020 23:23:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Feb 2020 23:23:41 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 10 Feb 2020 23:23:41 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Feb 2020 23:23:42 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c490acaaae4f31e0ad3ea48c9943bbbb2115a6ce613cee1eae14854ca9c77830`  
		Last Modified: Mon, 10 Feb 2020 23:26:10 GMT  
		Size: 46.5 MB (46510603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0658c893621ea7e3a94be3bde316bef8e52f49fa0f878c5d9f60bd4c438374`  
		Last Modified: Mon, 10 Feb 2020 23:26:01 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:571c7f5baa933668359aad9802ef048fb0c522b782333248fa2f5e07595f9d6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:d241c5143fff7f234c6b2b56980979e69b6a02a8acdd4c96a4edf70a3c6688dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158228534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7078e29bd7b317f71822cded25a54899216da7ab71126a3492314f6cba57f25a`
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
# Wed, 05 Feb 2020 23:32:40 GMT
ENV KONG_VERSION=2.0.1
# Wed, 05 Feb 2020 23:32:45 GMT
RUN yum install -y -q unzip 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Mon, 10 Feb 2020 23:24:49 GMT
RUN useradd kong 	&& mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all
# Mon, 10 Feb 2020 23:24:49 GMT
USER kong
# Mon, 10 Feb 2020 23:24:49 GMT
COPY file:4c514f433339e8232479c5f83c4abe18fa083902b64cf695d83937fc4947437c in /docker-entrypoint.sh 
# Mon, 10 Feb 2020 23:24:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Feb 2020 23:24:50 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 10 Feb 2020 23:24:50 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Feb 2020 23:24:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e0519344698532b61d589f23f1f1283696c4aea5a0bc98f0723c5804873560`  
		Last Modified: Wed, 05 Feb 2020 23:35:01 GMT  
		Size: 6.6 MB (6569287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f829582a1bcfcff29fd617e62f3b45de4821e42649777d8323c27500a82be6b`  
		Last Modified: Mon, 10 Feb 2020 23:27:29 GMT  
		Size: 75.9 MB (75878180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905d795beaef376eabf9019dbfd316fae1c2c7ec3b6793aa72ab12125f6442e6`  
		Last Modified: Mon, 10 Feb 2020 23:26:30 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:1993bd333fdd9863eabe3589a8342ea6f346f3ce55dce8bd4a6fbd42f659206a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:df5f1753c7b94726eb81979b87fe6eec1ffbfe57691f37d6b05e04e12095865f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49297922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0b5d6876a0302b6b0883cf04d23f14473ce610d531376b0ce99acc68edae59`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:21:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 05 Feb 2020 23:31:52 GMT
ENV KONG_VERSION=2.0.1
# Wed, 05 Feb 2020 23:31:52 GMT
ENV KONG_SHA256=170e3f230640cef9e307fd8411287b05a1ba9162b3fc1b53417f199869dcf065
# Mon, 10 Feb 2020 23:23:40 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc
# Mon, 10 Feb 2020 23:23:41 GMT
USER kong
# Mon, 10 Feb 2020 23:23:41 GMT
COPY file:4c514f433339e8232479c5f83c4abe18fa083902b64cf695d83937fc4947437c in /docker-entrypoint.sh 
# Mon, 10 Feb 2020 23:23:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Feb 2020 23:23:41 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 10 Feb 2020 23:23:41 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Feb 2020 23:23:42 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c490acaaae4f31e0ad3ea48c9943bbbb2115a6ce613cee1eae14854ca9c77830`  
		Last Modified: Mon, 10 Feb 2020 23:26:10 GMT  
		Size: 46.5 MB (46510603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0658c893621ea7e3a94be3bde316bef8e52f49fa0f878c5d9f60bd4c438374`  
		Last Modified: Mon, 10 Feb 2020 23:26:01 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:6884b1b187f62ee9c877de29ff6bfc37712b2b55951074369770664c0b918d46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:29330b524e13be5cca2ab14111305d4ca9dba90e39daaaed6c4068ee5289b1b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.8 MB (84759132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10032c0185ac4c470fbf652a91c2789a6e2316c1a5bb2fd98c52edc7dab058f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:58:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:58:48 GMT
ENV KONG_VERSION=2.0.1
# Fri, 21 Feb 2020 23:59:08 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb
# Fri, 21 Feb 2020 23:59:09 GMT
COPY file:da5de9257b8a314f62615a4ecc2736080e316da14d00bd323efd2be62c23222d in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:59:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:59:09 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:59:09 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:59:09 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bde84fdc6c62e356ce7c83a9a99b038153653abfdc0749ea975850dbc4e4db`  
		Last Modified: Sat, 22 Feb 2020 00:01:41 GMT  
		Size: 40.6 MB (40565549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53e6f859c77fafc346d3f1522a724dbbcbc031d7efbfbd3db3aca2ebd145c80`  
		Last Modified: Sat, 22 Feb 2020 00:01:32 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:b004232c06b70ec67fa73a376be87950cf8b2795495641cdd04ad58b2bd14c99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79179962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e3f50b87ada1237fa10e0f0ca9e13c372a4f227842d7d603d24c0aef6fbbaa6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:50:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:50:03 GMT
ENV KONG_VERSION=2.0.1
# Fri, 21 Feb 2020 23:50:42 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb
# Fri, 21 Feb 2020 23:50:45 GMT
COPY file:da5de9257b8a314f62615a4ecc2736080e316da14d00bd323efd2be62c23222d in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:50:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:50:48 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:50:49 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:50:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c254c68615ac69e67f51f050f2a39cf48e4249c3513d062dc57aa5fbf166a03e`  
		Last Modified: Fri, 21 Feb 2020 23:54:32 GMT  
		Size: 39.2 MB (39237789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e154dc7a5f6ff7ce51e8c36d94402558a03d22c8b7d76e27d6adb19f0d4c75ac`  
		Last Modified: Fri, 21 Feb 2020 23:54:18 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
