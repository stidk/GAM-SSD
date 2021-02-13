# GAM-SSD
GAM-SSD is built based on PaddleDetection suite

#### 1.we suggest you use paddle aistudio online directly without install any packets.
#### 2.you need to download open dataset pascalvoc.zip yourself. Then run the command lines to build dataset.

```
!unzip -q /home/aistudio/data/data4379/pascalvoc.zip -d /home/aistudio/PaddleDetection-release-0.4/dataset/voc'
!python /home/aistudio/PaddleDetection-release-0.4/dataset/voc/create_list.py -d '/home/aistudio/PaddleDetection-release-0.4/dataset/voc/pascalvoc'
```

note data4379 is self-defined.

#### 3.run the command lines to train and test.

```
%cd ~/PaddleDetection-release-0.4
!python tools/train.py -c ssd_r101_300_voc.yml --eval 
(!python tools/train.py -c ssd_r50_300_voc.yml --eval )
```

#### 4.opendataset NWPUVHR-10.zip is provided in "dataset" folder
