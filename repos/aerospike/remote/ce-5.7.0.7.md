## `aerospike:ce-5.7.0.7`

```console
$ docker pull aerospike@sha256:7fdefa68152becfb93354f07bfa561b820ca91a5a0049490f3194735381acb71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-5.7.0.7` - linux; amd64

```console
$ docker pull aerospike@sha256:4d93a48fdbd4745985a5c0fa9fe42af1478859c152bf1a39657e8c598cd6ba37
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81526557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28970d1ea1680937ca3be53805023e254834a39c79a86d2cfdcddbba99e4a301`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:02:48 GMT
ENV AEROSPIKE_VERSION=5.7.0.7
# Tue, 28 Sep 2021 02:03:14 GMT
ENV AEROSPIKE_SHA256=9cb4afd5305e2192813ce4551f3943917c5b25d2a372d8f8cf2b4f55ae376034
# Tue, 28 Sep 2021 02:03:34 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Tue, 28 Sep 2021 02:03:35 GMT
COPY file:1897c4aae07efbc61bf2d8c2c7b0dfb0990174e11cc787eac71d5adf767abaed in /etc/aerospike/aerospike.template.conf 
# Tue, 28 Sep 2021 02:03:35 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Tue, 28 Sep 2021 02:03:35 GMT
EXPOSE 3000 3001 3002
# Tue, 28 Sep 2021 02:03:35 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 28 Sep 2021 02:03:35 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5667e38ab59f6a8b05082ecc5ec4d27d2c9d54deae1ded27e6103e150c9ddd`  
		Last Modified: Tue, 28 Sep 2021 02:04:08 GMT  
		Size: 54.4 MB (54378543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95abdf5a2012e13790b548794c919be960cd3110fece314e7f6210c806b8be43`  
		Last Modified: Tue, 28 Sep 2021 02:04:01 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387346a9a218d8c2775fd9b88ff6540ecad0f8e26e8eeb2239fb80adc77cd3c7`  
		Last Modified: Tue, 28 Sep 2021 02:04:04 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
