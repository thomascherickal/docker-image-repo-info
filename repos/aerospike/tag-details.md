<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.0.0.18`](#aerospike50018)
-	[`aerospike:5.1.0.15`](#aerospike51015)
-	[`aerospike:5.2.0.7`](#aerospike5207)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.0.0.18`

```console
$ docker pull aerospike@sha256:974b2abba7d4ebd4764f6fb03d08e5d3323208260116c2ddbfa09e0827f6078f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.0.0.18` - linux; amd64

```console
$ docker pull aerospike@sha256:4f4464ad22e26377323b39e008e45056561364867aa29c6b26b658f3bf7c3cac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.8 MB (59782978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ea237304351732c586dc0f57e6d364bfaf0802859bac19e019fab2d6062e8b`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 05:57:53 GMT
ENV AEROSPIKE_VERSION=5.0.0.18
# Wed, 18 Nov 2020 05:57:53 GMT
ENV AEROSPIKE_SHA256=108cbf5c90542a2760549a934a71f6267899c6589b1e21bf8a5d79ac9665ff18
# Wed, 18 Nov 2020 05:58:13 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 18 Nov 2020 05:58:13 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 18 Nov 2020 05:58:14 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 18 Nov 2020 05:58:14 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 18 Nov 2020 05:58:14 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 18 Nov 2020 05:58:14 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f01e67a12ec19336efc124dba050e34966b5d95bdb7775b54662e81045b40b`  
		Last Modified: Wed, 18 Nov 2020 05:59:34 GMT  
		Size: 37.3 MB (37253263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c40c8e3760219ece36d9616d6dee2a7eb6078e3387d76b9eb43b5d2785515bc`  
		Last Modified: Wed, 18 Nov 2020 05:59:23 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50de72d45c308703189f1eb595240211d0002811f1edf90abaca2be41bbc403`  
		Last Modified: Wed, 18 Nov 2020 05:59:24 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.1.0.15`

```console
$ docker pull aerospike@sha256:160e31f9e2d054fe2b3a558a3375377b98b31d3ad3bcc7c4f7209da4e43b8bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.1.0.15` - linux; amd64

```console
$ docker pull aerospike@sha256:2e2e7ccd03f82e55adbdccbf22ceb0abfa41c877674af71348a0d08cf958e3fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67216962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:909a9cd72f1b29bee74ff872be479b6513121226d9f711ebbf8a5bb22f84a53f`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 05:58:19 GMT
ENV AEROSPIKE_VERSION=5.1.0.15
# Wed, 18 Nov 2020 05:58:19 GMT
ENV AEROSPIKE_SHA256=e356aa2b6cc4e93d6030f1f8f5c598a8c2a17f00723e82d89c77dc9266ed67bc
# Wed, 18 Nov 2020 05:58:40 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 18 Nov 2020 05:58:40 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 18 Nov 2020 05:58:40 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 18 Nov 2020 05:58:40 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 18 Nov 2020 05:58:41 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 18 Nov 2020 05:58:41 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2ba0b386dace8d3a57b1adc22ed94da33e607db3e7a8506d3fa3c1f098b549`  
		Last Modified: Wed, 18 Nov 2020 05:59:48 GMT  
		Size: 44.7 MB (44687243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a69fbec82d8667bef2f9d6416e8abe98426c3962e28e1af7711fc99e4a66598`  
		Last Modified: Wed, 18 Nov 2020 05:59:38 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dffa74950c51437d1456cbda9f2bc0011c599aa8ad566f43503dc26d91476e8`  
		Last Modified: Wed, 18 Nov 2020 05:59:38 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.2.0.7`

```console
$ docker pull aerospike@sha256:4ee617950476bce828e148d231cb3e209c0c0bf906a269ba617095ecd0dfc840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.2.0.7` - linux; amd64

```console
$ docker pull aerospike@sha256:c9633e8c0d4c3054f5099b26758fe32ba94e8cf39206e06980dcc8ebb91fbf1d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67133888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58f0c9a663d11a966448619daceaafcd8165ea4a1223087f64651f448364e9a9`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 05:58:48 GMT
ENV AEROSPIKE_VERSION=5.2.0.7
# Wed, 18 Nov 2020 05:58:48 GMT
ENV AEROSPIKE_SHA256=5f64b516be56f16a708991785d9525c18dc16f73418070738c3e5dd3dcae7ea8
# Wed, 18 Nov 2020 05:59:11 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 18 Nov 2020 05:59:11 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 18 Nov 2020 05:59:12 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 18 Nov 2020 05:59:12 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 18 Nov 2020 05:59:12 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 18 Nov 2020 05:59:12 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee4ca5131e1d8f81e18c4b04103695bcb8ee63af05cc2731a08b4dbae020b06`  
		Last Modified: Wed, 18 Nov 2020 06:00:04 GMT  
		Size: 44.6 MB (44604172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2abbd6b8920677d4e83288e4af49a3c36d796c8ec4d96518f44cb6e8a34143c`  
		Last Modified: Wed, 18 Nov 2020 05:59:53 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2728479151082ff2e2d8897461f0f1b095e417dcad03ee2c68d1086ce915c799`  
		Last Modified: Wed, 18 Nov 2020 05:59:53 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:4ee617950476bce828e148d231cb3e209c0c0bf906a269ba617095ecd0dfc840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:c9633e8c0d4c3054f5099b26758fe32ba94e8cf39206e06980dcc8ebb91fbf1d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67133888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58f0c9a663d11a966448619daceaafcd8165ea4a1223087f64651f448364e9a9`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 05:58:48 GMT
ENV AEROSPIKE_VERSION=5.2.0.7
# Wed, 18 Nov 2020 05:58:48 GMT
ENV AEROSPIKE_SHA256=5f64b516be56f16a708991785d9525c18dc16f73418070738c3e5dd3dcae7ea8
# Wed, 18 Nov 2020 05:59:11 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 18 Nov 2020 05:59:11 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 18 Nov 2020 05:59:12 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 18 Nov 2020 05:59:12 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 18 Nov 2020 05:59:12 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 18 Nov 2020 05:59:12 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee4ca5131e1d8f81e18c4b04103695bcb8ee63af05cc2731a08b4dbae020b06`  
		Last Modified: Wed, 18 Nov 2020 06:00:04 GMT  
		Size: 44.6 MB (44604172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2abbd6b8920677d4e83288e4af49a3c36d796c8ec4d96518f44cb6e8a34143c`  
		Last Modified: Wed, 18 Nov 2020 05:59:53 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2728479151082ff2e2d8897461f0f1b095e417dcad03ee2c68d1086ce915c799`  
		Last Modified: Wed, 18 Nov 2020 05:59:53 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
