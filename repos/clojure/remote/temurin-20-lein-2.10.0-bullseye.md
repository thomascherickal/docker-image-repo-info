## `clojure:temurin-20-lein-2.10.0-bullseye`

```console
$ docker pull clojure@sha256:fba8223a680e2336084a887893ace467a8a28bd5375b69b1a54966b2fb65a481
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-lein-2.10.0-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:4fdd61dbad6193f6607d56b887f5af5aaac18b2814252f77c31d40ae9e47e508
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.1 MB (276113946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c42d7b5f7130ff5a835a84eba4b037002ec993828e8f06021be87d60a838911`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:18:50 GMT
COPY dir:0f9b663d61413099f20817ab55258941c09987290b8ce360d0fb2fab00ddddda in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:18:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:18:52 GMT
ENV LEIN_VERSION=2.10.0
# Wed, 12 Apr 2023 08:18:52 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 08:18:52 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:19:07 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 12 Apr 2023 08:19:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 08:19:07 GMT
ENV LEIN_ROOT=1
# Wed, 12 Apr 2023 08:19:10 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 12 Apr 2023 08:19:10 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 08:19:10 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 08:19:10 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb7d4bc5e99617b9205b6de7fb6d4899b028181001a97de7705ce560e55a602`  
		Last Modified: Wed, 12 Apr 2023 08:26:22 GMT  
		Size: 202.8 MB (202800557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00aaa28bede4a8d7640145c0c3c14b398d976a9376bb7ae6712d2e27a5be04e2`  
		Last Modified: Wed, 12 Apr 2023 08:26:09 GMT  
		Size: 13.9 MB (13860979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7d4f1e6aea02c5350271fa5101599df00a03ae8112a91a9a523abcd1d082b5`  
		Last Modified: Wed, 12 Apr 2023 08:26:08 GMT  
		Size: 4.4 MB (4399278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bce20f223033dab729ef85e3cfa7445b2db0c20239a26aa68dbb0be76444846`  
		Last Modified: Wed, 12 Apr 2023 08:26:08 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-lein-2.10.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:05dfed198737a8e095bfca7160ab2cf53990bc66d8fa897d488516f180a473a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.1 MB (273114300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cfad60bbc954e732278b25ed44c7591492cca4fea5b1c75e144e88b73e8c0c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:25:31 GMT
COPY dir:66b65f1974fed4b5bc3675e6b378c93a3ba9feeabfec7eeabd6d1d0b07fd5fa4 in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:25:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:25:36 GMT
ENV LEIN_VERSION=2.10.0
# Wed, 12 Apr 2023 01:25:36 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 01:25:36 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:25:52 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 12 Apr 2023 01:25:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 01:25:52 GMT
ENV LEIN_ROOT=1
# Wed, 12 Apr 2023 01:25:54 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 12 Apr 2023 01:25:54 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 01:25:55 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 01:25:55 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc51dd626337cedfa8259e3da03cef96eece3f3118695f388ae26fd81e82bd`  
		Last Modified: Wed, 12 Apr 2023 01:32:34 GMT  
		Size: 201.2 MB (201160086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0c8848f552f1b3e2213b9d394ca2eb04751b274f4060177b7e5b0446c03bcb`  
		Last Modified: Wed, 12 Apr 2023 01:32:23 GMT  
		Size: 13.8 MB (13849042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e64ad53e7fdd556dcd82733cf2b80f4b807e9f2c99b13137a96396759f7ff5`  
		Last Modified: Wed, 12 Apr 2023 01:32:22 GMT  
		Size: 4.4 MB (4399245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f84672af51b3da36d091e93edf10f8c6f3772c152a5714abade377bbf4874e`  
		Last Modified: Wed, 12 Apr 2023 01:32:22 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
