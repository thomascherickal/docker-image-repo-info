<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `api-firewall`

-	[`api-firewall:0.6.9`](#api-firewall069)
-	[`api-firewall:latest`](#api-firewalllatest)

## `api-firewall:0.6.9`

```console
$ docker pull api-firewall@sha256:c5318488bd8345b5fae9c73cc74d68fb4188b3382931e0e100cf96ab856ba63c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; 386

### `api-firewall:0.6.9` - linux; 386

```console
$ docker pull api-firewall@sha256:0abdf9aa023600002e6da07ff0df3a4a6b6504b2902851c35bff3346872cfb27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7852547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030228d056fee4ea49f1ea31a8d0448f0d2002f9e9749c17c919573a2116d5ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 13 Sep 2022 23:38:19 GMT
ENV APIFW_PATH=/opt/api-firewall
# Tue, 13 Sep 2022 23:38:20 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 23:38:21 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Tue, 13 Sep 2022 23:38:22 GMT
ENV APIFIREWALL_VERSION=v0.6.9
# Tue, 13 Sep 2022 23:38:24 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='12f0b039e84f71298ebc17777910cdd7618e76f65f3356d2e890c3b45f01ef19';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='4f31329e9f2391460450e83096b0b17afa08649e17870f8667f1187aacc5ae00';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='acdce9e1e3d5ecc46be56d3a6b5a70a84de44c53d342a02b8e5f848624ae4b16';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Tue, 13 Sep 2022 23:38:26 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Tue, 13 Sep 2022 23:38:26 GMT
USER api-firewall
# Tue, 13 Sep 2022 23:38:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 23:38:28 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ea01151e49b0feeb818b1340300dc6c2c1623782685713ed0a3758a34275a8`  
		Last Modified: Tue, 13 Sep 2022 23:38:41 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20570c6fdc149273b2162b29616c1a15b4a7da8cc1bf65d422fb1e8563e1dfe`  
		Last Modified: Tue, 13 Sep 2022 23:38:41 GMT  
		Size: 5.0 MB (5043868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5c5db1005409861d9989a02a9626b8b179d32535f883039f0c416704531caf`  
		Last Modified: Tue, 13 Sep 2022 23:38:41 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `api-firewall:latest`

```console
$ docker pull api-firewall@sha256:d798d049fbf7ad98715fb705ef388d0966037d9a563ed78ecc9bcf35bd33823c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:latest` - linux; amd64

```console
$ docker pull api-firewall@sha256:c2ddf78dead8053c2fc2934c8596e081ac575a6f0fdd35f4824703681e3728f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7579923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2557517f85256294702dafbd88e3fb62c567277548bffe6ff868eb4ba657a36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:47:39 GMT
ENV APIFW_PATH=/opt/api-firewall
# Tue, 09 Aug 2022 17:47:39 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 17:47:39 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Tue, 09 Aug 2022 17:47:39 GMT
ENV APIFIREWALL_VERSION=v0.6.8
# Tue, 09 Aug 2022 17:47:41 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='af8e49e7ebf19d68b4dcf09a0f0b04b36a5c6e3f556549cb48852fcebac03892';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='b15fa8bfb98d23760eac894002db79420cdc321c1f1baabf60fba54556dfdab7';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='d37c9cef562788caf0177224516c555808251a6d79a368b4902424d57037d023';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Tue, 09 Aug 2022 17:47:41 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Tue, 09 Aug 2022 17:47:41 GMT
USER api-firewall
# Tue, 09 Aug 2022 17:47:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 17:47:41 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e62924cbb5cae95f3719d409db2c9d3db9b2566cefe562b49879111b3c78b66`  
		Last Modified: Tue, 09 Aug 2022 17:47:49 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41a238989c27ee4f9089df52b4f5af75ea74f4fae1d6a8d1586008974d67787`  
		Last Modified: Tue, 09 Aug 2022 17:47:50 GMT  
		Size: 4.8 MB (4754859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f619bbb80421d4f9885e17d2514dce73fb8adcd9dfc1aaec17f007a71dba1b`  
		Last Modified: Tue, 09 Aug 2022 17:47:49 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:b7aee27e00caef24ca96b57665bb144b9b439e23dc3812091db6d66ce792fcac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7180199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c51bca350d4818e8e4496cdca3e0c1f1417df0c6bbde661efccaa283580b57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:08:37 GMT
ENV APIFW_PATH=/opt/api-firewall
# Wed, 10 Aug 2022 05:08:38 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 05:08:39 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Wed, 10 Aug 2022 05:08:40 GMT
ENV APIFIREWALL_VERSION=v0.6.8
# Wed, 10 Aug 2022 05:08:42 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='af8e49e7ebf19d68b4dcf09a0f0b04b36a5c6e3f556549cb48852fcebac03892';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='b15fa8bfb98d23760eac894002db79420cdc321c1f1baabf60fba54556dfdab7';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='d37c9cef562788caf0177224516c555808251a6d79a368b4902424d57037d023';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Wed, 10 Aug 2022 05:08:44 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Wed, 10 Aug 2022 05:08:44 GMT
USER api-firewall
# Wed, 10 Aug 2022 05:08:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 05:08:46 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13ab663c8e7ed005ee832cb2ccb6e28be83a104f521e9cd4ccc243c41704126`  
		Last Modified: Wed, 10 Aug 2022 05:08:59 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095228fb65dca5b600f4f4e869e280ab53df8a65a5af6247f1957ce4659492b9`  
		Last Modified: Wed, 10 Aug 2022 05:09:00 GMT  
		Size: 4.5 MB (4460203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b30d0e56cfd261c4094b87053d2833936c3bfd679b7f539ad5fbb1a8b37e41`  
		Last Modified: Wed, 10 Aug 2022 05:08:59 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; 386

```console
$ docker pull api-firewall@sha256:0abdf9aa023600002e6da07ff0df3a4a6b6504b2902851c35bff3346872cfb27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7852547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030228d056fee4ea49f1ea31a8d0448f0d2002f9e9749c17c919573a2116d5ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 13 Sep 2022 23:38:19 GMT
ENV APIFW_PATH=/opt/api-firewall
# Tue, 13 Sep 2022 23:38:20 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 23:38:21 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Tue, 13 Sep 2022 23:38:22 GMT
ENV APIFIREWALL_VERSION=v0.6.9
# Tue, 13 Sep 2022 23:38:24 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='12f0b039e84f71298ebc17777910cdd7618e76f65f3356d2e890c3b45f01ef19';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='4f31329e9f2391460450e83096b0b17afa08649e17870f8667f1187aacc5ae00';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='acdce9e1e3d5ecc46be56d3a6b5a70a84de44c53d342a02b8e5f848624ae4b16';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Tue, 13 Sep 2022 23:38:26 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Tue, 13 Sep 2022 23:38:26 GMT
USER api-firewall
# Tue, 13 Sep 2022 23:38:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 23:38:28 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ea01151e49b0feeb818b1340300dc6c2c1623782685713ed0a3758a34275a8`  
		Last Modified: Tue, 13 Sep 2022 23:38:41 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20570c6fdc149273b2162b29616c1a15b4a7da8cc1bf65d422fb1e8563e1dfe`  
		Last Modified: Tue, 13 Sep 2022 23:38:41 GMT  
		Size: 5.0 MB (5043868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5c5db1005409861d9989a02a9626b8b179d32535f883039f0c416704531caf`  
		Last Modified: Tue, 13 Sep 2022 23:38:41 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
