## Giải thích về config

### Basic Config
```
{
    "trainer":{
        "lr":0.001, --Learning Rate
        "train_log_file":"data/log/train.log", --Train log file path
        
        "run_val":false, --Run validate with val dataset or not?
        "val_log_file":"data/log/val.log", --Val log file path
        
        "checkpoint_folder": "data/checkpoint/", --Folder to store checkpoint
        "checkpoint_name_format": "{encoder}_{decoder}_{epoch}_{bleu1}.pt", --Name of checkpoint format, support model.info, num epoch and metrics
        
        "metric":[ --List of metric to evaluate beside loss
            "bleu1", 
            "bleu4"
        ],

        "cider_train":false 
    },

    "model":{
        "encoder": "resnet18", --Model encoder type - listed in <add later>
        "decoder": "bi_lstm", --Model decoder path - listed in <add later>
        
        "info":{ --info to store checkpoint
            "encoder": "resnet",
            "decoder": "bi_lstm"
        },

        "pretrain":false, --use pretrain weight or not
        "model_weight":"" -- pretrain weight path
        
    },

    "dataloader":{
        "train_data_folder":null, --train data folder prefix
        "train_txt":null, --Txt label for train data

        "val_txt":null,
        "val_data_folder":null,

        "batch_size":32,
        "num_workers":2
    
    
    }
}
```
Note: My code always use GPU.