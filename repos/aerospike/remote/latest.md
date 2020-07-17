## `aerospike:latest`

```console
$ docker pull aerospike@sha256:a9b49b1bb2d29437a0e0d124b14151b3b8b4962daa40e933c42153ef6cec076c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:722b6b1863ca8d36446f2f9f27e471975561e0942f5bcf1ba3510dac1168cbe5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53092232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a9471131f1e780e2702583d175c32cc746801f7137d591fbf124a50746e7247`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:35 GMT
ADD file:57b431451a292755d0f13673f5f3bea9f62aea36c7a1b59d34d7d200ba134fea in / 
# Tue, 09 Jun 2020 01:23:35 GMT
CMD ["bash"]
# Fri, 17 Jul 2020 20:20:16 GMT
ENV AEROSPIKE_VERSION=5.0.0.10
# Fri, 17 Jul 2020 20:20:16 GMT
ENV AEROSPIKE_SHA256=cf56e1dfabf73508491c669a9eaf32b97ddb91863e4bd78cd0cec64bc53fd0ca
# Fri, 17 Jul 2020 20:20:32 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Fri, 17 Jul 2020 20:20:32 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Fri, 17 Jul 2020 20:20:32 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Fri, 17 Jul 2020 20:20:33 GMT
VOLUME [/opt/aerospike/data]
# Fri, 17 Jul 2020 20:20:33 GMT
EXPOSE 3000 3001 3002 3003
# Fri, 17 Jul 2020 20:20:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Jul 2020 20:20:33 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:7d2977b12acb33f192e3f20b7e15a467cc8f3f5124a15d975a6d4afe5fa3d258`  
		Last Modified: Tue, 09 Jun 2020 01:28:13 GMT  
		Size: 22.5 MB (22519600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7798fab2dd766f5e8b3994f4440394f86ac3e283081fd45542683d208dfb9cb6`  
		Last Modified: Fri, 17 Jul 2020 20:21:02 GMT  
		Size: 30.6 MB (30570579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4254bf99ed31f3462f661060bb9609f38ff75a740b2b7ff7369fddab2d765946`  
		Last Modified: Fri, 17 Jul 2020 20:20:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5044fc2818042842c38de000be7b55fc946d0f97d941c52c5e11e5e5138c1576`  
		Last Modified: Fri, 17 Jul 2020 20:20:57 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
