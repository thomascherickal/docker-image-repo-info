## `openjdk:14-ea-15-jdk-alpine3.10`

```console
$ docker pull openjdk@sha256:cce1b63801f5e83dd11f0e5d0c59d76d39fb243239a07b2ce39fcd04172698fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:14-ea-15-jdk-alpine3.10` - linux; amd64

```console
$ docker pull openjdk@sha256:4830e128a03c6fca8e9d31325321c6f8cb851aaa70664c6a7027b68f218c1d66
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.5 MB (201514011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f131b41d707eaa7637e0dd09b32249bf9acf1b38c876a94c291dcd0c55481c85`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:15:00 GMT
ENV JAVA_HOME=/opt/openjdk-14
# Thu, 23 Jan 2020 22:15:00 GMT
ENV PATH=/opt/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jan 2020 22:15:00 GMT
ENV JAVA_VERSION=14-ea+15
# Thu, 23 Jan 2020 22:15:00 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/alpine/15/binaries/openjdk-14-ea+15_linux-x64-musl_bin.tar.gz
# Thu, 23 Jan 2020 22:15:01 GMT
ENV JAVA_SHA256=76091da1b6ed29788f0cf85454d23900a4134286e5feb571247e5861f618d3cd
# Thu, 23 Jan 2020 22:16:42 GMT
RUN set -eux; 		wget -O /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		java -Xshare:dump; 		java --version; 	javac --version
# Thu, 23 Jan 2020 22:16:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7429ae8c261d6aa4d644ad3ea6a358cb2363e002bc4b2ca644cf5968e1ed3eb`  
		Last Modified: Thu, 23 Jan 2020 22:19:12 GMT  
		Size: 198.7 MB (198727049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
