## `amazoncorretto:latest`

```console
$ docker pull amazoncorretto@sha256:39d68b316cf804a4f5303734e322003f1eb9f8d4ef242aa4f46fc5305ae22980
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:332c2f24ea056e182312ab5059c7e4f40c73a330d355827181e5d2194001a198
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.8 MB (182849657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aec62b94b0fdc911598bc34b243dff16f1c6293ed300a2480f76c2f00a58d2c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:46:32 GMT
ADD file:119ae574c5d5b6e59e83ecadbe4c8dc4e7b535508e63704e74939df696c9b9a1 in / 
# Wed, 01 Apr 2020 06:46:33 GMT
CMD ["/bin/bash"]
# Wed, 15 Apr 2020 00:19:31 GMT
ARG version=1.8.0_252.b09-1
# Wed, 15 Apr 2020 00:19:52 GMT
# ARGS: version=1.8.0_252.b09-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && yum install -y fontconfig     && yum clean all
# Wed, 15 Apr 2020 00:19:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:a8d577519c9fb37ef239a77026a16c019d20cce14b25867f57a44459b3bbf387`  
		Last Modified: Wed, 01 Apr 2020 06:48:00 GMT  
		Size: 61.7 MB (61655014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e78d35593828bd24975e861c85b720f12a97d42ed375649d75754100cbfa6b`  
		Last Modified: Wed, 15 Apr 2020 00:20:59 GMT  
		Size: 121.2 MB (121194643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e2c8c9dd92cbc1319c9ff65d140343d2be0f970461944a9a86285573acc6a924
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.3 MB (168327590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:537c63a263c9a137d18ee71d0bbc094b437a24c28e35ac47336f2836d90821f7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 05:22:43 GMT
ADD file:40b8f329ad6d591029e1a4cde76c1d097315b136796d31bb9d3df35183423c14 in / 
# Wed, 01 Apr 2020 05:22:46 GMT
CMD ["/bin/bash"]
# Wed, 15 Apr 2020 00:39:52 GMT
ARG version=1.8.0_252.b09-1
# Wed, 15 Apr 2020 00:40:33 GMT
# ARGS: version=1.8.0_252.b09-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && yum install -y fontconfig     && yum clean all
# Wed, 15 Apr 2020 00:40:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:01d0a3bd5b98a6512409a10e5e5b065e87b794f924f3f9f7662939925aac631b`  
		Last Modified: Wed, 01 Apr 2020 05:24:01 GMT  
		Size: 63.1 MB (63072580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d0cb5285429fdf5fd8cfbf08f7e50f7c35c0aa470a38b035be5426c034c1f5`  
		Last Modified: Wed, 15 Apr 2020 00:42:15 GMT  
		Size: 105.3 MB (105255010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
