# train_apollo_seg
NOTE: TensorRT no longer supports Relu API used in this model.

### dataset
download v1.0-trainval only!!!

### create dataset
```
 python3 create_dataset_from_nusc.py  --dataroot /home/bruce/Downloads/dataset/nuscenes --save_dir /home/bruce/Downloads/dataset/apollo_seg_data --nusc_version v1.0-trainval
```

### train 
```
python3 train_bcnn.py --data_path /home/bruce/Downloads/dataset/apollo_seg_data --batch_size 25 --max_epoch 150 --pretrained_model checkpoints/bcnn_latestmodel_20220421_1510.pt

```

### empty trash fast way 
```
cd .local/share/Trash/
sudo rm -r *
```
