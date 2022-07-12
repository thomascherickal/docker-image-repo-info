## `hylang:python3.9-windowsservercore-1809`

```console
$ docker pull hylang@sha256:3bd7f7811fac712147077744b13462b97e22770b78d99fd1e456f332c7bb8a3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `hylang:python3.9-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull hylang@sha256:a10822c6379e8034600e7a7aa03d28c52b48a2c0477abca9feae686860512e75
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2731661897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7b7d1017b5394f81f8047dd9c59b20446b72ef38d448f72ee71fb031ea884b2`
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
# Tue, 12 Jul 2022 20:54:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Tue, 12 Jul 2022 20:54:22 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Tue, 12 Jul 2022 20:55:46 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 12 Jul 2022 20:55:47 GMT
CMD ["python"]
# Tue, 12 Jul 2022 21:15:48 GMT
ENV HY_VERSION=0.24.0
# Tue, 12 Jul 2022 21:15:49 GMT
ENV HYRULE_VERSION=0.2
# Tue, 12 Jul 2022 21:17:29 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Tue, 12 Jul 2022 21:17:31 GMT
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
	-	`sha256:9ab65bb13129dbb4aace2b5bd1e3bbb7a773f3a4bbfbd299958f4001e56e3c57`  
		Last Modified: Tue, 12 Jul 2022 20:58:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec529924819fd669bbbce9b3b2a17709ba7974eb5c719cddd60e50836dbc6946`  
		Last Modified: Tue, 12 Jul 2022 20:58:14 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478155fc0d3a94d1be4e9e359b07209970bb3c2846770a719404f7e499849340`  
		Last Modified: Tue, 12 Jul 2022 20:58:15 GMT  
		Size: 3.5 MB (3481700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50479e14532aa6758aa8567d6e670253b811f8a7e183e40fbe24b5ee696fa861`  
		Last Modified: Tue, 12 Jul 2022 20:58:14 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb029016e634ffbeb78e28ca19b7f9ce73e91aa0afce9f1ebec32f3ffe297a3`  
		Last Modified: Tue, 12 Jul 2022 21:19:42 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653bbdb4ee485475e2e6dc31b52b8092025d8f062f55e7e48e26705190ec4e8f`  
		Last Modified: Tue, 12 Jul 2022 21:19:42 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdc7b0e55fa783f5fc52ee2089042a5a3573267e0a623df4262cf9079764081`  
		Last Modified: Tue, 12 Jul 2022 21:19:44 GMT  
		Size: 4.4 MB (4408901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23fffa703c2c4b6d42a35327f09a6d218854b1f57725d6d0578909c5abc1cb1`  
		Last Modified: Tue, 12 Jul 2022 21:19:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
