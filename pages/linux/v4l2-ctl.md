# v4l2-ctl

> Control video devices.
> More information: <https://manned.org/v4l2-ctl>.

- List all video devices:

`v4l2-ctl {{[-A|--list-devices]}}`

- List supported video formats and resolutions of default video device `/dev/video0`:

`v4l2-ctl --list-formats-ext`

- List supported video formats and resolutions of a specific video device:

`v4l2-ctl --list-formats-ext {{[-d|--device]}} {{path/to/video_device}}`

- Get all details of a video device:

`v4l2-ctl --all {{[-d|--device]}} {{path/to/video_device}}`

- Capture a JPEG photo with a specific resolution from video device:

`v4l2-ctl {{[-d|--device]}} {{path/to/video_device}} --set-fmt-video=width={{width}},height={{height}},pixelformat=MJPG --stream-mmap --stream-to={{path/to/output.jpg}} --stream-count=1`

- Capture a raw video stream from video device:

`v4l2-ctl {{[-d|--device]}} {{path/to/video_device}} --set-fmt-video=width={{width}},height={{height}},pixelformat={{format}} --stream-mmap --stream-to={{path/to/output}} --stream-count={{number_of_frames_to_capture}}`

- List all video device's controls and their values:

`v4l2-ctl {{[-l|--list-ctrls]}} {{[-d|--device]}} {{path/to/video_device}}`

- Set the value of a video device control:

`v4l2-ctl {{[-d|--device]}} {{path/to/video_device}} {{[-c|--set-ctrl]}} {{control_name}}={{value}}`
