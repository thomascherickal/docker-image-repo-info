<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:ce-6.0.0.1`](#aerospikece-6001)
-	[`aerospike:ee-6.0.0.1`](#aerospikeee-6001)

## `aerospike:ce-6.0.0.1`

```console
$ docker pull aerospike@sha256:529e32cc7952c3184244a551e518e3aca86fc5d5ce07bc1533bbd7cdbf9dec90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-6.0.0.1` - linux; amd64

```console
$ docker pull aerospike@sha256:08c065e6c4775db9dafd3084e18bb959baeabce7861572f49a66abfce6f9b489
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100928564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21c9b66a611a76add9c83109fc9ea0031381c87e69c52277c6fb7317b7d84d7d`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:46:46 GMT
ENV AEROSPIKE_VERSION=6.0.0.1
# Thu, 23 Jun 2022 00:47:14 GMT
ENV AEROSPIKE_SHA256=79aa40b1028798b5f13e23f295c1e1af187419b9410e23ebb692e350286fac5a
# Thu, 23 Jun 2022 00:47:34 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Thu, 23 Jun 2022 00:47:34 GMT
COPY file:57aa54f8d05380c639ff298f99e0387bafe493553aa29e39911c8342f60a0f0e in /etc/aerospike/aerospike.template.conf 
# Thu, 23 Jun 2022 00:47:35 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Thu, 23 Jun 2022 00:47:35 GMT
EXPOSE 3000 3001 3002
# Thu, 23 Jun 2022 00:47:35 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Thu, 23 Jun 2022 00:47:35 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9801b5487d1fb6e5b0cebb303085bd4136fe10411728f4baef65dea294902bb6`  
		Last Modified: Thu, 23 Jun 2022 00:48:11 GMT  
		Size: 73.8 MB (73786491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a18eb19c079df37b565dc319f81e510a88879a75d596c11d1f4086822918365`  
		Last Modified: Thu, 23 Jun 2022 00:48:01 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d5bfbcfcb1402317cb10cd468545dcfcd43e9a4bf41ead217f7dc64b11a6d2`  
		Last Modified: Thu, 23 Jun 2022 00:48:02 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:ee-6.0.0.1`

```console
$ docker pull aerospike@sha256:a4e8cb7b676ee6c2661aab17414fe115b0f5644f02d8ef6b9c4fd30da4c1fe9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ee-6.0.0.1` - linux; amd64

```console
$ docker pull aerospike@sha256:1473755689158ad75ac3fbcb4c71f5f117c9814a18a0f88722a1c3da44d58133
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.3 MB (103321191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337e76ac840fd3214a45640ad0de76554c6425c13ec3f2e496b027a1f3d15b61`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:46:46 GMT
ENV AEROSPIKE_VERSION=6.0.0.1
# Thu, 23 Jun 2022 00:46:46 GMT
ENV AEROSPIKE_SHA256=d470ca9717b563726e8084ab6fc89f2889aefd1f6aa8ef9145ac38e0b42945a1
# Thu, 23 Jun 2022 00:46:46 GMT
ENV AS_TINI_SHA256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940
# Thu, 23 Jun 2022 00:47:08 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps wget python python3 python3-distutils lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static -O /usr/bin/as-tini-static   && echo "$AS_TINI_SHA256 /usr/bin/as-tini-static" | sha256sum -c -   && chmod +x /usr/bin/as-tini-static   && wget "https://download.aerospike.com/artifacts/aerospike-server-enterprise/${AEROSPIKE_VERSION}/aerospike-server-enterprise-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Thu, 23 Jun 2022 00:47:09 GMT
COPY file:fa3bf0bd6c8130f09c26d82e9992baa4f2fe9ac69fee03e01b296f89984a97e0 in /etc/aerospike/aerospike.template.conf 
# Thu, 23 Jun 2022 00:47:09 GMT
COPY file:31b6a51a1d9d91f22433472f07f6ddfe3cea3bb07f460dd69c4187bc7fd20fdf in /entrypoint.sh 
# Thu, 23 Jun 2022 00:47:09 GMT
EXPOSE 3000 3001 3002
# Thu, 23 Jun 2022 00:47:09 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Thu, 23 Jun 2022 00:47:09 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fcd7d4a0ba8643674bcceb74c64bff11a38d2635cf6b436c5682c6fa97791f`  
		Last Modified: Thu, 23 Jun 2022 00:47:54 GMT  
		Size: 76.2 MB (76179054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec04b5e10598104b17a05f05b0150ac9012b7b471af9473a32bf743e30583800`  
		Last Modified: Thu, 23 Jun 2022 00:47:45 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1d98641deb54d6e881846e7a65db167739f3a6858395924c38f4a0bfa6cd99`  
		Last Modified: Thu, 23 Jun 2022 00:47:44 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
