1. About

This plugin is developed to be used in Saleae Logic Analyzer application. It implements
ISO 7816-3 contact protocol decoding. In current release the following features are
available:
	* initial ETU recovery using clock signal
	* cold / warm reset
	* full ISO compliant ATR parsing (negotiable and specific mode supported)
	* PPS handling
	* T1 frames decoding - I/S/R
	* bytes and frames visialization in Saleae UI
	* suspend time resistant (no clock)

2. Documentation

The basic documentation is available from GitHub [doc folder!](doc/)

3. Releases

2017.11.04 - v0.9.3:
	* Mac version available
	* first release candidate for 1.0
	
2017.11.03 - v0.9.2:
	* bit-decoder rewritten
	* better support for RESET detection

2017.10.31 - v0.9.0.1:
	* ISO 7816 state machine to parse ATR, optional PPS and T1 transmission
	* full 7816 compliant ATR parser, including negotiable and specific mode detection
	* T1 frame parser with I/S/R block decoder
	* checksum validation - LRC
	
4. How to build it

There are project files available for:
	* XCode
	* Visual Studio 2017

This build assumes that Saleae SDK is available on the same lavel as project folder:
	* On Windows:
		[projects]\
				  \Saleae7816
			      \sdk\include
			      \sdk\lib
			
	* On Mac:
		[projects]/
				  /Saleae7816
				  /AnalyzerSDK/lib/
				  /AnalyzerSDK/include/
		
The best way to get Saleae SDK is to clone it directly from GitHub's repository:
[Saleae SDK!](https://github.com/saleae/AnalyzerSDK.git)

5. License information
Available in Licenses.txt
