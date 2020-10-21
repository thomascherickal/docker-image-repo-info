## `arangodb:latest`

```console
$ docker pull arangodb@sha256:e8173f33ebb2048b29685dfb5b5a2397cf65353a4a1b98ebb6414d104eb2f4e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:e6d27abfe67cf286234f01fc29ec22a5025cfc3729e8989c302c9df1471e46b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127978306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddf07df96ced3f4891a9a31fb4c55cd994d366b6a60b157a4f4d2c49badac01d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 19 Aug 2020 19:19:32 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 20 Oct 2020 23:48:43 GMT
ENV ARANGO_VERSION=3.7.3
# Tue, 20 Oct 2020 23:48:43 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Tue, 20 Oct 2020 23:48:43 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.3-1_amd64.deb
# Tue, 20 Oct 2020 23:48:44 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.3-1_amd64.deb
# Tue, 20 Oct 2020 23:48:44 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.3-1_amd64.deb.asc
# Tue, 20 Oct 2020 23:49:14 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 20 Oct 2020 23:49:15 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 20 Oct 2020 23:49:15 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 20 Oct 2020 23:49:16 GMT
COPY file:3a0ad717437ce87e5e260280982f3288fcfff74b46a1f17e5cd07f64d64ee5fa in /entrypoint.sh 
# Tue, 20 Oct 2020 23:49:16 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 20 Oct 2020 23:49:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Oct 2020 23:49:16 GMT
EXPOSE 8529
# Tue, 20 Oct 2020 23:49:16 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6165cae7ad6a92a606da0d90b4b97a72050a95da21aefc46ac1fe6120158d24`  
		Last Modified: Tue, 20 Oct 2020 23:49:50 GMT  
		Size: 125.2 MB (125162549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d9e77c864eb446107fc9ee3aadcea6de1e7a35d670ff1c8f61331ae34bbd0c`  
		Last Modified: Tue, 20 Oct 2020 23:49:28 GMT  
		Size: 2.2 KB (2181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92f35f1d36f6de1a70ffcdedc2190f5178ea461ec3743a65a3f7de05d96c3b6`  
		Last Modified: Tue, 20 Oct 2020 23:49:28 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
