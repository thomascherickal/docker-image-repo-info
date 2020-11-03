## `nats:nanoserver`

```console
$ docker pull nats@sha256:8df462388279bce76a4510fbb4c7af8520f71ecaf9a3778457c560f352a4708f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:nanoserver` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:3b8d6e0b7c69852dc23b45a96fef7142a8af7be8283756ed974c14f58e297291
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105252874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f5cc81e8fe22627c10e8a8c0e8c031081c1422b5fa7a1b9e0d6376a4df1600`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 03 Nov 2020 00:20:01 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Tue, 03 Nov 2020 00:20:02 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 03 Nov 2020 00:20:03 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:20:03 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 03 Nov 2020 00:20:04 GMT
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
	-	`sha256:a832cb76fb4365aa1898af094abe8919525832b45cff3095989d35854e50266d`  
		Last Modified: Tue, 03 Nov 2020 00:24:20 GMT  
		Size: 4.0 MB (4042693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30d14e997b712ff68025da8149e86cb4e26053db26f63189bb11be34d9c4570`  
		Last Modified: Tue, 03 Nov 2020 00:24:19 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a5619f119bfa73b08a55556d063fe6774602e03b6694241acdf544d8877e81`  
		Last Modified: Tue, 03 Nov 2020 00:24:18 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eaf47aa7239eb1b644c54510809eb1fac633a32d7472f6eaed679c9016fee0`  
		Last Modified: Tue, 03 Nov 2020 00:24:19 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2638a3eddd847bb58e977d2986b5fea2b056b1ce34e1c991ea6686a340621a69`  
		Last Modified: Tue, 03 Nov 2020 00:24:18 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
