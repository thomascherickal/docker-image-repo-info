## `api-firewall:latest`

```console
$ docker pull api-firewall@sha256:c60116726e92fdfc93e808ad09ca06a1917cc17bb33e7ec3a354730c3f198713
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:latest` - linux; amd64

```console
$ docker pull api-firewall@sha256:d96bad24ad185c8a7e8926645c2361a8df38bd50e4966de7a0b5d8f37af3c44f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8914291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e31c38302ee23f3bd9fe64067d483f8b658f23adcc44207e60a4cd23c8b20e95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Fri, 16 Dec 2022 18:19:25 GMT
ENV APIFW_PATH=/opt/api-firewall
# Fri, 16 Dec 2022 18:19:25 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 18:19:26 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Fri, 16 Dec 2022 18:19:26 GMT
ENV APIFIREWALL_VERSION=v0.6.10
# Fri, 16 Dec 2022 18:19:28 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='774d29f694142984e11e31443398a973a882d19c491e06390de13f0ceabd04a4';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='6ef69fbafb2503c7b01681d39138ea1abe99da910912fde33b1c317a819d2804';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='a9ccd2757bb4703b70aeea44b8aa992ce0dc1025d36accf311a023d87b1b6f57';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Fri, 16 Dec 2022 18:19:28 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Fri, 16 Dec 2022 18:19:29 GMT
USER api-firewall
# Fri, 16 Dec 2022 18:19:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Dec 2022 18:19:29 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d1ba519f3f5dace47b10bf782d3efefbebe2e2f219a702c79f43f5f053c781`  
		Last Modified: Fri, 16 Dec 2022 18:19:37 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71ac454eeac4da269751f26d64817a93960cc8b11f729a1007d9d5774cff39a`  
		Last Modified: Fri, 16 Dec 2022 18:19:38 GMT  
		Size: 5.5 MB (5542027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c142feb87dabe26f309b2276077c340166d2f71f9cdbd05fc7f0632b5a630847`  
		Last Modified: Fri, 16 Dec 2022 18:19:37 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:f59fdd7b0c3c8eac791859bc83290a4b61b192d10079fa12aa997235efadbc22
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8428223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b039139104a75a910c81c8d167834e9a543337256e9d8cbd0fc75c451e11549f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Fri, 16 Dec 2022 18:53:52 GMT
ENV APIFW_PATH=/opt/api-firewall
# Fri, 16 Dec 2022 18:53:52 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 18:53:52 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Fri, 16 Dec 2022 18:53:52 GMT
ENV APIFIREWALL_VERSION=v0.6.10
# Fri, 16 Dec 2022 18:53:55 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='774d29f694142984e11e31443398a973a882d19c491e06390de13f0ceabd04a4';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='6ef69fbafb2503c7b01681d39138ea1abe99da910912fde33b1c317a819d2804';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='a9ccd2757bb4703b70aeea44b8aa992ce0dc1025d36accf311a023d87b1b6f57';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Fri, 16 Dec 2022 18:53:55 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Fri, 16 Dec 2022 18:53:55 GMT
USER api-firewall
# Fri, 16 Dec 2022 18:53:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Dec 2022 18:53:55 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7770a2bf8d0670267c867aca01d2ed0ced5d6d48847ba06e7af1b49a246b648`  
		Last Modified: Fri, 16 Dec 2022 18:54:04 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9295650c6457ac6c67b42d45d9104401c6ce33193f37333ae4ed2227dbfa9f`  
		Last Modified: Fri, 16 Dec 2022 18:54:05 GMT  
		Size: 5.2 MB (5167474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3746125874adf0d660fc1f43dc75a91a0ac4ee55be99232bf77f0e8d98eae40`  
		Last Modified: Fri, 16 Dec 2022 18:54:04 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; 386

```console
$ docker pull api-firewall@sha256:f1c848d797d97308b286979f32f0932770811a7e3450ef1ad35abf6db1db7d3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8812492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d2bd8344bd9921db008adf8fb226ca1dc80fc0bf48e2c3cbb3b60ed0721f2f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Fri, 16 Dec 2022 18:38:20 GMT
ENV APIFW_PATH=/opt/api-firewall
# Fri, 16 Dec 2022 18:38:21 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Dec 2022 18:38:22 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Fri, 16 Dec 2022 18:38:23 GMT
ENV APIFIREWALL_VERSION=v0.6.10
# Fri, 16 Dec 2022 18:38:27 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='774d29f694142984e11e31443398a973a882d19c491e06390de13f0ceabd04a4';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='6ef69fbafb2503c7b01681d39138ea1abe99da910912fde33b1c317a819d2804';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='a9ccd2757bb4703b70aeea44b8aa992ce0dc1025d36accf311a023d87b1b6f57';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Fri, 16 Dec 2022 18:38:29 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Fri, 16 Dec 2022 18:38:29 GMT
USER api-firewall
# Fri, 16 Dec 2022 18:38:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Dec 2022 18:38:31 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef0000e0588b330ce189c5d0ff8ef593c7240f6a07bde9d4cd34c818e8b2e82`  
		Last Modified: Fri, 16 Dec 2022 18:38:49 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbaf22c7a330976acf03d7f47db03eecb8e88d2cb6c5212a55eadaf8c8dda8a`  
		Last Modified: Fri, 16 Dec 2022 18:38:50 GMT  
		Size: 5.4 MB (5402437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7985bb2a0ccf7ef172b85bdd7ffb9b2d068bbe8b3096a3b160e2ecf380a9ef`  
		Last Modified: Fri, 16 Dec 2022 18:38:49 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
