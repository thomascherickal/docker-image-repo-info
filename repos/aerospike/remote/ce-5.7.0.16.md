## `aerospike:ce-5.7.0.16`

```console
$ docker pull aerospike@sha256:4caffca3ec1d6f28ee917072b1980278f4957b031e60510ec4af3a25c292e10b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-5.7.0.16` - linux; amd64

```console
$ docker pull aerospike@sha256:19a627cc017558169fe9b1afc00f3373b6bdcd1ab316c780fc76d87c44bde7b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81544921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f96d8f3327305719597d7bce38f214b2adb34d34034e2f661c873e985aa1754`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:25:56 GMT
ENV AEROSPIKE_VERSION=5.7.0.16
# Wed, 20 Apr 2022 15:26:19 GMT
ENV AEROSPIKE_SHA256=31d54cd60c48a365f761ba35f7e2914f36d6c1b09e6143bec3c7ce68fb1a4409
# Wed, 20 Apr 2022 15:26:37 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 20 Apr 2022 15:26:38 GMT
COPY file:1897c4aae07efbc61bf2d8c2c7b0dfb0990174e11cc787eac71d5adf767abaed in /etc/aerospike/aerospike.template.conf 
# Wed, 20 Apr 2022 15:26:38 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Wed, 20 Apr 2022 15:26:38 GMT
EXPOSE 3000 3001 3002
# Wed, 20 Apr 2022 15:26:38 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 20 Apr 2022 15:26:38 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fe87bf87708baecbfa1c3c14014e5d34eb1ef5a91548e8f6459ac3370d7a12`  
		Last Modified: Wed, 20 Apr 2022 15:27:16 GMT  
		Size: 54.4 MB (54402240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d002d80fa9c3721439005c71a6c2b435be0d9eb977049391da5d90314d2425`  
		Last Modified: Wed, 20 Apr 2022 15:27:08 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe1e5f5fcd832ea232ed33472d6206b9de4ed9f36590991233ae2f32583dd7a`  
		Last Modified: Wed, 20 Apr 2022 15:27:08 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
