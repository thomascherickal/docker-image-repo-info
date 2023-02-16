## `eclipse-temurin:19-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:b234888aee598b9c4ccbe87095ca3c32d8d873145a0255507fba023ff5b58bdb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `eclipse-temurin:19-windowsservercore` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:8cf9214ae45b8d65756449d18677f8bcee1704b63bee77f636cc751129e4f67e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2046666815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:219821098b90e750f409bf79b5a9334436a44a446d56087dcb6bc507b387fc2f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:20:54 GMT
ENV JAVA_VERSION=jdk-19.0.2+7
# Wed, 15 Feb 2023 23:22:27 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_x64_windows_hotspot_19.0.2_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_x64_windows_hotspot_19.0.2_7.msi ;     Write-Host ('Verifying sha256 (b2372bd728a5a708a4ce5ec6cc8b46489e5292051f4993568ec1d5f395f7e06e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b2372bd728a5a708a4ce5ec6cc8b46489e5292051f4993568ec1d5f395f7e06e') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-19' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 15 Feb 2023 23:23:12 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 15 Feb 2023 23:23:13 GMT
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
	-	`sha256:e7ddcbf6bbcb07dff97ccd7f5e5ed5a3400deeae9ea0f2bdcf7cc83bfe386f95`  
		Last Modified: Thu, 16 Feb 2023 07:17:32 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49feba9ed6dc221a63d5555baac9e70d14eadc4e81c9377c8e1aa9c6a96fd795`  
		Last Modified: Thu, 16 Feb 2023 07:18:12 GMT  
		Size: 366.7 MB (366733673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb14f3b578d8fa31df15b2a16a3b318f9b089fae95d1ed2fef01d8786c6e8bd6`  
		Last Modified: Thu, 16 Feb 2023 07:17:33 GMT  
		Size: 582.5 KB (582547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23971dbccd1309568754433b618b72931e96b5e2d37b8f2bba4e2c320edb6421`  
		Last Modified: Thu, 16 Feb 2023 07:17:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:19-windowsservercore` - windows version 10.0.17763.4010; amd64

```console
$ docker pull eclipse-temurin@sha256:f7024572e43f4a76cdb4ed3c1f66308e203557f3798f22229d8ce4e047fa9ab5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2333441017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd73742988a15dbd57f4142c1772e59fbc088cba79fd1887c09b1faaff321157`
-	Default Command: `["jshell"]`
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
# Wed, 15 Feb 2023 23:25:34 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_x64_windows_hotspot_19.0.2_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_x64_windows_hotspot_19.0.2_7.msi ;     Write-Host ('Verifying sha256 (b2372bd728a5a708a4ce5ec6cc8b46489e5292051f4993568ec1d5f395f7e06e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b2372bd728a5a708a4ce5ec6cc8b46489e5292051f4993568ec1d5f395f7e06e') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-19' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 15 Feb 2023 23:27:02 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 15 Feb 2023 23:27:03 GMT
CMD ["jshell"]
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
	-	`sha256:2031d11aeedba2f14078d42e6992f6e2caac7387d0bb8bf9f8922052b978cef4`  
		Last Modified: Thu, 16 Feb 2023 07:19:05 GMT  
		Size: 366.5 MB (366509755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43712a309419e5ce589cb0621e98747815c2de55ff3eb2edc2ede9b64bd821b8`  
		Last Modified: Thu, 16 Feb 2023 07:18:27 GMT  
		Size: 4.0 MB (3969250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc011be2347194bfcdbf46a25d124221124dec93263da7e297550a1a732baad`  
		Last Modified: Thu, 16 Feb 2023 07:18:23 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
