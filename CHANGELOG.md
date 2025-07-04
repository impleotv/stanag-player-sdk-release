Change Log
==========

### Ver. 4.2.14 (16/06/25)
 Low level Ver. 1.7.15 (15/6/25)
- Fixing the pid name detection in the demux filter

### Ver. 4.2.13 (03/06/25)
- New mkdocs Manual
- Low level Ver. 1.7.14 (28/5/25)
	- Fixing memory leak in encoder and in AV1 decoder 

### Ver. 4.2.12 (15/05/25)
- MISB 601. Add tag 140 (WeaponsStores)
- Add nodeinfo QR code in demo app 

### Ver. 4.2.10 (12/05/25)
- Low level Ver. 1.7.13 (11/5/25)
	- Fix decoder state machine stability while playing corrupted content

### Ver. 4.2.8 (10/04/25)
- Low level Ver. 1.7.11 (9/4/25)
	- Fix exception on decoding stop 

### Ver. 4.2.7 (03/04/25)
- Low level 1.7.10 
	- Fixing demux of h265 with bad syntax

### Ver. 4.2.6 (16/03/25)
- Modify setup

### Ver. 4.2.6 (16/03/25)
- Modify setup

### Ver. 4.2.5 (24/02/25)
- low level Ver. 1.7.9 (23/2/25)
	- Added API for enable/disable transport discontinuity events (default is ignore discontinuity)

### Ver. 4.2.4 (19/02/25)
- Replace x32 h264 encoder with x64
- low level Ver. 1.7.8 (19/2/25)
	- Fixed resolution detection in HEVC
	- supporting synthetic video insertion and dynamic input resolution change in encoder
	- fixing a regression bug in video capture mode
	- Supporting aspect ration dynamic change in encoder

### Ver. 4.2.4 (19/02/25)
- Replace x32 h264 encoder with x64
- low level Ver. 1.7.8 (19/2/25)
	- Fixed resolution detection in HEVC
	- supporting synthetic video insertion and dynamic input resolution change in encoder
	- fixing a regression bug in video capture mode
	- Supporting aspect ration dynamic change in encoder

### Ver. 4.2.3 (09/02/25)
- Update time server implementation

### Ver. 4.2.2 (04/02/25)
- low level
	- MPEG-TS detection fixes
### Ver. 4.2.1 (30/01/25)
- low level
 - Adding support for AV1 in RTP input and in decoding
 - AV1 stabilization fixes

### Ver. 4.2.0 (12/01/25)
- low level
 - Upgrading ffmpeg to 5.1.2
 - Use Filters v1.7
 
### Ver. 4.1.5 (29/12/24)
- low level
 - fix playback stability in switch sources
 - improve time jumps resync handling

### Ver. 4.1.4 (15/11/24)
- low level
	- support decoding of H265 with P10 pixel format

### Ver. 4.1.3 (22/10/24)
- low level
	- Stabilize smoothing filter
	- Add StreamDeliverySmoother.dll to setup

### Ver. 4.1.2 (16/10/24)
- low level
	- Fix RTSP if more than 4 tracks
	- Fix Directx renderer dead-lock in low delay

### Ver. 4.1.1 (10/09/24)
- low level modifications
	- Comply with H264 SEI NAL in the beginning of PES

### Ver. 4.1.0 (14/08/24)
- low level modifications
- MisbCore VMTI modifications
	- Add MISB903.6 support 

### Ver. 4.0.7 (05/06/24)
- low level
	- Fix aspect ratio and vertical flip in video snapshot
	- Fix handling of H265 decoding using Elecard, when callback requires RGB
	
### Ver. 4.0.6 (26/05/24)
- low level 
	- Add an option to select the gpu device performing the hw accelerated decoding


### Ver. 4.0.5 (19/05/24)
- low level 
	- Complete support for pull demux with MPEG-PROGRAM input
	- Complete fix for IIS crash

### Ver. 4.0.4 (13/05/24)
- low level 
	- Modify Log Trace to avoid crash when running in IIS
	- Add Program stream push demux
	- Add option for buffer writes in StCore instead of UDP input

### Ver. 4.0.1 (2/05/24)
- low level 
	- Fix pause handling in VideoOverlayMixer
	- improve D3d video renderer performance
	
### Ver. 4.0.0 (1/05/24)
- Move to .Net 4.7.2
- Add JWT license
- Modify samples setup structure

- Modify low level 
	- Add delay option in videoOverlayMixer
	- Add option to override aspect ratio in VideoOverlayMixer
	- Improvements in presentation filters
	- Initial latency configuration fixes
	- Fix aspect ratio handling
	- Improve logging of monitored events (specifically for video renderer)

### Ver. 3.12.1 (01/04/24)
- Modify base NodeInfo 

### Ver. 3.12.0 (26/03/24)
- Modify NodeInfo format
Low level:
- Improving performance in D3d rendering
- Fixing VideoOverlayMixer in handling I420 pixel format

### Ver. 3.11.5 (24/03/24)
- Update MisbCore
	- Remove length from VMTI Location (tag 17)
	- Remove length from VMTI Velocity and Acceleration DLP 
### Ver. 3.11.4 (19/03/24)
 Improving the playback smoothness in D3d rendering
 
### Ver. 3.11.3 (12/03/24)
 DirectX mode playback improvements.

### Ver. 3.11.2 (10/03/24)
Low level changes:
- Add support for EVR renderer
- Add debug monitoring points for D3D9 Renderer
- Add an ini patch to disable footer search. To use it, 
To activate the patch, DemuxFilter.ini containing the following should be copied to Filters folder
[Parsing]
FooterSearchIsDisabled=1

### Ver. 3.11.1 (22/02/24)
- Update low level
- Add option for async callback of sync frames
- Modify StCore interface
### Ver. 3.10.17 (15/02/24)
- Update low level
### Ver. 3.10.16 (11/02/24)
- Added new property in IStCoreWr - SequenceHeaderInsertionIntervalMsec
- Update low level
### Ver. 3.10.15 (22/01/24)
- Update low level
- Lver modification
### Ver. 3.10.14 (15/01/24)
- Update low level
- A fix in listening on multicast address when specifying nic
- Graphic overlay fix: supporting unicode text overlay insertion (for hebrew)
### Ver. 3.10.13 (03/01/24)
- Update low level (Injector memory leak)
### Ver. 3.10.12 (27/12/23)
- Update low level
### Ver. 3.10.11 (22/12/23)
- Update low level (finalize integration)
### Ver. 3.10.10 (14/12/23)
- Update low level
### Ver. 3.10.9 (13/12/23)
- Update low level
### Ver. 3.10.8 (10/12/23)
- Update low level
- Add support for external decoder configuration dll (optional Decoder Configuration plugin)
- TsParser version is 3.9.6
### Ver. 3.10.7 (06/12/23)
- Update low level
### Ver. 3.10.6 (30/11/23)
- Supporting DirectX renderer in display cards which do not support YV12
- Supporting QuickSync decoding in PCs that did not support it
### Ver. 3.10.5 (26/11/23)
- Low level update. Quicksync related
### Ver. 3.10.4 (12/10-/23)
- Fix long VMTI tracker (over 14 items)
### Ver. 3.10.3 (23/08/23)
- Low level update. 
- Support the sps information provided in an rtp packet with a format STAP-A 
- Fix the SequenceHeaderInsertionOnKeyFrames property did not reach its destination in the DVR mode
### Ver. 3.10.2 (16/07/23)
- Fix BER-OID Encoding/Decoding for VMTI Target ID
### Ver. 3.10.1 (27/06/23)
- Low level update. Decoder memory leak fix
### Ver. 3.10.0 (23/05/23)
- Low level update. FFmpeg version change
- Add api for configuring decoding hw acceleration type
### Ver. 3.9.9 (16/05/23)
- Update low level
### Ver. 3.9.8 (11/05/23)
- Update low level
### Ver. 3.9.7 (11/04/23)
- Add JWT authentication for HLS
### Ver. 3.9.5 (02/02/23)
- Update MisbCore. Add VCip support to VMTI
### Ver. 3.9.4 (14/08/22)
- Update MisbCore (fix VMTI target id)
### Ver. 3.9.2 (09/08/22)
- Update low level
- Add tags 115, 116, 121, 122, 128, 138, 139
### Ver. 3.9.1 (03/07/22)
- Update low level
### Ver. 3.9.0 (4/05/22)
-Add StServer VMS mission/sensor playback
### Ver. 3.8.17 (01/05/22)
- Update low level
### Ver. 3.8.14 (27/02/22)
- Update MisbCore (VObject)

### Ver. 3.8.13 (17/02/22)
- Update low level (RTSP related improvements)
### Ver. 3.8.11 (19/12/21)
- Update low level
### Ver. 3.8.10 (23/11/21)
- Update low level
- Add time restricted license support
- Move to vc142 and correspoding boost libraries
### Ver. 3.8.9.2 (11/11/21)
- Update StCore VS runtime to 2019
### Ver. 3.8.9.2 (11/11/21)
- Update VS runtime to 2019
### Ver. 3.8.9.1 (02/11/21)
- Update MisbCore
### Ver. 3.8.9
- Add FrameAccurecyRequiresSequenceHeaders property 
- Move to VS2019
- Low level update
### Ver. 3.8.7.7 (27/06/21)
- Low level update
- MisbCore Fix Rvt decoding (remove hard coded write to disk)

### Ver. 3.8.7.6 (14/06/21)
- MisbCore user defined data
- Add IgnorePidInInput 
### Ver. 3.8.7.5 (13/05/21)
- MisbCore update (activation)
### Ver. 3.8.7.4 (5/05/21)
- MisbCore update
- Recompiled in VS2019

### Ver. 3.8.7.3 (29/04/21)
- Low level update

### Ver. 3.8.7.1 (05/04/21)
- Fix potential HLS duration issues
- HLS split on discontinuity
- I frame manifest with split segments-  
- Low level update

### Ver. 3.8.7 (31/03/21)
- Fix HLS duration (with discontinuity) 
- Remove EnforcedDecoder
- Low level update
### Ver. 3.8.6 (15/02/21)
- HLS Offset culture fix
### Ver. 3.8.6 (07/02/21)
- Add ContiguousDemuxedVideo
- Add IsHlsManifestDurationAccurate - if the reported segments duration is accurate enough, so that internal PTS detection can be skipped
### Ver. 3.8.5
- Low level update

### Ver. 3.8.4.2
- Low level update
### Ver. 3.8.4
- Fix RTSP (tcp)
- Enable FIPS Compliant authorization

### Ver. 3.8.3
- Low level update (StCore 3.8.3)

### Ver. 3.8.0
- MisbCore
- Move to .NET 4.6.1
- decodedData now passed as JObject

### Ver. 3.7.15
- Low level update

### Ver. 3.7.14.1
- Fix  each stop->start creates additional output channel with the same IP and port.

### Ver. 3.7.14
- Low level update

### Ver. 3.7.11
- Low delay fixes
- Adding option to modify incoming PTS in Injector according to local CPU time

### Ver. 3.7.10
- Low level update
- 0.0.0.0 binding

### Ver. 3.7.9
- Add Klv pid selection to demo app
- Low level update

### Ver. 3.7.8
- Add Direct X overlay sample

### Ver. 3.7.7
- Encoder profile and framerate changes

### Ver. 3.7.6
- Low level changes (Injector robustness)
- Fix missing Klv after seek
- Fix audio pid mux

### Ver. 3.7.5
- Low level change. Fix DVR Klv serialization

### Ver. 3.7.4
- Low level change to allow burst packet processing 

### Ver. 3.7.3
- Low level update
- Add logger module
- Add MinKlvPacket == 0

### Ver. 3.7.1
- Fix high bitrate injection
- Fix CRF GOP structure injection

### Ver. 3.7.0
- BER-OID tags

### Ver. 3.6.1
- Synthetic Video fixes in low level filters and StCore.dll
- General fixes in low level filter

### Ver. 3.6.0
- Low level update
- Fix high bitrate ingest
- Fix EC_COMPLETE without video decoding

### Ver. 3.5.1
- StCore compiled with vc141 and boost 1.71

### Ver. 3.5.0
- Low level update
- Add Overlay to WPF demo app 

### Ver. 3.4.3
- Low level update

### Ver. 3.4.2
- Low level update
- MISB 601 tags added
- MISB 903 fix

### Ver. 3.4.2
- Low level update

### Ver. 3.4.1
- New property - CopySyncFrameVideoData
- New method CreateBitmapFromFrameBuffer(StCoreWr.VideoFrameInfoWr frameInfo) provides conversion from YUV to RGB bitmap


### Ver. 3.4.0
- Low level update
- MISB 0903 fix

### Ver. 3.3.5
- Low level update
- GetSnapshot fix
- Misb2Kml update

### Ver. 3.3.4
- Low level update

### Ver. 3.3.2
- Low level update
= Transcoding from EG104.5 to MISB0601
- Conditional HEVC support

### Ver. 3.3.1
- Low level update

### Ver. 3.3.0
- Major change: DVR mode integrated
- Added PushToPullFilter.dll
- Interface change:	
	- CKlvPlayer constructor override added CKlvPlayer(bool fDvrMode)	
	- Method added: 
		GoToLive 
		GetAvailableRange 
	- Property added:
		IsDvrMode
		DvrLocalBufferSize
		DVR_RefTimeMatchModed
		TimeMatchPid
	- Player_State changed	
	- StepForward() and StepBackward() now return bool
- Demo applications updated.
	Console and Winforms applications implement DVR functionality

### Ver. 3.2.0
- Low level update
Fixing the busy manifest file in case of hls parse error
- Tolerating comma in the end of hls manifest line
- Fixing the audio playback problems (please verify and let me know)
- Completing the reverse playback:
a. Playback should be smooth and stable now.
b. fast reverse uses I frames only (if the hls provides I frames manifest)
c. Added a property to MinimalRateForIFramesPlayback to HlsConfigParams in IStCoreLib::HlsSource() property. It means in which rate to use I frame only. Default is rate > 1 or rate < -1
- In Frame Accuracy mode a TimeToRender will always be 50 msec 

### Ver. 3.1.2
- Low level update
- ST1204 WindowID allocation fix 

### Ver. 3.1.1
- GetCurrentPosition override for stream (low level returns 0 for some reason)

### Ver. 3.1.0
- Low level changes (step forward / backward, ff, reverse)
- IStCoreLib - interface update
    ISyncFrameInfo changed to ISynchronizedFrameInfo
    SelectAudioToRender added
    FrameStep replaced with StepForward() / StepBackward()
- Removing the filter SyncSampleGrabberFilter, 
- Adding the following filters:
	SampleSynchronizerFilter
	SyncSampleFrameAccuracyFilter
	SyncSampleDispatcherFilter

### Ver. 3.0.38
- Low level changes (step forward)
- IStCoreLib - FrameAccuracyMode added

### Ver. 3.0.37
- SetRate / GetRate after stop fix
- Error handling in HLS

### Ver. 3.0.36
- Low level updated.
- HLS fast forward

### Ver. 3.0.35
- Low level updated.

### Ver. 3.0.33
- Low level updated.
- DecodeAll flag added to decoder ini

### Ver. 3.0.32
- Stream subtype added to PidInfo
- Number of scale cores added

### Ver. 3.0.31
- HLS update
- KlvDecoder filter update
- Running event after resume
- Packet sampling fixed

### Ver. 3.0.30
- HLS support
- Running event after seek (currently in hls only)

### Ver. 3.0.29
- KlvDecoder now looks for entire klv packet start

### Ver. 3.0.28
- Low level filters change
- Target location added
- VMTI detailed json changes 
### Ver. 3.0.27
- PES per frame duration fixed
- Changed VTracker_LDS to 105 according to revision 0903.3

### Ver. 3.0.26
- ISyncFrameInfo::GetStreamInfo2 implementation
- KlvPacket Sampling implemented on StCoreWr level


### Ver. 3.0.25
- KlvPacket Sampling added
- Output NIC added 

### Ver. 3.0.24.1
- Some logs added

### Ver. 3.0.24
- Fix Init return value 


### Ver. 3.0.22
- Recorder removed
 

### Ver. 3.0.20
- Fixed Audio
- Removed error reporting on stop (stream playback without source) 


### Ver. 3.0.18
- StPlayer licensing support added.

### Ver. 3.0.17
- StExporter support added.

### Ver. 3.0.16
- Compressed video frames DTS reporting.

### Ver. 3.0.16
- Low level changes
- HW accelerated decoding
- New setup
- Fix for 2fps file

### Ver. 3.0.10
- File target added

### Ver. 3.0.9
- License activation fix
- RAW Klv Items array added to KlvFrameInfoWr

### Ver. 3.0.7
- Updated filters
- Low level interfaces changed
- Added StCoreWr that encapsulates a Low level common Player / Injector functionality. 
- Removed old data / video events. OnSyncFrameEvent takes care of all the cases 

### Ver. 3.0.6
- Updated filters

### Ver. 3.0.5
- Updated filters

### Ver. 3.0.0
*First release*



