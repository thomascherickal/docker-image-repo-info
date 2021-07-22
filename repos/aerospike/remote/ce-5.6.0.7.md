## `aerospike:ce-5.6.0.7`

```console
$ docker pull aerospike@sha256:09d4adc8ef8f7d5aa48426874a5fcc3fb9d90a725b7ba6ee1a619daf2ebb69b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-5.6.0.7` - linux; amd64

```console
$ docker pull aerospike@sha256:c41377ab3e8a3ec9b55bc485e2c8347fbf522dc828ed3c6104a0b65b34b75028
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80606729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a075c4e0ab79c8a91d45e0c685aadeed2929965c0a5966cfb954565d73a44d9`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:32:39 GMT
ENV AEROSPIKE_VERSION=5.6.0.7
# Thu, 22 Jul 2021 01:33:30 GMT
ENV AEROSPIKE_SHA256=a8693ee9eae5e818828066c0a091cb5cf0c2795c548308948582c2f7f04942ca
# Thu, 22 Jul 2021 01:34:12 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Thu, 22 Jul 2021 01:34:13 GMT
COPY file:1897c4aae07efbc61bf2d8c2c7b0dfb0990174e11cc787eac71d5adf767abaed in /etc/aerospike/aerospike.template.conf 
# Thu, 22 Jul 2021 01:34:14 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Thu, 22 Jul 2021 01:34:14 GMT
EXPOSE 3000 3001 3002
# Thu, 22 Jul 2021 01:34:15 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Thu, 22 Jul 2021 01:34:15 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de676a7cf803eae0d430de9c17143b807062573e8a5b11f62b4c1be32098b01e`  
		Last Modified: Thu, 22 Jul 2021 01:34:56 GMT  
		Size: 53.5 MB (53458912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a349efdfdb7986e6a2b8e04961b5d376290e1019e094499a8ddf4e55928888`  
		Last Modified: Thu, 22 Jul 2021 01:34:49 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d90f09f2f32acf1e082f7ad803295c653a75cd542f6c3cca3ca27f04edcd08`  
		Last Modified: Thu, 22 Jul 2021 01:34:51 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
