![Schema](./icon.png)

# Icon Badge

Add badge to any image (png, jpg, svg).

## Install

Available on [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=VladislavAntonyuk.launch-icon-badge-task)

## Features

Draw banners on top of your icons.

## Based on

You will find a complete tutorial here:

[https://damienaicheh.github.io/azure/devops/2020/01/09/easily-differentiate-versions-of-your-applications-using-azure-devops-en](https://damienaicheh.github.io/azure/devops/2020/01/09/easily-differentiate-versions-of-your-applications-using-azure-devops-en)


## Example of variable export for developing the project on a Mac:

```
export INPUT_SourceFolder="./../samples/AppIcon" &&
export INPUT_Contents="**/*.png" &&
export INPUT_BannerVersionNamePosition="bottomRight" &&
export INPUT_BannerVersionNumberPosition="none" &&
export INPUT_BannerVersionNameText="mvp" &&
export INPUT_BannerVersionNameColor="#C5000D" &&
export INPUT_BannerVersionNameTextColor="#FFFFFF" &&
export INPUT_BannerVersionNumberTextColor="#FFFFFF" &&
export INPUT_BannerVersionNumberText="1.2.3" &&
export INPUT_BannerVersionNumberColor="#34424F"
```

## Dev

```
npm install -g typescript
npm install -g tfx-cli

cd launchIconBadgeTask
npm install
tsc
cd ..

tfx extension create --manifest-globs vss-extension.json
```