# 2030 Financial AI: Investment Predictions & Sharia Compliance 🚀
import streamlit as st
import numpy as np
from sklearn.linear_model import LinearRegression

# 🌟 Future-proof prediction model
def predict_returns(years: int) -> float:
    model = LinearRegression()
    X = np.array([[1], [2], [3], [4], [5]])  # Time (years) as predictor
    y = np.array([100, 200, 300, 400, 500])  # Hypothetical investment returns
    model.fit(X, y)  # Training the model on data
    return model.predict([[years]])[0]  # Predicting return for given years

# 🔒 Sharia Compliance Check for Ethical Investment
def check_compliance(investment_type: str) -> dict:
    forbidden_investments = ['alcohol', 'gambling', 'tobacco', 'weapons']
    if investment_type.lower() in forbidden_investments:
        return {"compliant": False, "message": "🚫 This investment violates Sharia principles."}
    return {"compliant": True, "message": "✅ This investment is Sharia-compliant!"}

# 🧠 Streamlit UI - The Future of Interactivity 🌐
st.set_page_config(page_title="AI Financial Advisor 2030", page_icon="💡", layout="wide")

# Header
st.title("AI Financial Prediction & Sharia Compliance 2030 🤖")
st.subheader("Empowering Financial Decisions with AI & Ethical Guidelines ⚖️")

# **Investment Return Prediction**
st.header("Investment Return Prediction 📈")

# User Input: Number of Years
years = st.slider('Select the number of years for your investment prediction:', min_value=1, max_value=50, value=5)

# Predicting returns based on input years
if st.button('Predict Investment Returns 🚀'):
    predicted_return = predict_returns(years)
    st.write(f"💸 The predicted returns for {years} years is: ${predicted_return:.2f}")

# **Sharia Compliance Check**
st.header("Sharia Compliance Check 🔐")

# User Input: Investment type
investment_type = st.text_input('Enter the type of investment (e.g., stocks, alcohol, gambling):', "")

# Checking compliance
if st.button('Check Compliance 🔍'):
    compliance_result = check_compliance(investment_type)
    if compliance_result['compliant']:
        st.success(compliance_result['message'])
    else:
        st.error(compliance_result['message'])

# Cool footer with futuristic style
st.markdown("""--- 
&copy; 2030 Financial AI Advisors 💡 | Empowering ethical and smart financial choices! 🚀
""")
