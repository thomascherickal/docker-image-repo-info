<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.16`](#emqx4416)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.20`](#emqx5020)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:d0c7a636891e44bfdc8c66697fec9b5cb94675210cb090cffd732a6219ab5284
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:b594671f1c8c001b76971e896ec29f4aea1b4ce35e471f418b7e190d66bdfe8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81272225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df18f1b36fce0936fd74b9faf314e3a01d83c037091286efb92131b581fe822`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 23 Mar 2023 06:38:30 GMT
ENV EMQX_VERSION=4.4.16
# Thu, 23 Mar 2023 06:38:30 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 23 Mar 2023 06:38:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 23 Mar 2023 06:38:34 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:35 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:35 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:35 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 23 Mar 2023 06:38:35 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:35 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:35 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7216294cbe2d1311e293a82d22eb3f71da435b2b9bb7ad9900eaaeb14d68d2b7`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 2.6 MB (2569460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca85a7d40cdb8392bb213cc3b9efc98bcb416df588c86b55eb174485340016cb`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93644246d8ba201ec9c154bf77410efda76bbc02af25c4d8c89b5bef6aa7e90e`  
		Last Modified: Thu, 23 Mar 2023 06:39:05 GMT  
		Size: 47.3 MB (47286145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1172e73e519b49b8ecabc31cf1807694cf854572647611963d00191e5c03612`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:5077868044732549104a37735bbeb9eeea04990428ec84565089b9f912a27b4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72700174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b721a7424bef3c917f99584f6ede9bdd469bf8bf89ca3187bf5fd2fa3f563f5c`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:40 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:22:40 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 23 Mar 2023 07:22:40 GMT
ENV EMQX_VERSION=4.4.16
# Thu, 23 Mar 2023 07:22:40 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 23 Mar 2023 07:22:44 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 23 Mar 2023 07:22:44 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 07:22:44 GMT
USER emqx
# Thu, 23 Mar 2023 07:22:45 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 07:22:45 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 23 Mar 2023 07:22:45 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 23 Mar 2023 07:22:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:22:45 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a2fca160acd6916ee9f7a44af39ca048ec3dba62c3d8276915f397320d937d`  
		Last Modified: Thu, 23 Mar 2023 07:23:07 GMT  
		Size: 2.6 MB (2559254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602fe4683989e6650cbe1071564b8e4029b4eacf0814ee226b81bfa86c6df9fe`  
		Last Modified: Thu, 23 Mar 2023 07:23:07 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4d7f2460db59baf21229445904a5c93abb98a720847d234328af163a73069b`  
		Last Modified: Thu, 23 Mar 2023 07:23:10 GMT  
		Size: 40.1 MB (40073001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b619deebd0c236156f78632f97bd2738a18a1a8edf1e4cabdeb0d403c57810db`  
		Last Modified: Thu, 23 Mar 2023 07:23:07 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:d0c7a636891e44bfdc8c66697fec9b5cb94675210cb090cffd732a6219ab5284
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:b594671f1c8c001b76971e896ec29f4aea1b4ce35e471f418b7e190d66bdfe8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81272225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df18f1b36fce0936fd74b9faf314e3a01d83c037091286efb92131b581fe822`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 23 Mar 2023 06:38:30 GMT
ENV EMQX_VERSION=4.4.16
# Thu, 23 Mar 2023 06:38:30 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 23 Mar 2023 06:38:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 23 Mar 2023 06:38:34 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:35 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:35 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:35 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 23 Mar 2023 06:38:35 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:35 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:35 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7216294cbe2d1311e293a82d22eb3f71da435b2b9bb7ad9900eaaeb14d68d2b7`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 2.6 MB (2569460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca85a7d40cdb8392bb213cc3b9efc98bcb416df588c86b55eb174485340016cb`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93644246d8ba201ec9c154bf77410efda76bbc02af25c4d8c89b5bef6aa7e90e`  
		Last Modified: Thu, 23 Mar 2023 06:39:05 GMT  
		Size: 47.3 MB (47286145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1172e73e519b49b8ecabc31cf1807694cf854572647611963d00191e5c03612`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:5077868044732549104a37735bbeb9eeea04990428ec84565089b9f912a27b4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72700174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b721a7424bef3c917f99584f6ede9bdd469bf8bf89ca3187bf5fd2fa3f563f5c`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:40 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:22:40 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 23 Mar 2023 07:22:40 GMT
ENV EMQX_VERSION=4.4.16
# Thu, 23 Mar 2023 07:22:40 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 23 Mar 2023 07:22:44 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 23 Mar 2023 07:22:44 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 07:22:44 GMT
USER emqx
# Thu, 23 Mar 2023 07:22:45 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 07:22:45 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 23 Mar 2023 07:22:45 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 23 Mar 2023 07:22:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:22:45 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a2fca160acd6916ee9f7a44af39ca048ec3dba62c3d8276915f397320d937d`  
		Last Modified: Thu, 23 Mar 2023 07:23:07 GMT  
		Size: 2.6 MB (2559254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602fe4683989e6650cbe1071564b8e4029b4eacf0814ee226b81bfa86c6df9fe`  
		Last Modified: Thu, 23 Mar 2023 07:23:07 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4d7f2460db59baf21229445904a5c93abb98a720847d234328af163a73069b`  
		Last Modified: Thu, 23 Mar 2023 07:23:10 GMT  
		Size: 40.1 MB (40073001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b619deebd0c236156f78632f97bd2738a18a1a8edf1e4cabdeb0d403c57810db`  
		Last Modified: Thu, 23 Mar 2023 07:23:07 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.16`

```console
$ docker pull emqx@sha256:d0c7a636891e44bfdc8c66697fec9b5cb94675210cb090cffd732a6219ab5284
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.16` - linux; amd64

```console
$ docker pull emqx@sha256:b594671f1c8c001b76971e896ec29f4aea1b4ce35e471f418b7e190d66bdfe8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81272225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df18f1b36fce0936fd74b9faf314e3a01d83c037091286efb92131b581fe822`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 23 Mar 2023 06:38:30 GMT
ENV EMQX_VERSION=4.4.16
# Thu, 23 Mar 2023 06:38:30 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 23 Mar 2023 06:38:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 23 Mar 2023 06:38:34 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:35 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:35 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:35 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 23 Mar 2023 06:38:35 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:35 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:35 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7216294cbe2d1311e293a82d22eb3f71da435b2b9bb7ad9900eaaeb14d68d2b7`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 2.6 MB (2569460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca85a7d40cdb8392bb213cc3b9efc98bcb416df588c86b55eb174485340016cb`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93644246d8ba201ec9c154bf77410efda76bbc02af25c4d8c89b5bef6aa7e90e`  
		Last Modified: Thu, 23 Mar 2023 06:39:05 GMT  
		Size: 47.3 MB (47286145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1172e73e519b49b8ecabc31cf1807694cf854572647611963d00191e5c03612`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.16` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:5077868044732549104a37735bbeb9eeea04990428ec84565089b9f912a27b4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72700174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b721a7424bef3c917f99584f6ede9bdd469bf8bf89ca3187bf5fd2fa3f563f5c`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:40 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:22:40 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 23 Mar 2023 07:22:40 GMT
ENV EMQX_VERSION=4.4.16
# Thu, 23 Mar 2023 07:22:40 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 23 Mar 2023 07:22:44 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 23 Mar 2023 07:22:44 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 07:22:44 GMT
USER emqx
# Thu, 23 Mar 2023 07:22:45 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 07:22:45 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 23 Mar 2023 07:22:45 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 23 Mar 2023 07:22:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:22:45 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a2fca160acd6916ee9f7a44af39ca048ec3dba62c3d8276915f397320d937d`  
		Last Modified: Thu, 23 Mar 2023 07:23:07 GMT  
		Size: 2.6 MB (2559254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602fe4683989e6650cbe1071564b8e4029b4eacf0814ee226b81bfa86c6df9fe`  
		Last Modified: Thu, 23 Mar 2023 07:23:07 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4d7f2460db59baf21229445904a5c93abb98a720847d234328af163a73069b`  
		Last Modified: Thu, 23 Mar 2023 07:23:10 GMT  
		Size: 40.1 MB (40073001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b619deebd0c236156f78632f97bd2738a18a1a8edf1e4cabdeb0d403c57810db`  
		Last Modified: Thu, 23 Mar 2023 07:23:07 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:21e51fb5166e95b30c99a3db4caaaaba01c3f348dccebc8b8eaf9917be16f0bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:db94e86eb5708484aab7d72866c3d1b818f7e42dede79087db3b8336b42a0e4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d1da644611bb001ea426cb7a35d17c79f355acbf8da9596e94eb45f573f24a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:43 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:44 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 06:38:44 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 06:38:44 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 06:38:44 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 06:38:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 06:38:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 06:38:50 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:50 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 06:38:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad234a8e621d243ffc2889b413a9971003cc42ee7ba32a7ac16473122c6d6364`  
		Last Modified: Thu, 23 Mar 2023 06:39:16 GMT  
		Size: 3.0 MB (2987658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e02c887fbcfd1b399b200e621a473094afcaf8febe6e035caf150ebf9136c32`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ae335101f863f32be81ae4b486dcc876bf277f52d0b0494d63afec80df7254`  
		Last Modified: Thu, 23 Mar 2023 06:39:23 GMT  
		Size: 66.8 MB (66809463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77081c8225be9c363811f449115fd687c67abcb09ab1dcd47bd66bedf39998ff`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:6a1b1c6ce45d16021a9f7918304c06944c18c74bed427e48bb9e8b765febbc32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b283d91c28a2acbf3e64a9a80c4f0f01870a6d67017851a02375a1b143ed73a2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:22:52 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 07:22:52 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 07:22:52 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 07:22:52 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 07:22:52 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 07:22:56 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 07:22:57 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 07:22:57 GMT
USER emqx
# Thu, 23 Mar 2023 07:22:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 07:22:57 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 07:22:57 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 07:22:57 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:22:57 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32acc0199b24e0cbce1256b7b9514920ac6dedaed2a2ee404a0957d036012bc`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 3.0 MB (3002755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a325419b9b6ebe9519e9bc7472f523d98e68e6d85caf8a71f9faca4312e840`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dbcf1d13c0e388979d7b8bcc5fdf8bf3fe726f66acc75db68c05d6e95ed960`  
		Last Modified: Thu, 23 Mar 2023 07:23:27 GMT  
		Size: 59.2 MB (59233253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707cf29e287e7364281910e03782cba6bbaae6644b6c17e6b092b7f59e7a8fad`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:21e51fb5166e95b30c99a3db4caaaaba01c3f348dccebc8b8eaf9917be16f0bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:db94e86eb5708484aab7d72866c3d1b818f7e42dede79087db3b8336b42a0e4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d1da644611bb001ea426cb7a35d17c79f355acbf8da9596e94eb45f573f24a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:43 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:44 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 06:38:44 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 06:38:44 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 06:38:44 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 06:38:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 06:38:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 06:38:50 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:50 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 06:38:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad234a8e621d243ffc2889b413a9971003cc42ee7ba32a7ac16473122c6d6364`  
		Last Modified: Thu, 23 Mar 2023 06:39:16 GMT  
		Size: 3.0 MB (2987658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e02c887fbcfd1b399b200e621a473094afcaf8febe6e035caf150ebf9136c32`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ae335101f863f32be81ae4b486dcc876bf277f52d0b0494d63afec80df7254`  
		Last Modified: Thu, 23 Mar 2023 06:39:23 GMT  
		Size: 66.8 MB (66809463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77081c8225be9c363811f449115fd687c67abcb09ab1dcd47bd66bedf39998ff`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:6a1b1c6ce45d16021a9f7918304c06944c18c74bed427e48bb9e8b765febbc32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b283d91c28a2acbf3e64a9a80c4f0f01870a6d67017851a02375a1b143ed73a2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:22:52 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 07:22:52 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 07:22:52 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 07:22:52 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 07:22:52 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 07:22:56 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 07:22:57 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 07:22:57 GMT
USER emqx
# Thu, 23 Mar 2023 07:22:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 07:22:57 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 07:22:57 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 07:22:57 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:22:57 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32acc0199b24e0cbce1256b7b9514920ac6dedaed2a2ee404a0957d036012bc`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 3.0 MB (3002755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a325419b9b6ebe9519e9bc7472f523d98e68e6d85caf8a71f9faca4312e840`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dbcf1d13c0e388979d7b8bcc5fdf8bf3fe726f66acc75db68c05d6e95ed960`  
		Last Modified: Thu, 23 Mar 2023 07:23:27 GMT  
		Size: 59.2 MB (59233253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707cf29e287e7364281910e03782cba6bbaae6644b6c17e6b092b7f59e7a8fad`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.20`

```console
$ docker pull emqx@sha256:21e51fb5166e95b30c99a3db4caaaaba01c3f348dccebc8b8eaf9917be16f0bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.20` - linux; amd64

```console
$ docker pull emqx@sha256:db94e86eb5708484aab7d72866c3d1b818f7e42dede79087db3b8336b42a0e4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d1da644611bb001ea426cb7a35d17c79f355acbf8da9596e94eb45f573f24a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:43 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:44 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 06:38:44 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 06:38:44 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 06:38:44 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 06:38:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 06:38:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 06:38:50 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:50 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 06:38:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad234a8e621d243ffc2889b413a9971003cc42ee7ba32a7ac16473122c6d6364`  
		Last Modified: Thu, 23 Mar 2023 06:39:16 GMT  
		Size: 3.0 MB (2987658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e02c887fbcfd1b399b200e621a473094afcaf8febe6e035caf150ebf9136c32`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ae335101f863f32be81ae4b486dcc876bf277f52d0b0494d63afec80df7254`  
		Last Modified: Thu, 23 Mar 2023 06:39:23 GMT  
		Size: 66.8 MB (66809463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77081c8225be9c363811f449115fd687c67abcb09ab1dcd47bd66bedf39998ff`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.20` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:6a1b1c6ce45d16021a9f7918304c06944c18c74bed427e48bb9e8b765febbc32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b283d91c28a2acbf3e64a9a80c4f0f01870a6d67017851a02375a1b143ed73a2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:22:52 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 07:22:52 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 07:22:52 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 07:22:52 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 07:22:52 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 07:22:56 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 07:22:57 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 07:22:57 GMT
USER emqx
# Thu, 23 Mar 2023 07:22:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 07:22:57 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 07:22:57 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 07:22:57 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:22:57 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32acc0199b24e0cbce1256b7b9514920ac6dedaed2a2ee404a0957d036012bc`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 3.0 MB (3002755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a325419b9b6ebe9519e9bc7472f523d98e68e6d85caf8a71f9faca4312e840`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dbcf1d13c0e388979d7b8bcc5fdf8bf3fe726f66acc75db68c05d6e95ed960`  
		Last Modified: Thu, 23 Mar 2023 07:23:27 GMT  
		Size: 59.2 MB (59233253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707cf29e287e7364281910e03782cba6bbaae6644b6c17e6b092b7f59e7a8fad`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:21e51fb5166e95b30c99a3db4caaaaba01c3f348dccebc8b8eaf9917be16f0bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:db94e86eb5708484aab7d72866c3d1b818f7e42dede79087db3b8336b42a0e4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d1da644611bb001ea426cb7a35d17c79f355acbf8da9596e94eb45f573f24a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:43 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:44 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 06:38:44 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 06:38:44 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 06:38:44 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 06:38:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 06:38:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 06:38:50 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:50 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 06:38:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad234a8e621d243ffc2889b413a9971003cc42ee7ba32a7ac16473122c6d6364`  
		Last Modified: Thu, 23 Mar 2023 06:39:16 GMT  
		Size: 3.0 MB (2987658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e02c887fbcfd1b399b200e621a473094afcaf8febe6e035caf150ebf9136c32`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ae335101f863f32be81ae4b486dcc876bf277f52d0b0494d63afec80df7254`  
		Last Modified: Thu, 23 Mar 2023 06:39:23 GMT  
		Size: 66.8 MB (66809463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77081c8225be9c363811f449115fd687c67abcb09ab1dcd47bd66bedf39998ff`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:6a1b1c6ce45d16021a9f7918304c06944c18c74bed427e48bb9e8b765febbc32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b283d91c28a2acbf3e64a9a80c4f0f01870a6d67017851a02375a1b143ed73a2`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:22:52 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 07:22:52 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 07:22:52 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 07:22:52 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 07:22:52 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 07:22:56 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 07:22:57 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 07:22:57 GMT
USER emqx
# Thu, 23 Mar 2023 07:22:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 07:22:57 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 07:22:57 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 07:22:57 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:22:57 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32acc0199b24e0cbce1256b7b9514920ac6dedaed2a2ee404a0957d036012bc`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 3.0 MB (3002755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a325419b9b6ebe9519e9bc7472f523d98e68e6d85caf8a71f9faca4312e840`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dbcf1d13c0e388979d7b8bcc5fdf8bf3fe726f66acc75db68c05d6e95ed960`  
		Last Modified: Thu, 23 Mar 2023 07:23:27 GMT  
		Size: 59.2 MB (59233253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707cf29e287e7364281910e03782cba6bbaae6644b6c17e6b092b7f59e7a8fad`  
		Last Modified: Thu, 23 Mar 2023 07:23:22 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
