# HFGYOLO
implement of "HFG-YOLO: A Real-Time Detector with High-level Feature Gathering for Blood Cell Detection"

# Install
	!pip install -r requirements.txt


# Performance on BCCD Dataset
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95)
                   all         73        967      0.889      0.916      0.944      0.676
             Platelets         73         76      0.916      0.861      0.937      0.542
                   RBC         73        819      0.784      0.887      0.906      0.657
                   WBC         73         72      0.967          1      0.988      0.829

# Performance on LISC Dataset
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95)
                   all         52         59      0.976      0.989      0.995      0.849
              Basophil         52         14      0.925          1      0.995      0.879
            Eosinophil         52         11      0.984          1      0.995      0.904
            Lymphocyte         52         10       0.97          1      0.995      0.859
              Monocyte         52         10          1       0.99      0.995      0.761
            Neutrophil         52         14          1      0.954      0.995       0.84

# Performance on WBCDD Dataset
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95):
                   all        144        263      0.895      0.879      0.956      0.795
            Neutrophil        144        204      0.971          1      0.989      0.845
              Monocyte        144         11      0.712      0.901      0.905      0.763
            Eosinophil        144          6          1        0.8      0.995      0.856
            Lymphocyte        144         37      0.886      0.892       0.93       0.77
              Basophil        144          5      0.905        0.8      0.962      0.741

# Performance on COCO2017
	AveragePrecision(AP)@[IoU=0.50:0.95|area=all|maxDets=100]=0.495
	AveragePrecision(AP)@[IoU=0.50|area=all|maxDets=100]=0.663
	AveragePrecision(AP)@[IoU=0.75|area=all|maxDets=100]=0.539
	AveragePrecision(AP)@[IoU=0.50:0.95|area=small|maxDets=100]=0.305
	AveragePrecision(AP)@[IoU=0.50:0.95|area=medium|maxDets=100]=0.548
	AveragePrecision(AP)@[IoU=0.50:0.95|area=large|maxDets=100]=0.665
	AverageRecall(AR)@[IoU=0.50:0.95|area=all|maxDets=1]=0.378
	AverageRecall(AR)@[IoU=0.50:0.95|area=all|maxDets=10]=0.625
	AverageRecall(AR)@[IoU=0.50:0.95|area=all|maxDets=100]=0.676
	AverageRecall(AR)@[IoU=0.50:0.95|area=small|maxDets=100]=0.496
	AverageRecall(AR)@[IoU=0.50:0.95|area=medium|maxDets=100]=0.735
	AverageRecall(AR)@[IoU=0.50:0.95|area=large|maxDets=100]=0.826
