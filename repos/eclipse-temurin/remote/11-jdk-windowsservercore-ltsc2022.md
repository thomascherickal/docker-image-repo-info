## `eclipse-temurin:11-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:1f550f60f76d6257ae375225aa97855cb71f71564a517090f61774b2571ec0fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `eclipse-temurin:11-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:27f20bf9727e7bafdc4d8a7f1078739930b0a93be10a7da5766b7093c3ef4779
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047239392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c24e5e81c86f0f4d206949adeb8f93ac685fc049912fd4e48d6e516f5df24b61`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 22:53:34 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Wed, 15 Feb 2023 22:55:04 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_windows_hotspot_11.0.18_10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_windows_hotspot_11.0.18_10.msi ;     Write-Host ('Verifying sha256 (71e84c14606d1478147b46c3687486af0b51886192ff3b6239e51c1af413c688) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '71e84c14606d1478147b46c3687486af0b51886192ff3b6239e51c1af413c688') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 15 Feb 2023 22:55:58 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 15 Feb 2023 22:55:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2242edd992fe2715e0e711282bbd2b026dd13edc61a122516cd40af2729058`  
		Last Modified: Thu, 16 Feb 2023 07:11:00 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f3bbf0748dc5083beed2c08739174ea3e96d13534f645535abe96b7dbaa84a`  
		Last Modified: Thu, 16 Feb 2023 07:11:38 GMT  
		Size: 367.3 MB (367305293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091848017696d23d3bdb19d5273036a7fae488ae5de6c205c169c4b0235d53e6`  
		Last Modified: Thu, 16 Feb 2023 07:11:01 GMT  
		Size: 583.5 KB (583492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa6fabbebcc81b7c9259f7e6270d190b75441cd082d278263cbb1a78a87c97`  
		Last Modified: Thu, 16 Feb 2023 07:11:00 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
