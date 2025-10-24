<h1>Supply Chain Delivery Delay Prediction</h1>

<h2>1. Project Overview & Business Problem</h2>
<p>
In a time of significant global shipping disruption, supply chain predictability has become a critical business advantage. 
For a high-volume sporting goods store, unexpected shipment delays can lead to stock-outs, increased emergency freight costs, 
and decreased customer loyalty.
</p>

<p><b>Business Goal:</b> To proactively identify high-risk shipments before they become late.</p>
<p><b>Project Goal:</b> To develop and evaluate a supervised machine learning pipeline that accurately predicts the likelihood of a shipment being delayed. 
This allows the business to move from a reactive to a proactive logistics model.</p>

<hr>

<h2>2. Data Source</h2>
<p>
The dataset used (<b>GA.csv</b>) contains historical logistics and shipment data for the sporting goods store. 
Each row represents a single shipment with features including:
</p>

<ul>
  <li><i>(User: Please add 3–5 key features from your dataset here)</i></li>
  <li>Carrier</li>
  <li>Origin_Port</li>
  <li>Warehouse_Location</li>
  <li>Item_Category</li>
  <li>Promised_Delivery_Date</li>
</ul>

<p><b>Target Variable:</b> On_Time (1) / Delayed (0)</p>

<hr>

<h2>3. Analytical Methodology</h2>
<p>The project followed a structured data mining process to ensure a robust and reliable final model.</p>

<h3>3.1. Data Preprocessing</h3>
<ul>
  <li><b>Handling Missing Values:</b> Assessed and imputed missing data to ensure dataset completeness.</li>
  <li><b>Categorical Encoding:</b> Used <code>sklearn.preprocessing.LabelEncoder</code> to convert categorical features (e.g., carrier names, port codes) into numerical format.</li>
  <li><b>Feature Scaling:</b> Applied <code>sklearn.preprocessing.StandardScaler</code> to normalize numerical features and prevent scale bias.</li>
</ul>

<h3>3.2. Feature Engineering & Selection</h3>
<p>To identify the most impactful predictors of delay, two feature selection techniques were implemented:</p>
<ul>
  <li><b>Recursive Feature Elimination (RFE):</b> Iteratively removed the weakest features to find the optimal subset.</li>
  <li><b>Sequential Feature Selector (SFS):</b> Tested features incrementally to build the most powerful predictive set.</li>
</ul>

<h3>3.3. Model Building & Evaluation</h3>
<p>Four classification models were trained and evaluated to identify the best-performing algorithm for this business problem:</p>
<ul>
  <li>Decision Tree Classifier</li>
  <li>Random Forest Classifier</li>
  <li>LightGBM (LGBM) Classifier</li>
  <li>XGBoost (XGB) Classifier</li>
</ul>

<p>
Models were rigorously evaluated using cross-validation and assessed on <b>Accuracy</b>, <b>Precision</b>, <b>Recall</b>, and <b>F1-Score</b>.
</p>

<hr>

<h2>4. Key Findings & Results</h2>
<p><i>(User: Please update this section with your final results from the report/notebook)</i></p>

<p>
The model comparison revealed that the <b>XGBoost Classifier</b> provided the best balance of performance and efficiency, achieving a final Accuracy of 
<b>[XX.X]%</b>.
</p>

<ul>
  <li><b>Key Predictors:</b> [Feature 1], [Feature 2], [Feature 3]</li>
  <li><b>Model Performance:</b> The final model demonstrated strong recall in identifying delayed shipments — critical for proactive logistics.</li>
</ul>

<p><i>(Placeholder: Add a screenshot of your best model’s confusion matrix or performance plot here.)</i></p>

<hr>

<h2>5. Business Recommendations & Impact</h2>
<p>
The insights from this model empower the sporting goods store to take specific, data-driven actions:
</p>
<ul>
  <li><b>Proactive Intervention:</b> Flag high-risk shipments in the logistics dashboard as soon as they are booked, enabling alternate shipping decisions.</li>
  <li><b>Optimized Inventory:</b> Adjust safety stock levels for routes consistently flagged as high-risk, reducing stock-out likelihood.</li>
  <li><b>Improved Customer Service:</b> Proactively communicate with customers regarding unavoidable delays to manage expectations and maintain satisfaction.</li>
</ul>

<hr>

<h2>6. Technology Stack</h2>
<ul>
  <li><b>Data Analysis:</b> Pandas, NumPy</li>
  <li><b>Data Visualization:</b> Matplotlib, Seaborn</li>
  <li><b>Machine Learning:</b> Scikit-learn, XGBoost, LightGBM</li>
  <li><b>Feature Selection:</b> Mlxtend</li>
  <li><b>Environment:</b> Google Colab, Python 3</li>
</ul>

<hr>

<h2>How to Navigate This Repository</h2>
<ul>
  <li><b>/README.md:</b> (This file) High-level project overview.</li>
  <li><b>/Supply Chain ML.ipynb:</b> Complete Jupyter Notebook with Python code, data analysis, and model development.</li>
  <li><b>/Supply Chain Report.pdf:</b> Formal report detailing background, methodology, and findings.</li>
</ul>

<br>
<p align="center">
  <i>Example Visual

Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
