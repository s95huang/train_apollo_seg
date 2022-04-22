# train_apollo_seg

### dataset
download v1.0-trainval only!!!

### create dataset
```
 python3 create_dataset_from_nusc.py  --dataroot /home/bruce/Downloads/dataset/nuscenes --save_dir /home/bruce/Downloads/dataset/apollo_seg_data --nusc_version v1.0-trainval
```

### train 
```
 python3 train_bcnn.py --data_path /home/bruce/Downloads/dataset/nuscenes/dataset_apollo_seg --batch_size 24 --max_epoch 150 --pretrained_model checkpoints/train_1_1025_ep.pt

```

### empty trash fast way 
```
cd .local/share/Trash/
sudo rm -r *
```
