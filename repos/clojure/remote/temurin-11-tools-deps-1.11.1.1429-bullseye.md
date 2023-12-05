## `clojure:temurin-11-tools-deps-1.11.1.1429-bullseye`

```console
$ docker pull clojure@sha256:0a54eaa2c19cb51e93480b91fc95947fa49a36e02ad3f42aa1b2303a723d0786
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-11-tools-deps-1.11.1.1429-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:f834f1d822a22413f68fcc33a8fcae6cec509d33af0474eea6922e3f818a70f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.4 MB (272421309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:789decfbd70eca0c760db773d262173a9dbebd548bd037e6897d39a9094e9419`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 09:55:14 GMT
COPY dir:d20aeb749bf0b3fe533952f7903b6aa08724fe8bf03e369130d4e2a6ff71bd3f in /opt/java/openjdk 
# Sat, 02 Dec 2023 09:55:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 18:26:49 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:26:49 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:27:06 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 05 Dec 2023 18:27:07 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:27:07 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100270be7c7a032e8711a8951a07234acf8e56368673f84b3d9df6b333e239f7`  
		Last Modified: Sat, 02 Dec 2023 10:14:22 GMT  
		Size: 145.3 MB (145266419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ea94ee3ca23496b386c4dde587562f1cc1b78e2e5a04cd21aeede02670b7fb`  
		Last Modified: Tue, 05 Dec 2023 18:38:58 GMT  
		Size: 72.1 MB (72096369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853ce6416bc79819e12b0c84de567ef6db2f2eb8e24e2175442e050b48da651e`  
		Last Modified: Tue, 05 Dec 2023 18:38:50 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
