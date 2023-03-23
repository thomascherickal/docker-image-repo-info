<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.16`](#emqx4416)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.20`](#emqx5020)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:363339f822db774f2b40a76bbdb542e4342a9fe69024ac4add0ffa73eff51c29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:b594671f1c8c001b76971e896ec29f4aea1b4ce35e471f418b7e190d66bdfe8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81272225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df18f1b36fce0936fd74b9faf314e3a01d83c037091286efb92131b581fe822`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 23 Mar 2023 06:38:30 GMT
ENV EMQX_VERSION=4.4.16
# Thu, 23 Mar 2023 06:38:30 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 23 Mar 2023 06:38:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 23 Mar 2023 06:38:34 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:35 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:35 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:35 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 23 Mar 2023 06:38:35 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:35 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:35 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7216294cbe2d1311e293a82d22eb3f71da435b2b9bb7ad9900eaaeb14d68d2b7`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 2.6 MB (2569460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca85a7d40cdb8392bb213cc3b9efc98bcb416df588c86b55eb174485340016cb`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93644246d8ba201ec9c154bf77410efda76bbc02af25c4d8c89b5bef6aa7e90e`  
		Last Modified: Thu, 23 Mar 2023 06:39:05 GMT  
		Size: 47.3 MB (47286145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1172e73e519b49b8ecabc31cf1807694cf854572647611963d00191e5c03612`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4e9ebe772c56e5076b7d356635a535cf5565d54c26264c0848393a3a91f757a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72700283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e4a8802d3708ed0e9e04e9eba2393ce51bc8cae915d012bf4f4374b1d66882`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 15 Mar 2023 23:40:08 GMT
ENV EMQX_VERSION=4.4.16
# Wed, 15 Mar 2023 23:40:08 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 15 Mar 2023 23:40:11 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 15 Mar 2023 23:40:12 GMT
WORKDIR /opt/emqx
# Wed, 15 Mar 2023 23:40:12 GMT
USER emqx
# Wed, 15 Mar 2023 23:40:12 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 15 Mar 2023 23:40:12 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 15 Mar 2023 23:40:12 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 15 Mar 2023 23:40:12 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 15 Mar 2023 23:40:12 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ea117f9b26bad2c79fea1dafb19b2ccbfb0e0744061d7743a5aea0c0e38af7`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 2.6 MB (2559230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde159950f1c178189d5f614a5405bd1df5caabc1ebd2bfc1e35376f9bd0e19`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4e303f3e8ae9c4c0212bb811a988e668b8fb253f34804cf455d4b4179c1ccf`  
		Last Modified: Wed, 15 Mar 2023 23:40:31 GMT  
		Size: 40.1 MB (40073017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209dd83a5db4a0f1352247f1e19e02a3a54ee87fb2e45771e96d01045483e4aa`  
		Last Modified: Wed, 15 Mar 2023 23:40:26 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:363339f822db774f2b40a76bbdb542e4342a9fe69024ac4add0ffa73eff51c29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:b594671f1c8c001b76971e896ec29f4aea1b4ce35e471f418b7e190d66bdfe8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81272225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df18f1b36fce0936fd74b9faf314e3a01d83c037091286efb92131b581fe822`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 23 Mar 2023 06:38:30 GMT
ENV EMQX_VERSION=4.4.16
# Thu, 23 Mar 2023 06:38:30 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 23 Mar 2023 06:38:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 23 Mar 2023 06:38:34 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:35 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:35 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:35 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 23 Mar 2023 06:38:35 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:35 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:35 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7216294cbe2d1311e293a82d22eb3f71da435b2b9bb7ad9900eaaeb14d68d2b7`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 2.6 MB (2569460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca85a7d40cdb8392bb213cc3b9efc98bcb416df588c86b55eb174485340016cb`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93644246d8ba201ec9c154bf77410efda76bbc02af25c4d8c89b5bef6aa7e90e`  
		Last Modified: Thu, 23 Mar 2023 06:39:05 GMT  
		Size: 47.3 MB (47286145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1172e73e519b49b8ecabc31cf1807694cf854572647611963d00191e5c03612`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4e9ebe772c56e5076b7d356635a535cf5565d54c26264c0848393a3a91f757a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72700283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e4a8802d3708ed0e9e04e9eba2393ce51bc8cae915d012bf4f4374b1d66882`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 15 Mar 2023 23:40:08 GMT
ENV EMQX_VERSION=4.4.16
# Wed, 15 Mar 2023 23:40:08 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 15 Mar 2023 23:40:11 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 15 Mar 2023 23:40:12 GMT
WORKDIR /opt/emqx
# Wed, 15 Mar 2023 23:40:12 GMT
USER emqx
# Wed, 15 Mar 2023 23:40:12 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 15 Mar 2023 23:40:12 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 15 Mar 2023 23:40:12 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 15 Mar 2023 23:40:12 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 15 Mar 2023 23:40:12 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ea117f9b26bad2c79fea1dafb19b2ccbfb0e0744061d7743a5aea0c0e38af7`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 2.6 MB (2559230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde159950f1c178189d5f614a5405bd1df5caabc1ebd2bfc1e35376f9bd0e19`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4e303f3e8ae9c4c0212bb811a988e668b8fb253f34804cf455d4b4179c1ccf`  
		Last Modified: Wed, 15 Mar 2023 23:40:31 GMT  
		Size: 40.1 MB (40073017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209dd83a5db4a0f1352247f1e19e02a3a54ee87fb2e45771e96d01045483e4aa`  
		Last Modified: Wed, 15 Mar 2023 23:40:26 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.16`

```console
$ docker pull emqx@sha256:363339f822db774f2b40a76bbdb542e4342a9fe69024ac4add0ffa73eff51c29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.16` - linux; amd64

```console
$ docker pull emqx@sha256:b594671f1c8c001b76971e896ec29f4aea1b4ce35e471f418b7e190d66bdfe8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81272225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df18f1b36fce0936fd74b9faf314e3a01d83c037091286efb92131b581fe822`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 23 Mar 2023 06:38:30 GMT
ENV EMQX_VERSION=4.4.16
# Thu, 23 Mar 2023 06:38:30 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 23 Mar 2023 06:38:34 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 23 Mar 2023 06:38:34 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:35 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:35 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:35 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 23 Mar 2023 06:38:35 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:35 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:35 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7216294cbe2d1311e293a82d22eb3f71da435b2b9bb7ad9900eaaeb14d68d2b7`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 2.6 MB (2569460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca85a7d40cdb8392bb213cc3b9efc98bcb416df588c86b55eb174485340016cb`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93644246d8ba201ec9c154bf77410efda76bbc02af25c4d8c89b5bef6aa7e90e`  
		Last Modified: Thu, 23 Mar 2023 06:39:05 GMT  
		Size: 47.3 MB (47286145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1172e73e519b49b8ecabc31cf1807694cf854572647611963d00191e5c03612`  
		Last Modified: Thu, 23 Mar 2023 06:39:01 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.16` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:4e9ebe772c56e5076b7d356635a535cf5565d54c26264c0848393a3a91f757a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72700283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e4a8802d3708ed0e9e04e9eba2393ce51bc8cae915d012bf4f4374b1d66882`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:03 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Wed, 15 Mar 2023 23:40:08 GMT
ENV EMQX_VERSION=4.4.16
# Wed, 15 Mar 2023 23:40:08 GMT
ENV OTP=otp24.3.4.2-1
# Wed, 15 Mar 2023 23:40:11 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="901b76ea2bee68729b75280740ca31b1af5b358d331422d1653dc342ee830324"; fi;     if [ ${arch} = "arm64" ]; then sha256="1224f53d0ee98390c286f3bbd9af2f294c2fa4ccb79342343d803fa234165c6e"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Wed, 15 Mar 2023 23:40:12 GMT
WORKDIR /opt/emqx
# Wed, 15 Mar 2023 23:40:12 GMT
USER emqx
# Wed, 15 Mar 2023 23:40:12 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 15 Mar 2023 23:40:12 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Wed, 15 Mar 2023 23:40:12 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Wed, 15 Mar 2023 23:40:12 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 15 Mar 2023 23:40:12 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ea117f9b26bad2c79fea1dafb19b2ccbfb0e0744061d7743a5aea0c0e38af7`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 2.6 MB (2559230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde159950f1c178189d5f614a5405bd1df5caabc1ebd2bfc1e35376f9bd0e19`  
		Last Modified: Wed, 01 Mar 2023 03:21:50 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4e303f3e8ae9c4c0212bb811a988e668b8fb253f34804cf455d4b4179c1ccf`  
		Last Modified: Wed, 15 Mar 2023 23:40:31 GMT  
		Size: 40.1 MB (40073017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209dd83a5db4a0f1352247f1e19e02a3a54ee87fb2e45771e96d01045483e4aa`  
		Last Modified: Wed, 15 Mar 2023 23:40:26 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:46adab905ef1bf96fb4aa8b069fa55a254886b5383f8ef6a4b6502c6374c6296
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:db94e86eb5708484aab7d72866c3d1b818f7e42dede79087db3b8336b42a0e4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d1da644611bb001ea426cb7a35d17c79f355acbf8da9596e94eb45f573f24a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:43 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:44 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 06:38:44 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 06:38:44 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 06:38:44 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 06:38:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 06:38:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 06:38:50 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:50 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 06:38:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad234a8e621d243ffc2889b413a9971003cc42ee7ba32a7ac16473122c6d6364`  
		Last Modified: Thu, 23 Mar 2023 06:39:16 GMT  
		Size: 3.0 MB (2987658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e02c887fbcfd1b399b200e621a473094afcaf8febe6e035caf150ebf9136c32`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ae335101f863f32be81ae4b486dcc876bf277f52d0b0494d63afec80df7254`  
		Last Modified: Thu, 23 Mar 2023 06:39:23 GMT  
		Size: 66.8 MB (66809463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77081c8225be9c363811f449115fd687c67abcb09ab1dcd47bd66bedf39998ff`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:13e95e2fef6dbd597b66a357807ceb71cba9ee2526562f9e3a1c1b8ccd84c33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e912e5f1bdce506ce56157f5a78282b230d9c95b6700df96645f9f25e4dce4b5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 21:48:23 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 21:48:23 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 21:48:23 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 21:48:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 21:48:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 21:48:28 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 21:48:28 GMT
USER emqx
# Fri, 10 Mar 2023 21:48:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 21:48:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 21:48:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 21:48:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 21:48:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b403af0a79322aefc651ac609b98935d96017c8baa135e28307c6e9cc0691aff`  
		Last Modified: Fri, 10 Mar 2023 21:49:03 GMT  
		Size: 59.2 MB (59233251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f7b75ab2328825c25f602efb49a16223ab44d99a65a2e8a15856390f623199`  
		Last Modified: Fri, 10 Mar 2023 21:48:57 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:46adab905ef1bf96fb4aa8b069fa55a254886b5383f8ef6a4b6502c6374c6296
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:db94e86eb5708484aab7d72866c3d1b818f7e42dede79087db3b8336b42a0e4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d1da644611bb001ea426cb7a35d17c79f355acbf8da9596e94eb45f573f24a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:43 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:44 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 06:38:44 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 06:38:44 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 06:38:44 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 06:38:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 06:38:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 06:38:50 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:50 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 06:38:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad234a8e621d243ffc2889b413a9971003cc42ee7ba32a7ac16473122c6d6364`  
		Last Modified: Thu, 23 Mar 2023 06:39:16 GMT  
		Size: 3.0 MB (2987658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e02c887fbcfd1b399b200e621a473094afcaf8febe6e035caf150ebf9136c32`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ae335101f863f32be81ae4b486dcc876bf277f52d0b0494d63afec80df7254`  
		Last Modified: Thu, 23 Mar 2023 06:39:23 GMT  
		Size: 66.8 MB (66809463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77081c8225be9c363811f449115fd687c67abcb09ab1dcd47bd66bedf39998ff`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:13e95e2fef6dbd597b66a357807ceb71cba9ee2526562f9e3a1c1b8ccd84c33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e912e5f1bdce506ce56157f5a78282b230d9c95b6700df96645f9f25e4dce4b5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 21:48:23 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 21:48:23 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 21:48:23 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 21:48:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 21:48:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 21:48:28 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 21:48:28 GMT
USER emqx
# Fri, 10 Mar 2023 21:48:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 21:48:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 21:48:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 21:48:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 21:48:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b403af0a79322aefc651ac609b98935d96017c8baa135e28307c6e9cc0691aff`  
		Last Modified: Fri, 10 Mar 2023 21:49:03 GMT  
		Size: 59.2 MB (59233251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f7b75ab2328825c25f602efb49a16223ab44d99a65a2e8a15856390f623199`  
		Last Modified: Fri, 10 Mar 2023 21:48:57 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.20`

```console
$ docker pull emqx@sha256:46adab905ef1bf96fb4aa8b069fa55a254886b5383f8ef6a4b6502c6374c6296
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.20` - linux; amd64

```console
$ docker pull emqx@sha256:db94e86eb5708484aab7d72866c3d1b818f7e42dede79087db3b8336b42a0e4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d1da644611bb001ea426cb7a35d17c79f355acbf8da9596e94eb45f573f24a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:43 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:44 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 06:38:44 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 06:38:44 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 06:38:44 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 06:38:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 06:38:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 06:38:50 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:50 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 06:38:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad234a8e621d243ffc2889b413a9971003cc42ee7ba32a7ac16473122c6d6364`  
		Last Modified: Thu, 23 Mar 2023 06:39:16 GMT  
		Size: 3.0 MB (2987658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e02c887fbcfd1b399b200e621a473094afcaf8febe6e035caf150ebf9136c32`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ae335101f863f32be81ae4b486dcc876bf277f52d0b0494d63afec80df7254`  
		Last Modified: Thu, 23 Mar 2023 06:39:23 GMT  
		Size: 66.8 MB (66809463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77081c8225be9c363811f449115fd687c67abcb09ab1dcd47bd66bedf39998ff`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.20` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:13e95e2fef6dbd597b66a357807ceb71cba9ee2526562f9e3a1c1b8ccd84c33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e912e5f1bdce506ce56157f5a78282b230d9c95b6700df96645f9f25e4dce4b5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 21:48:23 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 21:48:23 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 21:48:23 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 21:48:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 21:48:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 21:48:28 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 21:48:28 GMT
USER emqx
# Fri, 10 Mar 2023 21:48:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 21:48:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 21:48:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 21:48:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 21:48:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b403af0a79322aefc651ac609b98935d96017c8baa135e28307c6e9cc0691aff`  
		Last Modified: Fri, 10 Mar 2023 21:49:03 GMT  
		Size: 59.2 MB (59233251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f7b75ab2328825c25f602efb49a16223ab44d99a65a2e8a15856390f623199`  
		Last Modified: Fri, 10 Mar 2023 21:48:57 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:46adab905ef1bf96fb4aa8b069fa55a254886b5383f8ef6a4b6502c6374c6296
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:db94e86eb5708484aab7d72866c3d1b818f7e42dede79087db3b8336b42a0e4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101213537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d1da644611bb001ea426cb7a35d17c79f355acbf8da9596e94eb45f573f24a`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:38:43 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:38:44 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 23 Mar 2023 06:38:44 GMT
ENV EMQX_VERSION=5.0.20
# Thu, 23 Mar 2023 06:38:44 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Thu, 23 Mar 2023 06:38:44 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Thu, 23 Mar 2023 06:38:44 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 23 Mar 2023 06:38:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 23 Mar 2023 06:38:50 GMT
WORKDIR /opt/emqx
# Thu, 23 Mar 2023 06:38:50 GMT
USER emqx
# Thu, 23 Mar 2023 06:38:50 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 23 Mar 2023 06:38:50 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 23 Mar 2023 06:38:50 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 23 Mar 2023 06:38:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:38:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad234a8e621d243ffc2889b413a9971003cc42ee7ba32a7ac16473122c6d6364`  
		Last Modified: Thu, 23 Mar 2023 06:39:16 GMT  
		Size: 3.0 MB (2987658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e02c887fbcfd1b399b200e621a473094afcaf8febe6e035caf150ebf9136c32`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ae335101f863f32be81ae4b486dcc876bf277f52d0b0494d63afec80df7254`  
		Last Modified: Thu, 23 Mar 2023 06:39:23 GMT  
		Size: 66.8 MB (66809463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77081c8225be9c363811f449115fd687c67abcb09ab1dcd47bd66bedf39998ff`  
		Last Modified: Thu, 23 Mar 2023 06:39:15 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:13e95e2fef6dbd597b66a357807ceb71cba9ee2526562f9e3a1c1b8ccd84c33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92303842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e912e5f1bdce506ce56157f5a78282b230d9c95b6700df96645f9f25e4dce4b5`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Fri, 10 Mar 2023 21:48:23 GMT
ENV EMQX_VERSION=5.0.20
# Fri, 10 Mar 2023 21:48:23 GMT
ENV AMD64_SHA256=88711b32e20676d11e3101bbb0e655d9ebf045a7735c190df0c26a230db8fac0
# Fri, 10 Mar 2023 21:48:23 GMT
ENV ARM64_SHA256=519fb1b14478e7fcc9ca74017bb4b09355e5d90def0c5d807e11165864388cd9
# Fri, 10 Mar 2023 21:48:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 10 Mar 2023 21:48:27 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Fri, 10 Mar 2023 21:48:28 GMT
WORKDIR /opt/emqx
# Fri, 10 Mar 2023 21:48:28 GMT
USER emqx
# Fri, 10 Mar 2023 21:48:28 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 10 Mar 2023 21:48:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 10 Mar 2023 21:48:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 10 Mar 2023 21:48:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 10 Mar 2023 21:48:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b403af0a79322aefc651ac609b98935d96017c8baa135e28307c6e9cc0691aff`  
		Last Modified: Fri, 10 Mar 2023 21:49:03 GMT  
		Size: 59.2 MB (59233251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f7b75ab2328825c25f602efb49a16223ab44d99a65a2e8a15856390f623199`  
		Last Modified: Fri, 10 Mar 2023 21:48:57 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
