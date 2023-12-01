<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `api-firewall`

-	[`api-firewall:0.6.14`](#api-firewall0614)
-	[`api-firewall:latest`](#api-firewalllatest)

## `api-firewall:0.6.14`

```console
$ docker pull api-firewall@sha256:28020694734ad937f328bf30f2e37734c3f669c93ca92725ece87fd71251107d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:0.6.14` - linux; amd64

```console
$ docker pull api-firewall@sha256:754766435f157156139c7633e7b5903c9fe6ee7f265469627d824e4c450f7dee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13744880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aa1872989ad5f9106f5ee416d2e50fcadad30c0ebbc5e47d603a0625e0d398e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:14 GMT
ENV APIFW_PATH=/opt/api-firewall
# Sat, 21 Oct 2023 00:05:14 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 00:05:15 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Wed, 29 Nov 2023 23:22:03 GMT
ENV APIFIREWALL_VERSION=v0.6.14
# Wed, 29 Nov 2023 23:22:05 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='d42c2350217da3831e227f5d9e20adbace1a262fc7f94fb46d9de1b8bf5e5548';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='83716032269cf05ba916c0a91c384527ea23f527f5cfb1cde61b0687d41145e5';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='ccfb44e9cfd06a9a21c3b7c283e95890e94b5f0011b73b7e64f86638475efd97';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Wed, 29 Nov 2023 23:22:05 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Wed, 29 Nov 2023 23:22:05 GMT
USER api-firewall
# Wed, 29 Nov 2023 23:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Nov 2023 23:22:05 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72514a13876f7849ac739ec3d2953fab27acb567431b80b8cb0b867edd999ab`  
		Last Modified: Sat, 21 Oct 2023 00:05:31 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3581d143453bc4468fe204afd8b8e93106a363d61a1087b405a4c0f34ee3354a`  
		Last Modified: Wed, 29 Nov 2023 23:22:15 GMT  
		Size: 10.3 MB (10341352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc3fa25b7ce36ffa97b74b43b627896cc637d6470f59a22fdb7214f2499c984`  
		Last Modified: Wed, 29 Nov 2023 23:22:14 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:0.6.14` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:e7369d561d11f6c8a54f74fe52573ec32bf67857bfc5657e51e895d89f3baef1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12932122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c0b352c32881b57c47f983c6e64a15d2a26064d311aa384bae8b44c352935a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:54:06 GMT
ENV APIFW_PATH=/opt/api-firewall
# Fri, 01 Dec 2023 02:54:06 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Dec 2023 02:54:07 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Fri, 01 Dec 2023 02:54:07 GMT
ENV APIFIREWALL_VERSION=v0.6.14
# Fri, 01 Dec 2023 02:54:09 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='d42c2350217da3831e227f5d9e20adbace1a262fc7f94fb46d9de1b8bf5e5548';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='83716032269cf05ba916c0a91c384527ea23f527f5cfb1cde61b0687d41145e5';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='ccfb44e9cfd06a9a21c3b7c283e95890e94b5f0011b73b7e64f86638475efd97';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Fri, 01 Dec 2023 02:54:09 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Fri, 01 Dec 2023 02:54:09 GMT
USER api-firewall
# Fri, 01 Dec 2023 02:54:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 02:54:09 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0d2a72e8aaff6ef6733fdfa07b2ab1b93a090a52148f0e5e5679fe5a087f32`  
		Last Modified: Fri, 01 Dec 2023 02:54:16 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b34b931cb348fe9bee1c07a236b0a159eb2452643ebe80f95f9691bb7719c4`  
		Last Modified: Fri, 01 Dec 2023 02:54:17 GMT  
		Size: 9.6 MB (9597530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c01c4314fd522e83bb168e20f8d1baa1546161166c896ef78bdae31dcdce43`  
		Last Modified: Fri, 01 Dec 2023 02:54:16 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:0.6.14` - linux; 386

```console
$ docker pull api-firewall@sha256:4c2a34e12e2bea01769a836b80f3c3f90edb383b0bb67e2af8f274cb57432fc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.2 MB (12240275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43cd01e4a4456901557645bdc3c3b3f58cbf29aa447ebccf805cfe844f203223`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:04:46 GMT
ENV APIFW_PATH=/opt/api-firewall
# Sat, 21 Oct 2023 00:04:46 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 00:04:47 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Wed, 29 Nov 2023 22:38:17 GMT
ENV APIFIREWALL_VERSION=v0.6.14
# Wed, 29 Nov 2023 22:38:20 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='d42c2350217da3831e227f5d9e20adbace1a262fc7f94fb46d9de1b8bf5e5548';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='83716032269cf05ba916c0a91c384527ea23f527f5cfb1cde61b0687d41145e5';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='ccfb44e9cfd06a9a21c3b7c283e95890e94b5f0011b73b7e64f86638475efd97';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Wed, 29 Nov 2023 22:38:20 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Wed, 29 Nov 2023 22:38:21 GMT
USER api-firewall
# Wed, 29 Nov 2023 22:38:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Nov 2023 22:38:21 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750c2f1a84d2797a7edb6e815ba9a41c6f0aa7db75673d299dee25db0d40e5a2`  
		Last Modified: Sat, 21 Oct 2023 00:05:05 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a21eb1044a2471a8ebe2043822ab796774e3e2fc8f752fec16f31f7a4ef5a3`  
		Last Modified: Wed, 29 Nov 2023 22:38:30 GMT  
		Size: 9.0 MB (9002957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41ea9823e25e4b511fd2e4ff0f1aa91f2ab494403e502653bec2dfc68e1c2d4`  
		Last Modified: Wed, 29 Nov 2023 22:38:28 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `api-firewall:latest`

```console
$ docker pull api-firewall@sha256:28020694734ad937f328bf30f2e37734c3f669c93ca92725ece87fd71251107d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:latest` - linux; amd64

```console
$ docker pull api-firewall@sha256:754766435f157156139c7633e7b5903c9fe6ee7f265469627d824e4c450f7dee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13744880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aa1872989ad5f9106f5ee416d2e50fcadad30c0ebbc5e47d603a0625e0d398e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:14 GMT
ENV APIFW_PATH=/opt/api-firewall
# Sat, 21 Oct 2023 00:05:14 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 00:05:15 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Wed, 29 Nov 2023 23:22:03 GMT
ENV APIFIREWALL_VERSION=v0.6.14
# Wed, 29 Nov 2023 23:22:05 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='d42c2350217da3831e227f5d9e20adbace1a262fc7f94fb46d9de1b8bf5e5548';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='83716032269cf05ba916c0a91c384527ea23f527f5cfb1cde61b0687d41145e5';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='ccfb44e9cfd06a9a21c3b7c283e95890e94b5f0011b73b7e64f86638475efd97';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Wed, 29 Nov 2023 23:22:05 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Wed, 29 Nov 2023 23:22:05 GMT
USER api-firewall
# Wed, 29 Nov 2023 23:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Nov 2023 23:22:05 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72514a13876f7849ac739ec3d2953fab27acb567431b80b8cb0b867edd999ab`  
		Last Modified: Sat, 21 Oct 2023 00:05:31 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3581d143453bc4468fe204afd8b8e93106a363d61a1087b405a4c0f34ee3354a`  
		Last Modified: Wed, 29 Nov 2023 23:22:15 GMT  
		Size: 10.3 MB (10341352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc3fa25b7ce36ffa97b74b43b627896cc637d6470f59a22fdb7214f2499c984`  
		Last Modified: Wed, 29 Nov 2023 23:22:14 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:e7369d561d11f6c8a54f74fe52573ec32bf67857bfc5657e51e895d89f3baef1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12932122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c0b352c32881b57c47f983c6e64a15d2a26064d311aa384bae8b44c352935a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:54:06 GMT
ENV APIFW_PATH=/opt/api-firewall
# Fri, 01 Dec 2023 02:54:06 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Dec 2023 02:54:07 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Fri, 01 Dec 2023 02:54:07 GMT
ENV APIFIREWALL_VERSION=v0.6.14
# Fri, 01 Dec 2023 02:54:09 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='d42c2350217da3831e227f5d9e20adbace1a262fc7f94fb46d9de1b8bf5e5548';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='83716032269cf05ba916c0a91c384527ea23f527f5cfb1cde61b0687d41145e5';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='ccfb44e9cfd06a9a21c3b7c283e95890e94b5f0011b73b7e64f86638475efd97';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Fri, 01 Dec 2023 02:54:09 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Fri, 01 Dec 2023 02:54:09 GMT
USER api-firewall
# Fri, 01 Dec 2023 02:54:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 02:54:09 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0d2a72e8aaff6ef6733fdfa07b2ab1b93a090a52148f0e5e5679fe5a087f32`  
		Last Modified: Fri, 01 Dec 2023 02:54:16 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b34b931cb348fe9bee1c07a236b0a159eb2452643ebe80f95f9691bb7719c4`  
		Last Modified: Fri, 01 Dec 2023 02:54:17 GMT  
		Size: 9.6 MB (9597530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c01c4314fd522e83bb168e20f8d1baa1546161166c896ef78bdae31dcdce43`  
		Last Modified: Fri, 01 Dec 2023 02:54:16 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; 386

```console
$ docker pull api-firewall@sha256:4c2a34e12e2bea01769a836b80f3c3f90edb383b0bb67e2af8f274cb57432fc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.2 MB (12240275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43cd01e4a4456901557645bdc3c3b3f58cbf29aa447ebccf805cfe844f203223`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:04:46 GMT
ENV APIFW_PATH=/opt/api-firewall
# Sat, 21 Oct 2023 00:04:46 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 00:04:47 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Wed, 29 Nov 2023 22:38:17 GMT
ENV APIFIREWALL_VERSION=v0.6.14
# Wed, 29 Nov 2023 22:38:20 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='d42c2350217da3831e227f5d9e20adbace1a262fc7f94fb46d9de1b8bf5e5548';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='83716032269cf05ba916c0a91c384527ea23f527f5cfb1cde61b0687d41145e5';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='ccfb44e9cfd06a9a21c3b7c283e95890e94b5f0011b73b7e64f86638475efd97';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Wed, 29 Nov 2023 22:38:20 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Wed, 29 Nov 2023 22:38:21 GMT
USER api-firewall
# Wed, 29 Nov 2023 22:38:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Nov 2023 22:38:21 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750c2f1a84d2797a7edb6e815ba9a41c6f0aa7db75673d299dee25db0d40e5a2`  
		Last Modified: Sat, 21 Oct 2023 00:05:05 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a21eb1044a2471a8ebe2043822ab796774e3e2fc8f752fec16f31f7a4ef5a3`  
		Last Modified: Wed, 29 Nov 2023 22:38:30 GMT  
		Size: 9.0 MB (9002957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41ea9823e25e4b511fd2e4ff0f1aa91f2ab494403e502653bec2dfc68e1c2d4`  
		Last Modified: Wed, 29 Nov 2023 22:38:28 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
