# Point-defect-analysis-GUI
![image](https://github.com/wormschu/Point-defect-analysis-GUI/assets/56716689/79c8588a-636e-4f8f-9575-3439881ab4ed)
This is a program that finds MoTe2 point vacancy defects using pytorch-based deep learning. 
Also, it can be used without a separate GPU power. (If you have enough CPU power)

Through this program, you can quickly analyze your point defects and modify the deep learning results to complete better results.


## Getting started
This program was tested for stability in Python 3.9.0 version. Therefore, we recommend using version 3.9.0.

1. Git clone or download this repository.

2. utilize requirements.txt to install the required libraries.

```
pip install -r requirements.txt
```

3. Unzip CNN-1 and CNN-2 and place the same files in the same(default) directory.

4. Go to the current directory in the anaconda prompt window and enter the code below:

```
python dist/GUI_CPU.py
```

## How to use the program

1. Click “Load image” to load the STEM image you want to analyze.
![image](https://github.com/wormschu/Point-defect-analysis-GUI/assets/56716689/dbff1e7c-8700-4340-920d-98487cae88c3)

2. Press “Analysis” to run image analysis.![image](https://github.com/wormschu/Point-defect-analysis-GUI/assets/56716689/2bb5cf11-c461-40a4-a7e0-7866b5d2cfbf)

3. The basic gray color in the analyzed image is perfect, and the colors are differentiated for each defect.![image](https://github.com/wormschu/Point-defect-analysis-GUI/assets/56716689/c941b806-cd50-4632-ad4d-72b248985938)

4. When you click on the desired unit cell image, the corresponding unit cell appears in the “crop image” window on the right. (In this example, the unit cell indicated by the red arrow was clicked) ![image](https://github.com/wormschu/Point-defect-analysis-GUI/assets/56716689/c0052c08-fd1f-4d83-81f4-6649c9cd3e87)

5. You can perform intensity profiling on the crop unit cell image. After marking the two areas Te and Mo, you can use the slider on the right to specify the area. 
*Caution You need to take Te (left point) first.

If so, the green intensity graph below is drawn.![image](https://github.com/wormschu/Point-defect-analysis-GUI/assets/56716689/62d40464-bd18-4a69-828c-32e1f7c9ae25)

6. Designate a class worth comparing among the reference simulation defect classes and perform intensity profiling by comparing it to the crop unit cell image. (In this case, select VMo ![image](https://github.com/wormschu/Point-defect-analysis-GUI/assets/56716689/43e75f45-c1a6-4f34-8789-2494c925a154)

7. After profiling an arbitrary crop unit cell image, you can modify the results of deep learning analysis. Below, the unit cell in question was previously perfect, but it will change when you specify a different defect class and click “Label insert” above. ![image](https://github.com/wormschu/Point-defect-analysis-GUI/assets/56716689/1e1ea8ad-4aae-402a-8d72-0261f143948b)

8. When all analysis is complete, click the “Save” button. Then, the image below is created in the save folder in that directory.
![image](https://github.com/wormschu/Point-defect-analysis-GUI/assets/56716689/d032c515-e681-4b69-ae54-424c94b7c09e)






