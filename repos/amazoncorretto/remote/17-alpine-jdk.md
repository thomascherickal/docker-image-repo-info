## `amazoncorretto:17-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:d4715e627365f5a1487ece0a87f1ad4dcf67eddf0ae937fd61f43e57c347eb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4f0aaacb432a483fb06b79567ee74a5b7ce7218625e05ded20a3d057de92e75a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.9 MB (198930683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a8136cf53529ca159d604c8a823ab34c17f77986ebb604be5dec7f0e20740b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 17 Sep 2021 18:20:15 GMT
ARG version=17.0.0.35.1
# Fri, 17 Sep 2021 18:20:23 GMT
# ARGS: version=17.0.0.35.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Fri, 17 Sep 2021 18:20:24 GMT
ENV LANG=C.UTF-8
# Fri, 17 Sep 2021 18:20:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 17 Sep 2021 18:20:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0129aa7f582aeb95bed9cd254e70c135ee2a28bbc71ca382c177eb21b46fb06`  
		Last Modified: Fri, 17 Sep 2021 18:22:06 GMT  
		Size: 196.1 MB (196116237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
