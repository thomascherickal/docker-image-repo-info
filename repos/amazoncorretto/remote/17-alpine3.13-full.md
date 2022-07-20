## `amazoncorretto:17-alpine3.13-full`

```console
$ docker pull amazoncorretto@sha256:77d190b12c51a8d8eec38e918919b32a29dbacb6e907bcc1de01309e3718d223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.13-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c31603f83673b64a676e17f197bd3bbe82ae815eb56c3947aaef38876db63b20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194480949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5018176cd5c38835e00b09580652fa3d08afcf061886606795a2d25c2eb5f13e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:26 GMT
ADD file:e15461ac94648d9599df6304a53587fc8bfceaf6e111ee5917860e95ed9e751c in / 
# Tue, 19 Jul 2022 22:20:26 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 22:39:03 GMT
ARG version=17.0.4.8.1
# Tue, 19 Jul 2022 22:39:09 GMT
# ARGS: version=17.0.4.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 19 Jul 2022 22:39:09 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:39:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Jul 2022 22:39:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:627fad6f28f79c3907ad18a4399be4d810c0e1bb503fe3712217145c555b9d2f`  
		Last Modified: Tue, 19 Jul 2022 22:21:04 GMT  
		Size: 2.8 MB (2819330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503c3c8ff3bc2646651ef12f22f6c79ba4c5af964c10284c8aeed2cb29b2e35e`  
		Last Modified: Tue, 19 Jul 2022 22:47:06 GMT  
		Size: 191.7 MB (191661619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
