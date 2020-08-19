<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.5`](#arangodb35)
-	[`arangodb:3.5.5`](#arangodb355)
-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.5`](#arangodb365)
-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.1`](#arangodb371)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.5`

```console
$ docker pull arangodb@sha256:43598bf9d7fb0ed26ed05882ef15c0bb9066a1ebf6e73c2ca0d475246d3020f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5` - linux; amd64

```console
$ docker pull arangodb@sha256:3a0a9fe72cf6d11a8b3826939a267e03da552ed5547b9a1cc763c8c901ffb232
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.3 MB (117286153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ace622ab4890ec354c4a0c5432f40eee6a4df85e163e734d2b54acdc3ab6abf1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 19 Aug 2020 19:19:32 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 19 Aug 2020 19:19:32 GMT
ENV ARANGO_VERSION=3.5.5.1
# Wed, 19 Aug 2020 19:19:32 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Wed, 19 Aug 2020 19:19:33 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.5.1-1_amd64.deb
# Wed, 19 Aug 2020 19:19:33 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5.1-1_amd64.deb
# Wed, 19 Aug 2020 19:19:33 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5.1-1_amd64.deb.asc
# Wed, 19 Aug 2020 19:19:59 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 19 Aug 2020 19:20:00 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 19 Aug 2020 19:20:00 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Wed, 19 Aug 2020 19:20:00 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 19 Aug 2020 19:20:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 19:20:00 GMT
EXPOSE 8529
# Wed, 19 Aug 2020 19:20:00 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fd54a8bb06916d1e3db5627b265f40c929f60159429518bb69346821f547e0`  
		Last Modified: Wed, 19 Aug 2020 19:21:34 GMT  
		Size: 114.5 MB (114470371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018a4718e5dacc3fc6c4e7d0e6d329aa108e094db6196c00c45a1e502fc711c2`  
		Last Modified: Wed, 19 Aug 2020 19:21:14 GMT  
		Size: 2.2 KB (2205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9829441de346bad79496a3b52bab3c4e72299ba57f8ffdc7c04095958dfe3780`  
		Last Modified: Wed, 19 Aug 2020 19:21:14 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.5.5`

```console
$ docker pull arangodb@sha256:43598bf9d7fb0ed26ed05882ef15c0bb9066a1ebf6e73c2ca0d475246d3020f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5.5` - linux; amd64

```console
$ docker pull arangodb@sha256:3a0a9fe72cf6d11a8b3826939a267e03da552ed5547b9a1cc763c8c901ffb232
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.3 MB (117286153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ace622ab4890ec354c4a0c5432f40eee6a4df85e163e734d2b54acdc3ab6abf1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 19 Aug 2020 19:19:32 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 19 Aug 2020 19:19:32 GMT
ENV ARANGO_VERSION=3.5.5.1
# Wed, 19 Aug 2020 19:19:32 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Wed, 19 Aug 2020 19:19:33 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.5.1-1_amd64.deb
# Wed, 19 Aug 2020 19:19:33 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5.1-1_amd64.deb
# Wed, 19 Aug 2020 19:19:33 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5.1-1_amd64.deb.asc
# Wed, 19 Aug 2020 19:19:59 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 19 Aug 2020 19:20:00 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 19 Aug 2020 19:20:00 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Wed, 19 Aug 2020 19:20:00 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 19 Aug 2020 19:20:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 19:20:00 GMT
EXPOSE 8529
# Wed, 19 Aug 2020 19:20:00 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fd54a8bb06916d1e3db5627b265f40c929f60159429518bb69346821f547e0`  
		Last Modified: Wed, 19 Aug 2020 19:21:34 GMT  
		Size: 114.5 MB (114470371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018a4718e5dacc3fc6c4e7d0e6d329aa108e094db6196c00c45a1e502fc711c2`  
		Last Modified: Wed, 19 Aug 2020 19:21:14 GMT  
		Size: 2.2 KB (2205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9829441de346bad79496a3b52bab3c4e72299ba57f8ffdc7c04095958dfe3780`  
		Last Modified: Wed, 19 Aug 2020 19:21:14 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6`

```console
$ docker pull arangodb@sha256:c2f6190ca5f179dfb9de55c76d1e691c493bb81ca1b8dd98504cd90124dd022b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:030bf460cb04fdbfeef933b629217e53653f64f86571ac44875a390cfac47f86
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.9 MB (117907370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5b65537dcbc65fb0a68e1f071b5f926178d545b823d114324ddb55aab7b01d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 19 Aug 2020 19:19:32 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 19 Aug 2020 19:20:06 GMT
ENV ARANGO_VERSION=3.6.5
# Wed, 19 Aug 2020 19:20:06 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Wed, 19 Aug 2020 19:20:07 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.5-1_amd64.deb
# Wed, 19 Aug 2020 19:20:07 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.5-1_amd64.deb
# Wed, 19 Aug 2020 19:20:07 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.5-1_amd64.deb.asc
# Wed, 19 Aug 2020 19:20:31 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 19 Aug 2020 19:20:32 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 19 Aug 2020 19:20:32 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Wed, 19 Aug 2020 19:20:32 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 19 Aug 2020 19:20:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 19:20:32 GMT
EXPOSE 8529
# Wed, 19 Aug 2020 19:20:33 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450be81ce4cd52ae20da13909b3c64669fa9e31e193a57314d107c0328efbbc2`  
		Last Modified: Wed, 19 Aug 2020 19:22:01 GMT  
		Size: 115.1 MB (115091587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280f4fb5944979739b31c79b16b50784ee89904ebf1aaa339a1410da5d296ec8`  
		Last Modified: Wed, 19 Aug 2020 19:21:41 GMT  
		Size: 2.2 KB (2205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04260e549829f6f8002d924a96849287be0781627974f36ebf7c1acd19efddb2`  
		Last Modified: Wed, 19 Aug 2020 19:21:41 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.5`

```console
$ docker pull arangodb@sha256:c2f6190ca5f179dfb9de55c76d1e691c493bb81ca1b8dd98504cd90124dd022b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6.5` - linux; amd64

```console
$ docker pull arangodb@sha256:030bf460cb04fdbfeef933b629217e53653f64f86571ac44875a390cfac47f86
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.9 MB (117907370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5b65537dcbc65fb0a68e1f071b5f926178d545b823d114324ddb55aab7b01d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 19 Aug 2020 19:19:32 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 19 Aug 2020 19:20:06 GMT
ENV ARANGO_VERSION=3.6.5
# Wed, 19 Aug 2020 19:20:06 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Wed, 19 Aug 2020 19:20:07 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.5-1_amd64.deb
# Wed, 19 Aug 2020 19:20:07 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.5-1_amd64.deb
# Wed, 19 Aug 2020 19:20:07 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.5-1_amd64.deb.asc
# Wed, 19 Aug 2020 19:20:31 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 19 Aug 2020 19:20:32 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 19 Aug 2020 19:20:32 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Wed, 19 Aug 2020 19:20:32 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 19 Aug 2020 19:20:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 19:20:32 GMT
EXPOSE 8529
# Wed, 19 Aug 2020 19:20:33 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450be81ce4cd52ae20da13909b3c64669fa9e31e193a57314d107c0328efbbc2`  
		Last Modified: Wed, 19 Aug 2020 19:22:01 GMT  
		Size: 115.1 MB (115091587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280f4fb5944979739b31c79b16b50784ee89904ebf1aaa339a1410da5d296ec8`  
		Last Modified: Wed, 19 Aug 2020 19:21:41 GMT  
		Size: 2.2 KB (2205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04260e549829f6f8002d924a96849287be0781627974f36ebf7c1acd19efddb2`  
		Last Modified: Wed, 19 Aug 2020 19:21:41 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7`

```console
$ docker pull arangodb@sha256:a377d70a85296d7d3f36e7f217fb49fb305493dcd9f04b22f33c5ab77fd44c3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.7` - linux; amd64

```console
$ docker pull arangodb@sha256:7318f6987939e3c64d488c04b93595f2fda9e83e310875972ff2f7c7d388493a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126489106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16acb86d86d885f01a42c3b1418539f29572d28ea4c7de072f8b99daf9ee3240`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 19 Aug 2020 19:19:32 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 19 Aug 2020 19:20:40 GMT
ENV ARANGO_VERSION=3.7.1
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.1-1_amd64.deb
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.1-1_amd64.deb
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.1-1_amd64.deb.asc
# Wed, 19 Aug 2020 19:21:04 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 19 Aug 2020 19:21:05 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 19 Aug 2020 19:21:05 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Wed, 19 Aug 2020 19:21:05 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 19 Aug 2020 19:21:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 19:21:05 GMT
EXPOSE 8529
# Wed, 19 Aug 2020 19:21:06 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e18d7a6952f468a6d357610ecead8ae0106b9f8530cc1d1a39d5231990bfbb`  
		Last Modified: Wed, 19 Aug 2020 19:22:26 GMT  
		Size: 123.7 MB (123673325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a86ee0f636a04e632bc122de5bcb361f52cab2e44c1ae4f6a867023b8c0a0`  
		Last Modified: Wed, 19 Aug 2020 19:22:05 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c58742e8b12dde5ea4f74f39a89ad5a672fdd0b5b9c3d8ab93042cebb2688e`  
		Last Modified: Wed, 19 Aug 2020 19:22:05 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7.1`

```console
$ docker pull arangodb@sha256:a377d70a85296d7d3f36e7f217fb49fb305493dcd9f04b22f33c5ab77fd44c3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.7.1` - linux; amd64

```console
$ docker pull arangodb@sha256:7318f6987939e3c64d488c04b93595f2fda9e83e310875972ff2f7c7d388493a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126489106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16acb86d86d885f01a42c3b1418539f29572d28ea4c7de072f8b99daf9ee3240`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 19 Aug 2020 19:19:32 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 19 Aug 2020 19:20:40 GMT
ENV ARANGO_VERSION=3.7.1
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.1-1_amd64.deb
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.1-1_amd64.deb
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.1-1_amd64.deb.asc
# Wed, 19 Aug 2020 19:21:04 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 19 Aug 2020 19:21:05 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 19 Aug 2020 19:21:05 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Wed, 19 Aug 2020 19:21:05 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 19 Aug 2020 19:21:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 19:21:05 GMT
EXPOSE 8529
# Wed, 19 Aug 2020 19:21:06 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e18d7a6952f468a6d357610ecead8ae0106b9f8530cc1d1a39d5231990bfbb`  
		Last Modified: Wed, 19 Aug 2020 19:22:26 GMT  
		Size: 123.7 MB (123673325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a86ee0f636a04e632bc122de5bcb361f52cab2e44c1ae4f6a867023b8c0a0`  
		Last Modified: Wed, 19 Aug 2020 19:22:05 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c58742e8b12dde5ea4f74f39a89ad5a672fdd0b5b9c3d8ab93042cebb2688e`  
		Last Modified: Wed, 19 Aug 2020 19:22:05 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:a377d70a85296d7d3f36e7f217fb49fb305493dcd9f04b22f33c5ab77fd44c3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:7318f6987939e3c64d488c04b93595f2fda9e83e310875972ff2f7c7d388493a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126489106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16acb86d86d885f01a42c3b1418539f29572d28ea4c7de072f8b99daf9ee3240`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 19 Aug 2020 19:19:32 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 19 Aug 2020 19:20:40 GMT
ENV ARANGO_VERSION=3.7.1
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.1-1_amd64.deb
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.1-1_amd64.deb
# Wed, 19 Aug 2020 19:20:41 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.1-1_amd64.deb.asc
# Wed, 19 Aug 2020 19:21:04 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 19 Aug 2020 19:21:05 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 19 Aug 2020 19:21:05 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Wed, 19 Aug 2020 19:21:05 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 19 Aug 2020 19:21:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 19:21:05 GMT
EXPOSE 8529
# Wed, 19 Aug 2020 19:21:06 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e18d7a6952f468a6d357610ecead8ae0106b9f8530cc1d1a39d5231990bfbb`  
		Last Modified: Wed, 19 Aug 2020 19:22:26 GMT  
		Size: 123.7 MB (123673325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a86ee0f636a04e632bc122de5bcb361f52cab2e44c1ae4f6a867023b8c0a0`  
		Last Modified: Wed, 19 Aug 2020 19:22:05 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c58742e8b12dde5ea4f74f39a89ad5a672fdd0b5b9c3d8ab93042cebb2688e`  
		Last Modified: Wed, 19 Aug 2020 19:22:05 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
