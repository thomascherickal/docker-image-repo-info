## `aerospike:ee-5.6.0.5`

```console
$ docker pull aerospike@sha256:5dd07b0b97c8b812dc813221cdf156c1dc5ce02b524123ec3e94e187fb7e3fb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ee-5.6.0.5` - linux; amd64

```console
$ docker pull aerospike@sha256:e8d2430087e13f88e0b46ec48719e431b9cfed8cce16770c76d413ba56bb659b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82468401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba1de89285726e3dcf82d53c25a1d64f7b99de5bc33b07cc725c492242d3ae9`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 02 Jun 2021 19:52:44 GMT
ENV AEROSPIKE_VERSION=5.6.0.5
# Wed, 02 Jun 2021 19:52:44 GMT
ENV AEROSPIKE_SHA256=4beb4c5858e24736c9414da70a74e3c29a8d2c796bf1c3982cc502661f892bf1
# Wed, 02 Jun 2021 19:53:06 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian10" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 02 Jun 2021 19:53:07 GMT
COPY file:7d75174e09b209cf7f56b715636c2b8e08dd083d548e8cdc8517cabd512600b5 in /etc/aerospike/aerospike.template.conf 
# Wed, 02 Jun 2021 19:53:07 GMT
COPY file:31b6a51a1d9d91f22433472f07f6ddfe3cea3bb07f460dd69c4187bc7fd20fdf in /entrypoint.sh 
# Wed, 02 Jun 2021 19:53:07 GMT
EXPOSE 3000 3001 3002
# Wed, 02 Jun 2021 19:53:07 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 02 Jun 2021 19:53:08 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b466bb6322dd070cbdd99a30439ee82e64c29aaac6047b6b2c6e0fb901528cf`  
		Last Modified: Wed, 02 Jun 2021 19:53:54 GMT  
		Size: 55.3 MB (55320407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa88cb39e0d166afc2a850a947a2812a0dc7b3e4105a1dbe8bd62d95722fd760`  
		Last Modified: Wed, 02 Jun 2021 19:53:46 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44816c1344b802dfc3cb236a4b3b2e01c039117f0b6996350f8de601b9352fef`  
		Last Modified: Wed, 02 Jun 2021 19:53:46 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
