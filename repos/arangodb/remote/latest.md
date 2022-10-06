## `arangodb:latest`

```console
$ docker pull arangodb@sha256:1473513a62b3bc8d5b6bec88dfb3797df99fc5a1c7f637e07c5ebcd075902dde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:5871e58bc4205073ae72f93739d3d3f7c59df1234fb8b997bb19003d8e2267d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.2 MB (201164652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66558e1dbf6bbbf2f653b92e1d4fee19713c7b144f9fe9962ff239c931ea9564`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:51:41 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 06 Oct 2022 19:52:15 GMT
ENV ARANGO_VERSION=3.9.3
# Thu, 06 Oct 2022 19:52:15 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Thu, 06 Oct 2022 19:52:15 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.3-1_amd64.deb
# Thu, 06 Oct 2022 19:52:15 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.3-1_amd64.deb
# Thu, 06 Oct 2022 19:52:15 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.3-1_amd64.deb.asc
# Thu, 06 Oct 2022 19:52:42 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 06 Oct 2022 19:52:43 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 06 Oct 2022 19:52:44 GMT
RUN echo "UTC" > /etc/timezone
# Thu, 06 Oct 2022 19:52:44 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 06 Oct 2022 19:52:44 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 06 Oct 2022 19:52:44 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 06 Oct 2022 19:52:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 19:52:44 GMT
EXPOSE 8529
# Thu, 06 Oct 2022 19:52:44 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d2e28d78a90b0910e64739a3514b58212d33755fdf49b1fd7d1a1691c7620b`  
		Last Modified: Thu, 06 Oct 2022 19:53:52 GMT  
		Size: 198.3 MB (198334675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e24444b684c9850ee9d71c36862c5ea05ed8d03d6d178581d8d921d92443871`  
		Last Modified: Thu, 06 Oct 2022 19:53:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc405a118acd2437261c2391c38b4d3332ca39fbb5eae4d3e0a58895951e6336`  
		Last Modified: Thu, 06 Oct 2022 19:53:29 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca561580ab8f06159eb6a0687bfdee1a25232814c66f89bccd3ce9a879bd098`  
		Last Modified: Thu, 06 Oct 2022 19:53:29 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
