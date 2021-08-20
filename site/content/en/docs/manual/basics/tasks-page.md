---
title: 'Tasks page'
linkTitle: 'Tasks page'
weight: 2.5
description: 'Overview of the Tasks page.'
---

![](/images/image006_detrac.jpg)

The tasks page contains elements and each of them relates to a separate task. They are sorted in creation order.
Each element contains: task name, preview, progress bar, button `Open`, and menu `Actions`.
Each button is responsible for a in menu `Actions` specific function:

- `Dump Annotation` and `Export as a dataset` — download annotations or
  annotations and images in a specific format. The following formats are available:
  - [CVAT for video](/docs/manual/advanced/xml_format/#interpolation)
    is highlighted if a task has the interpolation mode.
  - [CVAT for images](/docs/manual/advanced/xml_format/#annotation)
    is highlighted if a task has the annotation mode.
  - [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/)
  - [(VOC) Segmentation mask](http://host.robots.ox.ac.uk/pascal/VOC/) —
    archive contains class and instance masks for each frame in the png
    format and a text file with the value of each color.
  - [YOLO](https://pjreddie.com/darknet/yolo/)
  - [COCO](http://cocodataset.org/#format-data)
  - [TFRecord](https://www.tensorflow.org/tutorials/load_data/tfrecord)
  - [MOT](https://motchallenge.net/)
  - [LabelMe 3.0](http://labelme.csail.mit.edu/Release3.0/)
  - [Datumaro](https://github.com/openvinotoolkit/cvat/tree/develop/cvat/apps/dataset_manager/formats/datumaro)
  - Point Cloud Format 1.0 (Available in 3d task)
  - Velodyn points format 1.0 (Available in 3d task)
- `Upload annotation` is available in the same formats as in `Dump annotation`.
  - [CVAT](/docs/manual/advanced/xml_format/) accepts both video and image sub-formats.
  - Point Cloud Format 1.0 (Available in 3d task)
  - Velodyn points format 1.0 (Available in 3d task)
- `Automatic Annotation` — automatic annotation with OpenVINO toolkit.
  Presence depends on how you build CVAT instance.
- `Export task` — Export a task into a zip archive.
  Read more in the [export/import a task](/docs/manual/advanced/export-import/) section.
- `Move to project` — Moving the task to the project (can be used to move a task from one project to another).
  Note that attributes reset during the moving process. In case of label mismatch,
  you can create or delete necessary labels in the project/task.
  Some task labels can be matched with the target project labels.
- `Delete` — delete task.

---

Push `Open` button to go to [task details](/docs/manual/basics/task-details/).