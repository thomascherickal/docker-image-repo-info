<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.0.0.21`](#aerospike50021)
-	[`aerospike:5.1.0.18`](#aerospike51018)
-	[`aerospike:5.2.0.10`](#aerospike52010)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.0.0.21`

```console
$ docker pull aerospike@sha256:f84df2396f609bf41d7002507be09a9619de03037516b6c9ecb3d8720228af36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.0.0.21` - linux; amd64

```console
$ docker pull aerospike@sha256:21aec67a9b18e465447884d209170b9ea56c7dd89ad86187ef8e0949153df231
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.8 MB (59783183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bd53bf76fa645a7041245896d36c01335f58569f5bbe1782cc2c7d040526630`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Wed, 02 Dec 2020 22:19:49 GMT
ENV AEROSPIKE_VERSION=5.0.0.21
# Wed, 02 Dec 2020 22:19:50 GMT
ENV AEROSPIKE_SHA256=67f3e77588ed17f75da1599f787373bdd2ef032fdc8e479a757b8b3f3289e007
# Wed, 02 Dec 2020 22:20:08 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 02 Dec 2020 22:20:08 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 02 Dec 2020 22:20:09 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 02 Dec 2020 22:20:09 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 02 Dec 2020 22:20:09 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 02 Dec 2020 22:20:09 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cbfca006d7195aa7bbaa6ed4d2a3ac8d3618537873a522fd490d2f5415917e`  
		Last Modified: Wed, 02 Dec 2020 22:21:13 GMT  
		Size: 37.3 MB (37253467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f8923145f527aa0bb295b2636113235bd92b969a6be8b37313407d0c68f8d0`  
		Last Modified: Wed, 02 Dec 2020 22:21:08 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01749a7d2817dd42173ef40a8236fb8cd5d1f4897ce662bec36b3355d6a09601`  
		Last Modified: Wed, 02 Dec 2020 22:21:08 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.1.0.18`

```console
$ docker pull aerospike@sha256:2f29977dc10974d8315dc2b7171765f8818e94dac98007fee2dc02061c3c2c99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.1.0.18` - linux; amd64

```console
$ docker pull aerospike@sha256:45ea85c705e7c345fbe8f8c31eb7ff9deff9ef830cbc22da27536362d9162156
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67216666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:234367ebee7abd42ff3622d87ad72b85aee93aafd4c39d598f5406ba2e547a8b`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Wed, 02 Dec 2020 22:20:15 GMT
ENV AEROSPIKE_VERSION=5.1.0.18
# Wed, 02 Dec 2020 22:20:15 GMT
ENV AEROSPIKE_SHA256=372d6c8dbdf00226908607d1561d717cd856f384bb6bd87a3269d1bc2533d555
# Wed, 02 Dec 2020 22:20:33 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 02 Dec 2020 22:20:33 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 02 Dec 2020 22:20:33 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 02 Dec 2020 22:20:33 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 02 Dec 2020 22:20:34 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 02 Dec 2020 22:20:34 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42df76b579f5709758f5a53594456cbf5433696f64d23c7842ae48f1a40ef92`  
		Last Modified: Wed, 02 Dec 2020 22:21:27 GMT  
		Size: 44.7 MB (44686949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cbf6a6962375d95ea2a4445681e32932656fab89deea73ba42b98fe8476b7a`  
		Last Modified: Wed, 02 Dec 2020 22:21:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f875809fbee29fc5fb11e765e41655c9a90725f027bba766324e928adfb9b2b0`  
		Last Modified: Wed, 02 Dec 2020 22:21:20 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.2.0.10`

```console
$ docker pull aerospike@sha256:46c2d19d68632769e58266852e2afc35b286945d1b3b545f629a1ee1e83b08de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.2.0.10` - linux; amd64

```console
$ docker pull aerospike@sha256:7d5c9d9dad448ef1cbfdf28f8b556233a98532214ee9743560c2f22bcc529002
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67133456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e5381aae1d1c057b2162d8218e48483936aa3d250b3fc8996c0585ab8b58b0`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Wed, 02 Dec 2020 22:20:40 GMT
ENV AEROSPIKE_VERSION=5.2.0.10
# Wed, 02 Dec 2020 22:20:40 GMT
ENV AEROSPIKE_SHA256=7b765d77cc391d7ea3991c335801972b703e01ac19b9116d266b5c0b57f1ca8d
# Wed, 02 Dec 2020 22:20:58 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 02 Dec 2020 22:20:58 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 02 Dec 2020 22:20:59 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 02 Dec 2020 22:20:59 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 02 Dec 2020 22:20:59 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 02 Dec 2020 22:20:59 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9931d16fcead8dbc4a81400c40d14aafbd07d33d8873a21615921446703d07`  
		Last Modified: Wed, 02 Dec 2020 22:21:55 GMT  
		Size: 44.6 MB (44603738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dba7dedfc03ec7b589456d2cc225e06b04a83007a271baf75b68616cca002ac`  
		Last Modified: Wed, 02 Dec 2020 22:21:48 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82263b92be05614db8490795a7d1c7ce0a931cd7fdb8cc5ce7e1b87e5b5ffcbb`  
		Last Modified: Wed, 02 Dec 2020 22:21:49 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:46c2d19d68632769e58266852e2afc35b286945d1b3b545f629a1ee1e83b08de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:7d5c9d9dad448ef1cbfdf28f8b556233a98532214ee9743560c2f22bcc529002
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67133456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e5381aae1d1c057b2162d8218e48483936aa3d250b3fc8996c0585ab8b58b0`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Wed, 02 Dec 2020 22:20:40 GMT
ENV AEROSPIKE_VERSION=5.2.0.10
# Wed, 02 Dec 2020 22:20:40 GMT
ENV AEROSPIKE_SHA256=7b765d77cc391d7ea3991c335801972b703e01ac19b9116d266b5c0b57f1ca8d
# Wed, 02 Dec 2020 22:20:58 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 02 Dec 2020 22:20:58 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 02 Dec 2020 22:20:59 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 02 Dec 2020 22:20:59 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 02 Dec 2020 22:20:59 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 02 Dec 2020 22:20:59 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9931d16fcead8dbc4a81400c40d14aafbd07d33d8873a21615921446703d07`  
		Last Modified: Wed, 02 Dec 2020 22:21:55 GMT  
		Size: 44.6 MB (44603738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dba7dedfc03ec7b589456d2cc225e06b04a83007a271baf75b68616cca002ac`  
		Last Modified: Wed, 02 Dec 2020 22:21:48 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82263b92be05614db8490795a7d1c7ce0a931cd7fdb8cc5ce7e1b87e5b5ffcbb`  
		Last Modified: Wed, 02 Dec 2020 22:21:49 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
