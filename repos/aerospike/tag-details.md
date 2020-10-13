<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.0.0.13`](#aerospike50013)
-	[`aerospike:5.1.0.10`](#aerospike51010)
-	[`aerospike:5.2.0.2`](#aerospike5202)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.0.0.13`

```console
$ docker pull aerospike@sha256:67a5b6a5151016d8569cf71a435f3a231a441a0c91a95310a085148e17b0fd6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.0.0.13` - linux; amd64

```console
$ docker pull aerospike@sha256:3d44bc2efe8589c00259c50930018c68b43f552c76b2dc46c7698b703a45b3d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58576330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bacd292bbbf648de0c283ed6675ce4c8e18d46c9b9148c776066622a97262861`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:07:22 GMT
ENV AEROSPIKE_VERSION=5.0.0.13
# Tue, 13 Oct 2020 02:07:22 GMT
ENV AEROSPIKE_SHA256=17850647ecb0b1e92714acbb8ae4e77034d292c6d891251a2bfaac3fe48bd03f
# Tue, 13 Oct 2020 02:07:40 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 13 Oct 2020 02:07:40 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 13 Oct 2020 02:07:40 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 13 Oct 2020 02:07:40 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 13 Oct 2020 02:07:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Oct 2020 02:07:41 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f7c8cd28a8caabf7186718acfd1249914aa96cb54c855c0bf9119422342a19`  
		Last Modified: Tue, 13 Oct 2020 02:08:48 GMT  
		Size: 36.1 MB (36052184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2c7a15e9bc99f03bd17a123e37bf600e5a980d2787b5d598dbf0a00ad8cbd8`  
		Last Modified: Tue, 13 Oct 2020 02:08:42 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1602c2ebd68de75cd391e2cbc80be51d7252bfd16a2087be322bf988fd9d87`  
		Last Modified: Tue, 13 Oct 2020 02:08:42 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.1.0.10`

```console
$ docker pull aerospike@sha256:3e5f689d431a14d690f589ef8a1f56cf4e1691f11d1a06f2c85f3f5d04e526d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.1.0.10` - linux; amd64

```console
$ docker pull aerospike@sha256:4075660b741d8eb2052dc36db6084bee8c1d0739fcea8688381265cd97bc9b41
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66024929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1159de391bea492b52163e56fab888db47b074e790e0d8e22b7f5e0f8ee7f9b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:07:47 GMT
ENV AEROSPIKE_VERSION=5.1.0.10
# Tue, 13 Oct 2020 02:07:48 GMT
ENV AEROSPIKE_SHA256=6e2bf927a092725385fbdb70ec90bc0b6431c5e0d3aa8bcc8c7f57c7ddf09cac
# Tue, 13 Oct 2020 02:08:05 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 13 Oct 2020 02:08:05 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 13 Oct 2020 02:08:05 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 13 Oct 2020 02:08:06 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 13 Oct 2020 02:08:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Oct 2020 02:08:06 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4461fba123ed98a0fbaad249382cf126fddf4bcf60be76da0d5ac5e6d373cce`  
		Last Modified: Tue, 13 Oct 2020 02:08:59 GMT  
		Size: 43.5 MB (43500783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ade7f31811b72ce197d081fc30b6528b67a46e37c922161e49f066a60ec5b15`  
		Last Modified: Tue, 13 Oct 2020 02:08:51 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b0d423a4eac756b64d39e1e5512d42246aa8cd46f019bb408b35187ee09b58`  
		Last Modified: Tue, 13 Oct 2020 02:08:51 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.2.0.2`

```console
$ docker pull aerospike@sha256:d71523c6dc8c1e6ce07a5d334c9359bd7eaf8ddda966a69ffafe603bb6db4e27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.2.0.2` - linux; amd64

```console
$ docker pull aerospike@sha256:4373020099cbd573237383d08f3c5c80e58e7809ce13e189f84d918af0ae71b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65942546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77cefb0b2db366341ae122429841ec8c54310ed0c889ac3fddfb9976551f8d05`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:08:13 GMT
ENV AEROSPIKE_VERSION=5.2.0.2
# Tue, 13 Oct 2020 02:08:13 GMT
ENV AEROSPIKE_SHA256=a60799791567b845d20aeaf73adf96ed2285d08145b3c5cac6746cc4e1f1f0d5
# Tue, 13 Oct 2020 02:08:31 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 13 Oct 2020 02:08:31 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 13 Oct 2020 02:08:31 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 13 Oct 2020 02:08:31 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 13 Oct 2020 02:08:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Oct 2020 02:08:32 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00e6f34fb632f1998297dae34a3fc45e1a6baa7c77e1f8ebf74b09c2e4c94b9`  
		Last Modified: Tue, 13 Oct 2020 02:09:11 GMT  
		Size: 43.4 MB (43418402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed7d72d257e69c61fdb01e075396c759ad5ac473c4f46d37e2312603bed5fc7`  
		Last Modified: Tue, 13 Oct 2020 02:09:02 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d186831b372e10b426dd0fa1e11c70beebb8418f827d5fc0aa3299dc7630d4`  
		Last Modified: Tue, 13 Oct 2020 02:09:02 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:d71523c6dc8c1e6ce07a5d334c9359bd7eaf8ddda966a69ffafe603bb6db4e27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:4373020099cbd573237383d08f3c5c80e58e7809ce13e189f84d918af0ae71b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65942546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77cefb0b2db366341ae122429841ec8c54310ed0c889ac3fddfb9976551f8d05`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:08:13 GMT
ENV AEROSPIKE_VERSION=5.2.0.2
# Tue, 13 Oct 2020 02:08:13 GMT
ENV AEROSPIKE_SHA256=a60799791567b845d20aeaf73adf96ed2285d08145b3c5cac6746cc4e1f1f0d5
# Tue, 13 Oct 2020 02:08:31 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 13 Oct 2020 02:08:31 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 13 Oct 2020 02:08:31 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 13 Oct 2020 02:08:31 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 13 Oct 2020 02:08:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Oct 2020 02:08:32 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00e6f34fb632f1998297dae34a3fc45e1a6baa7c77e1f8ebf74b09c2e4c94b9`  
		Last Modified: Tue, 13 Oct 2020 02:09:11 GMT  
		Size: 43.4 MB (43418402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed7d72d257e69c61fdb01e075396c759ad5ac473c4f46d37e2312603bed5fc7`  
		Last Modified: Tue, 13 Oct 2020 02:09:02 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d186831b372e10b426dd0fa1e11c70beebb8418f827d5fc0aa3299dc7630d4`  
		Last Modified: Tue, 13 Oct 2020 02:09:02 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
