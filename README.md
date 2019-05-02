# Phương pháp nghiên cứu khoa học <br> Image Captioning
## Danh sách thành viên
|MSSV|Họ và tên
|--|--
|1712060|Trần Vinh Hưng
|1712122|Nguyễn Tiến Phát
|1712168|Trần Lê Bá Thịnh

## Mục lục
1. [Cấu trúc thư mục](#folder_structure)
2. [Hướng dẫn sử dụng](#usage)

## <a name='folder_structure'>Folder Structure</a>
```
.
├──main_source/ - Main source code for experiment.
|   ├──  
|   |
|   ├──model/ - Models' class
|   |   ├──encoder/ - Image encoders' class
|   |   └──decoder/ - Sequence decoders' class
|   |
|   ├──trainer/ - Trainers
|   |
|   ├──dataloader/ - Dataloader/Dataset Class
|   |
|   ├──config/ - Config for model + training
|   |
|   └──utils/ - Other small scripts.
|      ├──metric.py - All metric for model.
|      └──loss.py - All loss function for model.
|
├──script/ - Helper + Warper script.
|
└──data/ - default data folder.
    ├──dataset_folder/
    |
    ├──checkpoint/ - Trained checkpoint for model.
    └──log/ - default log folder
```

## <a name='usage'>Hướng dẫn sử dụng</a>
Sẽ viết sau khi hoàn thành.