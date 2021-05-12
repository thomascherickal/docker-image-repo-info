## `aerospike:ee-5.5.0.9`

```console
$ docker pull aerospike@sha256:93dd21219b26ccc163f8732b22a595247ed86d4aeba8dd1988410f40dbc795e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ee-5.5.0.9` - linux; amd64

```console
$ docker pull aerospike@sha256:b728c6cc666c7eab45ef504b3a1820aa9ffbaa0c545391c381bee6aafa74e2c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76466660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd19df67e5de262814a0ea4d70c86d53de610ceb2f70b4385e10da98ea95eb6`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:48:39 GMT
ENV AEROSPIKE_VERSION=5.5.0.9
# Wed, 12 May 2021 01:48:39 GMT
ENV AEROSPIKE_SHA256=ae222dcb2e8deb10e1fe45b27d02f32749ec2259c62a292d253d176689b05a06
# Wed, 12 May 2021 01:49:07 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian9" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:49:08 GMT
COPY file:82161ba7b6e7d24ef9aeee8b19996114e9ff71c3928086ed1e58e01e82ee76a9 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:49:08 GMT
COPY file:11988df14ff2f0260ab7b8ccb322ee2d343b55791c51356df1d99639d16a6dbc in /entrypoint.sh 
# Wed, 12 May 2021 01:49:08 GMT
EXPOSE 3000 3001 3002
# Wed, 12 May 2021 01:49:09 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:49:09 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4d28478b0d5758137f998e0932a9ba89d6a883cc3d2c1b2c8edd2fef497c88`  
		Last Modified: Wed, 12 May 2021 01:52:17 GMT  
		Size: 53.9 MB (53936277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd5749258c6dd58e5600f83c6e45b1343ea458b9710770d987b745217f3ebc5`  
		Last Modified: Wed, 12 May 2021 01:52:06 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79f444a64949cb9febef2abc39735ef1b4f29e6f2518d32465948b021c10936`  
		Last Modified: Wed, 12 May 2021 01:52:06 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
