## `arangodb:latest`

```console
$ docker pull arangodb@sha256:4765a245dd98db23291f3e97c20a3a877911ef4457ea14e38b300cffd4448185
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:9fee4829c4932cf81aa03487ffad448ce1075f94b355ca8b718e7d3bfe0af288
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.7 MB (187715107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd44138cd5dcf3d9004415f243b0ddd8b3c8d5d01c0c31f5e2a9e49086d8c7a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 23:39:44 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 20 Nov 2021 02:19:20 GMT
ENV ARANGO_VERSION=3.8.3
# Sat, 20 Nov 2021 02:19:20 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Sat, 20 Nov 2021 02:19:21 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.3-1_amd64.deb
# Sat, 20 Nov 2021 02:19:21 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.3-1_amd64.deb
# Sat, 20 Nov 2021 02:19:21 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.3-1_amd64.deb.asc
# Sat, 20 Nov 2021 02:19:53 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 20 Nov 2021 02:19:55 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 20 Nov 2021 02:19:55 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 20 Nov 2021 02:19:55 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 20 Nov 2021 02:19:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 20 Nov 2021 02:19:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 20 Nov 2021 02:19:56 GMT
EXPOSE 8529
# Sat, 20 Nov 2021 02:19:56 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5e2fdaf015a10264372be3bb143c099966cdb1ad37ae93e2bfc7cc84f37dd6`  
		Last Modified: Sat, 20 Nov 2021 02:20:37 GMT  
		Size: 184.9 MB (184903285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fdda8e8e5d89f82b69a9edd12aa12ad26d882df1a6e8a19c84ec7d01ce1289`  
		Last Modified: Sat, 20 Nov 2021 02:20:10 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bae27f80def5a288691c1f22397af4f522523df24b4026e47b16fd9b74bc2`  
		Last Modified: Sat, 20 Nov 2021 02:20:10 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
