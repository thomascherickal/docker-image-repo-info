<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `api-firewall`

-	[`api-firewall:0.6.7`](#api-firewall067)
-	[`api-firewall:latest`](#api-firewalllatest)

## `api-firewall:0.6.7`

```console
$ docker pull api-firewall@sha256:3a1e672d843f78eab86ab17ddf18b4146ad183f8013d18e747c6ce41a7b1ada0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `api-firewall:0.6.7` - linux; amd64

```console
$ docker pull api-firewall@sha256:83ed14689034abc3c4381d92370ff5e4201bd859ee352cb82be635abdab1be93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7489394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f16c75595e1395e903a0443ba772cb948f2bce5e89096d90c11791eeae67e17a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 15:51:27 GMT
ENV APIFW_PATH=/opt/api-firewall
# Wed, 23 Mar 2022 15:51:27 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 15:51:27 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Wed, 23 Mar 2022 15:51:27 GMT
ENV APIFIREWALL_VERSION=v0.6.7
# Wed, 23 Mar 2022 15:51:29 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='fb61a3ca620340a76f97856ec30190de8422535c31d17ddc89019e87825d60b9';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='cdcd6679536e3e0fa0d5cdd8f422ef58f31f65c2d279228150c269c32641dd1d';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='0850d87b52624085265554605f46df5cda2a006d7b9dc9a7d369cdb9c9c88305';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Wed, 23 Mar 2022 15:51:30 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Wed, 23 Mar 2022 15:51:30 GMT
USER api-firewall
# Wed, 23 Mar 2022 15:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 15:51:30 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acceb8967e1e5a926749f5453b82fe09da548f422086fbff568c09427ab6917`  
		Last Modified: Wed, 23 Mar 2022 15:51:39 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de295fbc973b9190b81c015200c511fba4ae6a13329275614cae3a4076fae766`  
		Last Modified: Wed, 23 Mar 2022 15:51:40 GMT  
		Size: 4.7 MB (4675150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f48b6692cbc1fa2d797dab19fabfa923b5505bb4f7ba378966f7db5c8934134`  
		Last Modified: Wed, 23 Mar 2022 15:51:39 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:0.6.7` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:ddbe6fa4ab911657b7563fb88b15dc3b626e50fb1b01cb12ebd797eaae35791c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7102437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694ea1588584010e1581cdf1bea4a992306b0f409aed7df4e27ab0f3017fa037`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:02:36 GMT
ENV APIFW_PATH=/opt/api-firewall
# Thu, 24 Mar 2022 05:02:37 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 05:02:38 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Thu, 24 Mar 2022 05:02:39 GMT
ENV APIFIREWALL_VERSION=v0.6.7
# Thu, 24 Mar 2022 05:02:41 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='fb61a3ca620340a76f97856ec30190de8422535c31d17ddc89019e87825d60b9';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='cdcd6679536e3e0fa0d5cdd8f422ef58f31f65c2d279228150c269c32641dd1d';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='0850d87b52624085265554605f46df5cda2a006d7b9dc9a7d369cdb9c9c88305';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Thu, 24 Mar 2022 05:02:43 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Thu, 24 Mar 2022 05:02:43 GMT
USER api-firewall
# Thu, 24 Mar 2022 05:02:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:02:45 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd599eb1df02a34b9fa6b4abd3b0640e3935fcd2354982171ee4c89328c7410`  
		Last Modified: Thu, 24 Mar 2022 05:02:58 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff902ec5fe8af4f757845619ee7cf92cd1397cf07b467611c1a1ed6d8e9b0964`  
		Last Modified: Thu, 24 Mar 2022 05:02:59 GMT  
		Size: 4.4 MB (4386160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9273607dfcab1fec447db73e4e9cd486dd0884b29aa8d0c7bcb4e1242bd9c5f`  
		Last Modified: Thu, 24 Mar 2022 05:02:58 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `api-firewall:latest`

```console
$ docker pull api-firewall@sha256:3a1e672d843f78eab86ab17ddf18b4146ad183f8013d18e747c6ce41a7b1ada0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `api-firewall:latest` - linux; amd64

```console
$ docker pull api-firewall@sha256:83ed14689034abc3c4381d92370ff5e4201bd859ee352cb82be635abdab1be93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7489394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f16c75595e1395e903a0443ba772cb948f2bce5e89096d90c11791eeae67e17a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 15:51:27 GMT
ENV APIFW_PATH=/opt/api-firewall
# Wed, 23 Mar 2022 15:51:27 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 15:51:27 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Wed, 23 Mar 2022 15:51:27 GMT
ENV APIFIREWALL_VERSION=v0.6.7
# Wed, 23 Mar 2022 15:51:29 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='fb61a3ca620340a76f97856ec30190de8422535c31d17ddc89019e87825d60b9';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='cdcd6679536e3e0fa0d5cdd8f422ef58f31f65c2d279228150c269c32641dd1d';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='0850d87b52624085265554605f46df5cda2a006d7b9dc9a7d369cdb9c9c88305';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Wed, 23 Mar 2022 15:51:30 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Wed, 23 Mar 2022 15:51:30 GMT
USER api-firewall
# Wed, 23 Mar 2022 15:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 15:51:30 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acceb8967e1e5a926749f5453b82fe09da548f422086fbff568c09427ab6917`  
		Last Modified: Wed, 23 Mar 2022 15:51:39 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de295fbc973b9190b81c015200c511fba4ae6a13329275614cae3a4076fae766`  
		Last Modified: Wed, 23 Mar 2022 15:51:40 GMT  
		Size: 4.7 MB (4675150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f48b6692cbc1fa2d797dab19fabfa923b5505bb4f7ba378966f7db5c8934134`  
		Last Modified: Wed, 23 Mar 2022 15:51:39 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:ddbe6fa4ab911657b7563fb88b15dc3b626e50fb1b01cb12ebd797eaae35791c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7102437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694ea1588584010e1581cdf1bea4a992306b0f409aed7df4e27ab0f3017fa037`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:02:36 GMT
ENV APIFW_PATH=/opt/api-firewall
# Thu, 24 Mar 2022 05:02:37 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 05:02:38 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Thu, 24 Mar 2022 05:02:39 GMT
ENV APIFIREWALL_VERSION=v0.6.7
# Thu, 24 Mar 2022 05:02:41 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='fb61a3ca620340a76f97856ec30190de8422535c31d17ddc89019e87825d60b9';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='cdcd6679536e3e0fa0d5cdd8f422ef58f31f65c2d279228150c269c32641dd1d';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='0850d87b52624085265554605f46df5cda2a006d7b9dc9a7d369cdb9c9c88305';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Thu, 24 Mar 2022 05:02:43 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Thu, 24 Mar 2022 05:02:43 GMT
USER api-firewall
# Thu, 24 Mar 2022 05:02:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:02:45 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd599eb1df02a34b9fa6b4abd3b0640e3935fcd2354982171ee4c89328c7410`  
		Last Modified: Thu, 24 Mar 2022 05:02:58 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff902ec5fe8af4f757845619ee7cf92cd1397cf07b467611c1a1ed6d8e9b0964`  
		Last Modified: Thu, 24 Mar 2022 05:02:59 GMT  
		Size: 4.4 MB (4386160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9273607dfcab1fec447db73e4e9cd486dd0884b29aa8d0c7bcb4e1242bd9c5f`  
		Last Modified: Thu, 24 Mar 2022 05:02:58 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
