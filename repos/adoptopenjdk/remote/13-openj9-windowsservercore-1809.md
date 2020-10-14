## `adoptopenjdk:13-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:b09b5db7b1c2142c112a649fb4bfdfc4f20e90e61bad14d5a5bd22b0e84f725e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `adoptopenjdk:13-openj9-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:c3321b6d10406886f007c3f77c495ea46ec8110e306f09215c6eb7393b4d0255
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2773853440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e9a01bffb18a2061cbb3f3bd24fd50f7918250104702639d96412daeb45d8a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 20:02:07 GMT
ENV JAVA_VERSION=jdk-13.0.2+8_openj9-0.18.0
# Wed, 14 Oct 2020 20:04:43 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8_openj9-0.18.0/OpenJDK13U-jdk_x64_windows_openj9_13.0.2_8_openj9-0.18.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8_openj9-0.18.0/OpenJDK13U-jdk_x64_windows_openj9_13.0.2_8_openj9-0.18.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (b96fdec7f69ff3a36ed3b03774d7ad3fc9385c80de7d8df9c4e6b4fbec70dcd9) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b96fdec7f69ff3a36ed3b03774d7ad3fc9385c80de7d8df9c4e6b4fbec70dcd9') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Wed, 14 Oct 2020 20:04:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 14 Oct 2020 20:04:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105c0ba9b4ed053a20b7315b056334ef93dd8241059b48dd3410b8d674c038d2`  
		Last Modified: Wed, 14 Oct 2020 20:43:36 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76de197e14f7a8efc6fa391f58ab9de356cb58b3f3a2c062771dfd145ec93697`  
		Last Modified: Wed, 14 Oct 2020 20:44:09 GMT  
		Size: 399.8 MB (399758757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883f59e0e0b392eebb9d5ca5b56919eb0193d4822eb9f4897ff18d9c145531ca`  
		Last Modified: Wed, 14 Oct 2020 20:43:36 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882464ab9d9b620c1a29d8421379523ac5db547df04c0606a330d45af94b4b9b`  
		Last Modified: Wed, 14 Oct 2020 20:43:36 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
