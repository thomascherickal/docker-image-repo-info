## `openjdk:14-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:d2c01e677ab5307ee604c311676e673eed28755e89240dbedb7b7d5ab8413c87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:14-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:59c0f02be3023d82a56e0ca8e94ac9219d27d89ad708909481e88ee0d7e82f69
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.5 MB (256545138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88991ec1950573a258f3112fde83c067200c0c672744c4fee52335342e0c20e5`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Fri, 20 Dec 2019 01:46:43 GMT
ADD file:e662b0d428c91ed028fec1db2cccbeddea848eb36b32c8bfad324619b8e57d9f in / 
# Fri, 20 Dec 2019 01:46:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Dec 2019 02:05:13 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 20 Dec 2019 02:05:13 GMT
ENV LANG=en_US.UTF-8
# Fri, 20 Dec 2019 02:06:57 GMT
ENV JAVA_HOME=/usr/java/openjdk-14
# Fri, 20 Dec 2019 02:06:57 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 23:25:37 GMT
ENV JAVA_VERSION=14-ea+30
# Tue, 07 Jan 2020 23:25:38 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk14/30/GPL/openjdk-14-ea+30_linux-x64_bin.tar.gz
# Tue, 07 Jan 2020 23:25:38 GMT
ENV JAVA_SHA256=53a37319529ec0443d97e4fc138fc998fbfe7e32f3fc815c072d607fc31dd048
# Tue, 07 Jan 2020 23:26:29 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 07 Jan 2020 23:26:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:822ace0353cbeeb23baa4e10b00916d8aae76c005023f5807d16cd97e6339b9b`  
		Last Modified: Fri, 20 Dec 2019 01:48:50 GMT  
		Size: 42.7 MB (42725372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf4d0631bf4e4c98ff5629cdf7958d9db134bbabd5a323f89f8fd783ca4c524`  
		Last Modified: Fri, 20 Dec 2019 02:10:52 GMT  
		Size: 14.8 MB (14793038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80695a881860e965b77bb921640967260f520b13f9951668ec69db1d346d96e`  
		Last Modified: Tue, 07 Jan 2020 23:31:22 GMT  
		Size: 199.0 MB (199026728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
