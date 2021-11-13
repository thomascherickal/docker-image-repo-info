## `arangodb:latest`

```console
$ docker pull arangodb@sha256:cbcf2b5c7693e9729cedc60a0fc14662218b96c4a8bb3140be03b99bce78a1b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:48bad58b5e0b1959d1c1b7fec31bfeaa5e953086fc9fc89b0eb91d23a4a8386f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.6 MB (187591074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9138759ab9e3e39a59bdf86004705879f2459624b20cf7ae4ff21ad77fc38ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 23:39:44 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 12 Nov 2021 23:39:44 GMT
ENV ARANGO_VERSION=3.8.2
# Fri, 12 Nov 2021 23:39:44 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Fri, 12 Nov 2021 23:39:45 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.2-1_amd64.deb
# Fri, 12 Nov 2021 23:39:45 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.2-1_amd64.deb
# Fri, 12 Nov 2021 23:39:45 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.2-1_amd64.deb.asc
# Fri, 12 Nov 2021 23:40:14 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 12 Nov 2021 23:40:16 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 12 Nov 2021 23:40:16 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 12 Nov 2021 23:40:16 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 12 Nov 2021 23:40:16 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 12 Nov 2021 23:40:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Nov 2021 23:40:17 GMT
EXPOSE 8529
# Fri, 12 Nov 2021 23:40:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62feb238128b8a2f4b372cdd1a7ce1921b6c080aea48043c904d7746d41ab2d`  
		Last Modified: Fri, 12 Nov 2021 23:41:25 GMT  
		Size: 184.8 MB (184779258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a91d2bbdf2b2633509306c0f1d7f7fa57be91bf1bf3a9a332b26fbe0119b1d`  
		Last Modified: Fri, 12 Nov 2021 23:41:02 GMT  
		Size: 2.1 KB (2083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1d5d71552d223f80a4fd14324db4fe9732b86cbebaa31e18e13159b4b7a7b9`  
		Last Modified: Fri, 12 Nov 2021 23:41:02 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
