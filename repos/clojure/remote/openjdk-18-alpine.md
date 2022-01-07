## `clojure:openjdk-18-alpine`

```console
$ docker pull clojure@sha256:bb2e3efbfebd74d4c6900945640efbe4287714b346f3d5ca786e280a3b524fe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-18-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:0d3635a07260f275510345a21acc104ecae635cc9cd5975a5ab2ef02fb121e91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221402807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04bf7d8d80b77268691abd30cfc908c338ec041b2d7d2a07d9673eccfc7358d9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:45:32 GMT
RUN apk add --no-cache java-cacerts
# Tue, 30 Nov 2021 04:45:32 GMT
ENV JAVA_HOME=/opt/openjdk-18
# Tue, 30 Nov 2021 04:45:32 GMT
ENV PATH=/opt/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 04:45:32 GMT
ENV JAVA_VERSION=18-ea+11
# Tue, 30 Nov 2021 04:45:45 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/11/binaries/openjdk-18-ea+11_linux-x64-musl_bin.tar.gz'; 			downloadSha256='86fad9069587a5e9dd003e7354a69b2f720a05c12706d2f2345a0c8d90e56c47'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 30 Nov 2021 04:45:46 GMT
CMD ["jshell"]
# Fri, 07 Jan 2022 20:26:38 GMT
ENV CLOJURE_VERSION=1.10.3.1058
# Fri, 07 Jan 2022 20:26:39 GMT
WORKDIR /tmp
# Fri, 07 Jan 2022 20:26:45 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "980168025a3827bd7ed9d5ab1681ce29808ac8e6cbced3ab6683db8b365b54df *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Fri, 07 Jan 2022 20:26:45 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 07 Jan 2022 20:26:45 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 07 Jan 2022 20:26:46 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 07 Jan 2022 20:26:46 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae5de21b2241a24b653013bdda639de16f984789b28bbcb7108523b460d1e4`  
		Last Modified: Tue, 30 Nov 2021 04:55:25 GMT  
		Size: 932.2 KB (932205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3048de22201addf91c8f64e5382a33c2791d3c21a0906eefce3c4cb08d875839`  
		Last Modified: Tue, 30 Nov 2021 04:55:48 GMT  
		Size: 188.7 MB (188699653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a04cd86f84a2307886d5f0920dad95883ebc8276872e1deb3dcc918bdb6789`  
		Last Modified: Fri, 07 Jan 2022 20:36:05 GMT  
		Size: 29.0 MB (28951513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4b8d505aac90d14c421ff8c0be634f2295d83ca60da1a3438bbb3d40db4347`  
		Last Modified: Fri, 07 Jan 2022 20:36:03 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531dae15fd3d68a57db82059806bcb6760eb604cc9991fbe91ed4b79be843448`  
		Last Modified: Fri, 07 Jan 2022 20:36:03 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
