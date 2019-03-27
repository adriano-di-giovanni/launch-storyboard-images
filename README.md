# Launch storyboard images

## Setup

```bash
cordova platform add ios@4.5.5
open platforms/ios/LaunchStoryboardImages.xcworkspace/
```

In XCode, set `Launch screen file` to `CDVLaunchScreen.storyboard`

## Download placeholder images

Download placeholder images for both [configurations](#configurations)

```bash
npm run download
```

## Configurations <a name="configurations" />

Edit `config.xml` to add the relevant `<splash />` tags.

### Single-image launch screen

```html
<splash src="res/screen/ios/Default@2x~universal~anyany.png" />
```

### Multi-image launch screen

```html
<splash src="res/screen/ios/Default@2x~iphone~anyany.png" />
<splash src="res/screen/ios/Default@2x~iphone~comany.png" />
<splash src="res/screen/ios/Default@2x~iphone~comcom.png" />
<splash src="res/screen/ios/Default@3x~iphone~anyany.png" />
<splash src="res/screen/ios/Default@3x~iphone~anycom.png" />
<splash src="res/screen/ios/Default@3x~iphone~comany.png" />
<splash src="res/screen/ios/Default@2x~ipad~anyany.png" />
<splash src="res/screen/ios/Default@2x~ipad~comany.png" />
```
