<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:ce-6.0.0.2`](#aerospikece-6002)
-	[`aerospike:ee-6.0.0.2`](#aerospikeee-6002)

## `aerospike:ce-6.0.0.2`

```console
$ docker pull aerospike@sha256:572828aea163287b0b89d19948c8b008889ba355d9030a5d22afc95941d6e092
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-6.0.0.2` - linux; amd64

```console
$ docker pull aerospike@sha256:57e85d4b6eb72701c249f955decd20cbece7d4df4641703da057f57fd2718c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100927500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a3abddd02613fafecef4e5b08969dbe4b742e5346b21873aa8cb12e9aa06ffc`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:44:34 GMT
ENV AEROSPIKE_VERSION=6.0.0.2
# Tue, 12 Jul 2022 02:45:03 GMT
ENV AEROSPIKE_SHA256=c521897b21909dde726e067f5164a6397177feb84ae52712e224f2b694dbf7ad
# Tue, 12 Jul 2022 02:45:23 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Tue, 12 Jul 2022 02:45:23 GMT
COPY file:f497c4c6974a190f79a562efd9c9c0d6b753efe43e62c3fcc2536f74ad08238d in /etc/aerospike/aerospike.template.conf 
# Tue, 12 Jul 2022 02:45:23 GMT
COPY file:fe302e12e47afe1731a34ed4ed29328c6901a3f2c9e32e307220e65cb76d53a2 in /entrypoint.sh 
# Tue, 12 Jul 2022 02:45:23 GMT
EXPOSE 3000 3001 3002
# Tue, 12 Jul 2022 02:45:24 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 12 Jul 2022 02:45:24 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e14cfc1701870b6304989def95f3ed4438e54a11aacde82e5a5ffdd18f40246`  
		Last Modified: Tue, 12 Jul 2022 02:45:59 GMT  
		Size: 73.8 MB (73785819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b594286fc849e7ad2bdc7dbb44edd23e7343193894e9c46f3e1236b5868b7cf`  
		Last Modified: Tue, 12 Jul 2022 02:45:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada2670d73bd036a2b64d7edcff6a3336d7b832000fb05f9e675956dd8b4e7c2`  
		Last Modified: Tue, 12 Jul 2022 02:45:50 GMT  
		Size: 812.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:ee-6.0.0.2`

```console
$ docker pull aerospike@sha256:3513d708fe16a14b24f0522fa2c751a84ac122883665c51e56f4b8c93ca63872
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ee-6.0.0.2` - linux; amd64

```console
$ docker pull aerospike@sha256:4303f35812eaaa74d7ac416364f03be58aabdb5eae78a6dfcaa1ce32c4841a66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.3 MB (103319747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b93c5bad34f4f1485c6c818bf6b6e62798397bbbb5fc8850426a5dc89ee10c`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:44:34 GMT
ENV AEROSPIKE_VERSION=6.0.0.2
# Tue, 12 Jul 2022 02:44:35 GMT
ENV AEROSPIKE_SHA256=0b067053c3919cc41b90f519e4ea164ad1ed4d8bca934a877085ff0067469a65
# Tue, 12 Jul 2022 02:44:35 GMT
ENV AS_TINI_SHA256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940
# Tue, 12 Jul 2022 02:44:56 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps wget python python3 python3-distutils lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static -O /usr/bin/as-tini-static   && echo "$AS_TINI_SHA256 /usr/bin/as-tini-static" | sha256sum -c -   && chmod +x /usr/bin/as-tini-static   && wget "https://download.aerospike.com/artifacts/aerospike-server-enterprise/${AEROSPIKE_VERSION}/aerospike-server-enterprise-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Tue, 12 Jul 2022 02:44:57 GMT
COPY file:f56e2e33c0b4bb66affff75053eaed44661e723b8b33d3ef3c10e305b506c350 in /etc/aerospike/aerospike.template.conf 
# Tue, 12 Jul 2022 02:44:57 GMT
COPY file:697e2123680798e87da7a3f98d1d70e76ffec66f0e1aafa90ff25047a11cca52 in /entrypoint.sh 
# Tue, 12 Jul 2022 02:44:57 GMT
EXPOSE 3000 3001 3002
# Tue, 12 Jul 2022 02:44:57 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Tue, 12 Jul 2022 02:44:57 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ce2bbe9d9e07a88e1af13d270fe714ac37578a732d131fa50d86749582045b`  
		Last Modified: Tue, 12 Jul 2022 02:45:42 GMT  
		Size: 76.2 MB (76178011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a2c9684ebcc61855607718d21a2fc81b503bed18c00161e86f3d3432d38294`  
		Last Modified: Tue, 12 Jul 2022 02:45:33 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8f08acf26e55d92a90f920d73d97680d253ce98f98ec802ce39ed3d21b1d8e`  
		Last Modified: Tue, 12 Jul 2022 02:45:33 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
