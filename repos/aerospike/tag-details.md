<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:4.9.0.11`](#aerospike49011)
-	[`aerospike:5.0.0.11`](#aerospike50011)
-	[`aerospike:5.1.0.6`](#aerospike5106)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:4.9.0.11`

```console
$ docker pull aerospike@sha256:6cea592c4795537e590b1061b49ac54d43877f789a75a74f95cc212e74572178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.9.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:16fabc354e5d699412b19d3e35c0ef2dd949b2f95f4a27b4f5bc2148bbf8c81a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53208035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0721374062929d066468d72fcd033e8bb6bcb09ead7cae98d5cc6496f5016dbb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 04:15:32 GMT
ENV AEROSPIKE_VERSION=4.9.0.11
# Wed, 05 Aug 2020 04:15:32 GMT
ENV AEROSPIKE_SHA256=6e53582b74800b5e93224ed34f30d2c8a3c191c7d27284070347fc7d8bb13fec
# Wed, 05 Aug 2020 04:15:48 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 05 Aug 2020 04:15:49 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 05 Aug 2020 04:15:49 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 05 Aug 2020 04:15:49 GMT
VOLUME [/opt/aerospike/data]
# Wed, 05 Aug 2020 04:15:49 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 05 Aug 2020 04:15:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Aug 2020 04:15:49 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa85c12a4ce0ecdaf61499b401d2aecae07d38ef1ecfebb7a21dda5644310de`  
		Last Modified: Wed, 05 Aug 2020 04:16:32 GMT  
		Size: 30.7 MB (30683708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf44b117208249260d2675e7e5b2b2ea559ab00e7d9c90b07f0718f330a44a1`  
		Last Modified: Wed, 05 Aug 2020 04:16:27 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146a1f1533a0c8a4c812b98c0b7a0b9a395638b6690b95c051d1dbd58b56ffb5`  
		Last Modified: Wed, 05 Aug 2020 04:16:27 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.0.0.11`

```console
$ docker pull aerospike@sha256:6269b6273a809a56852880c9a0af17647bd4974428dacafdcf6609262ed2d5de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.0.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:65c7833a169438aebbbbed1961364baadc8efb4574ad3f98b2eebf5d61171ed0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58576357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:450ee9276e9941ad3722b943da2ea1b0755324df0533d4ef7974a9ae2b0793e1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Mon, 17 Aug 2020 22:19:28 GMT
ENV AEROSPIKE_VERSION=5.0.0.11
# Mon, 17 Aug 2020 22:19:28 GMT
ENV AEROSPIKE_SHA256=1df0eb6d966397572a5a350c72d76013eb7357c8d9614730a8e2b560c85d793a
# Mon, 17 Aug 2020 22:19:46 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Mon, 17 Aug 2020 22:19:46 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Mon, 17 Aug 2020 22:19:46 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Mon, 17 Aug 2020 22:19:46 GMT
VOLUME [/opt/aerospike/data]
# Mon, 17 Aug 2020 22:19:47 GMT
EXPOSE 3000 3001 3002 3003
# Mon, 17 Aug 2020 22:19:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 17 Aug 2020 22:19:47 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc64a48b793424ef387218d295c75e68cd4915e356ccfa60638a9fc7c318072`  
		Last Modified: Mon, 17 Aug 2020 22:20:30 GMT  
		Size: 36.1 MB (36052032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e414b2788f3f1136a5bd012052579e9d81e069b3a7aa2956e3ae40ae988f4d02`  
		Last Modified: Mon, 17 Aug 2020 22:20:24 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbc3d28f4d355c30ef1ea05802013712fc64192bca2515e69ae80bacc00edaf`  
		Last Modified: Mon, 17 Aug 2020 22:20:24 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.1.0.6`

```console
$ docker pull aerospike@sha256:065cbb8d3d7a9f4b34178d50a73c5f5d7fafcfb71314a61d2a354ac664699c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.1.0.6` - linux; amd64

```console
$ docker pull aerospike@sha256:88f1191ca783e74355000bc1e247c62a0ad3277bee025daafaed8504570192dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66011213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46bdce9abaaa743f1020ff9e923c022f1dae46b3301d6419ea39765a826e378c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Tue, 18 Aug 2020 20:19:30 GMT
ENV AEROSPIKE_VERSION=5.1.0.6
# Tue, 18 Aug 2020 20:19:31 GMT
ENV AEROSPIKE_SHA256=64d39a81286de648592add8a4de3037c4141d55a135dfeddfa4b3c6534c297e7
# Tue, 18 Aug 2020 20:19:48 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 18 Aug 2020 20:19:48 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 18 Aug 2020 20:19:48 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 18 Aug 2020 20:19:49 GMT
VOLUME [/opt/aerospike/data]
# Tue, 18 Aug 2020 20:19:49 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 18 Aug 2020 20:19:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 18 Aug 2020 20:19:49 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00c09823ef0005ce5ed526e2f1922828405cba3952c6d38fc5df9d3a1047f90`  
		Last Modified: Tue, 18 Aug 2020 20:20:07 GMT  
		Size: 43.5 MB (43486883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac08e522e5e9db03b0e3787896455e01fc38b8b7f3333c7fba70c70273e2a33c`  
		Last Modified: Tue, 18 Aug 2020 20:20:01 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb7643131170ce42d78dc6001424b3b0e73bd4630e34458a18319dcab4a9e5d`  
		Last Modified: Tue, 18 Aug 2020 20:20:00 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:065cbb8d3d7a9f4b34178d50a73c5f5d7fafcfb71314a61d2a354ac664699c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:88f1191ca783e74355000bc1e247c62a0ad3277bee025daafaed8504570192dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66011213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46bdce9abaaa743f1020ff9e923c022f1dae46b3301d6419ea39765a826e378c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Tue, 18 Aug 2020 20:19:30 GMT
ENV AEROSPIKE_VERSION=5.1.0.6
# Tue, 18 Aug 2020 20:19:31 GMT
ENV AEROSPIKE_SHA256=64d39a81286de648592add8a4de3037c4141d55a135dfeddfa4b3c6534c297e7
# Tue, 18 Aug 2020 20:19:48 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 18 Aug 2020 20:19:48 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 18 Aug 2020 20:19:48 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 18 Aug 2020 20:19:49 GMT
VOLUME [/opt/aerospike/data]
# Tue, 18 Aug 2020 20:19:49 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 18 Aug 2020 20:19:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 18 Aug 2020 20:19:49 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00c09823ef0005ce5ed526e2f1922828405cba3952c6d38fc5df9d3a1047f90`  
		Last Modified: Tue, 18 Aug 2020 20:20:07 GMT  
		Size: 43.5 MB (43486883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac08e522e5e9db03b0e3787896455e01fc38b8b7f3333c7fba70c70273e2a33c`  
		Last Modified: Tue, 18 Aug 2020 20:20:01 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb7643131170ce42d78dc6001424b3b0e73bd4630e34458a18319dcab4a9e5d`  
		Last Modified: Tue, 18 Aug 2020 20:20:00 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
