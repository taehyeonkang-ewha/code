1.	Description
This project, titled "Super-Fast and Accurate Nonlinear Foot Deformation Prediction Using Graph Neural Networks," includes preprocessing code to prepare results obtained from Abaqus for training a GNN, as well as the GNN training code.

2.	Enviroment
This project conducts in the Google Colab A100 GPU environment.

3.	Files
-	Models/ 1. make_csv.ipynb : The .rpt files from Abaqus are converted into .csv data for elements, nodes, and surface elements. The resulting files have been uploaded to the Data/csv directory.
-	Models/ 2. make_pt.ipynb The data in the Data/csv directory is converted into pt files for GNN training.
-	Models/ 3. GNN_final.ipynb : It includes GNN training code.
-	Models/ 4. Ux,y,z_plot.ipynb : This is the code for plotting Figure 5 from the paper. It plots the foot in 3D based on the model and the information about nodes and elements from Data/pt_output.
-	Data/csv : These are the .csv files generated by the code in make_csv.ipynb. They include the contents of elements, nodes, and surface elements from the Abaqus results for a single foot.
-	Data/pt_imput/ 0919_total_final.pt : This is the .pt file generated by the code in make_csv.ipynb. This file is used as input data in GNN_final.ipynb.
-	Data/pt_output : This is the .pt file generated by the code in GNN_final.ipynb. The subfolders contain .pt files representing models trained with datasets of sizes 50, 100, 150, and 186, respectively.

4.	Usage
A.	A. I have attached the preprocessed file (Data/pt_input/0919_total_final.pt). Please proceed with GNN training using this file.
B.	Please unzip the GNN_code folder on Google Drive and execute the code.
