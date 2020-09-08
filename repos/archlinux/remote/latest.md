## `archlinux:latest`

```console
$ docker pull archlinux@sha256:55d38aa4a7da0af27d3a949a551e81fdb30f26fe241135e2024711fd2a5676d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:7d1c7dd23c246895a34d6e8aa31eb29be573de2ce39b3e88315068e6d6cb5337
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131971290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90aeadc1688f28293eef65aee7ab4c080d3541b609c8c964261d734d0f5899e8`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 08 Sep 2020 19:20:30 GMT
ADD file:c1f0d6d9a87041de13180ef4b247a2410fc7950cb57f9f7f88dd382610722817 in / 
# Tue, 08 Sep 2020 19:20:33 GMT
RUN ldconfig && update-ca-trust && locale-gen
# Tue, 08 Sep 2020 19:20:34 GMT
RUN sh -c 'ls usr/lib/sysusers.d/*.conf | /usr/share/libalpm/scripts/systemd-hook sysusers '
# Tue, 08 Sep 2020 19:20:35 GMT
RUN ln -s /usr/lib/os-release /etc/os-release
# Tue, 08 Sep 2020 19:20:47 GMT
RUN pacman-key --init && pacman-key --populate archlinux
# Tue, 08 Sep 2020 19:20:48 GMT
RUN rm -rf etc/pacman.d/gnupg/{openpgp-revocs.d/,private-keys-v1.d/,pugring.gpg~,gnupg.S.}*
# Tue, 08 Sep 2020 19:20:48 GMT
ENV LANG=en_US.UTF-8
# Tue, 08 Sep 2020 19:20:48 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:cb935d5e749430e85932672b87cad9b38f00b683af62df0c8c08b6694db381e7`  
		Last Modified: Tue, 08 Sep 2020 19:21:25 GMT  
		Size: 128.5 MB (128527080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db807cf654f2da322070a102ae8961d16d053b449ddb5df5165d15bc095b5b3`  
		Last Modified: Tue, 08 Sep 2020 19:21:01 GMT  
		Size: 1.6 MB (1584523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1144bdd5f5c70a613efb5aac01b67e0959700c6ae58eeef4a8f31570117179`  
		Last Modified: Tue, 08 Sep 2020 19:21:00 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e029eb9f912a385b2c6461047f91077cc496669fabf8148b22f583fa6085c649`  
		Last Modified: Tue, 08 Sep 2020 19:21:01 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a944e1bfce9dd66d6854153bb8958ff3b5840d2a5099a67783a1e61dbe3673d`  
		Last Modified: Tue, 08 Sep 2020 19:21:01 GMT  
		Size: 1.9 MB (1858123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac07c34e00d18dd43c933f2e65099daf53bf5d23a1a730b58ad4e8e75c35d1e1`  
		Last Modified: Tue, 08 Sep 2020 19:21:01 GMT  
		Size: 299.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
