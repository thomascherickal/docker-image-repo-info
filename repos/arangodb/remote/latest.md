## `arangodb:latest`

```console
$ docker pull arangodb@sha256:b6b87197cf8780ff6b48ffc0320ff277c2bdea94cdba1044bd6a11a0190bec63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:7c672cfcfa934557eca7e2c7d2aeda2bf17aa53e484d63bbea27fa2886b0f859
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127871737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:658e449d84a02b9ef5381d991bc4896d6240329fae6ba54d7872bcfd7e23a7f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:53:15 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_VERSION=3.7.5
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.5-1_amd64.deb
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.5-1_amd64.deb
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.5-1_amd64.deb.asc
# Thu, 17 Dec 2020 00:54:52 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 17 Dec 2020 00:54:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 17 Dec 2020 00:54:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 17 Dec 2020 00:54:54 GMT
COPY file:3a0ad717437ce87e5e260280982f3288fcfff74b46a1f17e5cd07f64d64ee5fa in /entrypoint.sh 
# Thu, 17 Dec 2020 00:54:54 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 17 Dec 2020 00:54:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:54:54 GMT
EXPOSE 8529
# Thu, 17 Dec 2020 00:54:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65967002b80f430ae8596954d75fd93a36098009e8b34c6be9a4c0090ebcf5bf`  
		Last Modified: Thu, 17 Dec 2020 00:56:47 GMT  
		Size: 125.1 MB (125054433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5813d1695f2fb37735869e8765cc6c1569e1e13e2103a2ef1f7eb1a01fa57a`  
		Last Modified: Thu, 17 Dec 2020 00:56:22 GMT  
		Size: 2.2 KB (2180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e6d1a8ef864d22d7102ba531ed18b49429e7c17e106826a894580e8ef2281`  
		Last Modified: Thu, 17 Dec 2020 00:56:23 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
