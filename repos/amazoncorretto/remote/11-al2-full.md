## `amazoncorretto:11-al2-full`

```console
$ docker pull amazoncorretto@sha256:d482d0dc14c9a59289f0ab710d1b269c2d3e6c48a439e2ba28db85b9d24f0b65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:94efee2ddd101485faf736da62580b4cb8e258e567d3ab1cff66ddd3d7359f14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.7 MB (258735363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94ddbd0d48bdf24c097318bf992f3faf1ecb6ec04ce03535f7e30e8da7fe3af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:46:32 GMT
ADD file:119ae574c5d5b6e59e83ecadbe4c8dc4e7b535508e63704e74939df696c9b9a1 in / 
# Wed, 01 Apr 2020 06:46:33 GMT
CMD ["/bin/bash"]
# Wed, 15 Apr 2020 00:19:59 GMT
ARG version=11.0.7.10-1
# Wed, 15 Apr 2020 00:20:22 GMT
# ARGS: version=11.0.7.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && yum install -y fontconfig     && yum clean all
# Wed, 15 Apr 2020 00:20:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:a8d577519c9fb37ef239a77026a16c019d20cce14b25867f57a44459b3bbf387`  
		Last Modified: Wed, 01 Apr 2020 06:48:00 GMT  
		Size: 61.7 MB (61655014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9360d240c320d53a82f2663d7cd26ee90cfbdd239741faa22ecb522ab3fcb81a`  
		Last Modified: Wed, 15 Apr 2020 00:21:22 GMT  
		Size: 197.1 MB (197080349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:504e607e8a77f7cc3f94e2b3d9134cc517f2a7344493e07bad6c6ac18c4c725f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.0 MB (258969262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2608f599d911c103fd367a8679925ed323166686d92a68298e64da441b9d09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 05:22:43 GMT
ADD file:40b8f329ad6d591029e1a4cde76c1d097315b136796d31bb9d3df35183423c14 in / 
# Wed, 01 Apr 2020 05:22:46 GMT
CMD ["/bin/bash"]
# Wed, 15 Apr 2020 00:40:47 GMT
ARG version=11.0.7.10-1
# Wed, 15 Apr 2020 00:41:38 GMT
# ARGS: version=11.0.7.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && yum install -y fontconfig     && yum clean all
# Wed, 15 Apr 2020 00:41:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:01d0a3bd5b98a6512409a10e5e5b065e87b794f924f3f9f7662939925aac631b`  
		Last Modified: Wed, 01 Apr 2020 05:24:01 GMT  
		Size: 63.1 MB (63072580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09f801c0abde2b5d42256dba578cdd20f323e23c3b29ab4bf4cab62e3766989`  
		Last Modified: Wed, 15 Apr 2020 00:42:54 GMT  
		Size: 195.9 MB (195896682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
