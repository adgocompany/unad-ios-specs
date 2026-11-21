# UNAD iOS CocoaPods Specs

Public CocoaPods specifications for UNAD iOS SDK distributions.

## Installation

Add the public UNAD specs repository and the CocoaPods CDN to your Podfile, then select one SDK distribution:

```ruby
source 'https://github.com/adgocompany/unad-ios-specs.git'
source 'https://cdn.cocoapods.org/'

platform :ios, '13.0'

target 'YourApp' do
  use_frameworks!
  pod 'UNAD-Global', '2.9.24'
  # Alternatives: pod 'UNAD-All', '2.9.24' or pod 'UNAD-Cn', '2.9.24'
end
```

Run `pod install`. Choose one distribution: the variants are alternatives and are not intended to be installed together. Their third-party ad SDKs may have simulator architecture limitations; validate real ad delivery on a device.
