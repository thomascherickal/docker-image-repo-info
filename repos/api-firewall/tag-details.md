<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `api-firewall`

-	[`api-firewall:0.6.12`](#api-firewall0612)
-	[`api-firewall:0.6.13`](#api-firewall0613)
-	[`api-firewall:latest`](#api-firewalllatest)

## `api-firewall:0.6.12`

```console
$ docker pull api-firewall@sha256:4042ec2686cbcc75043e205917e3bb76e73da9258b625073b773d423253eb905
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:0.6.12` - linux; amd64

```console
$ docker pull api-firewall@sha256:8eb89b26d800fe14ead52e663eadec544a5131bfc892dbe4f166aa2074a05270
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10351649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d84a96f2af51cb205dbe635e1e11ac640337064738148afe40abe53f734085f`
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
# Sat, 21 Oct 2023 00:05:20 GMT
ENV APIFIREWALL_VERSION=v0.6.12
# Sat, 21 Oct 2023 00:05:22 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='4aabd47bdba440fa745fd084c111882d5022f4a6862b954e6cb6be713f4c8e48';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='9623844cfb2f6f4e629d80864d71bfee4e1277f81be4c126d83d25afdf3109f0';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='0fc470b278d0175dcb80ceb30f1508c1c18c01d42cb0ebf62f55d7f18f2424db';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Sat, 21 Oct 2023 00:05:22 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Sat, 21 Oct 2023 00:05:22 GMT
USER api-firewall
# Sat, 21 Oct 2023 00:05:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 00:05:23 GMT
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
	-	`sha256:85798c38562b356540bea40ef6d5f533de0313177a5ba79b9ac791f374daa14a`  
		Last Modified: Sat, 21 Oct 2023 00:05:42 GMT  
		Size: 6.9 MB (6948126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fd9df4bb62a380fda65205aa2cd0d81db624f944e89d830e9ed53756ac94e5`  
		Last Modified: Sat, 21 Oct 2023 00:05:41 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:0.6.12` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:4128cd7aebcf9faa53cb6f8ce118bddb48de73520b023fbae6efd0c63431f57a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9840753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:230e197d439eba7b9fa1639ce5ff207fbb9056c7f1d5e13947d2e6b63e12a302`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:18:14 GMT
ENV APIFW_PATH=/opt/api-firewall
# Sat, 21 Oct 2023 00:18:14 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 00:18:15 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Sat, 21 Oct 2023 00:18:19 GMT
ENV APIFIREWALL_VERSION=v0.6.12
# Sat, 21 Oct 2023 00:18:21 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='4aabd47bdba440fa745fd084c111882d5022f4a6862b954e6cb6be713f4c8e48';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='9623844cfb2f6f4e629d80864d71bfee4e1277f81be4c126d83d25afdf3109f0';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='0fc470b278d0175dcb80ceb30f1508c1c18c01d42cb0ebf62f55d7f18f2424db';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Sat, 21 Oct 2023 00:18:21 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Sat, 21 Oct 2023 00:18:22 GMT
USER api-firewall
# Sat, 21 Oct 2023 00:18:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 00:18:22 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220757af88f41767124b7c876a99b6e1eb0f3ea7bfa8fbb7e99b8cc6c926e09b`  
		Last Modified: Sat, 21 Oct 2023 00:18:31 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc08101e6841f57ffe333a0cc70ed7e370854fdff1a9112691ecc529b443e661`  
		Last Modified: Sat, 21 Oct 2023 00:18:40 GMT  
		Size: 6.5 MB (6507365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d19f52fc4650f06037cba4800be088db7751d41ae95ec8ec2891dabcbde2d2e`  
		Last Modified: Sat, 21 Oct 2023 00:18:40 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:0.6.12` - linux; 386

```console
$ docker pull api-firewall@sha256:621a7ffb17d0a6dacb10401fc117003f54e546774afb7dcefb349425b3a8f72f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8533827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39cb2040cc664ac1526ef28862ec42743d76964e1c5602f7053e9d121db57e60`
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
# Sat, 21 Oct 2023 00:04:53 GMT
ENV APIFIREWALL_VERSION=v0.6.12
# Sat, 21 Oct 2023 00:04:56 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='4aabd47bdba440fa745fd084c111882d5022f4a6862b954e6cb6be713f4c8e48';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='9623844cfb2f6f4e629d80864d71bfee4e1277f81be4c126d83d25afdf3109f0';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='0fc470b278d0175dcb80ceb30f1508c1c18c01d42cb0ebf62f55d7f18f2424db';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Sat, 21 Oct 2023 00:04:56 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Sat, 21 Oct 2023 00:04:56 GMT
USER api-firewall
# Sat, 21 Oct 2023 00:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 00:04:56 GMT
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
	-	`sha256:139c2a99b34479c42ae0082abbffa7f0b2657661d0f218dc011fa9d7a016d657`  
		Last Modified: Sat, 21 Oct 2023 00:05:18 GMT  
		Size: 5.3 MB (5296509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd01c762f04b30c0fd364a14186226f262f80c16584e040c4f41c3784473483`  
		Last Modified: Sat, 21 Oct 2023 00:05:16 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `api-firewall:0.6.13`

```console
$ docker pull api-firewall@sha256:a93637ca207fd6dfc9275be2c15a7fc7aa417a00fceb0b6e1c4b92168e7b473e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:0.6.13` - linux; amd64

```console
$ docker pull api-firewall@sha256:65d0e6347ef8641d9d5b1bbd1d51329851e658828f9badcfe764f71bdc28d936
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13732352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a5791c46ca3a5b6cb081eb8cd2cac873912483a1a8a922fb358bda3cda39228`
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
# Sat, 21 Oct 2023 00:05:15 GMT
ENV APIFIREWALL_VERSION=v0.6.13
# Sat, 21 Oct 2023 00:05:17 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='42bc189c8302221d37eea69297a0edd8aa485f8856225019f4773bbbe72b4363';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='186e46d26eb64ccc10ea07b91fc7602cff5eba13f13ec5314222a65f991f8717';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='898eb09cae9b314f302be6fb27e6618428ded24cddc569fe8c37b27a02977657';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Sat, 21 Oct 2023 00:05:17 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Sat, 21 Oct 2023 00:05:17 GMT
USER api-firewall
# Sat, 21 Oct 2023 00:05:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 00:05:17 GMT
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
	-	`sha256:87b3f1323e0532d9f679716e6ded80d8240431bfa1e5a2d2959ba50d27513eb0`  
		Last Modified: Sat, 21 Oct 2023 00:05:33 GMT  
		Size: 10.3 MB (10328825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad5eaacfc5e4ba4d3a91003b66965e2a4da6c79f39513ca23006a497de8d43`  
		Last Modified: Sat, 21 Oct 2023 00:05:31 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:0.6.13` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:b6a6475abe3a9eadacb5ca184190314577c7475eaf538ef2289d8b4e9cf9fe88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12916610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6efc3931449d30abdcc8aa430da35f0b4c912dadede771e94ed002f57457c4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:18:14 GMT
ENV APIFW_PATH=/opt/api-firewall
# Sat, 21 Oct 2023 00:18:14 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 00:18:15 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Sat, 21 Oct 2023 00:18:15 GMT
ENV APIFIREWALL_VERSION=v0.6.13
# Sat, 21 Oct 2023 00:18:17 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='42bc189c8302221d37eea69297a0edd8aa485f8856225019f4773bbbe72b4363';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='186e46d26eb64ccc10ea07b91fc7602cff5eba13f13ec5314222a65f991f8717';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='898eb09cae9b314f302be6fb27e6618428ded24cddc569fe8c37b27a02977657';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Sat, 21 Oct 2023 00:18:17 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Sat, 21 Oct 2023 00:18:17 GMT
USER api-firewall
# Sat, 21 Oct 2023 00:18:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 00:18:17 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220757af88f41767124b7c876a99b6e1eb0f3ea7bfa8fbb7e99b8cc6c926e09b`  
		Last Modified: Sat, 21 Oct 2023 00:18:31 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e259e4d610fab979e3e5b47b02a3350d9c7316f9acd4c9ecae8d3e5966e3d`  
		Last Modified: Sat, 21 Oct 2023 00:18:32 GMT  
		Size: 9.6 MB (9583218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d8d035bea4a21155d013778d56b93ed5bb2b0cce913608343405698c2e5d10`  
		Last Modified: Sat, 21 Oct 2023 00:18:30 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:0.6.13` - linux; 386

```console
$ docker pull api-firewall@sha256:ef6e0f17bdc37800374dd46168551abeb1704a59818f852a10de9b2d18ebb2f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.2 MB (12230530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a47a09fdd804cbf218ef4f6f72a52c8575c16f7519be17fb281d04decb0d1cdc`
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
# Sat, 21 Oct 2023 00:04:47 GMT
ENV APIFIREWALL_VERSION=v0.6.13
# Sat, 21 Oct 2023 00:04:50 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='42bc189c8302221d37eea69297a0edd8aa485f8856225019f4773bbbe72b4363';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='186e46d26eb64ccc10ea07b91fc7602cff5eba13f13ec5314222a65f991f8717';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='898eb09cae9b314f302be6fb27e6618428ded24cddc569fe8c37b27a02977657';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Sat, 21 Oct 2023 00:04:50 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Sat, 21 Oct 2023 00:04:50 GMT
USER api-firewall
# Sat, 21 Oct 2023 00:04:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 00:04:51 GMT
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
	-	`sha256:3fdbb8c6d72af77d72dacd4a75df9f2d1e30c49446a4c485cddcd30634a846d1`  
		Last Modified: Sat, 21 Oct 2023 00:05:08 GMT  
		Size: 9.0 MB (8993212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56b63db92237260c201db05e00226f7784665a803beb9e859c920b822153403`  
		Last Modified: Sat, 21 Oct 2023 00:05:05 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `api-firewall:latest`

```console
$ docker pull api-firewall@sha256:a93637ca207fd6dfc9275be2c15a7fc7aa417a00fceb0b6e1c4b92168e7b473e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:latest` - linux; amd64

```console
$ docker pull api-firewall@sha256:65d0e6347ef8641d9d5b1bbd1d51329851e658828f9badcfe764f71bdc28d936
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13732352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a5791c46ca3a5b6cb081eb8cd2cac873912483a1a8a922fb358bda3cda39228`
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
# Sat, 21 Oct 2023 00:05:15 GMT
ENV APIFIREWALL_VERSION=v0.6.13
# Sat, 21 Oct 2023 00:05:17 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='42bc189c8302221d37eea69297a0edd8aa485f8856225019f4773bbbe72b4363';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='186e46d26eb64ccc10ea07b91fc7602cff5eba13f13ec5314222a65f991f8717';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='898eb09cae9b314f302be6fb27e6618428ded24cddc569fe8c37b27a02977657';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Sat, 21 Oct 2023 00:05:17 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Sat, 21 Oct 2023 00:05:17 GMT
USER api-firewall
# Sat, 21 Oct 2023 00:05:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 00:05:17 GMT
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
	-	`sha256:87b3f1323e0532d9f679716e6ded80d8240431bfa1e5a2d2959ba50d27513eb0`  
		Last Modified: Sat, 21 Oct 2023 00:05:33 GMT  
		Size: 10.3 MB (10328825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad5eaacfc5e4ba4d3a91003b66965e2a4da6c79f39513ca23006a497de8d43`  
		Last Modified: Sat, 21 Oct 2023 00:05:31 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:b6a6475abe3a9eadacb5ca184190314577c7475eaf538ef2289d8b4e9cf9fe88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12916610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6efc3931449d30abdcc8aa430da35f0b4c912dadede771e94ed002f57457c4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:18:14 GMT
ENV APIFW_PATH=/opt/api-firewall
# Sat, 21 Oct 2023 00:18:14 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 00:18:15 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Sat, 21 Oct 2023 00:18:15 GMT
ENV APIFIREWALL_VERSION=v0.6.13
# Sat, 21 Oct 2023 00:18:17 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='42bc189c8302221d37eea69297a0edd8aa485f8856225019f4773bbbe72b4363';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='186e46d26eb64ccc10ea07b91fc7602cff5eba13f13ec5314222a65f991f8717';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='898eb09cae9b314f302be6fb27e6618428ded24cddc569fe8c37b27a02977657';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Sat, 21 Oct 2023 00:18:17 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Sat, 21 Oct 2023 00:18:17 GMT
USER api-firewall
# Sat, 21 Oct 2023 00:18:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 00:18:17 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220757af88f41767124b7c876a99b6e1eb0f3ea7bfa8fbb7e99b8cc6c926e09b`  
		Last Modified: Sat, 21 Oct 2023 00:18:31 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e259e4d610fab979e3e5b47b02a3350d9c7316f9acd4c9ecae8d3e5966e3d`  
		Last Modified: Sat, 21 Oct 2023 00:18:32 GMT  
		Size: 9.6 MB (9583218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d8d035bea4a21155d013778d56b93ed5bb2b0cce913608343405698c2e5d10`  
		Last Modified: Sat, 21 Oct 2023 00:18:30 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; 386

```console
$ docker pull api-firewall@sha256:ef6e0f17bdc37800374dd46168551abeb1704a59818f852a10de9b2d18ebb2f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.2 MB (12230530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a47a09fdd804cbf218ef4f6f72a52c8575c16f7519be17fb281d04decb0d1cdc`
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
# Sat, 21 Oct 2023 00:04:47 GMT
ENV APIFIREWALL_VERSION=v0.6.13
# Sat, 21 Oct 2023 00:04:50 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='42bc189c8302221d37eea69297a0edd8aa485f8856225019f4773bbbe72b4363';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='186e46d26eb64ccc10ea07b91fc7602cff5eba13f13ec5314222a65f991f8717';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='898eb09cae9b314f302be6fb27e6618428ded24cddc569fe8c37b27a02977657';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Sat, 21 Oct 2023 00:04:50 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Sat, 21 Oct 2023 00:04:50 GMT
USER api-firewall
# Sat, 21 Oct 2023 00:04:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 00:04:51 GMT
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
	-	`sha256:3fdbb8c6d72af77d72dacd4a75df9f2d1e30c49446a4c485cddcd30634a846d1`  
		Last Modified: Sat, 21 Oct 2023 00:05:08 GMT  
		Size: 9.0 MB (8993212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56b63db92237260c201db05e00226f7784665a803beb9e859c920b822153403`  
		Last Modified: Sat, 21 Oct 2023 00:05:05 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
