## `python:windowsservercore`

```console
$ docker pull python@sha256:8490bef914f8eddd0b8ba338582afe17756d873b2f097e621ec1aab16d696cf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `python:windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull python@sha256:ef925c7fb65b2acdef4e7446b7d84f253cdc00f64ab4ec080e1fe23e3cf8f84b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2370375451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68a31079b588203253a01657807130f970b2979a9fc1dac027a5a536faabc7a3`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:33:23 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 10 Aug 2022 15:37:43 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 10 Aug 2022 15:38:54 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:38:55 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 10 Aug 2022 15:38:56 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Fri, 12 Aug 2022 00:30:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Fri, 12 Aug 2022 00:30:58 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Fri, 12 Aug 2022 00:31:56 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Fri, 12 Aug 2022 00:31:58 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8259ecb0e5034b8fa5de016424036c94452d1ef91533fce60f0ac1e95aa4e543`  
		Last Modified: Wed, 10 Aug 2022 12:45:16 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dede03b6cf0aec7439df57efcd398f9967add637f94e63eb43e1e9e1e2323a60`  
		Last Modified: Wed, 10 Aug 2022 15:50:24 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ccdf04430f2c9ba909e3ecc8a520ae02e9d36fb78de306993068ce59dd6b4c`  
		Last Modified: Wed, 10 Aug 2022 15:50:31 GMT  
		Size: 49.6 MB (49553247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93185a5fc9a930e59aaf22153314017bf82bb0a51e77c2b590a5592969b48f1`  
		Last Modified: Wed, 10 Aug 2022 15:50:23 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b0703e53d54c77a5305ff44350e53c43c6bd9d99605bd32bd1b4cc4de54cd`  
		Last Modified: Wed, 10 Aug 2022 15:50:21 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37df7be63976b68156936ad98fd46c1a74aa1b4a813b653b40c91b9aa5dcab85`  
		Last Modified: Fri, 12 Aug 2022 00:37:55 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133f165f3900a58d58ebb00bd951f79c1261660e0959d237b4a8d3633e9f1a1d`  
		Last Modified: Fri, 12 Aug 2022 00:37:55 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb39ce55617a54ca0bffb3a5c8d2f4b82da40a8386708f7f475e6601c9672aa1`  
		Last Modified: Fri, 12 Aug 2022 00:37:57 GMT  
		Size: 3.9 MB (3921761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c22819d30b9e5cb74956a42d1f05c2bd3a08c6dc8ddaeb7d644d437ffd971a`  
		Last Modified: Fri, 12 Aug 2022 00:37:55 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull python@sha256:06d388465c4abdab6b6f92bdfda8d0d14e39c5657e20844a3b377e94aa7bfe10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2730681732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c8130865bbdffd801f0372ab8d83901e6f0fcfd2b25e30f412afc39f4a1271d`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:36:06 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 10 Aug 2022 15:39:55 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 10 Aug 2022 15:41:41 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:41:42 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 10 Aug 2022 15:41:43 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Fri, 12 Aug 2022 00:32:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Fri, 12 Aug 2022 00:32:12 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Fri, 12 Aug 2022 00:33:40 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Fri, 12 Aug 2022 00:33:41 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf7f9036f4e1337b79593a7830e9e5acd24d9c6156b36496a8e99b3a91d360e`  
		Last Modified: Wed, 10 Aug 2022 12:45:50 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e9fa325068b52725e5880e9b6ea7a5926be35230135379e22fa1193cf20517`  
		Last Modified: Wed, 10 Aug 2022 15:50:48 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de411daf4552f64dd58db33d7b68a1b9da181d414b4b4af95640354cf2a2200`  
		Last Modified: Wed, 10 Aug 2022 15:50:55 GMT  
		Size: 49.3 MB (49295737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81cd5bf54ff368f1fc2aa9de0b044513eff8066faf2a6d6bb3157d3c8f9a93c`  
		Last Modified: Wed, 10 Aug 2022 15:50:48 GMT  
		Size: 1.5 KB (1451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a427aa98aa3dba16e42f234416b7788e34da19d02d524b492adb9aca1ac2b741`  
		Last Modified: Wed, 10 Aug 2022 15:50:46 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131afb9cb6efa95575ac7637c299cc6ad47293b73e8f78aec6c674cb92aca07f`  
		Last Modified: Fri, 12 Aug 2022 00:38:12 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200edbc18cc5c5ccc76828251e9b04447c4c7616488cdf745454065ad1474dc2`  
		Last Modified: Fri, 12 Aug 2022 00:38:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1a52ae26c2b9ed3830e13b2ef0bf581ea6f6d90a9612d47e1ab5ed2420226c`  
		Last Modified: Fri, 12 Aug 2022 00:38:13 GMT  
		Size: 3.7 MB (3661937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d39b51b49a3f739641903f0e9cb345a5413379c9b3f77a23e205b57b5d978c`  
		Last Modified: Fri, 12 Aug 2022 00:38:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
