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
-	[`kong:1.5.0`](#kong150)
-	[`kong:1.5.0-alpine`](#kong150-alpine)
-	[`kong:1.5.0-centos`](#kong150-centos)
-	[`kong:1.5.0-ubuntu`](#kong150-ubuntu)
-	[`kong:1.5-centos`](#kong15-centos)
-	[`kong:1.5-ubuntu`](#kong15-ubuntu)
-	[`kong:2.0`](#kong20)
-	[`kong:2.0.0`](#kong200)
-	[`kong:2.0.0-alpine`](#kong200-alpine)
-	[`kong:2.0.0-centos`](#kong200-centos)
-	[`kong:2.0.0-ubuntu`](#kong200-ubuntu)
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
$ docker pull kong@sha256:04b6c1cff5115e5c9a8dee684791b0e076e886823c689a66c59fda08fa655ac3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1` - linux; amd64

```console
$ docker pull kong@sha256:9bdfbf1c6fa8d031c0c3496faff1b24b86ef2026b689466e81d69941fe147bcb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43989518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b9bb35d4a68aa5d73b5862972e9fe25c4aa4d2b771c17bd22dc1c1eb9e4eca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Mon, 21 Oct 2019 18:59:13 GMT
ENV KONG_VERSION=1.1.3
# Mon, 21 Oct 2019 18:59:13 GMT
ENV KONG_SHA256=834fc83540d77a0ea934ad2c7b59d7f50f9cf8750347ef0ffc572e1b508abbd4
# Mon, 21 Oct 2019 18:59:24 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Mon, 21 Oct 2019 18:59:25 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Mon, 21 Oct 2019 18:59:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:59:25 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 21 Oct 2019 18:59:25 GMT
STOPSIGNAL SIGTERM
# Mon, 21 Oct 2019 18:59:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a379ab2a41d409d75b1e5c57be9da44034ed37052e60145a5f2e4c2d7b498974`  
		Last Modified: Mon, 21 Oct 2019 19:01:12 GMT  
		Size: 41.2 MB (41201788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16375acceb40adebd6fbbcb3b014fe7f38fbda443e4d1ac0c2fbf0c0b5fd2acc`  
		Last Modified: Mon, 21 Oct 2019 19:00:59 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.1.3`

```console
$ docker pull kong@sha256:04b6c1cff5115e5c9a8dee684791b0e076e886823c689a66c59fda08fa655ac3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1.3` - linux; amd64

```console
$ docker pull kong@sha256:9bdfbf1c6fa8d031c0c3496faff1b24b86ef2026b689466e81d69941fe147bcb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43989518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b9bb35d4a68aa5d73b5862972e9fe25c4aa4d2b771c17bd22dc1c1eb9e4eca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Mon, 21 Oct 2019 18:59:13 GMT
ENV KONG_VERSION=1.1.3
# Mon, 21 Oct 2019 18:59:13 GMT
ENV KONG_SHA256=834fc83540d77a0ea934ad2c7b59d7f50f9cf8750347ef0ffc572e1b508abbd4
# Mon, 21 Oct 2019 18:59:24 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Mon, 21 Oct 2019 18:59:25 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Mon, 21 Oct 2019 18:59:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:59:25 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 21 Oct 2019 18:59:25 GMT
STOPSIGNAL SIGTERM
# Mon, 21 Oct 2019 18:59:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a379ab2a41d409d75b1e5c57be9da44034ed37052e60145a5f2e4c2d7b498974`  
		Last Modified: Mon, 21 Oct 2019 19:01:12 GMT  
		Size: 41.2 MB (41201788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16375acceb40adebd6fbbcb3b014fe7f38fbda443e4d1ac0c2fbf0c0b5fd2acc`  
		Last Modified: Mon, 21 Oct 2019 19:00:59 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.1.3-alpine`

```console
$ docker pull kong@sha256:04b6c1cff5115e5c9a8dee684791b0e076e886823c689a66c59fda08fa655ac3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.1.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:9bdfbf1c6fa8d031c0c3496faff1b24b86ef2026b689466e81d69941fe147bcb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43989518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b9bb35d4a68aa5d73b5862972e9fe25c4aa4d2b771c17bd22dc1c1eb9e4eca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Mon, 21 Oct 2019 18:59:13 GMT
ENV KONG_VERSION=1.1.3
# Mon, 21 Oct 2019 18:59:13 GMT
ENV KONG_SHA256=834fc83540d77a0ea934ad2c7b59d7f50f9cf8750347ef0ffc572e1b508abbd4
# Mon, 21 Oct 2019 18:59:24 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Mon, 21 Oct 2019 18:59:25 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Mon, 21 Oct 2019 18:59:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:59:25 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 21 Oct 2019 18:59:25 GMT
STOPSIGNAL SIGTERM
# Mon, 21 Oct 2019 18:59:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a379ab2a41d409d75b1e5c57be9da44034ed37052e60145a5f2e4c2d7b498974`  
		Last Modified: Mon, 21 Oct 2019 19:01:12 GMT  
		Size: 41.2 MB (41201788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16375acceb40adebd6fbbcb3b014fe7f38fbda443e4d1ac0c2fbf0c0b5fd2acc`  
		Last Modified: Mon, 21 Oct 2019 19:00:59 GMT  
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
$ docker pull kong@sha256:901f645a13623b91116449657627f4ca6388849e9e73e9ad77d926ab3f8e294e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2` - linux; amd64

```console
$ docker pull kong@sha256:d2e7dfc4e5cfb3db17a271302625a65047a1cf407b3abc1d638a5551ea35efa2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44479290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5ce71b9b43451567b55df11ed3b67b3cd066783a679180ae92068d60f83135`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 01:25:00 GMT
ENV KONG_VERSION=1.2.3
# Tue, 14 Jan 2020 01:25:01 GMT
ENV KONG_SHA256=4633380fdf5cc3706f53f8697e9789b57aaf06c6bdc67d31bc0dd043453947c3
# Tue, 14 Jan 2020 01:25:13 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 01:25:14 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 01:25:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 01:25:14 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 01:25:15 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 01:25:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de646e638f964e612ccb314e6fa8fcac3fa80dae3c3b833a6034ce5004a6b27`  
		Last Modified: Tue, 14 Jan 2020 01:28:28 GMT  
		Size: 41.7 MB (41691558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef3ec75b7225eefb0390eca4e5ba885a8e2dcf22598b152426ae37497bb2499`  
		Last Modified: Tue, 14 Jan 2020 01:28:16 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2.3`

```console
$ docker pull kong@sha256:901f645a13623b91116449657627f4ca6388849e9e73e9ad77d926ab3f8e294e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2.3` - linux; amd64

```console
$ docker pull kong@sha256:d2e7dfc4e5cfb3db17a271302625a65047a1cf407b3abc1d638a5551ea35efa2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44479290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5ce71b9b43451567b55df11ed3b67b3cd066783a679180ae92068d60f83135`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 01:25:00 GMT
ENV KONG_VERSION=1.2.3
# Tue, 14 Jan 2020 01:25:01 GMT
ENV KONG_SHA256=4633380fdf5cc3706f53f8697e9789b57aaf06c6bdc67d31bc0dd043453947c3
# Tue, 14 Jan 2020 01:25:13 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 01:25:14 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 01:25:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 01:25:14 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 01:25:15 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 01:25:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de646e638f964e612ccb314e6fa8fcac3fa80dae3c3b833a6034ce5004a6b27`  
		Last Modified: Tue, 14 Jan 2020 01:28:28 GMT  
		Size: 41.7 MB (41691558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef3ec75b7225eefb0390eca4e5ba885a8e2dcf22598b152426ae37497bb2499`  
		Last Modified: Tue, 14 Jan 2020 01:28:16 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2.3-alpine`

```console
$ docker pull kong@sha256:901f645a13623b91116449657627f4ca6388849e9e73e9ad77d926ab3f8e294e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:d2e7dfc4e5cfb3db17a271302625a65047a1cf407b3abc1d638a5551ea35efa2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44479290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5ce71b9b43451567b55df11ed3b67b3cd066783a679180ae92068d60f83135`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 01:25:00 GMT
ENV KONG_VERSION=1.2.3
# Tue, 14 Jan 2020 01:25:01 GMT
ENV KONG_SHA256=4633380fdf5cc3706f53f8697e9789b57aaf06c6bdc67d31bc0dd043453947c3
# Tue, 14 Jan 2020 01:25:13 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 01:25:14 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 01:25:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 01:25:14 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 01:25:15 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 01:25:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de646e638f964e612ccb314e6fa8fcac3fa80dae3c3b833a6034ce5004a6b27`  
		Last Modified: Tue, 14 Jan 2020 01:28:28 GMT  
		Size: 41.7 MB (41691558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef3ec75b7225eefb0390eca4e5ba885a8e2dcf22598b152426ae37497bb2499`  
		Last Modified: Tue, 14 Jan 2020 01:28:16 GMT  
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
$ docker pull kong@sha256:7898a744d66bdced75f4ea4221e7c25aebc17ded9145db0c0998844b9e19bbef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3` - linux; amd64

```console
$ docker pull kong@sha256:beea78d43416fd6d47b529772455bef04ed4642071487c62b48a1c3ef60537ae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44809656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50665dff4f01866f809d2771ac06bbd7d3892b83311fd87bbcf1b49752620a9b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 22:21:51 GMT
ENV KONG_VERSION=1.3.1
# Tue, 14 Jan 2020 22:21:51 GMT
ENV KONG_SHA256=61754e884ab7fb62e55ca3547736e14b9b603268f05d33927c17483458c89ddc
# Tue, 14 Jan 2020 22:22:00 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 22:22:00 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 22:22:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 22:22:01 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 22:22:01 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 22:22:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8aa5e7e9e3db580b18ffb5966e6793ee50f4c38f70bcf72a5e69d325aaace5`  
		Last Modified: Tue, 14 Jan 2020 22:24:59 GMT  
		Size: 42.0 MB (42021924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac4a4b3b3ab65bdce896b61447ac05d74a02d0975163db2811c9ddaf73353c`  
		Last Modified: Tue, 14 Jan 2020 22:24:51 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.1`

```console
$ docker pull kong@sha256:7898a744d66bdced75f4ea4221e7c25aebc17ded9145db0c0998844b9e19bbef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.1` - linux; amd64

```console
$ docker pull kong@sha256:beea78d43416fd6d47b529772455bef04ed4642071487c62b48a1c3ef60537ae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44809656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50665dff4f01866f809d2771ac06bbd7d3892b83311fd87bbcf1b49752620a9b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 22:21:51 GMT
ENV KONG_VERSION=1.3.1
# Tue, 14 Jan 2020 22:21:51 GMT
ENV KONG_SHA256=61754e884ab7fb62e55ca3547736e14b9b603268f05d33927c17483458c89ddc
# Tue, 14 Jan 2020 22:22:00 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 22:22:00 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 22:22:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 22:22:01 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 22:22:01 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 22:22:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8aa5e7e9e3db580b18ffb5966e6793ee50f4c38f70bcf72a5e69d325aaace5`  
		Last Modified: Tue, 14 Jan 2020 22:24:59 GMT  
		Size: 42.0 MB (42021924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac4a4b3b3ab65bdce896b61447ac05d74a02d0975163db2811c9ddaf73353c`  
		Last Modified: Tue, 14 Jan 2020 22:24:51 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.1-alpine`

```console
$ docker pull kong@sha256:7898a744d66bdced75f4ea4221e7c25aebc17ded9145db0c0998844b9e19bbef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:beea78d43416fd6d47b529772455bef04ed4642071487c62b48a1c3ef60537ae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44809656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50665dff4f01866f809d2771ac06bbd7d3892b83311fd87bbcf1b49752620a9b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 22:21:51 GMT
ENV KONG_VERSION=1.3.1
# Tue, 14 Jan 2020 22:21:51 GMT
ENV KONG_SHA256=61754e884ab7fb62e55ca3547736e14b9b603268f05d33927c17483458c89ddc
# Tue, 14 Jan 2020 22:22:00 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 22:22:00 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 22:22:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 22:22:01 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 22:22:01 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 22:22:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8aa5e7e9e3db580b18ffb5966e6793ee50f4c38f70bcf72a5e69d325aaace5`  
		Last Modified: Tue, 14 Jan 2020 22:24:59 GMT  
		Size: 42.0 MB (42021924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac4a4b3b3ab65bdce896b61447ac05d74a02d0975163db2811c9ddaf73353c`  
		Last Modified: Tue, 14 Jan 2020 22:24:51 GMT  
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
$ docker pull kong@sha256:ce73865100b97344eb5e9d5694c7d6c6d875b0e86726c89c9d44a7af197b2e44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:fc66beefadcc04bb30d8b68eb187ea673751c51db7f97b9dc34bd12e69d9b200
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81170585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d250fb1c9923fedab95d54bd55eb6e79c1091a2a6932c07e90fac6597680ff9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:58:01 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 16 Jan 2020 03:59:11 GMT
ENV KONG_VERSION=1.3.1
# Thu, 16 Jan 2020 03:59:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 16 Jan 2020 03:59:31 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 16 Jan 2020 03:59:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Jan 2020 03:59:31 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Jan 2020 03:59:32 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Jan 2020 03:59:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3abd855743ef9c5a5bd8d3f5885a6e9706b5e7cf083cf00ef79f7250885408c`  
		Last Modified: Thu, 16 Jan 2020 04:00:49 GMT  
		Size: 37.0 MB (37018970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cc1f97d6505b92a6cdf1e05879be91b1dcf4b3438036cc7c6f5a782560993e`  
		Last Modified: Thu, 16 Jan 2020 04:00:41 GMT  
		Size: 308.0 B  
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
$ docker pull kong@sha256:25c2aa3037f61f7f576c49882c205a4d8edc1003bc7a361d43f9ae38b7a3d9b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:fc66beefadcc04bb30d8b68eb187ea673751c51db7f97b9dc34bd12e69d9b200
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81170585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d250fb1c9923fedab95d54bd55eb6e79c1091a2a6932c07e90fac6597680ff9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:58:01 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 16 Jan 2020 03:59:11 GMT
ENV KONG_VERSION=1.3.1
# Thu, 16 Jan 2020 03:59:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 16 Jan 2020 03:59:31 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 16 Jan 2020 03:59:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Jan 2020 03:59:31 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Jan 2020 03:59:32 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Jan 2020 03:59:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3abd855743ef9c5a5bd8d3f5885a6e9706b5e7cf083cf00ef79f7250885408c`  
		Last Modified: Thu, 16 Jan 2020 04:00:49 GMT  
		Size: 37.0 MB (37018970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cc1f97d6505b92a6cdf1e05879be91b1dcf4b3438036cc7c6f5a782560993e`  
		Last Modified: Thu, 16 Jan 2020 04:00:41 GMT  
		Size: 308.0 B  
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
$ docker pull kong@sha256:a88c35cb8e7807966b6aaf1b41da3809b4b2c86ae50f7d036f90cb2aa747133a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4` - linux; amd64

```console
$ docker pull kong@sha256:e0740a0092bcd9fa57803ba815918f3622f6b7862c38b6c7db9e1b76bc4c4893
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44116155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047d4996f6afd73e35643ce1250fe4aa6504fa1e8e190942a0f154075af6420f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 22:20:00 GMT
ENV KONG_VERSION=1.4.3
# Tue, 14 Jan 2020 22:20:00 GMT
ENV KONG_SHA256=419d4e3d19f2d5c35ec6367e736b0d5509be4a7577d203008514a90f8dd5fdf1
# Tue, 14 Jan 2020 22:20:10 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 22:20:10 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 22:20:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 22:20:11 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 22:20:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 22:20:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efff247f0f0be1c48baef7a6084e579e819895ac650e8658328d72277d930da8`  
		Last Modified: Tue, 14 Jan 2020 22:24:14 GMT  
		Size: 41.3 MB (41328424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc63fcd4751cea13596e7526721665e012cb861f64db41cc5659c016403207c`  
		Last Modified: Tue, 14 Jan 2020 22:24:06 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.3`

```console
$ docker pull kong@sha256:a88c35cb8e7807966b6aaf1b41da3809b4b2c86ae50f7d036f90cb2aa747133a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4.3` - linux; amd64

```console
$ docker pull kong@sha256:e0740a0092bcd9fa57803ba815918f3622f6b7862c38b6c7db9e1b76bc4c4893
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44116155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047d4996f6afd73e35643ce1250fe4aa6504fa1e8e190942a0f154075af6420f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 22:20:00 GMT
ENV KONG_VERSION=1.4.3
# Tue, 14 Jan 2020 22:20:00 GMT
ENV KONG_SHA256=419d4e3d19f2d5c35ec6367e736b0d5509be4a7577d203008514a90f8dd5fdf1
# Tue, 14 Jan 2020 22:20:10 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 22:20:10 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 22:20:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 22:20:11 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 22:20:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 22:20:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efff247f0f0be1c48baef7a6084e579e819895ac650e8658328d72277d930da8`  
		Last Modified: Tue, 14 Jan 2020 22:24:14 GMT  
		Size: 41.3 MB (41328424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc63fcd4751cea13596e7526721665e012cb861f64db41cc5659c016403207c`  
		Last Modified: Tue, 14 Jan 2020 22:24:06 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.3-alpine`

```console
$ docker pull kong@sha256:a88c35cb8e7807966b6aaf1b41da3809b4b2c86ae50f7d036f90cb2aa747133a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:e0740a0092bcd9fa57803ba815918f3622f6b7862c38b6c7db9e1b76bc4c4893
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44116155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047d4996f6afd73e35643ce1250fe4aa6504fa1e8e190942a0f154075af6420f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 22:20:00 GMT
ENV KONG_VERSION=1.4.3
# Tue, 14 Jan 2020 22:20:00 GMT
ENV KONG_SHA256=419d4e3d19f2d5c35ec6367e736b0d5509be4a7577d203008514a90f8dd5fdf1
# Tue, 14 Jan 2020 22:20:10 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 22:20:10 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 22:20:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 22:20:11 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 22:20:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 22:20:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efff247f0f0be1c48baef7a6084e579e819895ac650e8658328d72277d930da8`  
		Last Modified: Tue, 14 Jan 2020 22:24:14 GMT  
		Size: 41.3 MB (41328424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc63fcd4751cea13596e7526721665e012cb861f64db41cc5659c016403207c`  
		Last Modified: Tue, 14 Jan 2020 22:24:06 GMT  
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
$ docker pull kong@sha256:10dcd2f640c3fb826e93c65751709d402aa1b5a6e8d411a8c73b01a239fa4f25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.4.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:24f292e66d7b50517c7124ac0b2c0ab1f64fc1715a77eece81c5e289595358fb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81137007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dcf1dcf7719f1f7e765f548f97c9771f4f8b584b9fa91aa6ee08b0eaf516b46`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:58:01 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 16 Jan 2020 03:58:41 GMT
ENV KONG_VERSION=1.4.3
# Thu, 16 Jan 2020 03:59:00 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 16 Jan 2020 03:59:00 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 16 Jan 2020 03:59:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Jan 2020 03:59:01 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Jan 2020 03:59:01 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Jan 2020 03:59:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf574948a848d22f35a50944eed358b29799173ab0e645b7dd53d6b2bec2a9c`  
		Last Modified: Thu, 16 Jan 2020 04:00:36 GMT  
		Size: 37.0 MB (36985392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777870d322002bfa63b5576d3506d1ad1b08aae0bb9ce60a9c8f08b484ec415c`  
		Last Modified: Thu, 16 Jan 2020 04:00:28 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.4.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:cd6d798dcc8501524178e6d941c2bf89b3761bb663e82ee4a499d1f298c548ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76220627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a5ea8dd0b3c36759c2603a6af8f93a5df1e8a197ce9a0fa43874252fc517783`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:26:42 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 16 Jan 2020 01:28:26 GMT
ENV KONG_VERSION=1.4.3
# Thu, 16 Jan 2020 01:29:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 16 Jan 2020 01:29:14 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 16 Jan 2020 01:29:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Jan 2020 01:29:16 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Jan 2020 01:29:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Jan 2020 01:29:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724c2342595ca43d29cbe4769bdf4aa42344bea10b0b2271b975d8ccbe85658a`  
		Last Modified: Thu, 16 Jan 2020 01:32:44 GMT  
		Size: 36.3 MB (36328122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb53b468a9076e898d0b200d524da2a9b40d2bce52b0f2f96c95f9fbebaeb9`  
		Last Modified: Thu, 16 Jan 2020 01:32:29 GMT  
		Size: 307.0 B  
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
$ docker pull kong@sha256:10dcd2f640c3fb826e93c65751709d402aa1b5a6e8d411a8c73b01a239fa4f25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:24f292e66d7b50517c7124ac0b2c0ab1f64fc1715a77eece81c5e289595358fb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81137007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dcf1dcf7719f1f7e765f548f97c9771f4f8b584b9fa91aa6ee08b0eaf516b46`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:58:01 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 16 Jan 2020 03:58:41 GMT
ENV KONG_VERSION=1.4.3
# Thu, 16 Jan 2020 03:59:00 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 16 Jan 2020 03:59:00 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 16 Jan 2020 03:59:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Jan 2020 03:59:01 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Jan 2020 03:59:01 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Jan 2020 03:59:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf574948a848d22f35a50944eed358b29799173ab0e645b7dd53d6b2bec2a9c`  
		Last Modified: Thu, 16 Jan 2020 04:00:36 GMT  
		Size: 37.0 MB (36985392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777870d322002bfa63b5576d3506d1ad1b08aae0bb9ce60a9c8f08b484ec415c`  
		Last Modified: Thu, 16 Jan 2020 04:00:28 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.4-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:cd6d798dcc8501524178e6d941c2bf89b3761bb663e82ee4a499d1f298c548ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76220627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a5ea8dd0b3c36759c2603a6af8f93a5df1e8a197ce9a0fa43874252fc517783`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:26:42 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 16 Jan 2020 01:28:26 GMT
ENV KONG_VERSION=1.4.3
# Thu, 16 Jan 2020 01:29:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 16 Jan 2020 01:29:14 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 16 Jan 2020 01:29:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Jan 2020 01:29:16 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Jan 2020 01:29:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Jan 2020 01:29:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724c2342595ca43d29cbe4769bdf4aa42344bea10b0b2271b975d8ccbe85658a`  
		Last Modified: Thu, 16 Jan 2020 01:32:44 GMT  
		Size: 36.3 MB (36328122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb53b468a9076e898d0b200d524da2a9b40d2bce52b0f2f96c95f9fbebaeb9`  
		Last Modified: Thu, 16 Jan 2020 01:32:29 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5`

```console
$ docker pull kong@sha256:985176eb68d4892f0e8314ae07be8f338c910a47211832635b7eb56754104a57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5` - linux; amd64

```console
$ docker pull kong@sha256:3c14ac08fd523ad5d3e99c4e51b4c8ee4c6d744bcffe5a0bbfaf6d4fee49a180
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44119155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f1a2d103c34b44e942f410e9138e6d1816b650f56760be681b91fa6c37f2a51`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 05:16:58 GMT
ENV KONG_VERSION=1.5.0
# Wed, 22 Jan 2020 05:16:58 GMT
ENV KONG_SHA256=74f4fe05b39bc3108611e9c52cb1faa788002e33551d3ab6ca0ec6ccfeeae2bd
# Wed, 22 Jan 2020 05:17:09 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 22 Jan 2020 05:17:09 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:17:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:17:09 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:17:09 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:17:10 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c1901f2a9a5dfd200e3c6770f8dc1fc7c6080ee361406ea8416fba2a4bb458`  
		Last Modified: Wed, 22 Jan 2020 05:20:39 GMT  
		Size: 41.3 MB (41331424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533a707b9f3feeb19d936ddd0f58849bb40b484003cb961fcaa7a05063452215`  
		Last Modified: Wed, 22 Jan 2020 05:20:29 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.0`

```console
$ docker pull kong@sha256:985176eb68d4892f0e8314ae07be8f338c910a47211832635b7eb56754104a57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5.0` - linux; amd64

```console
$ docker pull kong@sha256:3c14ac08fd523ad5d3e99c4e51b4c8ee4c6d744bcffe5a0bbfaf6d4fee49a180
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44119155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f1a2d103c34b44e942f410e9138e6d1816b650f56760be681b91fa6c37f2a51`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 05:16:58 GMT
ENV KONG_VERSION=1.5.0
# Wed, 22 Jan 2020 05:16:58 GMT
ENV KONG_SHA256=74f4fe05b39bc3108611e9c52cb1faa788002e33551d3ab6ca0ec6ccfeeae2bd
# Wed, 22 Jan 2020 05:17:09 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 22 Jan 2020 05:17:09 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:17:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:17:09 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:17:09 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:17:10 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c1901f2a9a5dfd200e3c6770f8dc1fc7c6080ee361406ea8416fba2a4bb458`  
		Last Modified: Wed, 22 Jan 2020 05:20:39 GMT  
		Size: 41.3 MB (41331424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533a707b9f3feeb19d936ddd0f58849bb40b484003cb961fcaa7a05063452215`  
		Last Modified: Wed, 22 Jan 2020 05:20:29 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.0-alpine`

```console
$ docker pull kong@sha256:985176eb68d4892f0e8314ae07be8f338c910a47211832635b7eb56754104a57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:3c14ac08fd523ad5d3e99c4e51b4c8ee4c6d744bcffe5a0bbfaf6d4fee49a180
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44119155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f1a2d103c34b44e942f410e9138e6d1816b650f56760be681b91fa6c37f2a51`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 05:16:58 GMT
ENV KONG_VERSION=1.5.0
# Wed, 22 Jan 2020 05:16:58 GMT
ENV KONG_SHA256=74f4fe05b39bc3108611e9c52cb1faa788002e33551d3ab6ca0ec6ccfeeae2bd
# Wed, 22 Jan 2020 05:17:09 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 22 Jan 2020 05:17:09 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:17:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:17:09 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:17:09 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:17:10 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c1901f2a9a5dfd200e3c6770f8dc1fc7c6080ee361406ea8416fba2a4bb458`  
		Last Modified: Wed, 22 Jan 2020 05:20:39 GMT  
		Size: 41.3 MB (41331424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533a707b9f3feeb19d936ddd0f58849bb40b484003cb961fcaa7a05063452215`  
		Last Modified: Wed, 22 Jan 2020 05:20:29 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.0-centos`

```console
$ docker pull kong@sha256:dca2703b0134640320ed8464a20803ed62b07e5b9af859b5f1cc2a70ad36a163
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:03ac70dad278568c00cbb265562f38fcd906d8086f77cdbc818b1fb1816e8e87
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151027842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:746ef0a7e8c2c6342f5e6b5745d9a3f0e6e25298ec3e546bddca41c42ceb3211`
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
# Wed, 22 Jan 2020 05:17:42 GMT
ENV KONG_VERSION=1.5.0
# Wed, 22 Jan 2020 05:17:42 GMT
ARG SU_EXEC_VERSION=0.2
# Wed, 22 Jan 2020 05:17:42 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Wed, 22 Jan 2020 05:18:20 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Wed, 22 Jan 2020 05:18:34 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 22 Jan 2020 05:18:35 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:18:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:18:35 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:18:35 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:18:35 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00283608292bb51ac66eca2a29fab0ca3760295113900eb08c51682006be364`  
		Last Modified: Wed, 22 Jan 2020 05:20:59 GMT  
		Size: 6.5 MB (6509460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25523276f8b222882c040bb9adee509a97cc57a616d250dc217ebce8098e0dac`  
		Last Modified: Wed, 22 Jan 2020 05:21:11 GMT  
		Size: 68.7 MB (68737074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9543bff8097bf8d706797b30113a7e4c519c201d8cb6417b1f0d6bcb3214df`  
		Last Modified: Wed, 22 Jan 2020 05:20:57 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5.0-ubuntu`

```console
$ docker pull kong@sha256:a63a4620f786731d16e64be13be8d16f79ebe54ad5457cee8bb2ad6ea87bb9ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.5.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e361acf5371878ae2e2cc1cb8ca362b93d5441aa39fb15eab0537ae2fa4157f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80528399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bcbeb6085027cd94d33f10f88aef93092b92d0557074825809c37a25bbe6f08`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:58:01 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 05:17:14 GMT
ENV KONG_VERSION=1.5.0
# Wed, 22 Jan 2020 05:17:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Wed, 22 Jan 2020 05:17:34 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:17:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:17:34 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:17:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:17:35 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b575cc0de6ffd40592d0acbb354adc1e094619a4de5bb3fd6675baf590b508c3`  
		Last Modified: Wed, 22 Jan 2020 05:20:53 GMT  
		Size: 36.4 MB (36376783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2a99d6dc61b5983e95e7145dda5056e9712fa1c3a63e953263eae7db06273e`  
		Last Modified: Wed, 22 Jan 2020 05:20:44 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.5.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:b7da00b560a125e860bb4c4fcefc66a4fc9c5720453729cf058c96004b6200b9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75284910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e85129bb60584b5da4011d9bd88ba8ee2e8c50032179320a912d12d4f0f8d04`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:26:42 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 02:59:54 GMT
ENV KONG_VERSION=1.5.0
# Wed, 22 Jan 2020 03:00:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Wed, 22 Jan 2020 03:00:33 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 03:00:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 03:00:34 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 03:00:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 03:00:35 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d9f4723092434f05a0dee0175f5571515d1b87d73dd492a653e04a74b1716d`  
		Last Modified: Wed, 22 Jan 2020 03:03:07 GMT  
		Size: 35.4 MB (35392404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be265a7ffc81e85a6656e8a38ea95d7be7f6025da6ba3229b7e016eaea60f720`  
		Last Modified: Wed, 22 Jan 2020 03:02:53 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5-centos`

```console
$ docker pull kong@sha256:dca2703b0134640320ed8464a20803ed62b07e5b9af859b5f1cc2a70ad36a163
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.5-centos` - linux; amd64

```console
$ docker pull kong@sha256:03ac70dad278568c00cbb265562f38fcd906d8086f77cdbc818b1fb1816e8e87
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151027842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:746ef0a7e8c2c6342f5e6b5745d9a3f0e6e25298ec3e546bddca41c42ceb3211`
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
# Wed, 22 Jan 2020 05:17:42 GMT
ENV KONG_VERSION=1.5.0
# Wed, 22 Jan 2020 05:17:42 GMT
ARG SU_EXEC_VERSION=0.2
# Wed, 22 Jan 2020 05:17:42 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Wed, 22 Jan 2020 05:18:20 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Wed, 22 Jan 2020 05:18:34 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 22 Jan 2020 05:18:35 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:18:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:18:35 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:18:35 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:18:35 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00283608292bb51ac66eca2a29fab0ca3760295113900eb08c51682006be364`  
		Last Modified: Wed, 22 Jan 2020 05:20:59 GMT  
		Size: 6.5 MB (6509460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25523276f8b222882c040bb9adee509a97cc57a616d250dc217ebce8098e0dac`  
		Last Modified: Wed, 22 Jan 2020 05:21:11 GMT  
		Size: 68.7 MB (68737074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9543bff8097bf8d706797b30113a7e4c519c201d8cb6417b1f0d6bcb3214df`  
		Last Modified: Wed, 22 Jan 2020 05:20:57 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.5-ubuntu`

```console
$ docker pull kong@sha256:a63a4620f786731d16e64be13be8d16f79ebe54ad5457cee8bb2ad6ea87bb9ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e361acf5371878ae2e2cc1cb8ca362b93d5441aa39fb15eab0537ae2fa4157f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80528399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bcbeb6085027cd94d33f10f88aef93092b92d0557074825809c37a25bbe6f08`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:58:01 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 05:17:14 GMT
ENV KONG_VERSION=1.5.0
# Wed, 22 Jan 2020 05:17:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Wed, 22 Jan 2020 05:17:34 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:17:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:17:34 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:17:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:17:35 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b575cc0de6ffd40592d0acbb354adc1e094619a4de5bb3fd6675baf590b508c3`  
		Last Modified: Wed, 22 Jan 2020 05:20:53 GMT  
		Size: 36.4 MB (36376783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2a99d6dc61b5983e95e7145dda5056e9712fa1c3a63e953263eae7db06273e`  
		Last Modified: Wed, 22 Jan 2020 05:20:44 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:b7da00b560a125e860bb4c4fcefc66a4fc9c5720453729cf058c96004b6200b9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75284910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e85129bb60584b5da4011d9bd88ba8ee2e8c50032179320a912d12d4f0f8d04`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:26:42 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 02:59:54 GMT
ENV KONG_VERSION=1.5.0
# Wed, 22 Jan 2020 03:00:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Wed, 22 Jan 2020 03:00:33 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 03:00:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 03:00:34 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 03:00:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 03:00:35 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d9f4723092434f05a0dee0175f5571515d1b87d73dd492a653e04a74b1716d`  
		Last Modified: Wed, 22 Jan 2020 03:03:07 GMT  
		Size: 35.4 MB (35392404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be265a7ffc81e85a6656e8a38ea95d7be7f6025da6ba3229b7e016eaea60f720`  
		Last Modified: Wed, 22 Jan 2020 03:02:53 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0`

```console
$ docker pull kong@sha256:9c630fcc43b8d30af115ded3221b85d4f9303f07a26be89586ce868be4d461d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0` - linux; amd64

```console
$ docker pull kong@sha256:28378817cc5df4fc77fb9e600a7fe54c4d37abc66b82989b61b8a77661dd14a8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49283901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b33f8116962ae37ebd9626c4342b20e377adc2f1b14f683ba93817a3cf7dc0fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 05:15:18 GMT
ENV KONG_VERSION=2.0.0
# Wed, 22 Jan 2020 05:15:18 GMT
ENV KONG_SHA256=5af1178111958b2e325c5b18690f4e7ddf064d28139ff38188b1e2e432ea99ff
# Wed, 22 Jan 2020 05:15:27 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 22 Jan 2020 05:15:27 GMT
USER kong
# Wed, 22 Jan 2020 05:15:27 GMT
COPY file:d4cc11e4d968fd7df92b7b157746b27dc40d08cd20ca769e15cffc687cea9b5c in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:15:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:15:28 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:15:28 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:15:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4dc4b9dfde879379bef6ef7826fc166ebccbd14b77c10cb51a3dd8c9f4f015`  
		Last Modified: Wed, 22 Jan 2020 05:19:50 GMT  
		Size: 46.5 MB (46496411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1bc1d108f206400e74912aabc759a8cca9c5d8ec1647fb3fa52f93147ec69a`  
		Last Modified: Wed, 22 Jan 2020 05:19:40 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.0`

```console
$ docker pull kong@sha256:9c630fcc43b8d30af115ded3221b85d4f9303f07a26be89586ce868be4d461d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.0` - linux; amd64

```console
$ docker pull kong@sha256:28378817cc5df4fc77fb9e600a7fe54c4d37abc66b82989b61b8a77661dd14a8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49283901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b33f8116962ae37ebd9626c4342b20e377adc2f1b14f683ba93817a3cf7dc0fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 05:15:18 GMT
ENV KONG_VERSION=2.0.0
# Wed, 22 Jan 2020 05:15:18 GMT
ENV KONG_SHA256=5af1178111958b2e325c5b18690f4e7ddf064d28139ff38188b1e2e432ea99ff
# Wed, 22 Jan 2020 05:15:27 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 22 Jan 2020 05:15:27 GMT
USER kong
# Wed, 22 Jan 2020 05:15:27 GMT
COPY file:d4cc11e4d968fd7df92b7b157746b27dc40d08cd20ca769e15cffc687cea9b5c in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:15:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:15:28 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:15:28 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:15:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4dc4b9dfde879379bef6ef7826fc166ebccbd14b77c10cb51a3dd8c9f4f015`  
		Last Modified: Wed, 22 Jan 2020 05:19:50 GMT  
		Size: 46.5 MB (46496411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1bc1d108f206400e74912aabc759a8cca9c5d8ec1647fb3fa52f93147ec69a`  
		Last Modified: Wed, 22 Jan 2020 05:19:40 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.0-alpine`

```console
$ docker pull kong@sha256:9c630fcc43b8d30af115ded3221b85d4f9303f07a26be89586ce868be4d461d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:28378817cc5df4fc77fb9e600a7fe54c4d37abc66b82989b61b8a77661dd14a8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49283901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b33f8116962ae37ebd9626c4342b20e377adc2f1b14f683ba93817a3cf7dc0fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 05:15:18 GMT
ENV KONG_VERSION=2.0.0
# Wed, 22 Jan 2020 05:15:18 GMT
ENV KONG_SHA256=5af1178111958b2e325c5b18690f4e7ddf064d28139ff38188b1e2e432ea99ff
# Wed, 22 Jan 2020 05:15:27 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 22 Jan 2020 05:15:27 GMT
USER kong
# Wed, 22 Jan 2020 05:15:27 GMT
COPY file:d4cc11e4d968fd7df92b7b157746b27dc40d08cd20ca769e15cffc687cea9b5c in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:15:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:15:28 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:15:28 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:15:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4dc4b9dfde879379bef6ef7826fc166ebccbd14b77c10cb51a3dd8c9f4f015`  
		Last Modified: Wed, 22 Jan 2020 05:19:50 GMT  
		Size: 46.5 MB (46496411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1bc1d108f206400e74912aabc759a8cca9c5d8ec1647fb3fa52f93147ec69a`  
		Last Modified: Wed, 22 Jan 2020 05:19:40 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.0-centos`

```console
$ docker pull kong@sha256:94f9efc544e95c4272994b288ab4705cac33101e091d6f0be4ec8b55a4109b4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:c8fa4ff0c035afa30e80eb1ab56066876fadee72ab926442060cdf853f14c803
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158205282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b68221ae244e42b58e051b3d0ca18008663b288f29bfd5b7e2d0979d892b6384`
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
# Wed, 22 Jan 2020 05:16:25 GMT
ENV KONG_VERSION=2.0.0
# Wed, 22 Jan 2020 05:16:31 GMT
RUN yum install -y -q unzip 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Wed, 22 Jan 2020 05:16:52 GMT
RUN useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 22 Jan 2020 05:16:52 GMT
USER kong
# Wed, 22 Jan 2020 05:16:52 GMT
COPY file:d4cc11e4d968fd7df92b7b157746b27dc40d08cd20ca769e15cffc687cea9b5c in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:16:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:16:53 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:16:53 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:16:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33393acb164820849236d8a316b267340d8ea03502e0bfb9c760a92740ec4b52`  
		Last Modified: Wed, 22 Jan 2020 05:20:12 GMT  
		Size: 6.6 MB (6569271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd358c1ff903f4b77bbf06d91d9532da73bddee5e4d6971ea438149eea106faf`  
		Last Modified: Wed, 22 Jan 2020 05:20:25 GMT  
		Size: 75.9 MB (75854944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2637114431d722670a4c3246ab50aba0bbac9c51f6bceccd8b19f1eed6310417`  
		Last Modified: Wed, 22 Jan 2020 05:20:10 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.0-ubuntu`

```console
$ docker pull kong@sha256:eebd00092815a0cddf223d4629392a68e199460dbe8efe46cbd01e3688782fcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:5b650d206b1d925d17d3015bd44b0a8851fdc8ae8d55801baeb15ddc2c0d5fd5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.7 MB (84698909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8899060e4ff76086e4dd26b4cbbb331b467d41bc38823ecfc361430d41b0cf20`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:58:01 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 05:15:32 GMT
ENV KONG_VERSION=2.0.0
# Wed, 22 Jan 2020 05:16:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Wed, 22 Jan 2020 05:16:15 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:16:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:16:15 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:16:15 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:16:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb016521f3fdb1c7ac1744d0c7d50371d9ce2b75c20d917576453cfe6330898e`  
		Last Modified: Wed, 22 Jan 2020 05:20:05 GMT  
		Size: 40.5 MB (40547294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f938e0500fbeb672cfa8c4cad0e6115376e97717febea926c18d8a47911f2848`  
		Last Modified: Wed, 22 Jan 2020 05:19:56 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:af79c8c02cdac24cbe631bf0e8b951b4772b7ce3c646e151b9d8bf414a17a5b8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.1 MB (79110195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6375b6a32edfdeae6064ffcdb18182e58691394e7d8722569342da056696aac8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:26:42 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 02:58:58 GMT
ENV KONG_VERSION=2.0.0
# Wed, 22 Jan 2020 02:59:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Wed, 22 Jan 2020 02:59:38 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 02:59:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 02:59:40 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 02:59:41 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 02:59:41 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2e2be7a0ac63f5d522d309775630611df3e4573cd105bc8dbdeef49a0ccecd`  
		Last Modified: Wed, 22 Jan 2020 03:02:47 GMT  
		Size: 39.2 MB (39217689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05ff493ddc94920bd81c3621aff87c90ad0a38dcc818bd15d508dacf0a3a286`  
		Last Modified: Wed, 22 Jan 2020 03:02:34 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-centos`

```console
$ docker pull kong@sha256:94f9efc544e95c4272994b288ab4705cac33101e091d6f0be4ec8b55a4109b4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:c8fa4ff0c035afa30e80eb1ab56066876fadee72ab926442060cdf853f14c803
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158205282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b68221ae244e42b58e051b3d0ca18008663b288f29bfd5b7e2d0979d892b6384`
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
# Wed, 22 Jan 2020 05:16:25 GMT
ENV KONG_VERSION=2.0.0
# Wed, 22 Jan 2020 05:16:31 GMT
RUN yum install -y -q unzip 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Wed, 22 Jan 2020 05:16:52 GMT
RUN useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 22 Jan 2020 05:16:52 GMT
USER kong
# Wed, 22 Jan 2020 05:16:52 GMT
COPY file:d4cc11e4d968fd7df92b7b157746b27dc40d08cd20ca769e15cffc687cea9b5c in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:16:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:16:53 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:16:53 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:16:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33393acb164820849236d8a316b267340d8ea03502e0bfb9c760a92740ec4b52`  
		Last Modified: Wed, 22 Jan 2020 05:20:12 GMT  
		Size: 6.6 MB (6569271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd358c1ff903f4b77bbf06d91d9532da73bddee5e4d6971ea438149eea106faf`  
		Last Modified: Wed, 22 Jan 2020 05:20:25 GMT  
		Size: 75.9 MB (75854944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2637114431d722670a4c3246ab50aba0bbac9c51f6bceccd8b19f1eed6310417`  
		Last Modified: Wed, 22 Jan 2020 05:20:10 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-ubuntu`

```console
$ docker pull kong@sha256:eebd00092815a0cddf223d4629392a68e199460dbe8efe46cbd01e3688782fcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:5b650d206b1d925d17d3015bd44b0a8851fdc8ae8d55801baeb15ddc2c0d5fd5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.7 MB (84698909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8899060e4ff76086e4dd26b4cbbb331b467d41bc38823ecfc361430d41b0cf20`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:58:01 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 05:15:32 GMT
ENV KONG_VERSION=2.0.0
# Wed, 22 Jan 2020 05:16:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Wed, 22 Jan 2020 05:16:15 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:16:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:16:15 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:16:15 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:16:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb016521f3fdb1c7ac1744d0c7d50371d9ce2b75c20d917576453cfe6330898e`  
		Last Modified: Wed, 22 Jan 2020 05:20:05 GMT  
		Size: 40.5 MB (40547294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f938e0500fbeb672cfa8c4cad0e6115376e97717febea926c18d8a47911f2848`  
		Last Modified: Wed, 22 Jan 2020 05:19:56 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:af79c8c02cdac24cbe631bf0e8b951b4772b7ce3c646e151b9d8bf414a17a5b8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.1 MB (79110195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6375b6a32edfdeae6064ffcdb18182e58691394e7d8722569342da056696aac8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:26:42 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 02:58:58 GMT
ENV KONG_VERSION=2.0.0
# Wed, 22 Jan 2020 02:59:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Wed, 22 Jan 2020 02:59:38 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 02:59:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 02:59:40 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 02:59:41 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 02:59:41 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2e2be7a0ac63f5d522d309775630611df3e4573cd105bc8dbdeef49a0ccecd`  
		Last Modified: Wed, 22 Jan 2020 03:02:47 GMT  
		Size: 39.2 MB (39217689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05ff493ddc94920bd81c3621aff87c90ad0a38dcc818bd15d508dacf0a3a286`  
		Last Modified: Wed, 22 Jan 2020 03:02:34 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:a88c35cb8e7807966b6aaf1b41da3809b4b2c86ae50f7d036f90cb2aa747133a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:e0740a0092bcd9fa57803ba815918f3622f6b7862c38b6c7db9e1b76bc4c4893
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44116155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047d4996f6afd73e35643ce1250fe4aa6504fa1e8e190942a0f154075af6420f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Tue, 14 Jan 2020 22:20:00 GMT
ENV KONG_VERSION=1.4.3
# Tue, 14 Jan 2020 22:20:00 GMT
ENV KONG_SHA256=419d4e3d19f2d5c35ec6367e736b0d5509be4a7577d203008514a90f8dd5fdf1
# Tue, 14 Jan 2020 22:20:10 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 14 Jan 2020 22:20:10 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Tue, 14 Jan 2020 22:20:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jan 2020 22:20:11 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jan 2020 22:20:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jan 2020 22:20:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efff247f0f0be1c48baef7a6084e579e819895ac650e8658328d72277d930da8`  
		Last Modified: Tue, 14 Jan 2020 22:24:14 GMT  
		Size: 41.3 MB (41328424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc63fcd4751cea13596e7526721665e012cb861f64db41cc5659c016403207c`  
		Last Modified: Tue, 14 Jan 2020 22:24:06 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:7a3d24cc151c71a3e6b21a0ce1d9abb02319310e27cba574d589fdd9bbe01b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:centos` - linux; amd64

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

## `kong:latest`

```console
$ docker pull kong@sha256:9c630fcc43b8d30af115ded3221b85d4f9303f07a26be89586ce868be4d461d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:28378817cc5df4fc77fb9e600a7fe54c4d37abc66b82989b61b8a77661dd14a8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49283901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b33f8116962ae37ebd9626c4342b20e377adc2f1b14f683ba93817a3cf7dc0fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 22 Jan 2020 05:15:18 GMT
ENV KONG_VERSION=2.0.0
# Wed, 22 Jan 2020 05:15:18 GMT
ENV KONG_SHA256=5af1178111958b2e325c5b18690f4e7ddf064d28139ff38188b1e2e432ea99ff
# Wed, 22 Jan 2020 05:15:27 GMT
RUN adduser -S kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 22 Jan 2020 05:15:27 GMT
USER kong
# Wed, 22 Jan 2020 05:15:27 GMT
COPY file:d4cc11e4d968fd7df92b7b157746b27dc40d08cd20ca769e15cffc687cea9b5c in /docker-entrypoint.sh 
# Wed, 22 Jan 2020 05:15:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jan 2020 05:15:28 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jan 2020 05:15:28 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jan 2020 05:15:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4dc4b9dfde879379bef6ef7826fc166ebccbd14b77c10cb51a3dd8c9f4f015`  
		Last Modified: Wed, 22 Jan 2020 05:19:50 GMT  
		Size: 46.5 MB (46496411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1bc1d108f206400e74912aabc759a8cca9c5d8ec1647fb3fa52f93147ec69a`  
		Last Modified: Wed, 22 Jan 2020 05:19:40 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:10dcd2f640c3fb826e93c65751709d402aa1b5a6e8d411a8c73b01a239fa4f25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:24f292e66d7b50517c7124ac0b2c0ab1f64fc1715a77eece81c5e289595358fb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81137007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dcf1dcf7719f1f7e765f548f97c9771f4f8b584b9fa91aa6ee08b0eaf516b46`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:58:01 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 16 Jan 2020 03:58:41 GMT
ENV KONG_VERSION=1.4.3
# Thu, 16 Jan 2020 03:59:00 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 16 Jan 2020 03:59:00 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 16 Jan 2020 03:59:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Jan 2020 03:59:01 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Jan 2020 03:59:01 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Jan 2020 03:59:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf574948a848d22f35a50944eed358b29799173ab0e645b7dd53d6b2bec2a9c`  
		Last Modified: Thu, 16 Jan 2020 04:00:36 GMT  
		Size: 37.0 MB (36985392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777870d322002bfa63b5576d3506d1ad1b08aae0bb9ce60a9c8f08b484ec415c`  
		Last Modified: Thu, 16 Jan 2020 04:00:28 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:cd6d798dcc8501524178e6d941c2bf89b3761bb663e82ee4a499d1f298c548ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76220627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a5ea8dd0b3c36759c2603a6af8f93a5df1e8a197ce9a0fa43874252fc517783`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:26:42 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 16 Jan 2020 01:28:26 GMT
ENV KONG_VERSION=1.4.3
# Thu, 16 Jan 2020 01:29:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 16 Jan 2020 01:29:14 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 16 Jan 2020 01:29:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Jan 2020 01:29:16 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Jan 2020 01:29:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Jan 2020 01:29:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724c2342595ca43d29cbe4769bdf4aa42344bea10b0b2271b975d8ccbe85658a`  
		Last Modified: Thu, 16 Jan 2020 01:32:44 GMT  
		Size: 36.3 MB (36328122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb53b468a9076e898d0b200d524da2a9b40d2bce52b0f2f96c95f9fbebaeb9`  
		Last Modified: Thu, 16 Jan 2020 01:32:29 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
