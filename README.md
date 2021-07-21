# MASKRCNN-damagecar
请先下载 Matterport  的MASKRCNN并正确安装，同时下载mask_rcnn_coco.h5
将本分支的customImage和custom_cardamage.py放到 MASKRCNN的根目录并解压。
训练
python3 custom_cardamage.py train --dataset=customImages/  --weights=coco

预测
python3 custom_cardamage.py splash --image=customImages/test/bitauto.jpg --weights=mask_rcnn_damage_0010.h5
