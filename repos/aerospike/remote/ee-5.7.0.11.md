## `aerospike:ee-5.7.0.11`

```console
$ docker pull aerospike@sha256:431f09d49f8f3beb174c7f489a51ab5753e84cb7d909b7c1e98c942518f184e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ee-5.7.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:ff44ff4832ad1ddf080d3193103ef8c5bf5ca1bdbd72bddefd53f0cff47e9adf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83905393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca26bdefd5eabc5267e495e8214327823a95698e4f7dfe646c6eb0931e31a9b7`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Fri, 11 Mar 2022 18:19:21 GMT
ENV AEROSPIKE_VERSION=5.7.0.11
# Fri, 11 Mar 2022 18:19:21 GMT
ENV AEROSPIKE_SHA256=f43f38680e39429976ef359f7b72034f8c1a9bf624d94826d61b898212e91766
# Fri, 11 Mar 2022 18:19:21 GMT
ENV AS_TINI_SHA256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940
# Fri, 11 Mar 2022 18:19:45 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps wget python python3 python3-distutils lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static -O /usr/bin/as-tini-static   && echo "$AS_TINI_SHA256 /usr/bin/as-tini-static" | sha256sum -c -   && chmod +x /usr/bin/as-tini-static   && wget "https://download.aerospike.com/artifacts/aerospike-server-enterprise/${AEROSPIKE_VERSION}/aerospike-server-enterprise-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Fri, 11 Mar 2022 18:19:45 GMT
COPY file:7d75174e09b209cf7f56b715636c2b8e08dd083d548e8cdc8517cabd512600b5 in /etc/aerospike/aerospike.template.conf 
# Fri, 11 Mar 2022 18:19:46 GMT
COPY file:31b6a51a1d9d91f22433472f07f6ddfe3cea3bb07f460dd69c4187bc7fd20fdf in /entrypoint.sh 
# Fri, 11 Mar 2022 18:19:46 GMT
EXPOSE 3000 3001 3002
# Fri, 11 Mar 2022 18:19:46 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Fri, 11 Mar 2022 18:19:46 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570cbaf8abc55360d9e1c8c4f40abc5438816bf1300795f7a102bca427a7f262`  
		Last Modified: Fri, 11 Mar 2022 18:20:34 GMT  
		Size: 56.7 MB (56749576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32ba73a5ac434be823a2be55aa1d1509f08119cd478ddd2282f1a679f6f134f`  
		Last Modified: Fri, 11 Mar 2022 18:20:22 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d405c9090ec55a218ad4e8feea58235f897745718b96a8f4f23b66870f106c`  
		Last Modified: Fri, 11 Mar 2022 18:20:22 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
