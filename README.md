# 1129homework

Data Pre-processing
1.	本次作業使用Bank資料並無空值。
2.	針對”job”、”marital”、”education”、”default”、”housing”、”loan”、”contact”、”month”、”poutcome”、”y”做label encoding。
3.	從原資料中分出y值，因為y值為output target。
4.	對原資料x做正規化(Standard Scaler)、特徵選擇(PCA)。
5.	根據老師上課規定，分割資料為8:2分法，以及random_state=1234。
Data Training
學生利用資料做Logstic Regression、Non-Linear SVM、Linear SVM、MLP、MLNN、Logistc Regression by MLNN，並輸出其score值。
1.	Logistic Regression分數約為0.8946。
2.	非線性SVM學生Kernel使用”rbf”進行，分數約為0.8955。
3.	線性SVM分數約為0.886。
4.	MLP分數約為0.8986。
5.	MLNN根據簡報上之規定，學生設置三層Dense(50，30，1)，並且因為PCA輸出的Component設定為16，因此input_shape設為16，分數約為0.9010。
6.	Logistc Regression by MLNN根據簡報上不設置隱藏層只設置輸出層，因此Dense為1，其分數約為0.8994。
