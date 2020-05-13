## `openjdk:8u252-jre-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:c17d25e3424556fdd9f5f997332b468ec0c4c815581da111c1d46710d49f9b28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `openjdk:8u252-jre-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull openjdk@sha256:facea7537745b0384975723cc225af0d2717d5637ffa66072ac6e1362423288f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1756414579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483953fdf9a7f9ce433281e791db4832d3f7765f158b97004310012f3102290d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:41:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 15:51:57 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 May 2020 15:52:19 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 13 May 2020 15:52:20 GMT
ENV JAVA_VERSION=8u252
# Wed, 13 May 2020 15:58:24 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Wed, 13 May 2020 15:58:25 GMT
ENV JAVA_URL_VERSION=8u252b09
# Wed, 13 May 2020 15:59:11 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77613e754ba9d62c0acd4ef271c4ee7d3af091b8c8b310afa404560a9d281f82`  
		Last Modified: Wed, 13 May 2020 13:00:20 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47082c93bcb98f4a5714b19c9bbcb17a08a2de52b0fe7176c6429cbfe07a3ec9`  
		Last Modified: Wed, 13 May 2020 16:28:10 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd679bcb211f1f18033a230fae912d8e5bc3ee0fee2547f3dc2eb3db6c78660`  
		Last Modified: Wed, 13 May 2020 16:28:08 GMT  
		Size: 344.8 KB (344794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce2e62e8bc5b09ad5c34abd52bfe2b4577a2ffa84df0e1f681b4a82e2546c61`  
		Last Modified: Wed, 13 May 2020 16:28:08 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dda76c4661995199cd6d22ec44123535c4c24e288656b69b5c23387ad9f4de3`  
		Last Modified: Wed, 13 May 2020 16:29:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3f65b5be6d87e2beaa1c93201b1e3bec03f41c3b95280f45bbce00c061de82`  
		Last Modified: Wed, 13 May 2020 16:29:42 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fe7555cbf4322fc6eac386acc0a6be4962c78ebda69ba9c9a80a276af5fb51`  
		Last Modified: Wed, 13 May 2020 16:29:48 GMT  
		Size: 37.7 MB (37731200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
