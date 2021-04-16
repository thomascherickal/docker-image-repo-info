## `aerospike:ee-5.5.0.9`

```console
$ docker pull aerospike@sha256:1b3158d6ff7d12b22969cc67668800c5ef794c58062c0a33a0dbccc2cec6db55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ee-5.5.0.9` - linux; amd64

```console
$ docker pull aerospike@sha256:ddde0bdbb89ecdc84cee491170d3f761e62f0f46130cc0907a622f03d3898016
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76466018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d611d912ae1c6f2c8acd762bf9f815433b3ed7faff407066f735c1e0d3f0a5b`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Thu, 15 Apr 2021 18:20:15 GMT
ENV AEROSPIKE_VERSION=5.5.0.9
# Thu, 15 Apr 2021 18:20:41 GMT
ENV AEROSPIKE_SHA256=ae222dcb2e8deb10e1fe45b27d02f32749ec2259c62a292d253d176689b05a06
# Thu, 15 Apr 2021 18:20:58 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian9" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Thu, 15 Apr 2021 18:20:59 GMT
COPY file:82161ba7b6e7d24ef9aeee8b19996114e9ff71c3928086ed1e58e01e82ee76a9 in /etc/aerospike/aerospike.template.conf 
# Thu, 15 Apr 2021 18:20:59 GMT
COPY file:11988df14ff2f0260ab7b8ccb322ee2d343b55791c51356df1d99639d16a6dbc in /entrypoint.sh 
# Thu, 15 Apr 2021 18:20:59 GMT
EXPOSE 3000 3001 3002
# Thu, 15 Apr 2021 18:21:00 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Thu, 15 Apr 2021 18:21:00 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445db9981579fca4ed6f412b94e46a2b3aaa7681a2a913ab3cc20f149cae8503`  
		Last Modified: Thu, 15 Apr 2021 18:22:16 GMT  
		Size: 53.9 MB (53935637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b2bdcde58051c58f77eaea86b0d529b0e7fcbc9d65817a652515ec236c7071`  
		Last Modified: Thu, 15 Apr 2021 18:22:08 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce06cbdf9f710dd740534dd0edb1ac87be08da66c6deb0b03f6bafcd39b27d0`  
		Last Modified: Thu, 15 Apr 2021 18:22:08 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
