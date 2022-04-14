<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.3`](#emqx43)
-	[`emqx:4.3.5`](#emqx435)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.2`](#emqx442)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:674040ad1e81136a848a502cdd3243ea4b243f7e227f123f2d942cb161619ac5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:a8cc1a6f9de8145267bea9777b9d7453f010b83f8412fb2e004793026957c446
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124617702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ec0eaa49dfce198abeaf6ab0180be6228c91cc5cc2264c224aee71d806be5f`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Thu, 14 Apr 2022 09:12:19 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 14 Apr 2022 09:12:19 GMT
ENV EMQX_VERSION=4.4.2
# Thu, 14 Apr 2022 09:12:19 GMT
ENV OTP=otp24.1.5-3
# Thu, 14 Apr 2022 09:12:25 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bbeb72effcbebab56a3331bdd51dbf5810121d9b2bc57a294d49e97bd9eed7f4"; fi;     if [ ${arch} = "arm64" ]; then sha256="13f6bc6b218f837bb8e7353e5470190152a8c8e19780762ad7fd0c828ef6fb29"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 14 Apr 2022 09:12:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Thu, 14 Apr 2022 09:12:31 GMT
WORKDIR /opt/emqx
# Thu, 14 Apr 2022 09:12:31 GMT
USER emqx
# Thu, 14 Apr 2022 09:12:31 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 14 Apr 2022 09:12:31 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 14 Apr 2022 09:12:31 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 14 Apr 2022 09:12:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 14 Apr 2022 09:12:31 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068c806eafc5202639c9aeed78d1ec82a48363e23a00846069bfcb7329e8fb71`  
		Last Modified: Thu, 14 Apr 2022 09:12:58 GMT  
		Size: 2.6 MB (2568082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ada06505b015d27cb80de131937085cfff3c1cec4e8190472ced4bb7c932c32`  
		Last Modified: Thu, 14 Apr 2022 09:13:02 GMT  
		Size: 45.3 MB (45333522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1c8ec051c937b294f60cf7f6e6c9d3f0770643d8021526ca4f58a51d018743`  
		Last Modified: Thu, 14 Apr 2022 09:13:03 GMT  
		Size: 45.3 MB (45336534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f95c9f02012412fe4621b0ecf035dc4443efbd8cc7ed6dd4d3df124df3c196a`  
		Last Modified: Thu, 14 Apr 2022 09:12:57 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3`

```console
$ docker pull emqx@sha256:bc8c36461462878775d5980bb94ba1b1ae9d9b74dc4fb90db80322ad3ad13d60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `emqx:4.3` - linux; amd64

```console
$ docker pull emqx@sha256:81ad1435ca97ae2f64d192f9341a4d61b1d9c1a90ba49f9a19fc1f8314ea3bd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62039120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06d653ff9517b9585af0ba815d1d5e0d68c5bef071cfbc5aa67b3cfe0e2a527c`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Thu, 14 Apr 2022 09:11:51 GMT
RUN groupadd -r -g 1000 emqx && useradd -r -m -u 1000 -g emqx emqx
# Thu, 14 Apr 2022 09:11:59 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates curl gnupg;     rm -rf /var/lib/apt/lists/*
# Thu, 14 Apr 2022 09:12:00 GMT
RUN set -eu;     key='FC841BA637755CA8487B1E3CC0B409463E640D53';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key";     mkdir -p /etc/apt/keyrings;     gpg --batch --export "$key" > /etc/apt/keyrings/emqx.gpg;     gpgconf --kill all;     rm -rf "$GNUPGHOME"
# Thu, 14 Apr 2022 09:12:00 GMT
ENV EMQX_VERSION=4.3.5
# Thu, 14 Apr 2022 09:12:09 GMT
RUN set -eu;     echo "deb [signed-by=/etc/apt/keyrings/emqx.gpg] https://repos.emqx.io/emqx-ce/deb/debian/ ./buster stable" >> /etc/apt/sources.list.d/emqx.list;     apt-get update;     apt-get install -y --no-install-recommends emqx="$EMQX_VERSION";     rm -rf /var/lib/apt/lists/*
# Thu, 14 Apr 2022 09:12:09 GMT
USER emqx
# Thu, 14 Apr 2022 09:12:09 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 14 Apr 2022 09:12:09 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Thu, 14 Apr 2022 09:12:09 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 14 Apr 2022 09:12:09 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb2859296bb6dba418da3361e6f3e12216aa0bd4dead25ac4c3a336a6e21432`  
		Last Modified: Thu, 14 Apr 2022 09:12:45 GMT  
		Size: 4.1 KB (4107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3598cc936079f566e21afe875e0b476ffb91aa9c857c9cc28b27e79a2c90d`  
		Last Modified: Thu, 14 Apr 2022 09:12:46 GMT  
		Size: 8.1 MB (8141559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059c60539660f9a5afcec1dccf67d27660ab39c5360c1f81d1841cfcca70d7ff`  
		Last Modified: Thu, 14 Apr 2022 09:12:45 GMT  
		Size: 874.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d921822e61450e819e6ab0043f0eda362c0e5af66f8910bf2bd581828b3190`  
		Last Modified: Thu, 14 Apr 2022 09:12:48 GMT  
		Size: 26.7 MB (26739570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449961cf15db2100119a0f9c073d68ec0d1b6ecd324f61fb09d951beebeb97b8`  
		Last Modified: Thu, 14 Apr 2022 09:12:45 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3.5`

```console
$ docker pull emqx@sha256:bc8c36461462878775d5980bb94ba1b1ae9d9b74dc4fb90db80322ad3ad13d60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `emqx:4.3.5` - linux; amd64

```console
$ docker pull emqx@sha256:81ad1435ca97ae2f64d192f9341a4d61b1d9c1a90ba49f9a19fc1f8314ea3bd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62039120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06d653ff9517b9585af0ba815d1d5e0d68c5bef071cfbc5aa67b3cfe0e2a527c`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Thu, 14 Apr 2022 09:11:51 GMT
RUN groupadd -r -g 1000 emqx && useradd -r -m -u 1000 -g emqx emqx
# Thu, 14 Apr 2022 09:11:59 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates curl gnupg;     rm -rf /var/lib/apt/lists/*
# Thu, 14 Apr 2022 09:12:00 GMT
RUN set -eu;     key='FC841BA637755CA8487B1E3CC0B409463E640D53';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key";     mkdir -p /etc/apt/keyrings;     gpg --batch --export "$key" > /etc/apt/keyrings/emqx.gpg;     gpgconf --kill all;     rm -rf "$GNUPGHOME"
# Thu, 14 Apr 2022 09:12:00 GMT
ENV EMQX_VERSION=4.3.5
# Thu, 14 Apr 2022 09:12:09 GMT
RUN set -eu;     echo "deb [signed-by=/etc/apt/keyrings/emqx.gpg] https://repos.emqx.io/emqx-ce/deb/debian/ ./buster stable" >> /etc/apt/sources.list.d/emqx.list;     apt-get update;     apt-get install -y --no-install-recommends emqx="$EMQX_VERSION";     rm -rf /var/lib/apt/lists/*
# Thu, 14 Apr 2022 09:12:09 GMT
USER emqx
# Thu, 14 Apr 2022 09:12:09 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 14 Apr 2022 09:12:09 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Thu, 14 Apr 2022 09:12:09 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 14 Apr 2022 09:12:09 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb2859296bb6dba418da3361e6f3e12216aa0bd4dead25ac4c3a336a6e21432`  
		Last Modified: Thu, 14 Apr 2022 09:12:45 GMT  
		Size: 4.1 KB (4107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3598cc936079f566e21afe875e0b476ffb91aa9c857c9cc28b27e79a2c90d`  
		Last Modified: Thu, 14 Apr 2022 09:12:46 GMT  
		Size: 8.1 MB (8141559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059c60539660f9a5afcec1dccf67d27660ab39c5360c1f81d1841cfcca70d7ff`  
		Last Modified: Thu, 14 Apr 2022 09:12:45 GMT  
		Size: 874.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d921822e61450e819e6ab0043f0eda362c0e5af66f8910bf2bd581828b3190`  
		Last Modified: Thu, 14 Apr 2022 09:12:48 GMT  
		Size: 26.7 MB (26739570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449961cf15db2100119a0f9c073d68ec0d1b6ecd324f61fb09d951beebeb97b8`  
		Last Modified: Thu, 14 Apr 2022 09:12:45 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:674040ad1e81136a848a502cdd3243ea4b243f7e227f123f2d942cb161619ac5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:a8cc1a6f9de8145267bea9777b9d7453f010b83f8412fb2e004793026957c446
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124617702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ec0eaa49dfce198abeaf6ab0180be6228c91cc5cc2264c224aee71d806be5f`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Thu, 14 Apr 2022 09:12:19 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 14 Apr 2022 09:12:19 GMT
ENV EMQX_VERSION=4.4.2
# Thu, 14 Apr 2022 09:12:19 GMT
ENV OTP=otp24.1.5-3
# Thu, 14 Apr 2022 09:12:25 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bbeb72effcbebab56a3331bdd51dbf5810121d9b2bc57a294d49e97bd9eed7f4"; fi;     if [ ${arch} = "arm64" ]; then sha256="13f6bc6b218f837bb8e7353e5470190152a8c8e19780762ad7fd0c828ef6fb29"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 14 Apr 2022 09:12:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Thu, 14 Apr 2022 09:12:31 GMT
WORKDIR /opt/emqx
# Thu, 14 Apr 2022 09:12:31 GMT
USER emqx
# Thu, 14 Apr 2022 09:12:31 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 14 Apr 2022 09:12:31 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 14 Apr 2022 09:12:31 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 14 Apr 2022 09:12:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 14 Apr 2022 09:12:31 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068c806eafc5202639c9aeed78d1ec82a48363e23a00846069bfcb7329e8fb71`  
		Last Modified: Thu, 14 Apr 2022 09:12:58 GMT  
		Size: 2.6 MB (2568082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ada06505b015d27cb80de131937085cfff3c1cec4e8190472ced4bb7c932c32`  
		Last Modified: Thu, 14 Apr 2022 09:13:02 GMT  
		Size: 45.3 MB (45333522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1c8ec051c937b294f60cf7f6e6c9d3f0770643d8021526ca4f58a51d018743`  
		Last Modified: Thu, 14 Apr 2022 09:13:03 GMT  
		Size: 45.3 MB (45336534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f95c9f02012412fe4621b0ecf035dc4443efbd8cc7ed6dd4d3df124df3c196a`  
		Last Modified: Thu, 14 Apr 2022 09:12:57 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.2`

```console
$ docker pull emqx@sha256:674040ad1e81136a848a502cdd3243ea4b243f7e227f123f2d942cb161619ac5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `emqx:4.4.2` - linux; amd64

```console
$ docker pull emqx@sha256:a8cc1a6f9de8145267bea9777b9d7453f010b83f8412fb2e004793026957c446
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124617702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ec0eaa49dfce198abeaf6ab0180be6228c91cc5cc2264c224aee71d806be5f`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Thu, 14 Apr 2022 09:12:19 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 14 Apr 2022 09:12:19 GMT
ENV EMQX_VERSION=4.4.2
# Thu, 14 Apr 2022 09:12:19 GMT
ENV OTP=otp24.1.5-3
# Thu, 14 Apr 2022 09:12:25 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bbeb72effcbebab56a3331bdd51dbf5810121d9b2bc57a294d49e97bd9eed7f4"; fi;     if [ ${arch} = "arm64" ]; then sha256="13f6bc6b218f837bb8e7353e5470190152a8c8e19780762ad7fd0c828ef6fb29"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 14 Apr 2022 09:12:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Thu, 14 Apr 2022 09:12:31 GMT
WORKDIR /opt/emqx
# Thu, 14 Apr 2022 09:12:31 GMT
USER emqx
# Thu, 14 Apr 2022 09:12:31 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 14 Apr 2022 09:12:31 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 14 Apr 2022 09:12:31 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 14 Apr 2022 09:12:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 14 Apr 2022 09:12:31 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068c806eafc5202639c9aeed78d1ec82a48363e23a00846069bfcb7329e8fb71`  
		Last Modified: Thu, 14 Apr 2022 09:12:58 GMT  
		Size: 2.6 MB (2568082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ada06505b015d27cb80de131937085cfff3c1cec4e8190472ced4bb7c932c32`  
		Last Modified: Thu, 14 Apr 2022 09:13:02 GMT  
		Size: 45.3 MB (45333522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1c8ec051c937b294f60cf7f6e6c9d3f0770643d8021526ca4f58a51d018743`  
		Last Modified: Thu, 14 Apr 2022 09:13:03 GMT  
		Size: 45.3 MB (45336534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f95c9f02012412fe4621b0ecf035dc4443efbd8cc7ed6dd4d3df124df3c196a`  
		Last Modified: Thu, 14 Apr 2022 09:12:57 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:674040ad1e81136a848a502cdd3243ea4b243f7e227f123f2d942cb161619ac5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:a8cc1a6f9de8145267bea9777b9d7453f010b83f8412fb2e004793026957c446
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124617702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ec0eaa49dfce198abeaf6ab0180be6228c91cc5cc2264c224aee71d806be5f`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Thu, 14 Apr 2022 09:12:19 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 14 Apr 2022 09:12:19 GMT
ENV EMQX_VERSION=4.4.2
# Thu, 14 Apr 2022 09:12:19 GMT
ENV OTP=otp24.1.5-3
# Thu, 14 Apr 2022 09:12:25 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="bbeb72effcbebab56a3331bdd51dbf5810121d9b2bc57a294d49e97bd9eed7f4"; fi;     if [ ${arch} = "arm64" ]; then sha256="13f6bc6b218f837bb8e7353e5470190152a8c8e19780762ad7fd0c828ef6fb29"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 14 Apr 2022 09:12:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Thu, 14 Apr 2022 09:12:31 GMT
WORKDIR /opt/emqx
# Thu, 14 Apr 2022 09:12:31 GMT
USER emqx
# Thu, 14 Apr 2022 09:12:31 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 14 Apr 2022 09:12:31 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 14 Apr 2022 09:12:31 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 14 Apr 2022 09:12:31 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 14 Apr 2022 09:12:31 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068c806eafc5202639c9aeed78d1ec82a48363e23a00846069bfcb7329e8fb71`  
		Last Modified: Thu, 14 Apr 2022 09:12:58 GMT  
		Size: 2.6 MB (2568082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ada06505b015d27cb80de131937085cfff3c1cec4e8190472ced4bb7c932c32`  
		Last Modified: Thu, 14 Apr 2022 09:13:02 GMT  
		Size: 45.3 MB (45333522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1c8ec051c937b294f60cf7f6e6c9d3f0770643d8021526ca4f58a51d018743`  
		Last Modified: Thu, 14 Apr 2022 09:13:03 GMT  
		Size: 45.3 MB (45336534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f95c9f02012412fe4621b0ecf035dc4443efbd8cc7ed6dd4d3df124df3c196a`  
		Last Modified: Thu, 14 Apr 2022 09:12:57 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
