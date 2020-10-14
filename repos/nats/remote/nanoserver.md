## `nats:nanoserver`

```console
$ docker pull nats@sha256:9e85991423c317f2c30e8cb9c63c064a6afc5225fea43f0b6ac9f1957f24dc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:nanoserver` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
