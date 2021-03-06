# UIColor-HexRGB
UIColor category that converts Hex and RGB color string values to UIColor.

## Supports color formats

- Hex string
	- fff (short, without #)
	- #fff (short, with #)
	- 00ff00 (long, without #)
	- #00ff00 (long, with #)
- RGB(A) string
	- 99,159,137 (without alpha)
	- 99,159,137,0.5 (with alpha)
- Hex integer
	- 0x00ff00

## Installation

- Add `UIColor+HexRGB.h` and `UIColor+HexRGB.h` to your project. 
- Or use CocoaPods: `pod 'UIColor-HexRGB'`.

## Requirements

Requires iOS 4.3 and above.

## Usage

``` cpp

  #import "UIColor+HexRGB.h"

  - (void)viewDidLoad {
  
    [super viewDidLoad];
      
    self.label1.backgroundColor = [UIColor colorWithHex: @"2eeea3"];  
  
    self.label2.backgroundColor = [UIColor colorWithHex: @"#fd482f"];  

    self.label3.backgroundColor = [UIColor colorWithRGB: @"99,159,137"];  
  
    self.label4.backgroundColor = [UIColor colorWithRGBA: @"137,99,59,0.5"];  

    self.label5.backgroundColor = [UIColor colorWithHex: @"0f0"];  
    
    self.label6.backgroundColor = [UIColor colorWithHexNum: 0xfd482f alpha: 0.5];  
  }
  
```

## Example

![Example](https://github.com/tinymind/UIColor-HexRGB/raw/master/example.png)