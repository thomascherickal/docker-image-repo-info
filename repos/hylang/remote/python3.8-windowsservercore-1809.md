## `hylang:python3.8-windowsservercore-1809`

```console
$ docker pull hylang@sha256:fe4464f40f2e7cb1ece2beff41bf57fb6f44fcc2118f5935f54af1c061590879
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `hylang:python3.8-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull hylang@sha256:95706f212ff4d4b2d9843ac01670556e5fcdc48a197db6ed652821978c3b6a97
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2383180993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe93b6b8aec72e2615437f55cd02badd21a624e7ef89e3fa421ebb99112f8c4`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 15:24:00 GMT
ENV PYTHON_VERSION=3.8.4
# Wed, 15 Jul 2020 15:24:01 GMT
ENV PYTHON_RELEASE=3.8.4
# Wed, 15 Jul 2020 15:25:50 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 15:25:52 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Wed, 15 Jul 2020 15:25:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Wed, 15 Jul 2020 15:25:54 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Wed, 15 Jul 2020 15:26:51 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 15:26:52 GMT
CMD ["python"]
# Thu, 16 Jul 2020 22:15:53 GMT
ENV HY_VERSION=0.19.0
# Thu, 16 Jul 2020 22:17:04 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Thu, 16 Jul 2020 22:17:05 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8800378e96ce1ab9252f1f4fb590257ec21a4d48ed4fb56b393294a47758122b`  
		Last Modified: Wed, 15 Jul 2020 16:07:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2958cc8a673c4d972bcafb99a17aa48d688863e59ec7fbfeadc36b7f91af2b8f`  
		Last Modified: Wed, 15 Jul 2020 16:07:22 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335ac9a3a1b324bbc3eb8d0f1fac324e532f50ebb64ea47691316fc0c3817e59`  
		Last Modified: Wed, 15 Jul 2020 16:07:31 GMT  
		Size: 57.2 MB (57216785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857729ab7ecbceec828ad47d393c4e3d3223b1bc9e3b7318b7f3edfe0220268a`  
		Last Modified: Wed, 15 Jul 2020 16:07:19 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b78691534b377277f4f91612dc3dd4604cb1dbc61bdc7f034d12b1aab05f70`  
		Last Modified: Wed, 15 Jul 2020 16:07:19 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b634d7f72775adc2a060388c20f9d43e5276436f8018a5215ac2df180fc5c39d`  
		Last Modified: Wed, 15 Jul 2020 16:07:20 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944cc92f43b30df0723925b35d954b45739f70f5ac5b5e396721329eb04efda6`  
		Last Modified: Wed, 15 Jul 2020 16:07:22 GMT  
		Size: 10.2 MB (10233963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c189e6e6d72acbb4e2af2ca6d83b79d461462930fe01d9fe6012c8b30bab08`  
		Last Modified: Wed, 15 Jul 2020 16:07:19 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e058ff2aa117f13cf91c3b93365df8c1149f32643e03a46ecadba61a193910`  
		Last Modified: Thu, 16 Jul 2020 22:43:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571d16778e187a93951ea8ac0cc819652f6cd11c57969c7ff3d62036e2f3b2a4`  
		Last Modified: Thu, 16 Jul 2020 22:43:43 GMT  
		Size: 5.5 MB (5527693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e70035401f3dd6204b8335bd2d32705926cbfb68ab0a9435a0069f7464aced6`  
		Last Modified: Thu, 16 Jul 2020 22:43:41 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
