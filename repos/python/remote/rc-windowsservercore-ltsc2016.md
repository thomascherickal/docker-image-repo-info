## `python:rc-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:f09e68dac3352065feae23c35cdbed2b7a930bf39053254d53d0e78ef593e35c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `python:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull python@sha256:5d6bb650f3daaaee022c3317f23b4f4ad1487a174574a50ff3555fa85abdc12f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5811323096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41eccf5eb74e647ae5fa864603b30eb806acf935b6ae4fdffd1a7155962fd0b`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 15:11:08 GMT
ENV PYTHON_VERSION=3.9.0b4
# Wed, 15 Jul 2020 15:11:08 GMT
ENV PYTHON_RELEASE=3.9.0
# Wed, 15 Jul 2020 15:13:48 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 15:13:49 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 15 Jul 2020 15:13:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 15 Jul 2020 15:13:52 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 15 Jul 2020 15:15:50 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 15:15:51 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c092947b8e0a4b70ab2057dc4d839f279a3e97a44dbbd5cf1c6d78625d19706`  
		Last Modified: Wed, 15 Jul 2020 16:06:01 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669e656db332a6c560d8c59bbca5791b50d32fd04f0d848f609cbfbc396103f0`  
		Last Modified: Wed, 15 Jul 2020 16:06:01 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd674549405d948fa68fc5e261c6a7cc39f0f2e978311a069b31768ea21af4c4`  
		Last Modified: Wed, 15 Jul 2020 16:06:11 GMT  
		Size: 58.5 MB (58460081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188c5057c62c16ebd66671dd8fa2f5ea5852b3ac6b228517ce774a4224a74c49`  
		Last Modified: Wed, 15 Jul 2020 16:05:58 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b16cbd68fc02b4db0e46b2447f1f621f9837378398fad7610d1722ac0450e46`  
		Last Modified: Wed, 15 Jul 2020 16:05:58 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a62f921fdee54169f1144917e019deee414b1099f9356de34c2928dfedc7cac`  
		Last Modified: Wed, 15 Jul 2020 16:05:58 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044a084f9497c4602cdb79648891a1ebdd0ce42cf242ebf248e198a68a217641`  
		Last Modified: Wed, 15 Jul 2020 16:06:03 GMT  
		Size: 15.4 MB (15392924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267879af5c9452d2fb96868b24e7aaa200c82fe7d9ac0d196f88461b6b85ecc3`  
		Last Modified: Wed, 15 Jul 2020 16:05:58 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
