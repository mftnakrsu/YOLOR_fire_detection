# YOLOR Fire Detection

Original paper: https://arxiv.org/abs/2105.04206
Original source code : https://github.com/WongKinYiu/yolor

*People “understand” the world via vision, hearing, tactile, and also the past experience. Human experience can be learned through normal learning (we call it explicit knowledge), or subconsciously (we call it implicit knowledge). These experiences learned through normal learning or subconsciously will be encoded and stored in the brain. Using these abundant experience as a huge database, human beings can effectively process data, even they were unseen beforehand. In this paper, we propose a unified network to encode implicit knowledge and explicit knowledge together, just like the human brain can learn knowledge from normal learning as well as subconsciousness learning. The unified network can generate a unified representation to simultaneously serve various tasks. We can perform kernel space alignment, prediction refinement, and multi-task learning in a convolutional neural network. The results demonstrate that when implicit knowledge is introduced into the neural network, it benefits the performance of all tasks. We further analyze the implicit representation learnt from the proposed unified network, and it shows great capability on catching the physical meaning of different tasks. The source code of this work is at : https://github.com/WongKinYiu/yolor.*

![unifued_network](https://user-images.githubusercontent.com/57320216/175899682-f363b4eb-463b-4ef9-a5d6-0c2bcd154124.png)

![performance](https://user-images.githubusercontent.com/57320216/175899731-e1fb92e3-e4ac-4d07-a659-8d83c38db9bd.png)

 ## Training
 
 Single GPU training:

    python train.py --batch-size 8 --img 1280 1280 --data coco.yaml --cfg cfg/yolor_p6.cfg --weights '' --device 0 --name yolor_p6 --hyp hyp.scratch.1280.yaml --epochs 300


## Some results

![train_batch0](https://user-images.githubusercontent.com/57320216/175908556-8e1e8553-9b5e-4eaa-9b8b-68319c8481e5.jpg)
![train_batch2](https://user-images.githubusercontent.com/57320216/175908566-e75fa9e8-e932-46e2-ae94-d7de3dd469bf.jpg)
![train_batch1](https://user-images.githubusercontent.com/57320216/175908572-8e4d4356-dd71-457e-ba3c-14ff7be0e6c3.jpg)
![test_batch2_labels](https://user-images.githubusercontent.com/57320216/175908580-56438ccc-fa28-4f9f-85eb-3d475e4102c8.jpg)
![test_batch0_labels](https://user-images.githubusercontent.com/57320216/175908610-d540cc51-b2a9-46c0-b14f-07a96e8c9ea3.jpg)
![test_batch1_labels](https://user-images.githubusercontent.com/57320216/175908622-007c20e2-d6d0-41c3-90df-5041500cd820.jpg)
