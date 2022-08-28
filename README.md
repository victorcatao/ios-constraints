# iOS-constraints

This is an extension written in Swift to help you with your iOS constraints.

# Usage

```swift
let myView = UIView()
view.addSubview(myView)
myView.backgroundColor = .red
myView
    .pin(.leading, to: view.leadingAnchor)
    .pin(.top, to: view.topAnchor)
    .pin(.trailing, to: view.trailingAnchor, constant: -10)
    .pin(.bottom, to: view.bottomAnchor)

let myView2 = UIView()
view.addSubview(myView2)
myView2.backgroundColor = .blue
myView2
    .pin(.centerX, to: view.centerXAnchor)
    .pin(.centerY, to: view.centerYAnchor)
    .pin(.height, relation: .equalToConstant, constant: 100)
    .pin(.width, to: view.widthAnchor, multiplier: 0.9)
```
