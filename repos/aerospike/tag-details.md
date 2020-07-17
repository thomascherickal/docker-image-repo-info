<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:4.8.0.14`](#aerospike48014)
-	[`aerospike:4.9.0.11`](#aerospike49011)
-	[`aerospike:5.0.0.10`](#aerospike50010)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:4.8.0.14`

```console
$ docker pull aerospike@sha256:68b34550d9e51b7238e71e7857b3f4f24e834563e6e11341518b338c114906d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.8.0.14` - linux; amd64

```console
$ docker pull aerospike@sha256:62fb7e2d936481593f85a6cdbbf65a38b784577a5cd71b3b4a75bf75aee1c46d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51854435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef7692f856cb25965606cfb8d5c0a599f0f19fddeeeac594991e05375d7347d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:35 GMT
ADD file:57b431451a292755d0f13673f5f3bea9f62aea36c7a1b59d34d7d200ba134fea in / 
# Tue, 09 Jun 2020 01:23:35 GMT
CMD ["bash"]
# Fri, 17 Jul 2020 20:19:32 GMT
ENV AEROSPIKE_VERSION=4.8.0.14
# Fri, 17 Jul 2020 20:19:33 GMT
ENV AEROSPIKE_SHA256=de224743e2a498711cc5a133f4df9124e0ced0ef2ef8033ff0cfd70cc5e9af50
# Fri, 17 Jul 2020 20:19:49 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Fri, 17 Jul 2020 20:19:49 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Fri, 17 Jul 2020 20:19:49 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Fri, 17 Jul 2020 20:19:49 GMT
VOLUME [/opt/aerospike/data]
# Fri, 17 Jul 2020 20:19:49 GMT
EXPOSE 3000 3001 3002 3003
# Fri, 17 Jul 2020 20:19:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Jul 2020 20:19:50 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:7d2977b12acb33f192e3f20b7e15a467cc8f3f5124a15d975a6d4afe5fa3d258`  
		Last Modified: Tue, 09 Jun 2020 01:28:13 GMT  
		Size: 22.5 MB (22519600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0791409487f08d01fff386c4528bd50f78215b128f437e4c49a61fdac6ea3019`  
		Last Modified: Fri, 17 Jul 2020 20:20:45 GMT  
		Size: 29.3 MB (29332783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911539315215de24a2d59f51447cd7261fc2d58fef0b2fde2b325f227c098c4a`  
		Last Modified: Fri, 17 Jul 2020 20:20:40 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dc01a1eb29326ad236a270f7e91e9b03135d991e0a3ef3716dd2b7b7acc8eb`  
		Last Modified: Fri, 17 Jul 2020 20:20:40 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:4.9.0.11`

```console
$ docker pull aerospike@sha256:ac188b95eac62aa1c4143d3034fae42ad2896a6eacab2c391d6b6fe094b1d71f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.9.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:a1b5b8db5a1234aff4fc01228d604eea2b6a7eb9c98c68ce20a7618c2d1d6bb9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53205316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf874df7b0d28aa954d45ded1f665d1f7fd16e9129e1e9f2295270e7dbae2837`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:35 GMT
ADD file:57b431451a292755d0f13673f5f3bea9f62aea36c7a1b59d34d7d200ba134fea in / 
# Tue, 09 Jun 2020 01:23:35 GMT
CMD ["bash"]
# Fri, 17 Jul 2020 20:19:54 GMT
ENV AEROSPIKE_VERSION=4.9.0.11
# Fri, 17 Jul 2020 20:19:54 GMT
ENV AEROSPIKE_SHA256=6e53582b74800b5e93224ed34f30d2c8a3c191c7d27284070347fc7d8bb13fec
# Fri, 17 Jul 2020 20:20:10 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Fri, 17 Jul 2020 20:20:10 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Fri, 17 Jul 2020 20:20:11 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Fri, 17 Jul 2020 20:20:11 GMT
VOLUME [/opt/aerospike/data]
# Fri, 17 Jul 2020 20:20:11 GMT
EXPOSE 3000 3001 3002 3003
# Fri, 17 Jul 2020 20:20:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Jul 2020 20:20:11 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:7d2977b12acb33f192e3f20b7e15a467cc8f3f5124a15d975a6d4afe5fa3d258`  
		Last Modified: Tue, 09 Jun 2020 01:28:13 GMT  
		Size: 22.5 MB (22519600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4c031876046ec24dfc2a2299ed047aff945ca524c25e0ecdf09718233f29ee`  
		Last Modified: Fri, 17 Jul 2020 20:20:53 GMT  
		Size: 30.7 MB (30683664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1db31b2f837f081fa875bb05dc66f29ba6f83917a46a2ed5a5dda3b00bcb93`  
		Last Modified: Fri, 17 Jul 2020 20:20:48 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed641fcf6ee1dac5c30af66130cd7350742e5066eb08182dd6d850b1b5720ab`  
		Last Modified: Fri, 17 Jul 2020 20:20:48 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.0.0.10`

```console
$ docker pull aerospike@sha256:a9b49b1bb2d29437a0e0d124b14151b3b8b4962daa40e933c42153ef6cec076c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.0.0.10` - linux; amd64

```console
$ docker pull aerospike@sha256:722b6b1863ca8d36446f2f9f27e471975561e0942f5bcf1ba3510dac1168cbe5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53092232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a9471131f1e780e2702583d175c32cc746801f7137d591fbf124a50746e7247`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:35 GMT
ADD file:57b431451a292755d0f13673f5f3bea9f62aea36c7a1b59d34d7d200ba134fea in / 
# Tue, 09 Jun 2020 01:23:35 GMT
CMD ["bash"]
# Fri, 17 Jul 2020 20:20:16 GMT
ENV AEROSPIKE_VERSION=5.0.0.10
# Fri, 17 Jul 2020 20:20:16 GMT
ENV AEROSPIKE_SHA256=cf56e1dfabf73508491c669a9eaf32b97ddb91863e4bd78cd0cec64bc53fd0ca
# Fri, 17 Jul 2020 20:20:32 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Fri, 17 Jul 2020 20:20:32 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Fri, 17 Jul 2020 20:20:32 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Fri, 17 Jul 2020 20:20:33 GMT
VOLUME [/opt/aerospike/data]
# Fri, 17 Jul 2020 20:20:33 GMT
EXPOSE 3000 3001 3002 3003
# Fri, 17 Jul 2020 20:20:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Jul 2020 20:20:33 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:7d2977b12acb33f192e3f20b7e15a467cc8f3f5124a15d975a6d4afe5fa3d258`  
		Last Modified: Tue, 09 Jun 2020 01:28:13 GMT  
		Size: 22.5 MB (22519600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7798fab2dd766f5e8b3994f4440394f86ac3e283081fd45542683d208dfb9cb6`  
		Last Modified: Fri, 17 Jul 2020 20:21:02 GMT  
		Size: 30.6 MB (30570579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4254bf99ed31f3462f661060bb9609f38ff75a740b2b7ff7369fddab2d765946`  
		Last Modified: Fri, 17 Jul 2020 20:20:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5044fc2818042842c38de000be7b55fc946d0f97d941c52c5e11e5e5138c1576`  
		Last Modified: Fri, 17 Jul 2020 20:20:57 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:a9b49b1bb2d29437a0e0d124b14151b3b8b4962daa40e933c42153ef6cec076c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:722b6b1863ca8d36446f2f9f27e471975561e0942f5bcf1ba3510dac1168cbe5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53092232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a9471131f1e780e2702583d175c32cc746801f7137d591fbf124a50746e7247`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:35 GMT
ADD file:57b431451a292755d0f13673f5f3bea9f62aea36c7a1b59d34d7d200ba134fea in / 
# Tue, 09 Jun 2020 01:23:35 GMT
CMD ["bash"]
# Fri, 17 Jul 2020 20:20:16 GMT
ENV AEROSPIKE_VERSION=5.0.0.10
# Fri, 17 Jul 2020 20:20:16 GMT
ENV AEROSPIKE_SHA256=cf56e1dfabf73508491c669a9eaf32b97ddb91863e4bd78cd0cec64bc53fd0ca
# Fri, 17 Jul 2020 20:20:32 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Fri, 17 Jul 2020 20:20:32 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Fri, 17 Jul 2020 20:20:32 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Fri, 17 Jul 2020 20:20:33 GMT
VOLUME [/opt/aerospike/data]
# Fri, 17 Jul 2020 20:20:33 GMT
EXPOSE 3000 3001 3002 3003
# Fri, 17 Jul 2020 20:20:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Jul 2020 20:20:33 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:7d2977b12acb33f192e3f20b7e15a467cc8f3f5124a15d975a6d4afe5fa3d258`  
		Last Modified: Tue, 09 Jun 2020 01:28:13 GMT  
		Size: 22.5 MB (22519600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7798fab2dd766f5e8b3994f4440394f86ac3e283081fd45542683d208dfb9cb6`  
		Last Modified: Fri, 17 Jul 2020 20:21:02 GMT  
		Size: 30.6 MB (30570579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4254bf99ed31f3462f661060bb9609f38ff75a740b2b7ff7369fddab2d765946`  
		Last Modified: Fri, 17 Jul 2020 20:20:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5044fc2818042842c38de000be7b55fc946d0f97d941c52c5e11e5e5138c1576`  
		Last Modified: Fri, 17 Jul 2020 20:20:57 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
