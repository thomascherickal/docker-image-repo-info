## `hylang:python3.9-windowsservercore-1809`

```console
$ docker pull hylang@sha256:6d0bf98dd6278c5a1b0b1d1a1bd88665071909c1afadfea0c394923a9950ea07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `hylang:python3.9-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull hylang@sha256:f8732a0653397d5d9c542271b9aaa1af8b6ac1844ede516496a948fdb103bbe9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2731729047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e368b81cce8b165705148d0bf65885134ec959f52290e076edecf8c931d8a16d`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 20:39:30 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 12 Jul 2022 20:52:27 GMT
ENV PYTHON_VERSION=3.9.13
# Tue, 12 Jul 2022 20:54:18 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 12 Jul 2022 20:54:19 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 12 Jul 2022 20:54:20 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 26 Jul 2022 23:25:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/49ca29908cfd49683da12f2d5a4fa5689539f9d9/public/get-pip.py
# Tue, 26 Jul 2022 23:25:26 GMT
ENV PYTHON_GET_PIP_SHA256=d077d469ce4c0beaf9cc97b73f8164ad20e68e0519f14dd886ce35d053721501
# Tue, 26 Jul 2022 23:26:55 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 26 Jul 2022 23:26:56 GMT
CMD ["python"]
# Tue, 26 Jul 2022 23:47:56 GMT
ENV HY_VERSION=0.24.0
# Tue, 26 Jul 2022 23:47:57 GMT
ENV HYRULE_VERSION=0.2
# Tue, 26 Jul 2022 23:49:31 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Tue, 26 Jul 2022 23:49:32 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd0516027c8a6601673dcaf848c8e71716c45847d56a15ebcda3c01ac2dd776`  
		Last Modified: Tue, 12 Jul 2022 20:56:51 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6016b3af48a8456bbebdeffeaf9590ea53ebfba24d9916a763db8dc550c1e371`  
		Last Modified: Tue, 12 Jul 2022 20:58:17 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2294b8751bc38a213d4a5fd1d776d805502f6f5b46dd410ab745b2d71cf08242`  
		Last Modified: Tue, 12 Jul 2022 20:58:23 GMT  
		Size: 51.7 MB (51712205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35971f6d97fd50ee880fe6facd852e1218c20c581ccefded32ce49f5155d5c25`  
		Last Modified: Tue, 12 Jul 2022 20:58:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40b2ffb46593c3d4fcc90e28027209ecc9eb2fa4dd17cf72fcb6b763c271c42`  
		Last Modified: Tue, 12 Jul 2022 20:58:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79378d5f0ebc51de7d021aa25817b2c8adbb915638bc2903266b969eceacfd39`  
		Last Modified: Tue, 26 Jul 2022 23:29:10 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffdb8b5e69150047d475728eda40b9e92500ff87a2c42f11664714dd71f7a2c`  
		Last Modified: Tue, 26 Jul 2022 23:29:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa69d9912c0ff85e7aeb660ba000b21c91490cc9bb261b858886d2b6b51ff5e7`  
		Last Modified: Tue, 26 Jul 2022 23:29:11 GMT  
		Size: 3.5 MB (3528626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fd479abe14d645cdb077e42210d7b8c6f44657b2b4c24da86d3a74342db37d`  
		Last Modified: Tue, 26 Jul 2022 23:29:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84460057789b93bf7a187649b75e3c98812bbf855c28bacf43499b72d4f2cf6`  
		Last Modified: Wed, 27 Jul 2022 12:05:03 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f1cc76856d10dbbc3101cf0ad0133e091523b9d04bfb11fd078ca5717da93c`  
		Last Modified: Wed, 27 Jul 2022 12:05:03 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c21ff59e51c8f0282755f8f7bbe919e330d609b9ca0bb6c027f9dfa7a4f4c8c`  
		Last Modified: Wed, 27 Jul 2022 12:05:06 GMT  
		Size: 4.4 MB (4429372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5f7609dc85126f0888afd98d2d980acf41fcfb5502c2485ab639b7d936d5da`  
		Last Modified: Wed, 27 Jul 2022 12:05:04 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
