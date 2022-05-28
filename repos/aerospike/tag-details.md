<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:ce-6.0.0.1`](#aerospikece-6001)
-	[`aerospike:ee-6.0.0.1`](#aerospikeee-6001)

## `aerospike:ce-6.0.0.1`

```console
$ docker pull aerospike@sha256:3e0719277e2d09be121c7d6d8c83fdab550444bd8cf429ed7a869346f459432f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-6.0.0.1` - linux; amd64

```console
$ docker pull aerospike@sha256:54f9da627778387dba110d2774139878f7857073969fa4b65288e743b625976f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100928599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21006a11ba2cf2658a80e4a84e843cde24f53749faa5c42a998b6ea6cca8ae97`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:37:15 GMT
ENV AEROSPIKE_VERSION=6.0.0.1
# Sat, 28 May 2022 02:37:43 GMT
ENV AEROSPIKE_SHA256=79aa40b1028798b5f13e23f295c1e1af187419b9410e23ebb692e350286fac5a
# Sat, 28 May 2022 02:38:03 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Sat, 28 May 2022 02:38:03 GMT
COPY file:57aa54f8d05380c639ff298f99e0387bafe493553aa29e39911c8342f60a0f0e in /etc/aerospike/aerospike.template.conf 
# Sat, 28 May 2022 02:38:03 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Sat, 28 May 2022 02:38:03 GMT
EXPOSE 3000 3001 3002
# Sat, 28 May 2022 02:38:04 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Sat, 28 May 2022 02:38:04 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14a175853546710711bebb3029dd9718b55db955ff235723be3b70ea255f5fb`  
		Last Modified: Sat, 28 May 2022 02:38:38 GMT  
		Size: 73.8 MB (73786423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe7b3dd79d4152d0ec2c48c4b746ad9fee78648836adcb837e0121b13eca560`  
		Last Modified: Sat, 28 May 2022 02:38:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f5cf4d83909fe4ca279a4f48313764e0e7089ea8ccf929f1cd3b213a5eabe4`  
		Last Modified: Sat, 28 May 2022 02:38:29 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:ee-6.0.0.1`

```console
$ docker pull aerospike@sha256:849b6969c6aa752ed87b8f6c0b76b15eaa58ee362859af0f81e57c3954e30d25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ee-6.0.0.1` - linux; amd64

```console
$ docker pull aerospike@sha256:413b08432e9d4ba87d2d314cbe355f00d7dcd9715825ac1861242c1590c31f03
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.3 MB (103321106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04e5698efd94577f79b658de306bd8f1ce57832b87ca69b5ac32d208dab7f265`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:37:15 GMT
ENV AEROSPIKE_VERSION=6.0.0.1
# Sat, 28 May 2022 02:37:15 GMT
ENV AEROSPIKE_SHA256=d470ca9717b563726e8084ab6fc89f2889aefd1f6aa8ef9145ac38e0b42945a1
# Sat, 28 May 2022 02:37:16 GMT
ENV AS_TINI_SHA256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940
# Sat, 28 May 2022 02:37:37 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps wget python python3 python3-distutils lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static -O /usr/bin/as-tini-static   && echo "$AS_TINI_SHA256 /usr/bin/as-tini-static" | sha256sum -c -   && chmod +x /usr/bin/as-tini-static   && wget "https://download.aerospike.com/artifacts/aerospike-server-enterprise/${AEROSPIKE_VERSION}/aerospike-server-enterprise-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Sat, 28 May 2022 02:37:38 GMT
COPY file:fa3bf0bd6c8130f09c26d82e9992baa4f2fe9ac69fee03e01b296f89984a97e0 in /etc/aerospike/aerospike.template.conf 
# Sat, 28 May 2022 02:37:38 GMT
COPY file:31b6a51a1d9d91f22433472f07f6ddfe3cea3bb07f460dd69c4187bc7fd20fdf in /entrypoint.sh 
# Sat, 28 May 2022 02:37:38 GMT
EXPOSE 3000 3001 3002
# Sat, 28 May 2022 02:37:38 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Sat, 28 May 2022 02:37:38 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55fa81c254f480a743bfb96e7f63ceafbe3f4e6756f2039fa24641cdd09a309`  
		Last Modified: Sat, 28 May 2022 02:38:22 GMT  
		Size: 76.2 MB (76178871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097d593fe8b34d11d1df2a1b27c37abe37db4f8a6fc9025030eebf2d61ab0534`  
		Last Modified: Sat, 28 May 2022 02:38:13 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e02cb2322f1c59c1a8611c29636bce240c09afc0a80be32c81f10421e0b6ed`  
		Last Modified: Sat, 28 May 2022 02:38:13 GMT  
		Size: 908.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
