# ClipCap
a pytorch implement of ClipCap

Training process:
1. pretrain CLIP
Image encoder is ResNet101, which had been pretrained on ImageNet
using BERT to help pretrain CLIP on Flickr8k(using image and text matching as pretext task), in order to make cnn become a map from image to semantic space.

2. transfer
using pretrained cnn as image encoder, GPT2 as text decoder
