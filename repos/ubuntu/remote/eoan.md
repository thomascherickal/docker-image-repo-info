## `ubuntu:eoan`

```console
$ docker pull ubuntu@sha256:bd5f4f235eb31768b2c5caf1988bbdc182d4fc3cb6ee4aca6c6d74613f256140
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:eoan` - linux; amd64

```console
$ docker pull ubuntu@sha256:9e9387cd5380eb96ace218a2f85ed25ac75563cd170f91852a73aefda6fa7834
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28307233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcbcfdcd50bb2843429176e15f5d3a851c899311f89ec607336c84f74809d731`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:56 GMT
ADD file:8d7cb00bd95f07ddb881fb10a625cff9db36796913fcf8e5dc6a1ef47a74ae45 in / 
# Thu, 16 Jan 2020 01:20:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:57 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:58 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:93956c6f8d9ea3e705e03e79d66a5c2acc9a4ac10ed6fb5c6cf654ba9c297df5`  
		Last Modified: Thu, 16 Jan 2020 01:22:09 GMT  
		Size: 28.3 MB (28275627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bddb84d1c5e5324fcc5efc270c7e081cc9966c125ac56c900dbca6b7a2fe06`  
		Last Modified: Thu, 16 Jan 2020 01:22:03 GMT  
		Size: 30.6 KB (30599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15fa850485767a7b5ef5a59fcd74b158b9a7faffef6254d4cf0c8d86d347e1ec`  
		Last Modified: Thu, 16 Jan 2020 01:22:03 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa40341c4fa46ae7bf3b1915da155fd05e53bcc06cfea0606a055b781dd14cc`  
		Last Modified: Thu, 16 Jan 2020 01:22:04 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:eoan` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d6e2cd39780f62a6af4ec24526fe159c739bef54fda7556b2bb273c384cf1fc4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23765824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63b834120392a47ba3b0a1c83bfb65cdbb527952c7dfa00734ab3677448e5ffe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:00:55 GMT
ADD file:2cc3ace63c3a3465d29e80a8566ab019f1fc722303b3f1be293030e2b0636c6c in / 
# Thu, 16 Jan 2020 01:01:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:01:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:01:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:01:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e94dc85965ded3acdf52aebf01a2a73fc92152fd21ae4aec73b18a2183ee3309`  
		Last Modified: Thu, 16 Jan 2020 01:04:57 GMT  
		Size: 23.7 MB (23734196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aac08e7e51e343024c582bf5d21c15ca3cad9f172262e28747943f7d3bab27b`  
		Last Modified: Thu, 16 Jan 2020 01:04:50 GMT  
		Size: 30.6 KB (30595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f018464aaad5eedcc7544c3ae9fa190ec7e129b9036cf0abe7db34021d0d71ef`  
		Last Modified: Thu, 16 Jan 2020 01:04:50 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707e607c278678f46214bf5eeae10043d39c1ce0329f2400c15bfd3827da0c85`  
		Last Modified: Thu, 16 Jan 2020 01:04:50 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:eoan` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:01769b437bc4e39929a3385ecb731fa513ad4f4c57cd3a1bb448912131d1a37f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26900094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd5d1582231892aa0471d5d274fa0df70fd956fed83cdee520fa15d21ceb4809`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:41:43 GMT
ADD file:3d26262e2d5ee80a9143203225aae1bff16d03a5175b1a2acdf7f577ffcadfcd in / 
# Thu, 16 Jan 2020 00:41:47 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:41:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:41:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:41:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b22be037f3b544f1ae0dacc6615fea807d306b4777ced7d365bece795d669468`  
		Last Modified: Thu, 16 Jan 2020 00:43:56 GMT  
		Size: 26.9 MB (26868630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9afd7353e0ca0552f898e42a65f120a9986a70dd5c09aae3468423c8a19e0b`  
		Last Modified: Thu, 16 Jan 2020 00:43:49 GMT  
		Size: 30.4 KB (30429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e5cabe9f6d8e4ea8380f04549c677f206ce39c390a0f0e86db9ba15e5d3883`  
		Last Modified: Thu, 16 Jan 2020 00:43:49 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730e3e1ca209c1b8022ec3dd7fb23f5e6f1b4b3ed5f4c76d8edbbf71ea3a8df8`  
		Last Modified: Thu, 16 Jan 2020 00:43:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:eoan` - linux; 386

```console
$ docker pull ubuntu@sha256:1e183653caccac1ed6b8caf714f827cbbe562f1be706db5e9853ece02df16798
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29073060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021a9fd9b59f5a9daf9c3dc558e4111fccbb4d794aaba5289a4330390dcf23fd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:39:21 GMT
ADD file:4c13e98f6fc840e5da5cb0f7785a8e82a92e72983a5cd05d0e5bddab446fee18 in / 
# Thu, 16 Jan 2020 00:39:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:39:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:39:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:39:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c291135c9b01620912513c1f0d8a0504da7354edc25070352cc18166738a84a3`  
		Last Modified: Thu, 16 Jan 2020 00:40:22 GMT  
		Size: 29.0 MB (29041359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:294dba4d145edfc7c6ca873f6b60ed7ae65c2c3970ba7caca8cef7c8fefe0b33`  
		Last Modified: Thu, 16 Jan 2020 00:40:15 GMT  
		Size: 30.7 KB (30693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a30417049082ff7a0aa58802fb490045b812cc7756938f3d86b99233e174f97`  
		Last Modified: Thu, 16 Jan 2020 00:40:15 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d0f1731d2bb5ffe106dc27137344e67f68f8667937027f4ba0d0d439eab39f`  
		Last Modified: Thu, 16 Jan 2020 00:40:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:eoan` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8d5f4274d82cf7ea75607d40391a953c14ff7b318e73a1d261f0a813a3977532
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33016808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4231684f67307d73a8be755bc88813f49637093812815f873e04252689a8f66`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:18:00 GMT
ADD file:338c6abf7fe08d965aacb0a08af1dd7186ed50c649b619983808f3df47c6bf0f in / 
# Thu, 16 Jan 2020 01:18:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:18:11 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:18:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:18:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:05c4f0b98df2d6829702866175d8b93505274d8c85477fe5413a05ea15ed6ad5`  
		Last Modified: Thu, 16 Jan 2020 01:20:30 GMT  
		Size: 33.0 MB (32985315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351b0559d8b1705ee53de2711f8fb5c8ad89ad09446fe96ee727171a44dab153`  
		Last Modified: Thu, 16 Jan 2020 01:20:23 GMT  
		Size: 30.5 KB (30463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f598a5290abd1ec449bdff3100dd86fc4391102151d376a276b4ed6629d587e`  
		Last Modified: Thu, 16 Jan 2020 01:20:23 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8919f20b1f503a3f264567118ddaeb63d410839e33a9fe4bfc17d6d8b2fd44c4`  
		Last Modified: Thu, 16 Jan 2020 01:20:23 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:eoan` - linux; s390x

```console
$ docker pull ubuntu@sha256:171de17887b1dc04b94256097c66b52cc743af8ca4901ccc49d26e8d2115aea7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26714648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b7b3bcaaef2f534139fc282e11f061f929d2a038793d1e1b5a266714049137e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:45:39 GMT
ADD file:d11f2d3df95bd823f561f866f276b3e1133a10b4fd24cd0af59926336d9c7fdc in / 
# Thu, 16 Jan 2020 00:45:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:45:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:45:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:45:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9f8ad320e3910721bade3f69e3e74f5511ad7245eafdd183ab893dbae79842dd`  
		Last Modified: Thu, 16 Jan 2020 00:46:37 GMT  
		Size: 26.7 MB (26682542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16061b26415dae4023599d79fe632126958d9fff628811e9eb72e6adc656eb3`  
		Last Modified: Thu, 16 Jan 2020 00:46:29 GMT  
		Size: 31.1 KB (31101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b599496909204045d2cdfb755a0ccd4b24ccb49453c1eee59a0d492116d92191`  
		Last Modified: Thu, 16 Jan 2020 00:46:29 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a550ce4958735714f310a9a407b7b63e71e5aefda4ad33e3dc544c5905daa`  
		Last Modified: Thu, 16 Jan 2020 00:46:29 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
