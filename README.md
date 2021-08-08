# hdcamera
Firmware repository for PlayStation HD Camera 


```
 lsusb -d 05a9:058c -v

Bus 002 Device 007: ID 05a9:058c OmniVision Technologies, Inc.
Device Descriptor:
  bLength                18
  bDescriptorType         1
  bcdUSB               3.20
  bDeviceClass          239 Miscellaneous Device
  bDeviceSubClass         2
  bDeviceProtocol         1 Interface Association
  bMaxPacketSize0         9
  idVendor           0x05a9 OmniVision Technologies, Inc.
  idProduct          0x058c
  bcdDevice            1.00
  iManufacturer           1 Omnivision Technologies, Inc.
  iProduct                2 USB Camera-OV580
  iSerial                 0
  bNumConfigurations      1
  Configuration Descriptor:
    bLength                 9
    bDescriptorType         2
    wTotalLength       0x026b
    bNumInterfaces          2
    bConfigurationValue     1
    iConfiguration          0
    bmAttributes         0x80
      (Bus Powered)
    MaxPower              512mA
    Interface Association:
      bLength                 8
      bDescriptorType        11
      bFirstInterface         0
      bInterfaceCount         2
      bFunctionClass         14 Video
      bFunctionSubClass       3 Video Interface Collection
      bFunctionProtocol       0
      iFunction               2 USB Camera-OV580
    Interface Descriptor:
      bLength                 9
      bDescriptorType         4
      bInterfaceNumber        0
      bAlternateSetting       0
      bNumEndpoints           0
      bInterfaceClass        14 Video
      bInterfaceSubClass      1 Video Control
      bInterfaceProtocol      0
      iInterface              2 USB Camera-OV580
      VideoControl Interface Descriptor:
        bLength                13
        bDescriptorType        36
        bDescriptorSubtype      1 (HEADER)
        bcdUVC               1.00
        wTotalLength       0x004d
        dwClockFrequency      125.000000MHz
        bInCollection           1
        baInterfaceNr( 0)       1
      VideoControl Interface Descriptor:
        bLength                18
        bDescriptorType        36
        bDescriptorSubtype      2 (INPUT_TERMINAL)
        bTerminalID             1
        wTerminalType      0x0201 Camera Sensor
        bAssocTerminal          0
        iTerminal               0
        wObjectiveFocalLengthMin      0
        wObjectiveFocalLengthMax      0
        wOcularFocalLength            0
        bControlSize                  3
        bmControls           0x0000000a
          Auto-Exposure Mode
          Exposure Time (Absolute)
      VideoControl Interface Descriptor:
        bLength                 9
        bDescriptorType        36
        bDescriptorSubtype      3 (OUTPUT_TERMINAL)
        bTerminalID             2
        wTerminalType      0x0101 USB Streaming
        bAssocTerminal          0
        bSourceID               3
        iTerminal               0
      VideoControl Interface Descriptor:
        bLength                11
        bDescriptorType        36
        bDescriptorSubtype      5 (PROCESSING_UNIT)
      Warning: Descriptor too short
        bUnitID                 3
        bSourceID               1
        wMaxMultiplier          0
        bControlSize            2
        bmControls     0x0000165f
          Brightness
          Contrast
          Hue
          Saturation
          Sharpness
          White Balance Temperature
          Gain
          Power Line Frequency
          White Balance Temperature, Auto
        iProcessing             2 USB Camera-OV580
        bmVideoStandards     0x1a
          NTSC - 525/60
          SECAM - 625/50
          NTSC - 625/50
      VideoControl Interface Descriptor:
        bLength                26
        bDescriptorType        36
        bDescriptorSubtype      6 (EXTENSION_UNIT)
        bUnitID                 4
        guidExtensionCode         {dd880f8a-1cba-4954-8a25-f7875967f0f7}
        bNumControl             1
        bNrPins                 1
        baSourceID( 0)          1
        bControlSize            1
        bmControls( 0)       0x01
        iExtension              2 USB Camera-OV580
    Interface Descriptor:
      bLength                 9
      bDescriptorType         4
      bInterfaceNumber        1
      bAlternateSetting       0
      bNumEndpoints           0
      bInterfaceClass        14 Video
      bInterfaceSubClass      2 Video Streaming
      bInterfaceProtocol      0
      iInterface              0
      VideoStreaming Interface Descriptor:
        bLength                            14
        bDescriptorType                    36
        bDescriptorSubtype                  1 (INPUT_HEADER)
        bNumFormats                         1
        wTotalLength                   0x01e5
        bEndPointAddress                  129
        bmInfo                              0
        bTerminalLink                       2
        bStillCaptureMethod                 0
        bTriggerSupport                     0
        bTriggerUsage                       0
        bControlSize                        1
        bmaControls( 0)                     0
      VideoStreaming Interface Descriptor:
        bLength                            27
        bDescriptorType                    36
        bDescriptorSubtype                  4 (FORMAT_UNCOMPRESSED)
        bFormatIndex                        1
        bNumFrameDescriptors               13
        guidFormat                            {32595559-0000-0010-8000-00aa00389b71}
        bBitsPerPixel                      16
        bDefaultFrameIndex                  1
        bAspectRatioX                       0
        bAspectRatioY                       0
        bmInterlaceFlags                 0x00
          Interlaced stream or variable: No
          Fields per frame: 2 fields
          Field 1 first: No
          Field pattern: Field 1 only
        bCopyProtect                        0
      VideoStreaming Interface Descriptor:
        bLength                            30
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                         1
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                            896
        wHeight                           256
        dwMinBitRate                   458752
        dwMaxBitRate                 13762560
        dwMaxVideoFrameBufferSize      458752
        dwDefaultFrameInterval          83333
        bFrameIntervalType                  1
        dwFrameInterval( 0)             83333
      VideoStreaming Interface Descriptor:
        bLength                            38
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                         2
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                           1920
        wHeight                          1080
        dwMinBitRate                  4147200
        dwMaxBitRate                124416000
        dwMaxVideoFrameBufferSize     4147200
        dwDefaultFrameInterval         333333
        bFrameIntervalType                  3
        dwFrameInterval( 0)            333333
        dwFrameInterval( 1)            666666
        dwFrameInterval( 2)           1250000
      VideoStreaming Interface Descriptor:
        bLength                            30
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                         3
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                            960
        wHeight                           520
        dwMinBitRate                   998400
        dwMaxBitRate                 29952000
        dwMaxVideoFrameBufferSize      998400
        dwDefaultFrameInterval         166666
        bFrameIntervalType                  1
        dwFrameInterval( 0)            166666
      VideoStreaming Interface Descriptor:
        bLength                            30
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                         4
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                            448
        wHeight                           256
        dwMinBitRate                   229376
        dwMaxBitRate                  6881280
        dwMaxVideoFrameBufferSize      229376
        dwDefaultFrameInterval          83333
        bFrameIntervalType                  1
        dwFrameInterval( 0)             83333
      VideoStreaming Interface Descriptor:
        bLength                            42
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                         5
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                           1280
        wHeight                           800
        dwMinBitRate                  2048000
        dwMaxBitRate                 61440000
        dwMaxVideoFrameBufferSize     2048000
        dwDefaultFrameInterval         166666
        bFrameIntervalType                  4
        dwFrameInterval( 0)            166666
        dwFrameInterval( 1)            333333
        dwFrameInterval( 2)            666666
        dwFrameInterval( 3)           1250000
      VideoStreaming Interface Descriptor:
        bLength                            30
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                         6
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                            640
        wHeight                           376
        dwMinBitRate                   481280
        dwMaxBitRate                 14438400
        dwMaxVideoFrameBufferSize      481280
        dwDefaultFrameInterval          83333
        bFrameIntervalType                  1
        dwFrameInterval( 0)             83333
      VideoStreaming Interface Descriptor:
        bLength                            30
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                         7
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                            320
        wHeight                           184
        dwMinBitRate                   117760
        dwMaxBitRate                  3532800
        dwMaxVideoFrameBufferSize      117760
        dwDefaultFrameInterval          41666
        bFrameIntervalType                  1
        dwFrameInterval( 0)             41666
      VideoStreaming Interface Descriptor:
        bLength                            38
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                         8
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                           5148
        wHeight                          1088
        dwMinBitRate                 11202048
        dwMaxBitRate                336061440
        dwMaxVideoFrameBufferSize    11202048
        dwDefaultFrameInterval         333333
        bFrameIntervalType                  3
        dwFrameInterval( 0)            333333
        dwFrameInterval( 1)            666666
        dwFrameInterval( 2)           1250000
      VideoStreaming Interface Descriptor:
        bLength                            38
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                         9
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                           3840
        wHeight                          1080
        dwMinBitRate                  8294400
        dwMaxBitRate                248832000
        dwMaxVideoFrameBufferSize     8294400
        dwDefaultFrameInterval         333333
        bFrameIntervalType                  3
        dwFrameInterval( 0)            333333
        dwFrameInterval( 1)            666666
        dwFrameInterval( 2)           1250000
      VideoStreaming Interface Descriptor:
        bLength                            30
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                        10
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                           1920
        wHeight                           520
        dwMinBitRate                  1996800
        dwMaxBitRate                 59904000
        dwMaxVideoFrameBufferSize     1996800
        dwDefaultFrameInterval         166666
        bFrameIntervalType                  1
        dwFrameInterval( 0)            166666
      VideoStreaming Interface Descriptor:
        bLength                            42
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                        11
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                           2560
        wHeight                           800
        dwMinBitRate                  4096000
        dwMaxBitRate                122880000
        dwMaxVideoFrameBufferSize     4096000
        dwDefaultFrameInterval         166666
        bFrameIntervalType                  4
        dwFrameInterval( 0)            166666
        dwFrameInterval( 1)            333333
        dwFrameInterval( 2)            666666
        dwFrameInterval( 3)           1250000
      VideoStreaming Interface Descriptor:
        bLength                            30
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                        12
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                           1280
        wHeight                           376
        dwMinBitRate                   962560
        dwMaxBitRate                 28876800
        dwMaxVideoFrameBufferSize      962560
        dwDefaultFrameInterval          83333
        bFrameIntervalType                  1
        dwFrameInterval( 0)             83333
      VideoStreaming Interface Descriptor:
        bLength                            30
        bDescriptorType                    36
        bDescriptorSubtype                  5 (FRAME_UNCOMPRESSED)
        bFrameIndex                        13
        bmCapabilities                   0x00
          Still image unsupported
        wWidth                            640
        wHeight                           184
        dwMinBitRate                   235520
        dwMaxBitRate                  7065600
        dwMaxVideoFrameBufferSize      235520
        dwDefaultFrameInterval          41666
        bFrameIntervalType                  1
        dwFrameInterval( 0)             41666
      VideoStreaming Interface Descriptor:
        bLength                             6
        bDescriptorType                    36
        bDescriptorSubtype                 13 (COLORFORMAT)
        bColorPrimaries                     1 (BT.709,sRGB)
        bTransferCharacteristics            1 (BT.709)
        bMatrixCoefficients                 4 (SMPTE 170M (BT.601))
    Interface Descriptor:
      bLength                 9
      bDescriptorType         4
      bInterfaceNumber        1
      bAlternateSetting       1
      bNumEndpoints           1
      bInterfaceClass        14 Video
      bInterfaceSubClass      2 Video Streaming
      bInterfaceProtocol      0
      iInterface              0
      Endpoint Descriptor:
        bLength                 7
        bDescriptorType         5
        bEndpointAddress     0x81  EP 1 IN
        bmAttributes            5
          Transfer Type            Isochronous
          Synch Type               Asynchronous
          Usage Type               Data
        wMaxPacketSize     0x0400  1x 1024 bytes
        bInterval               1
        bMaxBurst              15
        Mult                    2
Binary Object Store Descriptor:
  bLength                 5
  bDescriptorType        15
  wTotalLength       0x0016
  bNumDeviceCaps          2
  USB 2.0 Extension Device Capability:
    bLength                 7
    bDescriptorType        16
    bDevCapabilityType      2
    bmAttributes   0x00000002
      HIRD Link Power Management (LPM) Supported
  SuperSpeed USB Device Capability:
    bLength                10
    bDescriptorType        16
    bDevCapabilityType      3
    bmAttributes         0x00
    wSpeedsSupported   0x000c
      Device can operate at High Speed (480Mbps)
      Device can operate at SuperSpeed (5Gbps)
    bFunctionalitySupport   2
      Lowest fully-functional device speed is High Speed (480Mbps)
    bU1DevExitLat          10 micro seconds
    bU2DevExitLat          32 micro seconds
can't get debug descriptor: Resource temporarily unavailable
Device Status:     0x0f0c
  (Bus Powered)
  U1 Enabled
  U2 Enabled
```

 Credits
===========================
  
 - @hackinside for sharing usb raw traffic from beagle 5000 device from @totalphase 
 - @frangar @fjtrujy @psxdev aka "los nenes" playstation device and retro masters for their continuous support :P 
