## `amazoncorretto:8-alpine3.13-full`

```console
$ docker pull amazoncorretto@sha256:23fa377bf6aa6a0fe358965e7d995fc3c79333e30597158aa337009c61ad3902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.13-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4c16e9964195c8b3984fbc9638fcd369e882d5eec73d00254ab6cb2bff046b3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101619617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf8f472f4916c69c41a0bd56e53ce8504413e8ba1ea0e0ea4720dbd7c2e2718`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:14 GMT
ADD file:7fd90c097e2c4587dee91726d71abc02fa1aa6a3a3395c862206a4e14e0c299c in / 
# Tue, 09 Aug 2022 17:20:14 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:36:46 GMT
ARG version=8.342.07.4
# Tue, 09 Aug 2022 17:36:50 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 09 Aug 2022 17:36:51 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 17:36:51 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 09 Aug 2022 17:36:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:72cfd02ff4d01b1f319eed108b53120dea0185b916d2abeb4e6121879cbf7a65`  
		Last Modified: Tue, 09 Aug 2022 17:21:16 GMT  
		Size: 2.8 MB (2827571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301444c62b8b685037f3be4e258418b417d7fac18825c9fb895d136eef1e7c35`  
		Last Modified: Tue, 09 Aug 2022 17:40:46 GMT  
		Size: 98.8 MB (98792046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
