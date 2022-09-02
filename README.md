# Deep Learning for Pigmented Skin Lesions Recognition
### Abstact
Research has showed, skin cancer accounts for 1/3 of all diagnosed cancers worldwide. Therefore, scientists and Doctors have been researched on pigmented skin lesion for many years. Still, the average experts’ diagnosis has only about 60% accuracy. To improve diagnosis accuracy, we plan to implement advanced neural network model on diagnosis of pigmented skin lesions using 12-layer CNN, Resnet150v2, Inceptionv3, Vgg19. By comparison, Inceptionv3 model has best performance, with 89% accuracy on validation, 86% accuracy on test dataset. Overall, transfer learning models are always show better performance than training a model directly (CNN).

### Data Source
Tschandl, Philipp, 2018, ["The HAM10000 dataset, a large collection of multi-source dermatoscopic images of common pigmented skin lesions"](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T).      
- In data source, there are 100015 image for training, and 193 for test purpose. Below shows some sample data:
![image](https://user-images.githubusercontent.com/64514218/188054112-d9963a5d-2cf1-469c-9caf-e33892a2979a.png)
- Class distribution
![image](https://user-images.githubusercontent.com/64514218/188054290-59319c77-cc9b-43d2-bf45-eaa80e4aba39.png)
- Solve imbalanced issue by generate new images by resize, rotate and re-zooming and etc.
![image](https://user-images.githubusercontent.com/64514218/188054590-d01cf2ed-849a-4998-8e61-b32554a09a4c.png)
- Result
![image](https://user-images.githubusercontent.com/64514218/188054827-bb988585-be89-4c5c-9f44-dd9155158447.png)
![image](https://user-images.githubusercontent.com/64514218/188054836-06c34e24-5095-48ab-99c2-91f43820a966.png)
### Conclusion
We trained models that could automate diagnosis of skin lesions. Inception V3 is the best model for our dataset. Inception V3 is also the most efficient model using relative low parameters. Predictions for ‘nv’, ‘vasc’ is relatively high in our model while ‘bkl’, ‘akiec’ is relatively low. To improve, we could train a model for distinguishing the attention of images to improve performance.     
### Reference
[1]N Codella, V Rotemberg, P Tschandl, ME Celebi, S Dusza, D Gutman, B Helba, A Kalloo, K Liopyris, M Marchetti, H Kittler, A Halpern. "Skin Lesion Analysis Toward Melanoma Detection 2018: A Challenge Hosted by the International Skin Imaging Collaboration (ISIC)."; 2019   

[2]Tschandl P, Codella N, Akay BN, Argenziano G, Braun RP, Cabo H, Gutman D, Halpern A, Helba B, Hofmann-Wellenhof R, Lallas A, Lapins J, Longo C, Malvehy J, Marchetti MA, Marghoob A, Menzies S, Oakley A, Paoli J, Puig S, Rinner C, Rosendahl C, Scope A, Sinz C, Soyer HP, Thomas L, Zalaudek I, Kittler H. Comparison of the accuracy of human readers versus machine-learning algorithms for pigmented skin lesion classification: an open, web-based, international, diagnostic study. Lancet Oncol. 2019 

[3] Chaturvedi, S.S., Tembhurne, J.V. & Diwan, T. A multi-class skin Cancer classification using deep convolutional neural networks. Multimed Tools Appl 79, 28477–28498 (2020). https://doi.org/10.1007/s11042-020-09388-2 

[4] A. K. Sharma et al., "Dermatologist-Level Classification of Skin Cancer Using Cascaded Ensembling of Convolutional Neural Network and Handcrafted Features Based Deep Neural Network," in IEEE Access, vol. 10, pp. 17920-17932, 2022, doi: 10.1109/ACCESS.2022.3149824. 

[5] Tschandl, Philipp, 2018, "The HAM10000 dataset, a large collection of multi-source dermatoscopic images of common pigmented skin lesions", https://doi.org/10.7910/DVN/DBW86T, Harvard Dataverse, V3, UNF:6:/APKSsDGVDhwPBWzsStU5A== [fileUNF] 

[6] Simonyan, Karen, and Andrew Zisserman. "Very deep convolutional networks for large-scale image recognition." arXiv preprint arXiv:1409.1556 (2014). 

[7] Szegedy, Christian, et al. "Inception-v4, inception-resnet and the impact of residual connections on learning." Thirty-first AAAI conference on artificial intelligence. 2017. 
