CSV file link - https://www.kaggle.com/mlg-ulb/creditcardfraud
<h1>Credit Card Fraud Detection</h1>

<p>
    <strong>Description:</strong> This project analyzes a dataset containing credit card transactions to detect fraudulent activities. Various machine learning models are used to classify transactions as fraudulent (1) or non-fraudulent (0).
</p>

<h2>📊 Dataset Overview</h2>
<ul>
    <li>Contains transactions made by European cardholders in September 2013.</li>
    <li>Includes 284,807 transactions, with 492 labeled as fraud (0.172% of all transactions).</li>
    <li>Data is highly imbalanced, requiring careful handling.</li>
    <li>Features V1 to V28 are obtained via PCA transformation.</li>
    <li><code>Time</code> represents seconds elapsed since the first transaction.</li>
    <li><code>Amount</code> is the transaction value.</li>
</ul>

<h2>🧪 Models and Performance</h2>

<table border="1">
    <tr>
        <th>Model</th>
        <th>Accuracy</th>
        <th>AUC-ROC</th>
        <th>Precision</th>
    </tr>
    <tr>
        <td>Random Forest</td>
        <td>0.999579</td>
        <td>0.958198</td>
        <td>0.923729</td>
    </tr>
    <tr>
        <td>Gradient Boosting</td>
        <td>0.998584</td>
        <td>0.270283</td>
        <td>0.894737</td>
    </tr>
    <tr>
        <td>Extra Tree</td>
        <td>0.999181</td>
        <td>0.900483</td>
        <td>0.717105</td>
    </tr>
    <tr>
        <td>Decision Tree</td>
        <td>0.999228</td>
        <td>0.889495</td>
        <td>0.746479</td>
    </tr>
    <tr>
        <td>AdaBoost</td>
        <td>0.999403</td>
        <td>0.983902</td>
        <td>0.857143</td>
    </tr>
    <tr>
        <td>Stacking Classifier</td>
        <td>0.999544</td>
        <td>0.924676</td>
        <td>0.980198</td>
    </tr>
</table>

<h2>📌 Conclusion</h2>
<ul>
    <li><strong>Best Model:</strong> Stacking Classifier (clf) due to high precision and AUC-ROC scores.</li>
    <li>Random Forest is also highly effective with strong accuracy and precision.</li>
    <li>AdaBoost balances performance across accuracy, precision, and AUC-ROC.</li>
    <li>Gradient Boosting struggles with class separation despite good accuracy.</li>
    <li>Decision Tree and Extra Tree lag behind in precision, making them less ideal.</li>
</ul>

<h2>⚙️ Installation</h2>
<pre><code># Clone the repository
git clone https://github.com/username/repository.git

# Navigate to the project directory
cd repository

# Install dependencies
pip install -r requirements.txt
</code></pre>
