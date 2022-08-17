## `amazoncorretto:11-al2-full`

```console
$ docker pull amazoncorretto@sha256:4541bfc92b2da12cb4ff62938f53fe85b5ba22089394d9625a135adda32f5f2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:87423d53a823a722e022fc225edc635bb1d5c21584da9c8b938c338605253e12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.8 MB (209754417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d4d7e684bb1440d81d5c117a84d1dedbb895ee147d2c6022623b5019a1d78ba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 Aug 2022 00:20:15 GMT
ADD file:56a385790046ac5dfb85932009eb1e99c8593221e306b937274c477c05cc9886 in / 
# Fri, 12 Aug 2022 00:20:15 GMT
CMD ["/bin/bash"]
# Tue, 16 Aug 2022 23:19:42 GMT
ARG version=11.0.16.9-1
# Tue, 16 Aug 2022 23:20:07 GMT
# ARGS: version=11.0.16.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 16 Aug 2022 23:20:08 GMT
ENV LANG=C.UTF-8
# Tue, 16 Aug 2022 23:20:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:5e0be87f98fb0e8a6ecddb6b717178ddc6555638e6e89d39929d47654b79739d`  
		Last Modified: Mon, 01 Aug 2022 22:09:03 GMT  
		Size: 62.3 MB (62316216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e4ffb734538b9cdb672d02c688ccd9287d4f449db6f112d8bea459ca332064`  
		Last Modified: Tue, 16 Aug 2022 23:23:44 GMT  
		Size: 147.4 MB (147438201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:39f5189ba90113e0316fb2aa2e69499858f012982e909afbedac393cfa3d9e1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208497911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a3a2e2fb16707d03b24e1a7cb9c530ba78bc71fadbae7a1fb50dbe9394104f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 Aug 2022 00:39:26 GMT
ADD file:3ec97c6bec2a8682b0b4088021da97853effeb7dfafb69329cfcb5686c3dee30 in / 
# Fri, 12 Aug 2022 00:39:28 GMT
CMD ["/bin/bash"]
# Tue, 16 Aug 2022 22:39:34 GMT
ARG version=11.0.16.9-1
# Tue, 16 Aug 2022 22:39:50 GMT
# ARGS: version=11.0.16.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 16 Aug 2022 22:39:50 GMT
ENV LANG=C.UTF-8
# Tue, 16 Aug 2022 22:39:51 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:9f9c648afd7976bdc42d03595d6a1c1c502c47f18abb3f42a9a20b38e7d6e161`  
		Last Modified: Mon, 01 Aug 2022 22:09:01 GMT  
		Size: 63.9 MB (63927916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d20e7d3d53272bd500ea82cc4ab23c5061bff664fb11d26b004ce7a498b2b1`  
		Last Modified: Tue, 16 Aug 2022 22:41:29 GMT  
		Size: 144.6 MB (144569995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
