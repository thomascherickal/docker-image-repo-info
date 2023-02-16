## `eclipse-temurin:19-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:94d01c4a477dfc35b3826628dc9fc41d083a8cccfb8864b742e9973b75b8ba62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `eclipse-temurin:19-jre-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull eclipse-temurin@sha256:463dd9a38582c0dfee48dae286e77ed7f90cc974a0b20c9a6681aaedf61aff80
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2043973116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d31e193e2b4e7b7f602e17f66a937909a889478cff0eee84fde97c8adff4ee1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:23:26 GMT
ENV JAVA_VERSION=jdk-19.0.2+7
# Wed, 15 Feb 2023 23:31:49 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jre_x64_windows_hotspot_19.0.2_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jre_x64_windows_hotspot_19.0.2_7.msi ;     Write-Host ('Verifying sha256 (4ad4aae081243e6962eddd59c4fdfa33d1a3d79acb16d2700a40dc5d8e4861be) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '4ad4aae081243e6962eddd59c4fdfa33d1a3d79acb16d2700a40dc5d8e4861be') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-19' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 15 Feb 2023 23:33:12 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d564ad919e4881c69da9d5f1b42333a79fbfd414d0b2176c0dfe03bb953a70f`  
		Last Modified: Thu, 16 Feb 2023 07:18:23 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5582144d07937906aecca31bcdc595dbb5db534ca0423baddbc63f9f435831de`  
		Last Modified: Thu, 16 Feb 2023 07:20:34 GMT  
		Size: 77.7 MB (77668158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5224fc2a938b64af0ecfd1f85f9a2f868c577282099dbeb4b95c3ac0155e8fdd`  
		Last Modified: Thu, 16 Feb 2023 07:20:21 GMT  
		Size: 3.3 MB (3344239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
