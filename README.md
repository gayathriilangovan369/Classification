# Customer Purchase Prediction

## About the Project

This project is about predicting whether a customer will purchase a product or not based on their details.
The aim is to help companies target the right customers instead of sending promotions to everyone, which can reduce marketing costs.

---

## Dataset

The dataset contains:

* User ID
* Gender
* Age
* Estimated Salary
* Purchased (0 = No, 1 = Yes)

I removed the **User ID** column because it is just an identifier and does not help in prediction.

---

## Models Used

I tried three different models:

* Decision Tree
* Random Forest
* Support Vector Machine (SVC)

After comparing all three, I found that **Random Forest and SVC performed almost similarly**, but Random Forest had slightly better precision.

---

## Final Model Choice

I selected **Random Forest** for the final model.

Reason:

* It gave better precision (fewer wrong predictions)
* It helps reduce unnecessary marketing cost
* It works well without needing feature scaling

---

## Goal

The main goal is to **avoid targeting the wrong customers**.

So I focused more on:

* **Precision** → to reduce false positives (wrong customers)

---

## Model Performance

Accuracy: around **91%**

The model performs well and gives balanced results.

---

## How to Run

1. Install required libraries:

```id="r6y4jv"
pip install numpy pandas scikit-learn
```

2. Run the script:

```id="zrxq3f"
python app.py
```

3. Enter:

* Age
* Estimated Salary
* Gender

---

## Example

Input:

```id="v2a1ct"
Age: 30  
Salary: 50000  
Gender: Female  
```

Output:

```id="1bz0b2"
They will purchase
```

---

## What I Learned

* Removing unnecessary features improves model performance
* Importance of precision and recall
* Comparing multiple models before choosing one
* Random Forest works well for this type of problem

---

## Conclusion

This project shows how machine learning can help businesses make better decisions by predicting customer behavior and reducing unnecessary costs.

---
