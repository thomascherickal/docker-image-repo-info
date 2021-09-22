<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:ce-5.6.0.13`](#aerospikece-56013)
-	[`aerospike:ee-5.6.0.13`](#aerospikeee-56013)

## `aerospike:ce-5.6.0.13`

```console
$ docker pull aerospike@sha256:d1ff9fec0d24e6717847dd2e1049a6d58db2a7de4f425b34c0383c5ac9993015
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-5.6.0.13` - linux; amd64

```console
$ docker pull aerospike@sha256:64c9db8a6c3567ee41fdeffd7f12c277da293de9547554d57a9a7489ff40a4f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80604518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9f6458416bf936033ca81e6246f5d54f8e8f717c39e350752c5e8419aa2f336`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Wed, 22 Sep 2021 19:19:19 GMT
ENV AEROSPIKE_VERSION=5.6.0.13
# Wed, 22 Sep 2021 19:19:44 GMT
ENV AEROSPIKE_SHA256=cd8662ea0bc4d483a5b20ce647bec4912b0c1a9c591e3b3f66b8ddee14039da6
# Wed, 22 Sep 2021 19:20:03 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 22 Sep 2021 19:20:03 GMT
COPY file:1897c4aae07efbc61bf2d8c2c7b0dfb0990174e11cc787eac71d5adf767abaed in /etc/aerospike/aerospike.template.conf 
# Wed, 22 Sep 2021 19:20:04 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Wed, 22 Sep 2021 19:20:04 GMT
EXPOSE 3000 3001 3002
# Wed, 22 Sep 2021 19:20:04 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 22 Sep 2021 19:20:04 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f32397489a45e8245ace16415a0c81686d28074fe9caf5276451bedede9c920`  
		Last Modified: Wed, 22 Sep 2021 19:20:38 GMT  
		Size: 53.5 MB (53456654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcc302b8c4f32df961f3fcf121e7f60a8f50ee177002dc1646dc0368a823058`  
		Last Modified: Wed, 22 Sep 2021 19:20:30 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfcfd6b25b1cf56ab000ecc04af5ce6e7edc9a586a8e4f3d8de25aac1aeb7c7`  
		Last Modified: Wed, 22 Sep 2021 19:20:30 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:ee-5.6.0.13`

```console
$ docker pull aerospike@sha256:e6ec59f7c9f121428c61858467aefba7ce99060e32030ba3425c3810895dc765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ee-5.6.0.13` - linux; amd64

```console
$ docker pull aerospike@sha256:f7be47f80dbd4ee6c06fb435d3f2073a66291b09309a0f65858974c13d37cf29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82472463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:938051acac9dd88b52d2fef8ba3d9f34c4acff7d41c885e0139aa844483d10f4`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Wed, 22 Sep 2021 19:19:19 GMT
ENV AEROSPIKE_VERSION=5.6.0.13
# Wed, 22 Sep 2021 19:19:19 GMT
ENV AEROSPIKE_SHA256=408b23a16507e513908aaf87956da9c81b8a71d4f859701f740a98fe5798d28f
# Wed, 22 Sep 2021 19:19:39 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian10" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 22 Sep 2021 19:19:39 GMT
COPY file:7d75174e09b209cf7f56b715636c2b8e08dd083d548e8cdc8517cabd512600b5 in /etc/aerospike/aerospike.template.conf 
# Wed, 22 Sep 2021 19:19:40 GMT
COPY file:31b6a51a1d9d91f22433472f07f6ddfe3cea3bb07f460dd69c4187bc7fd20fdf in /entrypoint.sh 
# Wed, 22 Sep 2021 19:19:40 GMT
EXPOSE 3000 3001 3002
# Wed, 22 Sep 2021 19:19:40 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 22 Sep 2021 19:19:40 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936df63320a840a7220d2bd562a84fc2c0c1a42a5dc7826530a93e5f27283227`  
		Last Modified: Wed, 22 Sep 2021 19:20:23 GMT  
		Size: 55.3 MB (55324537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6777aeb1d7f858578d9d701c0f7d6cfaf7c62758c05d95b2f135090fac858d31`  
		Last Modified: Wed, 22 Sep 2021 19:20:15 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe341b5f96e9410511640f735f85b51779a9f56def3c7966531157cb9962a4c`  
		Last Modified: Wed, 22 Sep 2021 19:20:15 GMT  
		Size: 909.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
