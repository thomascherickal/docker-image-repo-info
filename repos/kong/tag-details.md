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
-	[`kong:1.2.2`](#kong122)
-	[`kong:1.2.2-alpine`](#kong122-alpine)
-	[`kong:1.2.2-centos`](#kong122-centos)
-	[`kong:1.2-centos`](#kong12-centos)
-	[`kong:1.3`](#kong13)
-	[`kong:1.3.0`](#kong130)
-	[`kong:1.3.0-alpine`](#kong130-alpine)
-	[`kong:1.3.0-centos`](#kong130-centos)
-	[`kong:1.3.0-ubuntu`](#kong130-ubuntu)
-	[`kong:1.3-centos`](#kong13-centos)
-	[`kong:1.3-ubuntu`](#kong13-ubuntu)
-	[`kong:1.4`](#kong14)
-	[`kong:1.4.0-ubuntu`](#kong140-ubuntu)
-	[`kong:1.4.2`](#kong142)
-	[`kong:1.4.2-alpine`](#kong142-alpine)
-	[`kong:1.4.2-centos`](#kong142-centos)
-	[`kong:1.4.2-ubuntu`](#kong142-ubuntu)
-	[`kong:1.4-centos`](#kong14-centos)
-	[`kong:1.4-ubuntu`](#kong14-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:centos`](#kongcentos)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:1.0`

```console
$ docker pull kong@sha256:a17d21b94ab8cfd1e79430226c25625e7379515a1407c27f302f497145db0b85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0` - linux; amd64

```console
$ docker pull kong@sha256:45154e68662930a789a612925134ca8d915c2730e2f8440fb98a091abc7a1110
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43704799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef5071c2216d5183a3c4c544f87c65bc4e3a32a9c3c2bb7f7eec97452e58d5d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 19 Dec 2019 23:21:54 GMT
ADD file:c7d28fcb71c026d7956b381180e4792c8219b04904e726a9266322ef5b256df8 in / 
# Thu, 19 Dec 2019 23:21:54 GMT
CMD ["/bin/sh"]
# Fri, 20 Dec 2019 00:12:02 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 20 Dec 2019 00:12:02 GMT
ENV KONG_VERSION=1.0.4
# Fri, 20 Dec 2019 00:12:03 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Fri, 20 Dec 2019 00:12:16 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 20 Dec 2019 00:12:17 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 20 Dec 2019 00:12:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 20 Dec 2019 00:12:17 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 20 Dec 2019 00:12:18 GMT
STOPSIGNAL SIGTERM
# Fri, 20 Dec 2019 00:12:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:63bc94deeb2884fd684a72d356164664538ee55cd82a9e65afe300a432092744`  
		Last Modified: Thu, 19 Dec 2019 23:22:17 GMT  
		Size: 2.8 MB (2801746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa33eb879afeb434211e761b49c5ad4d2252f7099d55d376e733e50a38be8d7`  
		Last Modified: Fri, 20 Dec 2019 00:13:26 GMT  
		Size: 40.9 MB (40902457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f8915980dc66adab368ea9734dec30276f570914dad1bf0d911bcc899b09eb`  
		Last Modified: Fri, 20 Dec 2019 00:13:12 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0.4`

```console
$ docker pull kong@sha256:a17d21b94ab8cfd1e79430226c25625e7379515a1407c27f302f497145db0b85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0.4` - linux; amd64

```console
$ docker pull kong@sha256:45154e68662930a789a612925134ca8d915c2730e2f8440fb98a091abc7a1110
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43704799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef5071c2216d5183a3c4c544f87c65bc4e3a32a9c3c2bb7f7eec97452e58d5d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 19 Dec 2019 23:21:54 GMT
ADD file:c7d28fcb71c026d7956b381180e4792c8219b04904e726a9266322ef5b256df8 in / 
# Thu, 19 Dec 2019 23:21:54 GMT
CMD ["/bin/sh"]
# Fri, 20 Dec 2019 00:12:02 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 20 Dec 2019 00:12:02 GMT
ENV KONG_VERSION=1.0.4
# Fri, 20 Dec 2019 00:12:03 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Fri, 20 Dec 2019 00:12:16 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 20 Dec 2019 00:12:17 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 20 Dec 2019 00:12:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 20 Dec 2019 00:12:17 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 20 Dec 2019 00:12:18 GMT
STOPSIGNAL SIGTERM
# Fri, 20 Dec 2019 00:12:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:63bc94deeb2884fd684a72d356164664538ee55cd82a9e65afe300a432092744`  
		Last Modified: Thu, 19 Dec 2019 23:22:17 GMT  
		Size: 2.8 MB (2801746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa33eb879afeb434211e761b49c5ad4d2252f7099d55d376e733e50a38be8d7`  
		Last Modified: Fri, 20 Dec 2019 00:13:26 GMT  
		Size: 40.9 MB (40902457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f8915980dc66adab368ea9734dec30276f570914dad1bf0d911bcc899b09eb`  
		Last Modified: Fri, 20 Dec 2019 00:13:12 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.0.4-alpine`

```console
$ docker pull kong@sha256:a17d21b94ab8cfd1e79430226c25625e7379515a1407c27f302f497145db0b85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.0.4-alpine` - linux; amd64

```console
$ docker pull kong@sha256:45154e68662930a789a612925134ca8d915c2730e2f8440fb98a091abc7a1110
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43704799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef5071c2216d5183a3c4c544f87c65bc4e3a32a9c3c2bb7f7eec97452e58d5d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 19 Dec 2019 23:21:54 GMT
ADD file:c7d28fcb71c026d7956b381180e4792c8219b04904e726a9266322ef5b256df8 in / 
# Thu, 19 Dec 2019 23:21:54 GMT
CMD ["/bin/sh"]
# Fri, 20 Dec 2019 00:12:02 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 20 Dec 2019 00:12:02 GMT
ENV KONG_VERSION=1.0.4
# Fri, 20 Dec 2019 00:12:03 GMT
ENV KONG_SHA256=65fd7df61cf526899e0197d78adbc42680a735eea261b2525f4b1d4f82d7503e
# Fri, 20 Dec 2019 00:12:16 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Fri, 20 Dec 2019 00:12:17 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Fri, 20 Dec 2019 00:12:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 20 Dec 2019 00:12:17 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 20 Dec 2019 00:12:18 GMT
STOPSIGNAL SIGTERM
# Fri, 20 Dec 2019 00:12:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:63bc94deeb2884fd684a72d356164664538ee55cd82a9e65afe300a432092744`  
		Last Modified: Thu, 19 Dec 2019 23:22:17 GMT  
		Size: 2.8 MB (2801746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa33eb879afeb434211e761b49c5ad4d2252f7099d55d376e733e50a38be8d7`  
		Last Modified: Fri, 20 Dec 2019 00:13:26 GMT  
		Size: 40.9 MB (40902457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f8915980dc66adab368ea9734dec30276f570914dad1bf0d911bcc899b09eb`  
		Last Modified: Fri, 20 Dec 2019 00:13:12 GMT  
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
$ docker pull kong@sha256:830cc509df7d57483deefcb8c45ad792b4dd6595ab3080eac3b619113c748563
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2` - linux; amd64

```console
$ docker pull kong@sha256:743606c61df7e14be01fe832357ffee48b666392f89780a70f501c9c3674f315
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44478555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f661e7ecc71bca013089489a717852a7588e597f97f9760ef64cc1c8154cc95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Mon, 21 Oct 2019 18:58:56 GMT
ENV KONG_VERSION=1.2.2
# Mon, 21 Oct 2019 18:58:56 GMT
ENV KONG_SHA256=76183d7e8ff084c86767b917da441001d0d779d35fa2464275b74226029a46bf
# Mon, 21 Oct 2019 18:59:04 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Mon, 21 Oct 2019 18:59:05 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Mon, 21 Oct 2019 18:59:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:59:05 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 21 Oct 2019 18:59:05 GMT
STOPSIGNAL SIGQUIT
# Mon, 21 Oct 2019 18:59:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db20d60030a7829f45890ffe512dec17f21080e557336653dde4c6f83df2a0f3`  
		Last Modified: Mon, 21 Oct 2019 19:00:53 GMT  
		Size: 41.7 MB (41690825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8706a175048b410b2421a5829c9d02fbd967d085f0954800d3be6f226ecf82`  
		Last Modified: Mon, 21 Oct 2019 19:00:44 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2.2`

```console
$ docker pull kong@sha256:830cc509df7d57483deefcb8c45ad792b4dd6595ab3080eac3b619113c748563
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2.2` - linux; amd64

```console
$ docker pull kong@sha256:743606c61df7e14be01fe832357ffee48b666392f89780a70f501c9c3674f315
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44478555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f661e7ecc71bca013089489a717852a7588e597f97f9760ef64cc1c8154cc95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Mon, 21 Oct 2019 18:58:56 GMT
ENV KONG_VERSION=1.2.2
# Mon, 21 Oct 2019 18:58:56 GMT
ENV KONG_SHA256=76183d7e8ff084c86767b917da441001d0d779d35fa2464275b74226029a46bf
# Mon, 21 Oct 2019 18:59:04 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Mon, 21 Oct 2019 18:59:05 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Mon, 21 Oct 2019 18:59:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:59:05 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 21 Oct 2019 18:59:05 GMT
STOPSIGNAL SIGQUIT
# Mon, 21 Oct 2019 18:59:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db20d60030a7829f45890ffe512dec17f21080e557336653dde4c6f83df2a0f3`  
		Last Modified: Mon, 21 Oct 2019 19:00:53 GMT  
		Size: 41.7 MB (41690825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8706a175048b410b2421a5829c9d02fbd967d085f0954800d3be6f226ecf82`  
		Last Modified: Mon, 21 Oct 2019 19:00:44 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2.2-alpine`

```console
$ docker pull kong@sha256:830cc509df7d57483deefcb8c45ad792b4dd6595ab3080eac3b619113c748563
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:743606c61df7e14be01fe832357ffee48b666392f89780a70f501c9c3674f315
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44478555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f661e7ecc71bca013089489a717852a7588e597f97f9760ef64cc1c8154cc95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Mon, 21 Oct 2019 18:58:56 GMT
ENV KONG_VERSION=1.2.2
# Mon, 21 Oct 2019 18:58:56 GMT
ENV KONG_SHA256=76183d7e8ff084c86767b917da441001d0d779d35fa2464275b74226029a46bf
# Mon, 21 Oct 2019 18:59:04 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Mon, 21 Oct 2019 18:59:05 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Mon, 21 Oct 2019 18:59:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:59:05 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 21 Oct 2019 18:59:05 GMT
STOPSIGNAL SIGQUIT
# Mon, 21 Oct 2019 18:59:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db20d60030a7829f45890ffe512dec17f21080e557336653dde4c6f83df2a0f3`  
		Last Modified: Mon, 21 Oct 2019 19:00:53 GMT  
		Size: 41.7 MB (41690825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8706a175048b410b2421a5829c9d02fbd967d085f0954800d3be6f226ecf82`  
		Last Modified: Mon, 21 Oct 2019 19:00:44 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2.2-centos`

```console
$ docker pull kong@sha256:8bb92d8ba69740aa221105fc73837adb97a7e971a6a1c09210b9f338d3867ae1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2.2-centos` - linux; amd64

```console
$ docker pull kong@sha256:70094e479290a0962ac8c3591fa1f7f02ae223818f04f66c30bf5c707d661f4f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150532146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:910ad4f48f37a4caf763c06e6fce6c74056908c7fea41f547512070afc01a8be`
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
# Tue, 12 Nov 2019 02:34:18 GMT
ENV KONG_VERSION=1.2.2
# Tue, 12 Nov 2019 02:34:19 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 12 Nov 2019 02:34:19 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 12 Nov 2019 02:34:59 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 12 Nov 2019 02:35:16 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 12 Nov 2019 02:35:17 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 12 Nov 2019 02:35:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Nov 2019 02:35:17 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 12 Nov 2019 02:35:17 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Nov 2019 02:35:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7084c5184f6cd2d991c9ad33750308e3cb7e59c30c7a7d49afdd36b02153433`  
		Last Modified: Tue, 12 Nov 2019 02:38:22 GMT  
		Size: 6.5 MB (6513631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f092f7a681deb628b1cc1f5a8e44a214e99091a1797b2dc3b948a452b7a71a22`  
		Last Modified: Tue, 12 Nov 2019 02:38:33 GMT  
		Size: 68.2 MB (68237208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210412ab16c42dae662ef46a2e9f7c7d4acbbacc1b650384d4dc1e73e4cef17a`  
		Last Modified: Tue, 12 Nov 2019 02:38:20 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.2-centos`

```console
$ docker pull kong@sha256:8bb92d8ba69740aa221105fc73837adb97a7e971a6a1c09210b9f338d3867ae1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.2-centos` - linux; amd64

```console
$ docker pull kong@sha256:70094e479290a0962ac8c3591fa1f7f02ae223818f04f66c30bf5c707d661f4f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150532146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:910ad4f48f37a4caf763c06e6fce6c74056908c7fea41f547512070afc01a8be`
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
# Tue, 12 Nov 2019 02:34:18 GMT
ENV KONG_VERSION=1.2.2
# Tue, 12 Nov 2019 02:34:19 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 12 Nov 2019 02:34:19 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 12 Nov 2019 02:34:59 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 12 Nov 2019 02:35:16 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.noarch.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 12 Nov 2019 02:35:17 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 12 Nov 2019 02:35:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Nov 2019 02:35:17 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 12 Nov 2019 02:35:17 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Nov 2019 02:35:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7084c5184f6cd2d991c9ad33750308e3cb7e59c30c7a7d49afdd36b02153433`  
		Last Modified: Tue, 12 Nov 2019 02:38:22 GMT  
		Size: 6.5 MB (6513631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f092f7a681deb628b1cc1f5a8e44a214e99091a1797b2dc3b948a452b7a71a22`  
		Last Modified: Tue, 12 Nov 2019 02:38:33 GMT  
		Size: 68.2 MB (68237208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210412ab16c42dae662ef46a2e9f7c7d4acbbacc1b650384d4dc1e73e4cef17a`  
		Last Modified: Tue, 12 Nov 2019 02:38:20 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3`

```console
$ docker pull kong@sha256:664fb9a9bd06632d64274bc158066787108038d59036abb01db63ffd3dfc0fdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3` - linux; amd64

```console
$ docker pull kong@sha256:b83ebd42c0114bfb76a2917e4681be9048224b98f53ee152250dc015a7294fa4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44775929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa61cd7bbe42d535c2b2aca7e27e60e79b36f4d7635d7d85675e64f4107aca31`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Mon, 21 Oct 2019 18:58:31 GMT
ENV KONG_VERSION=1.3.0
# Mon, 21 Oct 2019 18:58:31 GMT
ENV KONG_SHA256=566f2a8009cbd7eebd32843c2f03c8d5f736139110988dc12dee161046428112
# Mon, 21 Oct 2019 18:58:43 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Mon, 21 Oct 2019 18:58:43 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Mon, 21 Oct 2019 18:58:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:58:43 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 21 Oct 2019 18:58:43 GMT
STOPSIGNAL SIGQUIT
# Mon, 21 Oct 2019 18:58:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42ebd17864d94ae876cc8a3a343dbb834f4e51f8e43a887e434a9457bcedc37`  
		Last Modified: Mon, 21 Oct 2019 19:00:35 GMT  
		Size: 42.0 MB (41988199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d2881bb77efcbae182955056007de643bcbbab607d092e6e254f3756b994d0`  
		Last Modified: Mon, 21 Oct 2019 19:00:26 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.0`

```console
$ docker pull kong@sha256:664fb9a9bd06632d64274bc158066787108038d59036abb01db63ffd3dfc0fdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.0` - linux; amd64

```console
$ docker pull kong@sha256:b83ebd42c0114bfb76a2917e4681be9048224b98f53ee152250dc015a7294fa4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44775929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa61cd7bbe42d535c2b2aca7e27e60e79b36f4d7635d7d85675e64f4107aca31`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Mon, 21 Oct 2019 18:58:31 GMT
ENV KONG_VERSION=1.3.0
# Mon, 21 Oct 2019 18:58:31 GMT
ENV KONG_SHA256=566f2a8009cbd7eebd32843c2f03c8d5f736139110988dc12dee161046428112
# Mon, 21 Oct 2019 18:58:43 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Mon, 21 Oct 2019 18:58:43 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Mon, 21 Oct 2019 18:58:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:58:43 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 21 Oct 2019 18:58:43 GMT
STOPSIGNAL SIGQUIT
# Mon, 21 Oct 2019 18:58:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42ebd17864d94ae876cc8a3a343dbb834f4e51f8e43a887e434a9457bcedc37`  
		Last Modified: Mon, 21 Oct 2019 19:00:35 GMT  
		Size: 42.0 MB (41988199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d2881bb77efcbae182955056007de643bcbbab607d092e6e254f3756b994d0`  
		Last Modified: Mon, 21 Oct 2019 19:00:26 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.0-alpine`

```console
$ docker pull kong@sha256:664fb9a9bd06632d64274bc158066787108038d59036abb01db63ffd3dfc0fdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:b83ebd42c0114bfb76a2917e4681be9048224b98f53ee152250dc015a7294fa4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44775929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa61cd7bbe42d535c2b2aca7e27e60e79b36f4d7635d7d85675e64f4107aca31`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Mon, 21 Oct 2019 18:58:31 GMT
ENV KONG_VERSION=1.3.0
# Mon, 21 Oct 2019 18:58:31 GMT
ENV KONG_SHA256=566f2a8009cbd7eebd32843c2f03c8d5f736139110988dc12dee161046428112
# Mon, 21 Oct 2019 18:58:43 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata curl libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Mon, 21 Oct 2019 18:58:43 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Mon, 21 Oct 2019 18:58:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 21 Oct 2019 18:58:43 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 21 Oct 2019 18:58:43 GMT
STOPSIGNAL SIGQUIT
# Mon, 21 Oct 2019 18:58:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42ebd17864d94ae876cc8a3a343dbb834f4e51f8e43a887e434a9457bcedc37`  
		Last Modified: Mon, 21 Oct 2019 19:00:35 GMT  
		Size: 42.0 MB (41988199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d2881bb77efcbae182955056007de643bcbbab607d092e6e254f3756b994d0`  
		Last Modified: Mon, 21 Oct 2019 19:00:26 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.0-centos`

```console
$ docker pull kong@sha256:848a79f68cc4a5c741447a971c114cc21fd6082cc4e3c1d404d977b043dd01da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:84c7447154c6b52064d3634ebfd7bc263dd85055f5a6013b8a5a7a901840a75d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151044103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6abed9e2af5b2aa8952f2528f783b3d58033ebd0fb7b2beec16334c347c48db`
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
# Tue, 12 Nov 2019 02:33:12 GMT
ENV KONG_VERSION=1.3.0
# Tue, 12 Nov 2019 02:33:12 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 12 Nov 2019 02:33:13 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 12 Nov 2019 02:33:49 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 12 Nov 2019 02:34:07 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 12 Nov 2019 02:34:07 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 12 Nov 2019 02:34:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Nov 2019 02:34:07 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 12 Nov 2019 02:34:07 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Nov 2019 02:34:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e6d9970ea7feff3d9742d8902a6e5d64e6e37bfe9d7aa73413b99b0cdf3c85`  
		Last Modified: Tue, 12 Nov 2019 02:38:05 GMT  
		Size: 6.5 MB (6513663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68289c8ffcd2e8f542d3a4cf330a9714371612481fa547c789e0a7a4f004196`  
		Last Modified: Tue, 12 Nov 2019 02:38:15 GMT  
		Size: 68.7 MB (68749131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58cde6491b23e86120504cb451eccf3a24fff200012cd98e47471fbe650ba1c`  
		Last Modified: Tue, 12 Nov 2019 02:38:03 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3.0-ubuntu`

```console
$ docker pull kong@sha256:b363966cef8fa5dd47ff44a456bd4fc209e5ffbd1603985fda71b2e0345ba566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.3.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:5fd6795718efc663c362166cbce5d5ba481c4dd14d7627f23017cf39a935e123
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81087232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:045622e9a886bdbf1c062d8a5351a640cc2b931a671c894559be5b4f5747a9fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:51:55 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 19 Dec 2019 07:52:31 GMT
ENV KONG_VERSION=1.3.0
# Thu, 19 Dec 2019 07:52:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 19 Dec 2019 07:52:51 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 19 Dec 2019 07:52:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:52:51 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 19 Dec 2019 07:52:51 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 07:52:51 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef3654fac388b7cfa5ce65e3e46f2e2157e642c4fda18542f8a534e24735bd`  
		Last Modified: Thu, 19 Dec 2019 07:53:55 GMT  
		Size: 37.0 MB (36962121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f70fc691d9bb32a05e53439deb1d5906fcae9d207d91af2747fd91e7a7290`  
		Last Modified: Thu, 19 Dec 2019 07:53:44 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.3.0-ubuntu` - linux; arm64 variant v8

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

## `kong:1.3-centos`

```console
$ docker pull kong@sha256:848a79f68cc4a5c741447a971c114cc21fd6082cc4e3c1d404d977b043dd01da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.3-centos` - linux; amd64

```console
$ docker pull kong@sha256:84c7447154c6b52064d3634ebfd7bc263dd85055f5a6013b8a5a7a901840a75d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151044103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6abed9e2af5b2aa8952f2528f783b3d58033ebd0fb7b2beec16334c347c48db`
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
# Tue, 12 Nov 2019 02:33:12 GMT
ENV KONG_VERSION=1.3.0
# Tue, 12 Nov 2019 02:33:12 GMT
ARG SU_EXEC_VERSION=0.2
# Tue, 12 Nov 2019 02:33:13 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Tue, 12 Nov 2019 02:33:49 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Tue, 12 Nov 2019 02:34:07 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Tue, 12 Nov 2019 02:34:07 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Tue, 12 Nov 2019 02:34:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Nov 2019 02:34:07 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 12 Nov 2019 02:34:07 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Nov 2019 02:34:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e6d9970ea7feff3d9742d8902a6e5d64e6e37bfe9d7aa73413b99b0cdf3c85`  
		Last Modified: Tue, 12 Nov 2019 02:38:05 GMT  
		Size: 6.5 MB (6513663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68289c8ffcd2e8f542d3a4cf330a9714371612481fa547c789e0a7a4f004196`  
		Last Modified: Tue, 12 Nov 2019 02:38:15 GMT  
		Size: 68.7 MB (68749131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58cde6491b23e86120504cb451eccf3a24fff200012cd98e47471fbe650ba1c`  
		Last Modified: Tue, 12 Nov 2019 02:38:03 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.3-ubuntu`

```console
$ docker pull kong@sha256:b363966cef8fa5dd47ff44a456bd4fc209e5ffbd1603985fda71b2e0345ba566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:5fd6795718efc663c362166cbce5d5ba481c4dd14d7627f23017cf39a935e123
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81087232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:045622e9a886bdbf1c062d8a5351a640cc2b931a671c894559be5b4f5747a9fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:51:55 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 19 Dec 2019 07:52:31 GMT
ENV KONG_VERSION=1.3.0
# Thu, 19 Dec 2019 07:52:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 19 Dec 2019 07:52:51 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 19 Dec 2019 07:52:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:52:51 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 19 Dec 2019 07:52:51 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 07:52:51 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef3654fac388b7cfa5ce65e3e46f2e2157e642c4fda18542f8a534e24735bd`  
		Last Modified: Thu, 19 Dec 2019 07:53:55 GMT  
		Size: 37.0 MB (36962121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f70fc691d9bb32a05e53439deb1d5906fcae9d207d91af2747fd91e7a7290`  
		Last Modified: Thu, 19 Dec 2019 07:53:44 GMT  
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
$ docker pull kong@sha256:890a44c18d1f8e8043735b1ce6a607409f575aaf978ce36b923d9b441c0b2e9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4` - linux; amd64

```console
$ docker pull kong@sha256:027f0a48dd57f5d8ac06d6d5768807caaa03a2e674c8f5d2abb6e41faaea05ae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44082042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75cf2d6ba0b072e73094e8a1762d102655481daa1b32fd8a6347962f8e4a11f7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 11 Dec 2019 22:19:48 GMT
ENV KONG_VERSION=1.4.2
# Wed, 11 Dec 2019 22:19:48 GMT
ENV KONG_SHA256=edf917d956d697abb70f5f3f630d420ee699c6428bf953221cd8548eda490dcf
# Wed, 11 Dec 2019 22:19:58 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 11 Dec 2019 22:19:58 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Wed, 11 Dec 2019 22:19:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:19:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 11 Dec 2019 22:19:59 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Dec 2019 22:19:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76caeea1403bec7384884ee7560caf82e96cf98cd3d984e3fede3b3c5923b749`  
		Last Modified: Wed, 11 Dec 2019 22:22:42 GMT  
		Size: 41.3 MB (41294312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329f8ea00697d6d19b0113925a9cbf47a7aefc33767bd60045ce24f7efaa02ca`  
		Last Modified: Wed, 11 Dec 2019 22:22:31 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.0-ubuntu`

```console
$ docker pull kong@sha256:bf362e56c2fdc82de32afd55a5e8c80b11689985f38bb7c0a2567476ed4fa5b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.4.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:a60cf94cd375658c8e79dccccaef18670fe4b234f8db527851f031630083ad57
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81104756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511c55c319378c081f734f2cd21aa0d6e116e8c791f1ea8f81f5bbcca38a8ee5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:51:55 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 19 Dec 2019 07:51:56 GMT
ENV KONG_VERSION=1.4.2
# Thu, 19 Dec 2019 07:52:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 19 Dec 2019 07:52:18 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 19 Dec 2019 07:52:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:52:19 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 19 Dec 2019 07:52:19 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 07:52:19 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730355a76b4850ee7f9d2f735fcec23e7de250cb6ad9f1c92da08caff919c496`  
		Last Modified: Thu, 19 Dec 2019 07:53:39 GMT  
		Size: 37.0 MB (36979645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea51f27bd020a5b20650a4d577337a5330bf5397f148531a002237f4941ec341`  
		Last Modified: Thu, 19 Dec 2019 07:53:31 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.4.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:3b11312ff5566c40f219a964a1c911646ef3a54aa9888542638d2c201054ae71
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76201023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca23b8e72488bac200af48039ef1cf7233e58430279299d47f2562bc37b301a`
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
# Thu, 19 Dec 2019 07:46:45 GMT
ENV KONG_VERSION=1.4.2
# Thu, 19 Dec 2019 07:47:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 19 Dec 2019 07:47:28 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 19 Dec 2019 07:47:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:47:30 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 19 Dec 2019 07:47:31 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 07:47:32 GMT
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
	-	`sha256:ae187bbfe3d971b97dd69384838f0ceca9b2161f31866a2ba650a82ae734fcf6`  
		Last Modified: Thu, 19 Dec 2019 07:48:54 GMT  
		Size: 36.3 MB (36323826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083cc07e30ff149240e95b3fa7612e0f89e1bfe681379f40081f637f8db06b08`  
		Last Modified: Thu, 19 Dec 2019 07:48:40 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.2`

```console
$ docker pull kong@sha256:890a44c18d1f8e8043735b1ce6a607409f575aaf978ce36b923d9b441c0b2e9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4.2` - linux; amd64

```console
$ docker pull kong@sha256:027f0a48dd57f5d8ac06d6d5768807caaa03a2e674c8f5d2abb6e41faaea05ae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44082042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75cf2d6ba0b072e73094e8a1762d102655481daa1b32fd8a6347962f8e4a11f7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 11 Dec 2019 22:19:48 GMT
ENV KONG_VERSION=1.4.2
# Wed, 11 Dec 2019 22:19:48 GMT
ENV KONG_SHA256=edf917d956d697abb70f5f3f630d420ee699c6428bf953221cd8548eda490dcf
# Wed, 11 Dec 2019 22:19:58 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 11 Dec 2019 22:19:58 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Wed, 11 Dec 2019 22:19:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:19:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 11 Dec 2019 22:19:59 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Dec 2019 22:19:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76caeea1403bec7384884ee7560caf82e96cf98cd3d984e3fede3b3c5923b749`  
		Last Modified: Wed, 11 Dec 2019 22:22:42 GMT  
		Size: 41.3 MB (41294312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329f8ea00697d6d19b0113925a9cbf47a7aefc33767bd60045ce24f7efaa02ca`  
		Last Modified: Wed, 11 Dec 2019 22:22:31 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.2-alpine`

```console
$ docker pull kong@sha256:890a44c18d1f8e8043735b1ce6a607409f575aaf978ce36b923d9b441c0b2e9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:027f0a48dd57f5d8ac06d6d5768807caaa03a2e674c8f5d2abb6e41faaea05ae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44082042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75cf2d6ba0b072e73094e8a1762d102655481daa1b32fd8a6347962f8e4a11f7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 11 Dec 2019 22:19:48 GMT
ENV KONG_VERSION=1.4.2
# Wed, 11 Dec 2019 22:19:48 GMT
ENV KONG_SHA256=edf917d956d697abb70f5f3f630d420ee699c6428bf953221cd8548eda490dcf
# Wed, 11 Dec 2019 22:19:58 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 11 Dec 2019 22:19:58 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Wed, 11 Dec 2019 22:19:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:19:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 11 Dec 2019 22:19:59 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Dec 2019 22:19:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76caeea1403bec7384884ee7560caf82e96cf98cd3d984e3fede3b3c5923b749`  
		Last Modified: Wed, 11 Dec 2019 22:22:42 GMT  
		Size: 41.3 MB (41294312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329f8ea00697d6d19b0113925a9cbf47a7aefc33767bd60045ce24f7efaa02ca`  
		Last Modified: Wed, 11 Dec 2019 22:22:31 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.2-centos`

```console
$ docker pull kong@sha256:6ff5dd5576603b12133fe33ad949511c97bc7fed5df8a12edb9d3ee38ae850d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4.2-centos` - linux; amd64

```console
$ docker pull kong@sha256:e061b8bba0aab21b5f895612aa3d68fc669badc869ced2a45b4871051b2f4a73
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151016442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a205672e9fd293b011012b2488d9370905506813a09274a1d6ec489a097dcdf`
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
# Wed, 11 Dec 2019 22:20:49 GMT
ENV KONG_VERSION=1.4.2
# Wed, 11 Dec 2019 22:20:49 GMT
ARG SU_EXEC_VERSION=0.2
# Wed, 11 Dec 2019 22:20:49 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Wed, 11 Dec 2019 22:21:27 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Wed, 11 Dec 2019 22:21:43 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 11 Dec 2019 22:21:43 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Wed, 11 Dec 2019 22:21:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:21:44 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 11 Dec 2019 22:21:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Dec 2019 22:21:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4cd0ddf1a96ad908b6bce2a0c4093f0833e6289ead6d3b2aba5b632a1b326a`  
		Last Modified: Wed, 11 Dec 2019 22:23:04 GMT  
		Size: 6.5 MB (6509463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dede93e46215427b107e661256254efe0e21c305ae31e372e7dfe6fea8651038`  
		Last Modified: Wed, 11 Dec 2019 22:23:13 GMT  
		Size: 68.7 MB (68725671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5074025603d1c60b4b7ce8967692bf48eb5fc2f16d80a2bc3b4706530368a9b0`  
		Last Modified: Wed, 11 Dec 2019 22:23:02 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4.2-ubuntu`

**does not exist** (yet?)

## `kong:1.4-centos`

```console
$ docker pull kong@sha256:6ff5dd5576603b12133fe33ad949511c97bc7fed5df8a12edb9d3ee38ae850d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:1.4-centos` - linux; amd64

```console
$ docker pull kong@sha256:e061b8bba0aab21b5f895612aa3d68fc669badc869ced2a45b4871051b2f4a73
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151016442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a205672e9fd293b011012b2488d9370905506813a09274a1d6ec489a097dcdf`
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
# Wed, 11 Dec 2019 22:20:49 GMT
ENV KONG_VERSION=1.4.2
# Wed, 11 Dec 2019 22:20:49 GMT
ARG SU_EXEC_VERSION=0.2
# Wed, 11 Dec 2019 22:20:49 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Wed, 11 Dec 2019 22:21:27 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Wed, 11 Dec 2019 22:21:43 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 11 Dec 2019 22:21:43 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Wed, 11 Dec 2019 22:21:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:21:44 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 11 Dec 2019 22:21:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Dec 2019 22:21:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4cd0ddf1a96ad908b6bce2a0c4093f0833e6289ead6d3b2aba5b632a1b326a`  
		Last Modified: Wed, 11 Dec 2019 22:23:04 GMT  
		Size: 6.5 MB (6509463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dede93e46215427b107e661256254efe0e21c305ae31e372e7dfe6fea8651038`  
		Last Modified: Wed, 11 Dec 2019 22:23:13 GMT  
		Size: 68.7 MB (68725671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5074025603d1c60b4b7ce8967692bf48eb5fc2f16d80a2bc3b4706530368a9b0`  
		Last Modified: Wed, 11 Dec 2019 22:23:02 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:1.4-ubuntu`

```console
$ docker pull kong@sha256:bf362e56c2fdc82de32afd55a5e8c80b11689985f38bb7c0a2567476ed4fa5b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:1.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:a60cf94cd375658c8e79dccccaef18670fe4b234f8db527851f031630083ad57
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81104756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511c55c319378c081f734f2cd21aa0d6e116e8c791f1ea8f81f5bbcca38a8ee5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:51:55 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 19 Dec 2019 07:51:56 GMT
ENV KONG_VERSION=1.4.2
# Thu, 19 Dec 2019 07:52:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 19 Dec 2019 07:52:18 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 19 Dec 2019 07:52:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:52:19 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 19 Dec 2019 07:52:19 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 07:52:19 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730355a76b4850ee7f9d2f735fcec23e7de250cb6ad9f1c92da08caff919c496`  
		Last Modified: Thu, 19 Dec 2019 07:53:39 GMT  
		Size: 37.0 MB (36979645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea51f27bd020a5b20650a4d577337a5330bf5397f148531a002237f4941ec341`  
		Last Modified: Thu, 19 Dec 2019 07:53:31 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:1.4-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:3b11312ff5566c40f219a964a1c911646ef3a54aa9888542638d2c201054ae71
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76201023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca23b8e72488bac200af48039ef1cf7233e58430279299d47f2562bc37b301a`
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
# Thu, 19 Dec 2019 07:46:45 GMT
ENV KONG_VERSION=1.4.2
# Thu, 19 Dec 2019 07:47:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 19 Dec 2019 07:47:28 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 19 Dec 2019 07:47:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:47:30 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 19 Dec 2019 07:47:31 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 07:47:32 GMT
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
	-	`sha256:ae187bbfe3d971b97dd69384838f0ceca9b2161f31866a2ba650a82ae734fcf6`  
		Last Modified: Thu, 19 Dec 2019 07:48:54 GMT  
		Size: 36.3 MB (36323826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083cc07e30ff149240e95b3fa7612e0f89e1bfe681379f40081f637f8db06b08`  
		Last Modified: Thu, 19 Dec 2019 07:48:40 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:890a44c18d1f8e8043735b1ce6a607409f575aaf978ce36b923d9b441c0b2e9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:027f0a48dd57f5d8ac06d6d5768807caaa03a2e674c8f5d2abb6e41faaea05ae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44082042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75cf2d6ba0b072e73094e8a1762d102655481daa1b32fd8a6347962f8e4a11f7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 11 Dec 2019 22:19:48 GMT
ENV KONG_VERSION=1.4.2
# Wed, 11 Dec 2019 22:19:48 GMT
ENV KONG_SHA256=edf917d956d697abb70f5f3f630d420ee699c6428bf953221cd8548eda490dcf
# Wed, 11 Dec 2019 22:19:58 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 11 Dec 2019 22:19:58 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Wed, 11 Dec 2019 22:19:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:19:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 11 Dec 2019 22:19:59 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Dec 2019 22:19:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76caeea1403bec7384884ee7560caf82e96cf98cd3d984e3fede3b3c5923b749`  
		Last Modified: Wed, 11 Dec 2019 22:22:42 GMT  
		Size: 41.3 MB (41294312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329f8ea00697d6d19b0113925a9cbf47a7aefc33767bd60045ce24f7efaa02ca`  
		Last Modified: Wed, 11 Dec 2019 22:22:31 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:6ff5dd5576603b12133fe33ad949511c97bc7fed5df8a12edb9d3ee38ae850d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:e061b8bba0aab21b5f895612aa3d68fc669badc869ced2a45b4871051b2f4a73
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151016442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a205672e9fd293b011012b2488d9370905506813a09274a1d6ec489a097dcdf`
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
# Wed, 11 Dec 2019 22:20:49 GMT
ENV KONG_VERSION=1.4.2
# Wed, 11 Dec 2019 22:20:49 GMT
ARG SU_EXEC_VERSION=0.2
# Wed, 11 Dec 2019 22:20:49 GMT
ARG SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz
# Wed, 11 Dec 2019 22:21:27 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN yum install -y -q gcc make unzip 	&& curl -sL "${SU_EXEC_URL}" | tar -C /tmp -zxf - 	&& make -C "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& cp "/tmp/su-exec-${SU_EXEC_VERSION}/su-exec" /usr/bin 	&& rm -fr "/tmp/su-exec-${SU_EXEC_VERSION}" 	&& yum autoremove -y -q gcc make 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki
# Wed, 11 Dec 2019 22:21:43 GMT
# ARGS: SU_EXEC_URL=https://github.com/ncopa/su-exec/archive/v0.2.tar.gz SU_EXEC_VERSION=0.2
RUN useradd --uid 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm 	&& yum clean all 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 11 Dec 2019 22:21:43 GMT
COPY file:d93f710041d3a08d241deecc7328da1e955b07a618f0d374125d417e8a7e1640 in /docker-entrypoint.sh 
# Wed, 11 Dec 2019 22:21:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:21:44 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 11 Dec 2019 22:21:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Dec 2019 22:21:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4cd0ddf1a96ad908b6bce2a0c4093f0833e6289ead6d3b2aba5b632a1b326a`  
		Last Modified: Wed, 11 Dec 2019 22:23:04 GMT  
		Size: 6.5 MB (6509463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dede93e46215427b107e661256254efe0e21c305ae31e372e7dfe6fea8651038`  
		Last Modified: Wed, 11 Dec 2019 22:23:13 GMT  
		Size: 68.7 MB (68725671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5074025603d1c60b4b7ce8967692bf48eb5fc2f16d80a2bc3b4706530368a9b0`  
		Last Modified: Wed, 11 Dec 2019 22:23:02 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:890a44c18d1f8e8043735b1ce6a607409f575aaf978ce36b923d9b441c0b2e9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:027f0a48dd57f5d8ac06d6d5768807caaa03a2e674c8f5d2abb6e41faaea05ae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44082042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75cf2d6ba0b072e73094e8a1762d102655481daa1b32fd8a6347962f8e4a11f7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:58:07 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Wed, 11 Dec 2019 22:19:48 GMT
ENV KONG_VERSION=1.4.2
# Wed, 11 Dec 2019 22:19:48 GMT
ENV KONG_SHA256=edf917d956d697abb70f5f3f630d420ee699c6428bf953221cd8548eda490dcf
# Wed, 11 Dec 2019 22:19:58 GMT
RUN adduser -Su 1337 kong 	&& mkdir -p "/usr/local/kong" 	&& apk add --no-cache --virtual .build-deps curl wget tar ca-certificates 	&& apk add --no-cache libgcc openssl pcre perl tzdata libcap su-exec zip 	&& wget -O kong.tar.gz "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" 	&& echo "$KONG_SHA256 *kong.tar.gz" | sha256sum -c - 	&& tar -xzf kong.tar.gz -C /tmp 	&& rm -f kong.tar.gz 	&& cp -R /tmp/usr / 	&& rm -rf /tmp/usr 	&& cp -R /tmp/etc / 	&& rm -rf /tmp/etc 	&& apk del .build-deps 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 11 Dec 2019 22:19:58 GMT
COPY file:fe196e90eb453e834bdc492372019ad9f95e35142fa279d1622c213f32592fe9 in /docker-entrypoint.sh 
# Wed, 11 Dec 2019 22:19:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:19:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 11 Dec 2019 22:19:59 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Dec 2019 22:19:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76caeea1403bec7384884ee7560caf82e96cf98cd3d984e3fede3b3c5923b749`  
		Last Modified: Wed, 11 Dec 2019 22:22:42 GMT  
		Size: 41.3 MB (41294312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329f8ea00697d6d19b0113925a9cbf47a7aefc33767bd60045ce24f7efaa02ca`  
		Last Modified: Wed, 11 Dec 2019 22:22:31 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:bf362e56c2fdc82de32afd55a5e8c80b11689985f38bb7c0a2567476ed4fa5b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:a60cf94cd375658c8e79dccccaef18670fe4b234f8db527851f031630083ad57
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81104756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511c55c319378c081f734f2cd21aa0d6e116e8c791f1ea8f81f5bbcca38a8ee5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:51:55 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Thu, 19 Dec 2019 07:51:56 GMT
ENV KONG_VERSION=1.4.2
# Thu, 19 Dec 2019 07:52:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 19 Dec 2019 07:52:18 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 19 Dec 2019 07:52:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:52:19 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 19 Dec 2019 07:52:19 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 07:52:19 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730355a76b4850ee7f9d2f735fcec23e7de250cb6ad9f1c92da08caff919c496`  
		Last Modified: Thu, 19 Dec 2019 07:53:39 GMT  
		Size: 37.0 MB (36979645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea51f27bd020a5b20650a4d577337a5330bf5397f148531a002237f4941ec341`  
		Last Modified: Thu, 19 Dec 2019 07:53:31 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:3b11312ff5566c40f219a964a1c911646ef3a54aa9888542638d2c201054ae71
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76201023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca23b8e72488bac200af48039ef1cf7233e58430279299d47f2562bc37b301a`
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
# Thu, 19 Dec 2019 07:46:45 GMT
ENV KONG_VERSION=1.4.2
# Thu, 19 Dec 2019 07:47:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl 	&& dpkg -i kong.deb 	&& rm -rf kong.deb
# Thu, 19 Dec 2019 07:47:28 GMT
COPY file:a4763218d814cc99d340cb11497461af1e7b06c7ec7d19308fb1d59952ad34a4 in /docker-entrypoint.sh 
# Thu, 19 Dec 2019 07:47:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:47:30 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 19 Dec 2019 07:47:31 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 07:47:32 GMT
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
	-	`sha256:ae187bbfe3d971b97dd69384838f0ceca9b2161f31866a2ba650a82ae734fcf6`  
		Last Modified: Thu, 19 Dec 2019 07:48:54 GMT  
		Size: 36.3 MB (36323826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083cc07e30ff149240e95b3fa7612e0f89e1bfe681379f40081f637f8db06b08`  
		Last Modified: Thu, 19 Dec 2019 07:48:40 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
