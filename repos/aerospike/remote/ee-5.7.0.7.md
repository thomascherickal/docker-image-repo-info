## `aerospike:ee-5.7.0.7`

```console
$ docker pull aerospike@sha256:d637cb786c9e1f3add4b0e41248f01e9dc9cad4707722f1d13ba9ff1e6178b72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ee-5.7.0.7` - linux; amd64

```console
$ docker pull aerospike@sha256:02dd84f8d42a3eead5c7b3aa1763641a13b53a6a51baca68b61a0c193ec8e1cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83523558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ce19a81640096cc5e35b90a3a1c48f524b627c5b4acfebd89ef194b55fce030`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:02:48 GMT
ENV AEROSPIKE_VERSION=5.7.0.7
# Tue, 28 Sep 2021 02:02:49 GMT
ENV AEROSPIKE_SHA256=c0b51e4389b7809bf059015164e1f2ae26dae9205b53ad5dca121a071980ba8e
# Tue, 28 Sep 2021 02:03:10 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian10" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Tue, 28 Sep 2021 02:03:10 GMT
COPY file:7d75174e09b209cf7f56b715636c2b8e08dd083d548e8cdc8517cabd512600b5 in /etc/aerospike/aerospike.template.conf 
# Tue, 28 Sep 2021 02:03:11 GMT
COPY file:31b6a51a1d9d91f22433472f07f6ddfe3cea3bb07f460dd69c4187bc7fd20fdf in /entrypoint.sh 
# Tue, 28 Sep 2021 02:03:11 GMT
EXPOSE 3000 3001 3002
# Tue, 28 Sep 2021 02:03:11 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 28 Sep 2021 02:03:11 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ace2dab0de470d202d728be822cb17a6c26020674bd97a90dad3bc785b8123d`  
		Last Modified: Tue, 28 Sep 2021 02:03:54 GMT  
		Size: 56.4 MB (56375483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0581165861534a65a7c4d552efb9da12a58039325f0dc1b15067ce16daa8bc`  
		Last Modified: Tue, 28 Sep 2021 02:03:46 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea917f31f80724e0d90039c6f4530796ea30af1ee2f847025110585089dec5d`  
		Last Modified: Tue, 28 Sep 2021 02:03:46 GMT  
		Size: 909.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
