# GeneralFormatter

[![CI Status](http://img.shields.io/travis/OpenCraft/GeneralFormatter.svg?style=flat)](https://travis-ci.org/OpenCraft/GeneralFormatter)
[![Version](https://img.shields.io/cocoapods/v/GeneralFormatter.svg?style=flat)](http://cocoapods.org/pods/GeneralFormatter)
[![License](https://img.shields.io/cocoapods/l/GeneralFormatter.svg?style=flat)](http://cocoapods.org/pods/GeneralFormatter)
[![Platform](https://img.shields.io/cocoapods/p/GeneralFormatter.svg?style=flat)](http://cocoapods.org/pods/GeneralFormatter)

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Installation

GeneralFormatter is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod "GeneralFormatter"
```

## Usage

Link it directly on UITextFieldDelegate
```swift
func textField(_ textField: UITextField, shouldChangeCharactersIn range: NSRange, replacementString string: String) -> Bool {
    let formatter = GeneralFormatter(type: .cpfCnpj)
    return formatter.formatTextField(textField, shouldChangeCharactersIn: range, replacementString: string)
}
```

## Author

Uriel Battanoli, urielbattanoli@hotmail.com

## License

GeneralFormatter is available under the MIT license. See the LICENSE file for more info.