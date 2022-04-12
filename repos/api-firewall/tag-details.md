<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `api-firewall`

-	[`api-firewall:0.6.8`](#api-firewall068)
-	[`api-firewall:latest`](#api-firewalllatest)

## `api-firewall:0.6.8`

```console
$ docker pull api-firewall@sha256:d004f0d72c0eea4ba69c66281e0fcb969f59d2e5537e42994f066e419efe521e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:0.6.8` - linux; amd64

```console
$ docker pull api-firewall@sha256:4526e4516cc028da236dd42776c40742a823c7042ec31f81dfab53e06bfc9ce6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7570969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb80b988cf464b9a73d669e0b895b129bca1285e74393622c5613392ef25b85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:00:47 GMT
ENV APIFW_PATH=/opt/api-firewall
# Tue, 05 Apr 2022 04:00:47 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 04:00:48 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Mon, 11 Apr 2022 21:41:57 GMT
ENV APIFIREWALL_VERSION=v0.6.8
# Mon, 11 Apr 2022 21:41:59 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='af8e49e7ebf19d68b4dcf09a0f0b04b36a5c6e3f556549cb48852fcebac03892';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='b15fa8bfb98d23760eac894002db79420cdc321c1f1baabf60fba54556dfdab7';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='d37c9cef562788caf0177224516c555808251a6d79a368b4902424d57037d023';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Mon, 11 Apr 2022 21:41:59 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Mon, 11 Apr 2022 21:41:59 GMT
USER api-firewall
# Mon, 11 Apr 2022 21:42:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Apr 2022 21:42:00 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34205ad7e15a85fb6238ca662f347b83dd42d9181af0d2bb10ca0df5c7ee203`  
		Last Modified: Tue, 05 Apr 2022 04:00:59 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b805f02a44f2954e5716bd7a20319bfa2ba429e5fb219a9dd6e1b98a28f65883`  
		Last Modified: Mon, 11 Apr 2022 21:42:10 GMT  
		Size: 4.8 MB (4754856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b724ea0d37ea108975b074264b24ad06e1e75a09afa2a1ec3b5a7f2ab6527727`  
		Last Modified: Mon, 11 Apr 2022 21:42:09 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:0.6.8` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:0e4c607795b66b6b6f2eb70aa761526c3a41b242e96deef1b7de9271f352a886
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7178270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c54be4ab5dd86a67aabd60d6a8166bdc8ced62f6b10714a10fb5e120e2d110b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:36:28 GMT
ENV APIFW_PATH=/opt/api-firewall
# Tue, 05 Apr 2022 07:36:29 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 07:36:30 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Mon, 11 Apr 2022 21:39:22 GMT
ENV APIFIREWALL_VERSION=v0.6.8
# Mon, 11 Apr 2022 21:39:25 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='af8e49e7ebf19d68b4dcf09a0f0b04b36a5c6e3f556549cb48852fcebac03892';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='b15fa8bfb98d23760eac894002db79420cdc321c1f1baabf60fba54556dfdab7';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='d37c9cef562788caf0177224516c555808251a6d79a368b4902424d57037d023';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Mon, 11 Apr 2022 21:39:26 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Mon, 11 Apr 2022 21:39:26 GMT
USER api-firewall
# Mon, 11 Apr 2022 21:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Apr 2022 21:39:28 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dfcd6871e1e354662d6653b214f845c3e889d8c19e9a5fcad07ca5739ffcf4`  
		Last Modified: Tue, 05 Apr 2022 07:36:50 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d5878466c35e0cc296bb10f344fa83f24dc9812c494d10399de4f7c4fbe87c`  
		Last Modified: Mon, 11 Apr 2022 21:39:42 GMT  
		Size: 4.5 MB (4460239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23783ad6136c9fba58c1d937ea50c056dcb03f001b1680b8babbbebd86b125b`  
		Last Modified: Mon, 11 Apr 2022 21:39:41 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:0.6.8` - linux; 386

```console
$ docker pull api-firewall@sha256:b40aec4cfc52a8fe5a9456ddb04ed8cf10874da0e50837380a1065493ab82936
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7359074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31f0afdc57ca547b179055ab44e6e7e7314f593154cff599d994166743b214d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Mon, 11 Apr 2022 18:38:16 GMT
ENV APIFW_PATH=/opt/api-firewall
# Mon, 11 Apr 2022 18:38:17 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 11 Apr 2022 18:38:18 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Mon, 11 Apr 2022 20:51:33 GMT
ENV APIFIREWALL_VERSION=v0.6.8
# Mon, 11 Apr 2022 20:51:35 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='af8e49e7ebf19d68b4dcf09a0f0b04b36a5c6e3f556549cb48852fcebac03892';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='b15fa8bfb98d23760eac894002db79420cdc321c1f1baabf60fba54556dfdab7';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='d37c9cef562788caf0177224516c555808251a6d79a368b4902424d57037d023';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Mon, 11 Apr 2022 20:51:37 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Mon, 11 Apr 2022 20:51:37 GMT
USER api-firewall
# Mon, 11 Apr 2022 20:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Apr 2022 20:51:39 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20cab14fba821cd8c0fc673aec733daf0779494fc530da56ede285c7f1955d2`  
		Last Modified: Mon, 11 Apr 2022 20:51:53 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f53b231813de53e10bc6b009cc1a3c427239b29a2e2d4afecc399bfbbedb546`  
		Last Modified: Mon, 11 Apr 2022 20:51:54 GMT  
		Size: 4.5 MB (4538541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3953d9af67da8ac0c5a24a1880870f5528baf27d2a150f2390063726429d09ed`  
		Last Modified: Mon, 11 Apr 2022 20:51:53 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `api-firewall:latest`

```console
$ docker pull api-firewall@sha256:d004f0d72c0eea4ba69c66281e0fcb969f59d2e5537e42994f066e419efe521e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:latest` - linux; amd64

```console
$ docker pull api-firewall@sha256:4526e4516cc028da236dd42776c40742a823c7042ec31f81dfab53e06bfc9ce6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7570969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb80b988cf464b9a73d669e0b895b129bca1285e74393622c5613392ef25b85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:00:47 GMT
ENV APIFW_PATH=/opt/api-firewall
# Tue, 05 Apr 2022 04:00:47 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 04:00:48 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Mon, 11 Apr 2022 21:41:57 GMT
ENV APIFIREWALL_VERSION=v0.6.8
# Mon, 11 Apr 2022 21:41:59 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='af8e49e7ebf19d68b4dcf09a0f0b04b36a5c6e3f556549cb48852fcebac03892';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='b15fa8bfb98d23760eac894002db79420cdc321c1f1baabf60fba54556dfdab7';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='d37c9cef562788caf0177224516c555808251a6d79a368b4902424d57037d023';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Mon, 11 Apr 2022 21:41:59 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Mon, 11 Apr 2022 21:41:59 GMT
USER api-firewall
# Mon, 11 Apr 2022 21:42:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Apr 2022 21:42:00 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34205ad7e15a85fb6238ca662f347b83dd42d9181af0d2bb10ca0df5c7ee203`  
		Last Modified: Tue, 05 Apr 2022 04:00:59 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b805f02a44f2954e5716bd7a20319bfa2ba429e5fb219a9dd6e1b98a28f65883`  
		Last Modified: Mon, 11 Apr 2022 21:42:10 GMT  
		Size: 4.8 MB (4754856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b724ea0d37ea108975b074264b24ad06e1e75a09afa2a1ec3b5a7f2ab6527727`  
		Last Modified: Mon, 11 Apr 2022 21:42:09 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:0e4c607795b66b6b6f2eb70aa761526c3a41b242e96deef1b7de9271f352a886
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7178270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c54be4ab5dd86a67aabd60d6a8166bdc8ced62f6b10714a10fb5e120e2d110b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:36:28 GMT
ENV APIFW_PATH=/opt/api-firewall
# Tue, 05 Apr 2022 07:36:29 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 07:36:30 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Mon, 11 Apr 2022 21:39:22 GMT
ENV APIFIREWALL_VERSION=v0.6.8
# Mon, 11 Apr 2022 21:39:25 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='af8e49e7ebf19d68b4dcf09a0f0b04b36a5c6e3f556549cb48852fcebac03892';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='b15fa8bfb98d23760eac894002db79420cdc321c1f1baabf60fba54556dfdab7';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='d37c9cef562788caf0177224516c555808251a6d79a368b4902424d57037d023';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Mon, 11 Apr 2022 21:39:26 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Mon, 11 Apr 2022 21:39:26 GMT
USER api-firewall
# Mon, 11 Apr 2022 21:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Apr 2022 21:39:28 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dfcd6871e1e354662d6653b214f845c3e889d8c19e9a5fcad07ca5739ffcf4`  
		Last Modified: Tue, 05 Apr 2022 07:36:50 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d5878466c35e0cc296bb10f344fa83f24dc9812c494d10399de4f7c4fbe87c`  
		Last Modified: Mon, 11 Apr 2022 21:39:42 GMT  
		Size: 4.5 MB (4460239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23783ad6136c9fba58c1d937ea50c056dcb03f001b1680b8babbbebd86b125b`  
		Last Modified: Mon, 11 Apr 2022 21:39:41 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; 386

```console
$ docker pull api-firewall@sha256:b40aec4cfc52a8fe5a9456ddb04ed8cf10874da0e50837380a1065493ab82936
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7359074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31f0afdc57ca547b179055ab44e6e7e7314f593154cff599d994166743b214d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Mon, 11 Apr 2022 18:38:16 GMT
ENV APIFW_PATH=/opt/api-firewall
# Mon, 11 Apr 2022 18:38:17 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 11 Apr 2022 18:38:18 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Mon, 11 Apr 2022 20:51:33 GMT
ENV APIFIREWALL_VERSION=v0.6.8
# Mon, 11 Apr 2022 20:51:35 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='af8e49e7ebf19d68b4dcf09a0f0b04b36a5c6e3f556549cb48852fcebac03892';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='b15fa8bfb98d23760eac894002db79420cdc321c1f1baabf60fba54556dfdab7';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='d37c9cef562788caf0177224516c555808251a6d79a368b4902424d57037d023';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Mon, 11 Apr 2022 20:51:37 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Mon, 11 Apr 2022 20:51:37 GMT
USER api-firewall
# Mon, 11 Apr 2022 20:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Apr 2022 20:51:39 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20cab14fba821cd8c0fc673aec733daf0779494fc530da56ede285c7f1955d2`  
		Last Modified: Mon, 11 Apr 2022 20:51:53 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f53b231813de53e10bc6b009cc1a3c427239b29a2e2d4afecc399bfbbedb546`  
		Last Modified: Mon, 11 Apr 2022 20:51:54 GMT  
		Size: 4.5 MB (4538541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3953d9af67da8ac0c5a24a1880870f5528baf27d2a150f2390063726429d09ed`  
		Last Modified: Mon, 11 Apr 2022 20:51:53 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
