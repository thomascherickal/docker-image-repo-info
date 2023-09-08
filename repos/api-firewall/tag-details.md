<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `api-firewall`

-	[`api-firewall:0.6.12`](#api-firewall0612)
-	[`api-firewall:0.6.13`](#api-firewall0613)
-	[`api-firewall:latest`](#api-firewalllatest)

## `api-firewall:0.6.12`

```console
$ docker pull api-firewall@sha256:0a5349b376ee7c9bb0b55cb5d54f621ee9994009412675b1de8326ddf74ab321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:0.6.12` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:aface819e9655402cbeb1382ddfe9908162285a02d3167e5744be96065a56597
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9839693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f43aacb462bcee0fc554cd0f25169b2810bbf79a9cd78b0f7e7c387ebccc48f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Fri, 08 Sep 2023 21:41:12 GMT
ENV APIFW_PATH=/opt/api-firewall
# Fri, 08 Sep 2023 21:41:12 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Sep 2023 21:41:12 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Fri, 08 Sep 2023 21:41:17 GMT
ENV APIFIREWALL_VERSION=v0.6.12
# Fri, 08 Sep 2023 21:41:18 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='4aabd47bdba440fa745fd084c111882d5022f4a6862b954e6cb6be713f4c8e48';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='9623844cfb2f6f4e629d80864d71bfee4e1277f81be4c126d83d25afdf3109f0';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='0fc470b278d0175dcb80ceb30f1508c1c18c01d42cb0ebf62f55d7f18f2424db';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Fri, 08 Sep 2023 21:41:18 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Fri, 08 Sep 2023 21:41:18 GMT
USER api-firewall
# Fri, 08 Sep 2023 21:41:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Sep 2023 21:41:19 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a6cd65c13ed31bfd6114209258ad6f420b23bc6b2bd555e784f43a0fcfb1cf`  
		Last Modified: Fri, 08 Sep 2023 21:41:27 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcf6d033beb7f113e5db167dd3c98825fd83cd0a61e17862c329202fbc6392d`  
		Last Modified: Fri, 08 Sep 2023 21:41:36 GMT  
		Size: 6.5 MB (6507373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7cc9846fdd33474f2fe58bd483c10caeb0c197f8da4795568b59fae5af76c29`  
		Last Modified: Fri, 08 Sep 2023 21:41:36 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:0.6.12` - linux; 386

```console
$ docker pull api-firewall@sha256:c0ddbc5efe923f22d3c2818e465d3f484615d2245c60be2bda6cc48879244080
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8533208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49eac7ec272d04d19fb389112c959cbad7cf61c8a8a0cba6700a7925715a9b10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Fri, 08 Sep 2023 21:38:18 GMT
ENV APIFW_PATH=/opt/api-firewall
# Fri, 08 Sep 2023 21:38:18 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Sep 2023 21:38:19 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Fri, 08 Sep 2023 21:38:24 GMT
ENV APIFIREWALL_VERSION=v0.6.12
# Fri, 08 Sep 2023 21:38:27 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='4aabd47bdba440fa745fd084c111882d5022f4a6862b954e6cb6be713f4c8e48';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='9623844cfb2f6f4e629d80864d71bfee4e1277f81be4c126d83d25afdf3109f0';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='0fc470b278d0175dcb80ceb30f1508c1c18c01d42cb0ebf62f55d7f18f2424db';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Fri, 08 Sep 2023 21:38:27 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Fri, 08 Sep 2023 21:38:27 GMT
USER api-firewall
# Fri, 08 Sep 2023 21:38:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Sep 2023 21:38:28 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810732c4c5731539752999614fb1453fcd5a97a7ddfc937d972268903995410e`  
		Last Modified: Fri, 08 Sep 2023 21:38:36 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8066b6d49e0c3138853568efc45921ef59d9076e4066c960c407aa767e9d4447`  
		Last Modified: Fri, 08 Sep 2023 21:38:47 GMT  
		Size: 5.3 MB (5296502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f372339bc01455eb46c475ac1c9edc824910dac31834da7232ed0a80e6634b4`  
		Last Modified: Fri, 08 Sep 2023 21:38:46 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `api-firewall:0.6.13`

```console
$ docker pull api-firewall@sha256:b044a19f2a25c718a1b4d1088728d10c5320ffc9b726746277f69674ec2e07ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:0.6.13` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:465918228df7c86c16d2a1a09f0377be22c8014d5ae30ea0bf95213a612e6c5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12915513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df0ec54f2d4773ee57101cd55f0caec43070e9decac7f8c08f61d09414fc3f85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Fri, 08 Sep 2023 21:41:12 GMT
ENV APIFW_PATH=/opt/api-firewall
# Fri, 08 Sep 2023 21:41:12 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Sep 2023 21:41:12 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Fri, 08 Sep 2023 21:41:13 GMT
ENV APIFIREWALL_VERSION=v0.6.13
# Fri, 08 Sep 2023 21:41:14 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='42bc189c8302221d37eea69297a0edd8aa485f8856225019f4773bbbe72b4363';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='186e46d26eb64ccc10ea07b91fc7602cff5eba13f13ec5314222a65f991f8717';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='898eb09cae9b314f302be6fb27e6618428ded24cddc569fe8c37b27a02977657';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Fri, 08 Sep 2023 21:41:15 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Fri, 08 Sep 2023 21:41:15 GMT
USER api-firewall
# Fri, 08 Sep 2023 21:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Sep 2023 21:41:15 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a6cd65c13ed31bfd6114209258ad6f420b23bc6b2bd555e784f43a0fcfb1cf`  
		Last Modified: Fri, 08 Sep 2023 21:41:27 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd28568a9fdb843ae407ace5ae4f5ea4647d3a72a6b07cb5634c12f4e5e444b`  
		Last Modified: Fri, 08 Sep 2023 21:41:28 GMT  
		Size: 9.6 MB (9583193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d26e47ce6c8d97cf538d9116c1b3935d602b708784ce2fb8e9bbb6e48aa69c`  
		Last Modified: Fri, 08 Sep 2023 21:41:27 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:0.6.13` - linux; 386

```console
$ docker pull api-firewall@sha256:985c5476a5796a0c877475d689be13e5e11085fb0f954a149f438a7b64bb7b78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.2 MB (12229918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b11ad546836754b944d0331623808b0df7844f0b2d6cbfda64e5ad09041488e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Fri, 08 Sep 2023 21:38:18 GMT
ENV APIFW_PATH=/opt/api-firewall
# Fri, 08 Sep 2023 21:38:18 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Sep 2023 21:38:19 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Fri, 08 Sep 2023 21:38:19 GMT
ENV APIFIREWALL_VERSION=v0.6.13
# Fri, 08 Sep 2023 21:38:21 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='42bc189c8302221d37eea69297a0edd8aa485f8856225019f4773bbbe72b4363';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='186e46d26eb64ccc10ea07b91fc7602cff5eba13f13ec5314222a65f991f8717';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='898eb09cae9b314f302be6fb27e6618428ded24cddc569fe8c37b27a02977657';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Fri, 08 Sep 2023 21:38:22 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Fri, 08 Sep 2023 21:38:22 GMT
USER api-firewall
# Fri, 08 Sep 2023 21:38:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Sep 2023 21:38:22 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810732c4c5731539752999614fb1453fcd5a97a7ddfc937d972268903995410e`  
		Last Modified: Fri, 08 Sep 2023 21:38:36 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a80848339d19fca5533c84901c1d184c734b59a42f334588c233b0f2b64cd56`  
		Last Modified: Fri, 08 Sep 2023 21:38:38 GMT  
		Size: 9.0 MB (8993216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba7c9d79244812fe45486a3adc5053998ec5e22a579bb40dcb8ff2fa73e4161`  
		Last Modified: Fri, 08 Sep 2023 21:38:36 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `api-firewall:latest`

```console
$ docker pull api-firewall@sha256:a8e2b42ad2b44e63ee51ddc7896a6d99746e0c9ed9f80a59ca23db590fc86e4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:latest` - linux; amd64

```console
$ docker pull api-firewall@sha256:d87dfb27357591cf0c001138a692b8cc8a6e286fb596319f00dc11f1c6740016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8987306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:975bc7e72dc9951b0ceef3139162c004b2274a595b2a598508576a10682d0514`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:10:17 GMT
ENV APIFW_PATH=/opt/api-firewall
# Mon, 07 Aug 2023 20:10:17 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:10:17 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Mon, 07 Aug 2023 20:10:17 GMT
ENV APIFIREWALL_VERSION=v0.6.11
# Mon, 07 Aug 2023 20:10:19 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='c76cdb6c6185038ea619e364acc71066831de85aefe7e32f8fdbdcc110125cc1';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='786b645dd11cb34ce2ee512b1f75b8929095e25de0027bff5817dedc895eb883';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='351af5ba7af8a010c941416f863bfd52d3e4f04f6ebba77cdf388c37b39e7c75';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Mon, 07 Aug 2023 20:10:19 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Mon, 07 Aug 2023 20:10:19 GMT
USER api-firewall
# Mon, 07 Aug 2023 20:10:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:10:19 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc01ebde4290a0704589287422aa0dcbb6ce1b03aea189dc71b8723d1fc5000a`  
		Last Modified: Mon, 07 Aug 2023 20:10:39 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edafb5a7beb02c6363bbc5f59527765c1a80bc3b36ede856892088644c447221`  
		Last Modified: Mon, 07 Aug 2023 20:10:40 GMT  
		Size: 5.6 MB (5607142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02daa2b84e9dc5d35ef9e86d72a7a107f9198fefeb651e4483195a8a2b37888`  
		Last Modified: Mon, 07 Aug 2023 20:10:39 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:465918228df7c86c16d2a1a09f0377be22c8014d5ae30ea0bf95213a612e6c5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12915513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df0ec54f2d4773ee57101cd55f0caec43070e9decac7f8c08f61d09414fc3f85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Fri, 08 Sep 2023 21:41:12 GMT
ENV APIFW_PATH=/opt/api-firewall
# Fri, 08 Sep 2023 21:41:12 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Sep 2023 21:41:12 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Fri, 08 Sep 2023 21:41:13 GMT
ENV APIFIREWALL_VERSION=v0.6.13
# Fri, 08 Sep 2023 21:41:14 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='42bc189c8302221d37eea69297a0edd8aa485f8856225019f4773bbbe72b4363';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='186e46d26eb64ccc10ea07b91fc7602cff5eba13f13ec5314222a65f991f8717';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='898eb09cae9b314f302be6fb27e6618428ded24cddc569fe8c37b27a02977657';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Fri, 08 Sep 2023 21:41:15 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Fri, 08 Sep 2023 21:41:15 GMT
USER api-firewall
# Fri, 08 Sep 2023 21:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Sep 2023 21:41:15 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a6cd65c13ed31bfd6114209258ad6f420b23bc6b2bd555e784f43a0fcfb1cf`  
		Last Modified: Fri, 08 Sep 2023 21:41:27 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd28568a9fdb843ae407ace5ae4f5ea4647d3a72a6b07cb5634c12f4e5e444b`  
		Last Modified: Fri, 08 Sep 2023 21:41:28 GMT  
		Size: 9.6 MB (9583193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d26e47ce6c8d97cf538d9116c1b3935d602b708784ce2fb8e9bbb6e48aa69c`  
		Last Modified: Fri, 08 Sep 2023 21:41:27 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; 386

```console
$ docker pull api-firewall@sha256:985c5476a5796a0c877475d689be13e5e11085fb0f954a149f438a7b64bb7b78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.2 MB (12229918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b11ad546836754b944d0331623808b0df7844f0b2d6cbfda64e5ad09041488e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Fri, 08 Sep 2023 21:38:18 GMT
ENV APIFW_PATH=/opt/api-firewall
# Fri, 08 Sep 2023 21:38:18 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Sep 2023 21:38:19 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Fri, 08 Sep 2023 21:38:19 GMT
ENV APIFIREWALL_VERSION=v0.6.13
# Fri, 08 Sep 2023 21:38:21 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='42bc189c8302221d37eea69297a0edd8aa485f8856225019f4773bbbe72b4363';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='186e46d26eb64ccc10ea07b91fc7602cff5eba13f13ec5314222a65f991f8717';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='898eb09cae9b314f302be6fb27e6618428ded24cddc569fe8c37b27a02977657';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Fri, 08 Sep 2023 21:38:22 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Fri, 08 Sep 2023 21:38:22 GMT
USER api-firewall
# Fri, 08 Sep 2023 21:38:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Sep 2023 21:38:22 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810732c4c5731539752999614fb1453fcd5a97a7ddfc937d972268903995410e`  
		Last Modified: Fri, 08 Sep 2023 21:38:36 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a80848339d19fca5533c84901c1d184c734b59a42f334588c233b0f2b64cd56`  
		Last Modified: Fri, 08 Sep 2023 21:38:38 GMT  
		Size: 9.0 MB (8993216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba7c9d79244812fe45486a3adc5053998ec5e22a579bb40dcb8ff2fa73e4161`  
		Last Modified: Fri, 08 Sep 2023 21:38:36 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
