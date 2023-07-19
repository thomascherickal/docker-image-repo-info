## `amazoncorretto:20-al2-full`

```console
$ docker pull amazoncorretto@sha256:364659a8775123d9e7d2af20267572f497da58b2935c646d04c68937cae0f327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d4753af924ad86e37593422d090255fb3a306e562339fb0df9f870005eefd41e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.4 MB (223429903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e82f2f90cd04ac750e9c71824c2b63330bbd748ef1cfea3daf4ed649e13290e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Jul 2023 01:20:13 GMT
COPY dir:be29c71398840090bec7021ae8f2d354451564507602cf38257ad90a915b1838 in / 
# Thu, 13 Jul 2023 01:20:13 GMT
CMD ["/bin/bash"]
# Wed, 19 Jul 2023 00:30:48 GMT
ARG version=20.0.2.9-1
# Wed, 19 Jul 2023 00:31:11 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 19 Jul 2023 00:31:12 GMT
ENV LANG=C.UTF-8
# Wed, 19 Jul 2023 00:31:12 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:e90aa42bc48ff728ab10fd485b42144e863dfd8689dd6ea94c78ac0357ec5101`  
		Last Modified: Fri, 30 Jun 2023 00:09:38 GMT  
		Size: 62.5 MB (62485766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b2ff89d7b7c72e9465aa1d9ecbb1c64c2a5a707164c9a4a0cf0d0ea8f9abc3`  
		Last Modified: Wed, 19 Jul 2023 00:46:37 GMT  
		Size: 160.9 MB (160944137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:6f595b6bd4eef69a51deaebd73037314ac1b5547a2f9dd7dd040624da6296626
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.1 MB (223096876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:377e412353e3debd6c55c55647846189ae238d1a86a1f6e4fb87d1ac2130c784`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Jul 2023 00:40:00 GMT
COPY dir:a284fdf4a484ebc9131c665fc151094ec73265d07d353476272944e301722064 in / 
# Thu, 13 Jul 2023 00:40:01 GMT
CMD ["/bin/bash"]
# Wed, 19 Jul 2023 00:47:39 GMT
ARG version=20.0.2.9-1
# Wed, 19 Jul 2023 00:48:00 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 19 Jul 2023 00:48:01 GMT
ENV LANG=C.UTF-8
# Wed, 19 Jul 2023 00:48:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:20c8bca6ae5daad56b485a4b6f1f395a51727d69eb6a7566c53b00a366e46576`  
		Last Modified: Fri, 30 Jun 2023 17:38:06 GMT  
		Size: 64.1 MB (64128925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9c1d461287a70c892dd1c4136a82e354ee624fac135ba4ac1b4e188380d5f3`  
		Last Modified: Wed, 19 Jul 2023 01:02:06 GMT  
		Size: 159.0 MB (158967951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
