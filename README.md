#Fraud Detection Web App (Streamlit)

This project is a hands-on implementation of an end-to-end fraud detection workflow, built to translate a machine learning model into an interactive decision-support tool.

The application allows users to input transaction-level features (e.g., amount, balances, transaction type) and receive a real-time fraud prediction. The goal of the project was not just model inference, but to understand how analytical outputs can be operationalized through a simple, usable interface.

**Key components**

Data preprocessing and feature alignment for model inference

Streamlit-based UI for interactive inputs and predictions

Clear separation between model logic and presentation layer

This project reinforced the importance of reproducibility, dependency management, and designing analytics with the end user in mind.

** Tech Stack **
- Python
- Pandas, NumPy
- Scikit-learn
- Streamlit
- Jupyter Notebook
## Dataset

The dataset contains approximately **6.3 million financial transaction records** used for fraud detection. Transactions are labeled based on an existing fraud detection system, with a subset of records flagged as fraudulent.

Because the labels originate from a pre-existing algorithm, some transactions may be misclassified. This creates opportunities to explore where traditional rules-based approaches fail and how machine learning models can improve detection accuracy.

### Transaction Types

**CASH-IN**  
The process of increasing an account balance by depositing cash through a merchant.

**CASH-OUT**  
The withdrawal of cash from a merchant, resulting in a decrease in the account balance.

**DEBIT**  
A transaction similar to CASH-OUT, where funds are transferred from the mobile money service to a bank account.

**PAYMENT**  
The process of paying for goods or services, which decreases the sender’s balance and increases the receiver’s balance.

**TRANSFER**  
The process of sending money directly to another user within the mobile money platform.

### Notes on Data Usage

Due to the size of the dataset, raw data files are excluded from version control. Feature engineering and model training are demonstrated through the included notebooks, and the application focuses on inference using transaction-level inputs.

Future work could include additional feature engineering to better capture transaction behavior and identify weaknesses in existing fraud detection rules.
