## `eclipse-temurin:8u382-b05-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:09c59fc874eeb523e183b5308d951020dd05c2aad59b842d521947a19a2f7d94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:8u382-b05-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:f8d8ca327306241f7920198c9dbdf3ab3c6199d02ba5eaf736beb20af99b4d18
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1932344158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762cb1f04757b12c200de72b36f7c50f2d1cfcab10a9f42683fc524e46b88ea6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 01:35:11 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 11 Oct 2023 01:40:58 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_windows_hotspot_8u382b05.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_windows_hotspot_8u382b05.msi ;     Write-Host ('Verifying sha256 (e165227737bcc4d5c8c311cb36f8da148c552316d902f86d63c348b8ed0ca427) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e165227737bcc4d5c8c311cb36f8da148c552316d902f86d63c348b8ed0ca427') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 Oct 2023 01:41:22 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3580bf8e73d63dc0065816c423b493a740ba4c4d7918e3778d6c12b899455f`  
		Last Modified: Wed, 11 Oct 2023 07:19:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d287d04d5c0f639d61ebbe844a9e2de3c8eb774f7ee98f982d51c1eceb1f85d`  
		Last Modified: Wed, 11 Oct 2023 07:20:48 GMT  
		Size: 72.2 MB (72219260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d9f6bfaf82859df33f7c516c414ae61a4b4526cb56e8c8daf1536e77f3a33f`  
		Last Modified: Wed, 11 Oct 2023 07:20:41 GMT  
		Size: 279.2 KB (279170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
