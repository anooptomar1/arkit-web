# AR PointCloud

This demo shows the raw feature points from the scene analysis.

Refer to the [installation instructions](../../../../README.md#installation) before running this demo.

1. Open your terminal and run `yarn start` and `yarn tunnel` from the `component-arkit-web/Demos` directory
2. Copy the ngrok https url from terminal
3. Open `component-arkit-web/ARKitWeb.xcodeproj` in Xcode
4. Open `component-arkit-web/ARKitWeb/ViewController.swift`
5. Set the `POINTCLOUD_DATA` flag to true
6. Click the `Build Settings` tab
7. Scroll down and locate the `DEV_URL` flag
8. Edit `DEV_URL` field with `<ngrok_https>/pointcloud.html`
9. Click `Build and run`

## Notes

ARKit does not guarantee that the number and arrangement of raw feature points will remain stable between software releases, or even between subsequent frames in the same session.

[Reference](https://developer.apple.com/documentation/arkit/arframe/2887449-rawfeaturepoints)