## `clojure:temurin-11-tools-deps-1.11.1.1413-bullseye-slim`

```console
$ docker pull clojure@sha256:0656859cfaaf2ff20e7930f3044effbdda6817183fccf262eb4aaaeae71e4e38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1413-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:4f079a04e20de6eabff5b4267ef4a20c10c52f8b9e099dc058b0168904ba7403
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.7 MB (237738820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5be5eeab4abd2cc264a165647245549a01f295706cf21e0f210e08e526be72`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 31 Aug 2023 20:50:14 GMT
COPY dir:9c2351d5d5cdf669213a7cfcfa52bd6bd8e9fc36b0a8e93328276d7280e1bab3 in /opt/java/openjdk 
# Thu, 31 Aug 2023 23:22:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 23:29:53 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Thu, 31 Aug 2023 23:29:53 GMT
WORKDIR /tmp
# Thu, 31 Aug 2023 23:30:09 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 31 Aug 2023 23:30:10 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 31 Aug 2023 23:30:10 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d08bb3cc4c5f5565aedec30d167dd9f4534631431ccf2ef52db66770488b231`  
		Last Modified: Thu, 31 Aug 2023 20:54:04 GMT  
		Size: 144.8 MB (144826071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb17b28ef2a445e989d8bfd3d09186c77c4a76fba4671ab584bc49ff0ecc194`  
		Last Modified: Thu, 31 Aug 2023 23:43:17 GMT  
		Size: 61.5 MB (61494454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ca48bb3a573b38301600bfa5b4a6524749e4f29f3e6683299e20119b48934e`  
		Last Modified: Thu, 31 Aug 2023 23:43:10 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-1.11.1.1413-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:be441ff1da1d266eeac159f9b809d4eaa6a5c786bf761f5e03da7de871d83d51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233245223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fd9a834599802d32ac18021cc217f705f5ad9eb48ce3d07869d7734efd8230a`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 01:44:25 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Sat, 02 Sep 2023 01:44:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 01:46:52 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Sat, 02 Sep 2023 01:46:52 GMT
WORKDIR /tmp
# Sat, 02 Sep 2023 01:47:05 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 02 Sep 2023 01:47:06 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Sat, 02 Sep 2023 01:47:06 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b924b77d195ee682d4adf6c744cba3a607633e56b93e8e8d9161e1a29b17fc4c`  
		Last Modified: Sat, 02 Sep 2023 01:53:29 GMT  
		Size: 141.6 MB (141570383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595d2f1e1357fd877b171e9125bca1ac09221050f4a0b9a9123e1401dc8649d0`  
		Last Modified: Sat, 02 Sep 2023 01:54:49 GMT  
		Size: 61.6 MB (61611407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2a24af2e5c533a1700c34c329257d1ae2de7a72abe0c7f8f1abbbfaa8fc103`  
		Last Modified: Sat, 02 Sep 2023 01:54:40 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
