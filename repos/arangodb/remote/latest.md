## `arangodb:latest`

```console
$ docker pull arangodb@sha256:2ecc21012585e41ff4da61c62450d7463e97f4a0ed56a0bf8207cef395e134dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:570560a2ee939c89e4101da1ddd9957989b2af9ce00a4fea109e2aadbda2e2fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128341652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791766ee91cbaee919111db85adbdfd7bd3259cf0bd3e7d707959c8db5f73138`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:25:14 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 06 Mar 2021 07:25:50 GMT
ENV ARANGO_VERSION=3.7.9
# Sat, 06 Mar 2021 07:25:50 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Sat, 06 Mar 2021 07:25:51 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.9-1_amd64.deb
# Sat, 06 Mar 2021 07:25:51 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.9-1_amd64.deb
# Sat, 06 Mar 2021 07:25:51 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.9-1_amd64.deb.asc
# Sat, 06 Mar 2021 07:26:13 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 06 Mar 2021 07:26:15 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 06 Mar 2021 07:26:15 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 06 Mar 2021 07:26:15 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 06 Mar 2021 07:26:16 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 06 Mar 2021 07:26:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 06 Mar 2021 07:26:16 GMT
EXPOSE 8529
# Sat, 06 Mar 2021 07:26:16 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9263fb6d9a4f9e465ad9fa1af983d8546413132485f63e3bd2d2bf5d76e89c71`  
		Last Modified: Sat, 06 Mar 2021 07:27:26 GMT  
		Size: 125.5 MB (125523992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54295555e58deb2c4d3239cfb6e5b836a94a1788b5ae326fd6c4db4a9c33b18e`  
		Last Modified: Sat, 06 Mar 2021 07:27:03 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd64ea87594bb42167740600833918a1ea1f76244f250427cbc511942f37d7`  
		Last Modified: Sat, 06 Mar 2021 07:27:03 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
