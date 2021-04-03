## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:795115a3a3b1b5f4cbc7c017ddd52f46848199b694cff7aafbcb0c7d464925e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
