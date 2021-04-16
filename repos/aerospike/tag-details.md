<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.3.0.16`](#aerospike53016)
-	[`aerospike:5.4.0.11`](#aerospike54011)
-	[`aerospike:5.5.0.9`](#aerospike5509)
-	[`aerospike:ee-5.5.0.9`](#aerospikeee-5509)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.3.0.16`

```console
$ docker pull aerospike@sha256:31d0b435f604314e813d3c1c358cfaeb975e63f1d75877a9d350a1189d1b00fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.3.0.16` - linux; amd64

```console
$ docker pull aerospike@sha256:54ba99197625876811032132491f124cdbd88fe689e6235d6835d9142fb507c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74710040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:374ba444a1b3ec957ee2608e5985d6292add7085c6ae0b61ce0a65624d75b12d`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Thu, 15 Apr 2021 18:19:28 GMT
ENV AEROSPIKE_VERSION=5.3.0.16
# Thu, 15 Apr 2021 18:19:28 GMT
ENV AEROSPIKE_SHA256=9bcda09cf0c1570747a6d97e3de8a550b31ff6cd74700200a75539323229055d
# Thu, 15 Apr 2021 18:19:47 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Thu, 15 Apr 2021 18:19:48 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Thu, 15 Apr 2021 18:19:48 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Thu, 15 Apr 2021 18:19:48 GMT
EXPOSE 3000 3001 3002 3003
# Thu, 15 Apr 2021 18:19:48 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Thu, 15 Apr 2021 18:19:48 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bb83ed23bcfdefed052088c8db7e6cbd6387821567064ae65f7f3e4413e971`  
		Last Modified: Thu, 15 Apr 2021 18:21:22 GMT  
		Size: 52.2 MB (52179721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757c3c868f609ab9eec1cff3d0914ca3bcd62fc81a769aa361354790fc74cb98`  
		Last Modified: Thu, 15 Apr 2021 18:21:12 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436545266fab697fa5d2dd629f9425e5512d85a9a5c51f94c0e7666e181e264`  
		Last Modified: Thu, 15 Apr 2021 18:21:13 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.4.0.11`

```console
$ docker pull aerospike@sha256:5d0abcba0184030d7e9c42c045014f3e22bd7ddd0d76a5a0013d99a4a05770ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.4.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:e7a1dff57225cf51833d7ad56befae35fecb36d87aaf0aef3ebc2a2c2e035cd2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74733922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:635b4d63ec101dbae136bbfa2d553e6d73384a1bc98d0b6cd8c84cdbdc6ba9c2`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Thu, 15 Apr 2021 18:19:53 GMT
ENV AEROSPIKE_VERSION=5.4.0.11
# Thu, 15 Apr 2021 18:19:53 GMT
ENV AEROSPIKE_SHA256=8ce655f36b18bf89f2f0c687c594d222371c2330ffaaa9509697051d7994ebc7
# Thu, 15 Apr 2021 18:20:11 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Thu, 15 Apr 2021 18:20:12 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Thu, 15 Apr 2021 18:20:12 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Thu, 15 Apr 2021 18:20:12 GMT
EXPOSE 3000 3001 3002 3003
# Thu, 15 Apr 2021 18:20:12 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Thu, 15 Apr 2021 18:20:12 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f5d51a8e8c15b561b317c7289a07f166e42b3c5617c57f736020c8c7271d25`  
		Last Modified: Thu, 15 Apr 2021 18:21:39 GMT  
		Size: 52.2 MB (52203606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bd38dbe780ee054aef7853c97a5ef983d232bd8c334bfec897e2fb2ebd990`  
		Last Modified: Thu, 15 Apr 2021 18:21:30 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66f50c67719ad2b4221491b96f915bb33649fd77092dc45da50f23d60ca6290`  
		Last Modified: Thu, 15 Apr 2021 18:21:30 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.5.0.9`

```console
$ docker pull aerospike@sha256:a26a8b17bded550b130952bc012d435e52326de11fbe003f7e2dbc4d42006e9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.5.0.9` - linux; amd64

```console
$ docker pull aerospike@sha256:7a6dfa57401bda85c448186b92f705aa7803dede73c3c9a9a1761fee8b47edb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74775131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76214490c04cad1c54fd71962f4de374be2c4d8253966c05244c897796482374`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Thu, 15 Apr 2021 18:20:15 GMT
ENV AEROSPIKE_VERSION=5.5.0.9
# Thu, 15 Apr 2021 18:20:15 GMT
ENV AEROSPIKE_SHA256=3e4e8f35c4607a465781e8f6b662494ca16717300746064ae7a1c09fd3b5ac90
# Thu, 15 Apr 2021 18:20:33 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Thu, 15 Apr 2021 18:20:34 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Thu, 15 Apr 2021 18:20:34 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Thu, 15 Apr 2021 18:20:34 GMT
EXPOSE 3000 3001 3002 3003
# Thu, 15 Apr 2021 18:20:34 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Thu, 15 Apr 2021 18:20:34 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b52c9d72afa7575ab3e078e166fdaea9e54623b27f25dbf8522423c94b58731`  
		Last Modified: Thu, 15 Apr 2021 18:21:56 GMT  
		Size: 52.2 MB (52244813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d38b2c09d49bc80fe075781829b5e370346973b51b468166b086d8f134239d6`  
		Last Modified: Thu, 15 Apr 2021 18:21:49 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcce1b84cb4dc033a799e8465dad1903cb11ffd83371cca4867d36229ce6c1d`  
		Last Modified: Thu, 15 Apr 2021 18:21:48 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:ee-5.5.0.9`

```console
$ docker pull aerospike@sha256:1b3158d6ff7d12b22969cc67668800c5ef794c58062c0a33a0dbccc2cec6db55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ee-5.5.0.9` - linux; amd64

```console
$ docker pull aerospike@sha256:ddde0bdbb89ecdc84cee491170d3f761e62f0f46130cc0907a622f03d3898016
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76466018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d611d912ae1c6f2c8acd762bf9f815433b3ed7faff407066f735c1e0d3f0a5b`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Thu, 15 Apr 2021 18:20:15 GMT
ENV AEROSPIKE_VERSION=5.5.0.9
# Thu, 15 Apr 2021 18:20:41 GMT
ENV AEROSPIKE_SHA256=ae222dcb2e8deb10e1fe45b27d02f32749ec2259c62a292d253d176689b05a06
# Thu, 15 Apr 2021 18:20:58 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian9" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Thu, 15 Apr 2021 18:20:59 GMT
COPY file:82161ba7b6e7d24ef9aeee8b19996114e9ff71c3928086ed1e58e01e82ee76a9 in /etc/aerospike/aerospike.template.conf 
# Thu, 15 Apr 2021 18:20:59 GMT
COPY file:11988df14ff2f0260ab7b8ccb322ee2d343b55791c51356df1d99639d16a6dbc in /entrypoint.sh 
# Thu, 15 Apr 2021 18:20:59 GMT
EXPOSE 3000 3001 3002
# Thu, 15 Apr 2021 18:21:00 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Thu, 15 Apr 2021 18:21:00 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445db9981579fca4ed6f412b94e46a2b3aaa7681a2a913ab3cc20f149cae8503`  
		Last Modified: Thu, 15 Apr 2021 18:22:16 GMT  
		Size: 53.9 MB (53935637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b2bdcde58051c58f77eaea86b0d529b0e7fcbc9d65817a652515ec236c7071`  
		Last Modified: Thu, 15 Apr 2021 18:22:08 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce06cbdf9f710dd740534dd0edb1ac87be08da66c6deb0b03f6bafcd39b27d0`  
		Last Modified: Thu, 15 Apr 2021 18:22:08 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:a26a8b17bded550b130952bc012d435e52326de11fbe003f7e2dbc4d42006e9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:7a6dfa57401bda85c448186b92f705aa7803dede73c3c9a9a1761fee8b47edb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74775131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76214490c04cad1c54fd71962f4de374be2c4d8253966c05244c897796482374`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Thu, 15 Apr 2021 18:20:15 GMT
ENV AEROSPIKE_VERSION=5.5.0.9
# Thu, 15 Apr 2021 18:20:15 GMT
ENV AEROSPIKE_SHA256=3e4e8f35c4607a465781e8f6b662494ca16717300746064ae7a1c09fd3b5ac90
# Thu, 15 Apr 2021 18:20:33 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Thu, 15 Apr 2021 18:20:34 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Thu, 15 Apr 2021 18:20:34 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Thu, 15 Apr 2021 18:20:34 GMT
EXPOSE 3000 3001 3002 3003
# Thu, 15 Apr 2021 18:20:34 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Thu, 15 Apr 2021 18:20:34 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b52c9d72afa7575ab3e078e166fdaea9e54623b27f25dbf8522423c94b58731`  
		Last Modified: Thu, 15 Apr 2021 18:21:56 GMT  
		Size: 52.2 MB (52244813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d38b2c09d49bc80fe075781829b5e370346973b51b468166b086d8f134239d6`  
		Last Modified: Thu, 15 Apr 2021 18:21:49 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcce1b84cb4dc033a799e8465dad1903cb11ffd83371cca4867d36229ce6c1d`  
		Last Modified: Thu, 15 Apr 2021 18:21:48 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
