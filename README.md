# Architecture_Neural_Network

Modified the code given in the colab file, [MNIST Code](https://colab.research.google.com/drive/1uJZvJdi5VprOQHROtJIHy0mnY2afjNlx) to achieve 99.4% accuracy with less than 20k parameters. 

## About the code

* Updated the network to have less than 20K parameters

* Added batch norm after every layer except last layer

* Added Transition layer (Max pool followed by 1x1) to reduce the number of channels after every block

* Add GAP layer

* Also added a FC layer

* Added Drop out of 0.1 after every layer except last layer

## Training Log
```
epoch=1 Loss=0.44412562251091003 batch_id=00468: 100%|██████████| 469/469 [01:54<00:00,  4.11it/s]
Test set: Average loss: 0.3129, Accuracy: 9404/10000 (94.04%)

epoch=2 Loss=0.2500273585319519 batch_id=00468: 100%|██████████| 469/469 [01:51<00:00,  4.21it/s]
Test set: Average loss: 0.0805, Accuracy: 9776/10000 (97.76%)

epoch=3 Loss=0.09267383813858032 batch_id=00468: 100%|██████████| 469/469 [01:51<00:00,  4.21it/s]
Test set: Average loss: 0.0488, Accuracy: 9856/10000 (98.56%)

epoch=4 Loss=0.12326803058385849 batch_id=00468: 100%|██████████| 469/469 [01:53<00:00,  4.14it/s]
Test set: Average loss: 0.0351, Accuracy: 9891/10000 (98.91%)

epoch=5 Loss=0.12314474582672119 batch_id=00468: 100%|██████████| 469/469 [01:51<00:00,  4.22it/s]
Test set: Average loss: 0.0352, Accuracy: 9890/10000 (98.90%)

epoch=6 Loss=0.1000981554389 batch_id=00468: 100%|██████████| 469/469 [01:51<00:00,  4.19it/s]
Test set: Average loss: 0.0321, Accuracy: 9891/10000 (98.91%)

epoch=7 Loss=0.1693059355020523 batch_id=00468: 100%|██████████| 469/469 [01:50<00:00,  4.23it/s]
Test set: Average loss: 0.0287, Accuracy: 9920/10000 (99.20%)

epoch=8 Loss=0.07933757454156876 batch_id=00468: 100%|██████████| 469/469 [01:50<00:00,  4.26it/s]
Test set: Average loss: 0.0290, Accuracy: 9909/10000 (99.09%)

epoch=9 Loss=0.08264420181512833 batch_id=00468: 100%|██████████| 469/469 [01:52<00:00,  4.19it/s]
Test set: Average loss: 0.0253, Accuracy: 9923/10000 (99.23%)

epoch=10 Loss=0.14999134838581085 batch_id=00468: 100%|██████████| 469/469 [01:52<00:00,  4.18it/s]
Test set: Average loss: 0.0253, Accuracy: 9920/10000 (99.20%)

epoch=11 Loss=0.014465401880443096 batch_id=00468: 100%|██████████| 469/469 [01:51<00:00,  4.19it/s]
Test set: Average loss: 0.0221, Accuracy: 9932/10000 (99.32%)

epoch=12 Loss=0.07466579228639603 batch_id=00468: 100%|██████████| 469/469 [01:51<00:00,  4.22it/s]
Test set: Average loss: 0.0231, Accuracy: 9924/10000 (99.24%)

epoch=13 Loss=0.08549857139587402 batch_id=00468: 100%|██████████| 469/469 [01:53<00:00,  4.14it/s]
Test set: Average loss: 0.0225, Accuracy: 9927/10000 (99.27%)

epoch=14 Loss=0.12752537429332733 batch_id=00468: 100%|██████████| 469/469 [01:54<00:00,  4.10it/s]
Test set: Average loss: 0.0209, Accuracy: 9934/10000 (99.34%)

epoch=15 Loss=0.026830002665519714 batch_id=00468: 100%|██████████| 469/469 [01:52<00:00,  4.17it/s]
Test set: Average loss: 0.0201, Accuracy: 9930/10000 (99.30%)

epoch=16 Loss=0.03579358384013176 batch_id=00468: 100%|██████████| 469/469 [01:52<00:00,  4.17it/s]
Test set: Average loss: 0.0183, Accuracy: 9938/10000 (99.38%)

epoch=17 Loss=0.03332556411623955 batch_id=00468: 100%|██████████| 469/469 [01:50<00:00,  4.24it/s]
Test set: Average loss: 0.0183, Accuracy: 9945/10000 (99.45%)

epoch=18 Loss=0.027276964858174324 batch_id=00468: 100%|██████████| 469/469 [01:51<00:00,  4.22it/s]
Test set: Average loss: 0.0177, Accuracy: 9941/10000 (99.41%)

epoch=19 Loss=0.06910333037376404 batch_id=00468: 100%|██████████| 469/469 [01:51<00:00,  4.21it/s]
Test set: Average loss: 0.0171, Accuracy: 9940/10000 (99.40%)
```
## References
https://towardsdatascience.com/how-to-reduce-training-parameters-in-cnns-while-keeping-accuracy-99-a213034a9777
